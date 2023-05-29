# Comparing `tmp/feynml-0.2.0.tar.gz` & `tmp/feynml-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynml-0.2.0.tar", max compression
+gzip compressed data, was "feynml-0.2.1.tar", max compression
```

## Comparing `feynml-0.2.0.tar` & `feynml-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,47 @@
--rw-r--r--   0        0        0    35149 2023-05-27 19:29:52.352554 feynml-0.2.0/LICENSE
--rw-r--r--   0        0        0     2359 2023-05-27 19:29:52.352554 feynml-0.2.0/README.md
--rw-r--r--   0        0        0      179 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/__init__.py
--rw-r--r--   0        0        0      986 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/connector.py
--rw-r--r--   0        0        0     4769 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/feynmandiagram.py
--rw-r--r--   0        0        0     2496 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/feynml.py
--rw-r--r--   0        0        0     2452 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/head.py
--rw-r--r--   0        0        0      651 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/id.py
--rw-r--r--   0        0        0        0 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/interface/__init__.py
--rw-r--r--   0        0        0     2636 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/interface/hepmc.py
--rw-r--r--   0        0        0     4709 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/interface/lhe.py
--rw-r--r--   0        0        0     1569 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/interface/qgraf.py
--rw-r--r--   0        0        0     1301 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/interface/util.py
--rw-r--r--   0        0        0      385 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/labeled.py
--rw-r--r--   0        0        0     1035 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/leg.py
--rw-r--r--   0        0        0      303 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/line.py
--rw-r--r--   0        0        0      396 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/link.py
--rw-r--r--   0        0        0      400 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/meta.py
--rw-r--r--   0        0        0      563 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/momentum.py
--rw-r--r--   0        0        0     1385 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/particles.py
--rw-r--r--   0        0        0     3115 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/pdgid.py
--rw-r--r--   0        0        0      846 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/point.py
--rw-r--r--   0        0        0      207 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/propagator.py
--rw-r--r--   0        0        0      349 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/shape.py
--rw-r--r--   0        0        0     7878 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/sheet.py
--rw-r--r--   0        0        0      363 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/sourcing.py
--rw-r--r--   0        0        0     2839 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/styled.py
--rw-r--r--   0        0        0      364 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/targeting.py
--rw-r--r--   0        0        0      795 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/type.py
--rw-r--r--   0        0        0      425 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/vertex.py
--rw-r--r--   0        0        0      741 2023-05-27 19:29:52.356555 feynml-0.2.0/feynml/xml.py
--rw-r--r--   0        0        0     1893 2023-05-27 19:29:53.856692 feynml-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 feynml-0.2.0/setup.py
--rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 feynml-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-29 19:03:34.181465 feynml-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2359 2023-05-29 19:03:34.181465 feynml-0.2.1/README.md
+-rw-r--r--   0        0        0      179 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/__init__.py
+-rw-r--r--   0        0        0      986 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/connector.py
+-rw-r--r--   0        0        0     5497 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/feynmandiagram.py
+-rw-r--r--   0        0        0     3116 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/feynml.py
+-rw-r--r--   0        0        0     2959 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/head.py
+-rw-r--r--   0        0        0      651 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/id.py
+-rw-r--r--   0        0        0        0 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/__init__.py
+-rw-r--r--   0        0        0     1863 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/fermion.py
+-rw-r--r--   0        0        0     1843 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/feynmangraph.py
+-rw-r--r--   0        0        0      612 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/field.py
+-rw-r--r--   0        0        0     3443 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/insertions.py
+-rw-r--r--   0        0        0      129 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/particle.py
+-rw-r--r--   0        0        0     2384 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/propagator.py
+-rw-r--r--   0        0        0     1729 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/rule.py
+-rw-r--r--   0        0        0      635 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/sequenceform.py
+-rw-r--r--   0        0        0     2429 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/topology.py
+-rw-r--r--   0        0        0     7356 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/topologylist.py
+-rw-r--r--   0        0        0     1427 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/vector.py
+-rw-r--r--   0        0        0      896 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/vertex.py
+-rw-r--r--   0        0        0     2641 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/hepmc.py
+-rw-r--r--   0        0        0     4694 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/lhe.py
+-rw-r--r--   0        0        0     1569 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/qgraf.py
+-rw-r--r--   0        0        0      260 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/labeled.py
+-rw-r--r--   0        0        0     1035 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/leg.py
+-rw-r--r--   0        0        0      303 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/line.py
+-rw-r--r--   0        0        0      290 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/link.py
+-rw-r--r--   0        0        0      294 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/meta.py
+-rw-r--r--   0        0        0      563 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/momentum.py
+-rw-r--r--   0        0        0     1385 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/particles.py
+-rw-r--r--   0        0        0     3115 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/pdgid.py
+-rw-r--r--   0        0        0      846 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/point.py
+-rw-r--r--   0        0        0      207 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/propagator.py
+-rw-r--r--   0        0        0      349 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/shape.py
+-rw-r--r--   0        0        0     7878 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/sheet.py
+-rw-r--r--   0        0        0      363 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/sourcing.py
+-rw-r--r--   0        0        0     2804 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/styled.py
+-rw-r--r--   0        0        0      364 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/targeting.py
+-rw-r--r--   0        0        0      780 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/type.py
+-rw-r--r--   0        0        0     1608 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/util.py
+-rw-r--r--   0        0        0      425 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/vertex.py
+-rw-r--r--   0        0        0      756 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/xml.py
+-rw-r--r--   0        0        0     1893 2023-05-29 19:03:35.821460 feynml-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 feynml-0.2.1/setup.py
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 feynml-0.2.1/PKG-INFO
```

### Comparing `feynml-0.2.0/LICENSE` & `feynml-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/README.md` & `feynml-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/feynml/connector.py` & `feynml-0.2.1/feynml/connector.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/feynml/feynmandiagram.py` & `feynml-0.2.1/feynml/feynmandiagram.py`

 * *Files 20% similar despite different names*

```diff
@@ -70,14 +70,25 @@
     def has_id(self, id):
         for l in [self.propagators, self.vertices, self.legs]:
             for a in l:
                 if a.id == id:
                     return True
         return False
 
+    def get(self, lmbda):
+        ret = []
+        for l in [self.propagators, self.vertices, self.legs]:
+            for a in l:
+                try:
+                    if lmbda(a):
+                        ret.append(a)
+                except Exception:
+                    pass
+        return ret
+
     def get_point(self, idd):
         for v in self.vertices:
             if v.id == idd:
                 return v
         for leg in self.legs:
             if leg.id == idd:
                 return leg
@@ -152,7 +163,22 @@
 
     def get_sheet(self):
         return self.sheet
 
     def with_sheet(self, sheet):
         self.sheet = sheet
         return self
+
+    def has_vertex(self, vertex):
+        return vertex in self.vertices
+
+    def has_vertex_id(self, vertexid):
+        return self.get_vertex(vertexid) is not None
+
+    def has_leg(self, leg):
+        return leg in self.legs
+
+    def has_propagator(self, propagator):
+        return propagator in self.propagators
+
+    def has(self, obj):
+        return self.has_vertex(obj) or self.has_leg(obj) or self.has_propagator(obj)
```

### Comparing `feynml-0.2.0/feynml/feynml.py` & `feynml-0.2.1/feynml/feynml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
+import os
 import warnings
 from dataclasses import dataclass, field
 from importlib.metadata import version
 from typing import List, Optional
 
 import cssutils
+import smpl_io.io as io
 from smpl_doc import doc
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 from feynml.feynmandiagram import FeynmanDiagram
 from feynml.head import Head
@@ -55,14 +57,21 @@
     )
 
     diagrams: List[FeynmanDiagram] = field(
         default_factory=list,
         metadata={"name": "diagram", "type": "Element", "namespace": ""},
     )
 
+    def get_root(self):
+        return self.head.root
+
+    def with_root(self, root):
+        self.head.root = root
+        return self
+
     def get_diagram(self, idd):
         for d in self.diagrams:
             if d.id == idd:
                 return d
         return None
 
     def get_style(self, obj, xml=None):
@@ -79,7 +88,20 @@
 
     def get_sheet(self):
         return self.head.get_sheet()
 
     def with_sheet(self, sheet):
         self.head.with_sheet(sheet)
         return self
+
+    @classmethod
+    def from_xml_file(cls, file: str):
+        """Load self from XML file."""
+        # get parent directory of file
+        r = cls.from_xml(io.read(file))
+        # check if file exists
+        if os.path.isfile(file):
+            r.head.root = os.path.dirname(file) + "/"
+        elif file.startswith("http"):
+            # remove last file in url
+            r.head.root = "/".join(file.split("/")[:-1]) + "/"
+        return r
```

### Comparing `feynml-0.2.0/feynml/head.py` & `feynml-0.2.1/feynml/head.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         metadata={"name": "meta", "namespace": ""},
     )
     links: List[Link] = field(
         default_factory=list,
         metadata={"name": "link", "namespace": ""},
     )
     cached_links = {}
+    root = "."  # root directory for relative links
     title: Optional[str] = field(default=None, metadata={"type": "Element"})
 
     # description: Optional[str] = field(default="", metadata={"type": "Element"})
 
     # style: Optional[str] = field(default="", metadata={"type": "Element"})
     style: CSSSheet = field(
         default_factory=lambda: cssutils.parseString(""),
@@ -52,20 +53,30 @@
         """
         Return a dictionary of resolved links.
 
         If cached is True, then the cached resolved links are returned.
         """
         ret = {}
         for m in self.links:
-            if m.ref in self.cached_links and cached:
-                ret[m.ref] = self.cached_links[m.ref]
+            if m.rel in self.cached_links and cached:
+                ret[m.rel] = self.cached_links[m.rel]
             else:
-                ret[m.ref] = io.read(m.href)
+                # handle absolute or relative
+                if m.href.startswith("http"):
+                    print("Direct")
+                    ret[m.rel] = io.read(m.href)
+                    print(ret[m.rel])
+                elif m.href.startswith("/"):
+                    ret[m.rel] = io.read(m.href)
+                else:
+                    ret[m.rel] = io.read(self.root + m.href)
+                if m.rel == "stylesheet":
+                    ret[m.rel] = cssutils.parseString(ret[m.rel])
                 if cache:
-                    self.cached_links[m.ref] = ret[m.ref]
+                    self.cached_links[m.rel] = ret[m.rel]
         return ret
 
     def get_meta_dict(self):
         """
         Return a dictionary of meta tags.
         """
         return {m.name: m.content for m in self.metas}
```

### Comparing `feynml-0.2.0/feynml/id.py` & `feynml-0.2.1/feynml/id.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/feynml/interface/hepmc.py` & `feynml-0.2.1/feynml/interface/hepmc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import pyhepmc
 from pyhepmc import GenEvent
 
 from feynml.feynmandiagram import FeynmanDiagram
 from feynml.feynml import FeynML, Head, Meta
 from feynml.leg import Leg
 from feynml.propagator import Propagator
+from feynml.util import leg_id_wrap, propagator_id_wrap, vertex_id_wrap
 from feynml.vertex import Vertex
 
-from .util import leg_id_wrap, propagator_id_wrap, vertex_id_wrap
-
 # TODO add momenta?
 
 
 def hepmc_event_to_feynman(event: GenEvent) -> FeynmanDiagram:
     """
     Convert a GenEvent to a FeynmanDiagram.
```

### Comparing `feynml-0.2.0/feynml/interface/lhe.py` & `feynml-0.2.1/feynml/interface/lhe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import pylhe
 
 from feynml.feynmandiagram import FeynmanDiagram
 from feynml.feynml import FeynML, Head, Meta
 from feynml.leg import Leg
 from feynml.propagator import Propagator
+from feynml.util import leg_id_wrap, vertex_id_wrap
 from feynml.vertex import Vertex
 
-from .util import leg_id_wrap, propagator_id_wrap, vertex_id_wrap
-
 # TODO add momenta?
 
 
 def lhe_event_to_feynman(event: pylhe.LHEEvent) -> FeynmanDiagram:
     fd = FeynmanDiagram()
     hp = Vertex(id=vertex_id_wrap(0))
     fd.add(hp)
```

### Comparing `feynml-0.2.0/feynml/interface/qgraf.py` & `feynml-0.2.1/feynml/interface/qgraf.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/feynml/leg.py` & `feynml-0.2.1/feynml/leg.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/feynml/momentum.py` & `feynml-0.2.1/feynml/momentum.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/feynml/particles.py` & `feynml-0.2.1/feynml/particles.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/feynml/pdgid.py` & `feynml-0.2.1/feynml/pdgid.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/feynml/point.py` & `feynml-0.2.1/feynml/point.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/feynml/sheet.py` & `feynml-0.2.1/feynml/sheet.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.0/feynml/styled.py` & `feynml-0.2.1/feynml/styled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from dataclasses import dataclass, field
 from typing import Optional
 
 import cssutils
 from smpl_doc.doc import deprecated
-from smpl_util.util import withify
 from xsdata.formats.converter import Converter, converter
 
 # We don't want to see the cssutils warnings, since we have custom properties
 cssutils.log.setLevel(logging.CRITICAL)
 
 CSSString = cssutils.css.CSSStyleDeclaration
 CSSSheet = cssutils.css.CSSStyleSheet
```

### Comparing `feynml-0.2.0/feynml/type.py` & `feynml-0.2.1/feynml/type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from typing import List
 
 import cssutils
 import smpl_doc.doc as doc
 
 from feynml import shape, sheet
```

### Comparing `feynml-0.2.0/pyproject.toml` & `feynml-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feynml"
-version = "0.2.0"
+version = "0.2.1"
 description = "Feynman diagram markup language"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/feynml"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `feynml-0.2.0/setup.py` & `feynml-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['feynml', 'feynml.interface']
+['feynml', 'feynml.interface', 'feynml.interface.formcalc']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['cssselect',
  'cssutils',
@@ -19,15 +19,15 @@
  'xsdata[cli,lxml,soap]']
 
 extras_require = \
 {'interfaces': ['pyqgraf>=0.0.3', 'pyhepmc', 'pylhe']}
 
 setup_kwargs = {
     'name': 'feynml',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Feynman diagram markup language',
     'long_description': '# FeynML\n\nFeynML from <https://feynml.hepforge.org/>\n\nFeynML is a project to develop an XML dialect for describing Feynman diagrams as used in quantum field theory calculations. The primary aim is to unambiguously describe the structure of a diagram in XML, giving a de facto representation for diagram structure which can be easily translated into another representation.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynml.svg)\n\n\n[![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] [![Codacy Badge][cc c i]][cc c l]  [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Installation\n```sh\npip install [--user] feynml\n```\n\nor from cloned source:\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/feynml/>\n*   <https://apn-pucky.github.io/pyfeyn2/feynml/index.html>\n\n## Related:\n\n*   <https://github.com/APN-Pucky/pyfeyn2>\n\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n\n[pypi image]: https://badge.fury.io/py/feynml.svg\n[pypi link]: https://pypi.org/project/feynml/\n[pypi versions]: https://img.shields.io/pypi/pyversions/feynml.svg\n\n[a t link]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml/badge.svg\n\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/feynml&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/feynml&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/feynml?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/feynml/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/feynml',
```

### Comparing `feynml-0.2.0/PKG-INFO` & `feynml-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feynml
-Version: 0.2.0
+Version: 0.2.1
 Summary: Feynman diagram markup language
 Home-page: https://github.com/APN-Pucky/feynml
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

