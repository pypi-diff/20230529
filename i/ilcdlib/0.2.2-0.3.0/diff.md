# Comparing `tmp/ilcdlib-0.2.2.tar.gz` & `tmp/ilcdlib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-0.2.2.tar", max compression
+gzip compressed data, was "ilcdlib-0.3.0.tar", max compression
```

## Comparing `ilcdlib-0.2.2.tar` & `ilcdlib-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/LICENSE
--rw-r--r--   0        0        0     1761 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/README.md
--rw-r--r--   0        0        0     3341 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      837 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    11642 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/src/ilcdlib/common.py
--rw-r--r--   0        0        0     1330 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     1131 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     5221 2023-05-25 14:33:16.022257 ilcdlib-0.2.2/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     6330 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     4103 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3543 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3259 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0      837 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0     5167 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     2415 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     1152 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     1014 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     2832 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    15855 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0      837 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     6745 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     4728 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0     1435 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1705 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1294 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1206 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/type.py
--rw-r--r--   0        0        0     1576 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2382 2023-05-25 14:33:16.026257 ilcdlib-0.2.2/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 ilcdlib-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4949 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/README.md
+-rw-r--r--   0        0        0     3341 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    12504 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0     1334 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     1474 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     5329 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     6330 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     5749 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     4890 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3650 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3774 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0      837 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0     6967 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     2415 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     1152 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     1014 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     2832 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    17577 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0      837 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     1900 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1894 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1732 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7086 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     4728 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1705 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1294 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1206 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     1712 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2382 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6013 1970-01-01 00:00:00.000000 ilcdlib-0.3.0/PKG-INFO
```

### Comparing `ilcdlib-0.2.2/LICENSE` & `ilcdlib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/pyproject.toml` & `ilcdlib-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "0.2.2"
+version = "0.3.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
@@ -21,15 +21,15 @@
 
 [tool.poetry.scripts]
 ilcdtool = { callable = "ilcdlib:cli.entrypoint", extras = ["cli"] }
 
 [tool.poetry.dependencies]
 python = "^3.11"
 urllib3 = { version = ">=1.26.16,<2.0.0" }
-openepd = { version = ">=0.1.3,<1.0.0" }
+openepd = { version = ">=0.3.0,<1.0.0" }
 
 # Optional dependencies
 lxml = { version = "~=4.9.2", optional = true }
 cli-rack = { version = ">=1.0.6", optional = true }
 
 [tool.poetry.dev-dependencies]
 # Unit tests
@@ -57,15 +57,15 @@
 types-urllib3 = ">=1.26.2"
 
 [tool.poetry.extras]
 lxml = ["lxml"]
 cli = ["cli-rack"]
 
 [tool.commitizen]
-version = "0.2.2"
+version = "0.3.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/ilcdlib/__version__.py",
 ]
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/__init__.py` & `ilcdlib-0.3.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/__main__.py` & `ilcdlib-0.3.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/__version__.py` & `ilcdlib-0.3.0/src/ilcdlib/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.2.2"
+VERSION = "0.3.0"
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/cli.py` & `ilcdlib-0.3.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/common.py` & `ilcdlib-0.3.0/src/ilcdlib/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #  Find out more at www.BuildingTransparency.org
 #
 import abc
 import datetime
 from typing import IO, Literal, Self, Sequence, TextIO, overload
 
 from openepd.model.epd import Epd
+from openepd.model.lcia import ImpactSet
 from openepd.model.org import Org
 from openepd.model.pcr import Pcr
 
 from ilcdlib.const import IlcdDatasetType
 from ilcdlib.dto import IlcdReference
 from ilcdlib.reference_data import get_ilcd_epd_reference_data_provider
 from ilcdlib.type import LangDef, LocalizedStr
@@ -125,14 +126,16 @@
                 contact="http://lca.jrc.it/ILCD/Contact",
                 flow="http://lca.jrc.it/ILCD/Flow",
                 process="http://lca.jrc.it/ILCD/Process",
                 source="http://lca.jrc.it/ILCD/Source",
                 ug="http://lca.jrc.it/ILCD/UnitGroup",
                 fp="http://lca.jrc.it/ILCD/FlowProperty",
                 mm="http://www.matml.org/",
+                epd2013="http://www.iai.kit.edu/EPD/2013",
+                epd2019="http://www.iai.kit.edu/EPD/2019",
             )
         )
 
     def get_xml_tree(
         self, entity_type: str, entity_id: str, entity_version: str | None, *, allow_static_datasets: bool = True
     ) -> T_ET.Element:
         """
@@ -269,33 +272,48 @@
 
     def _get_external_tree(self, root: T_ET.Element, path: XmlPath) -> T_ET.Element | None:
         ref = self._get_reference(root, path)
         if ref is None:
             return None
         return self.get_xml_tree(ref.entity_type, ref.entity_id, ref.entity_version, allow_static_datasets=True)
 
+    def _get_external_binary(self, root: T_ET.Element, path: XmlPath) -> IO[bytes] | None:
+        ref = self._get_reference(root, path)
+        if ref is None:
+            return None
+        return self.data_provider.get_entity_stream(ref.entity_type, ref.entity_id, ref.entity_version, binary=True)
+
 
 class OpenEpdContactSupportReader(metaclass=abc.ABCMeta):
     """Base class for adding OpenEPD export support."""
 
     @abc.abstractmethod
-    def to_openepd_org(self, lang: LangDef) -> Org:
-        """Read as OpenEPD Org object."""
+    def to_openepd_org(self, lang: LangDef, base_url: str | None = None) -> Org:
+        """Read as openEPD Org object."""
         pass
 
 
 class OpenEpdPcrSupportReader(metaclass=abc.ABCMeta):
-    """Base class for adding OpenEPD export support."""
+    """Base class for adding openEPD export support."""
 
     @abc.abstractmethod
-    def to_openepd_pcr(self, lang: LangDef) -> Pcr:
-        """Read as OpenEPD Pcr object."""
+    def to_openepd_pcr(self, lang: LangDef, base_url: str | None = None) -> Pcr:
+        """Read as openEPD Pcr object."""
         pass
 
 
 class OpenEpdEdpSupportReader(metaclass=abc.ABCMeta):
-    """Base class for adding OpenEPD export support to EPD documents."""
+    """Base class for adding openEPD export support to EPD documents."""
 
     @abc.abstractmethod
-    def to_openepd_epd(self, lang: LangDef) -> Epd:
+    def to_openepd_epd(self, lang: LangDef, base_url: str | None = None) -> Epd:
         """Read as OpenEPD EPD object."""
         pass
+
+
+class OpenEpdImpactSetSupportReader(metaclass=abc.ABCMeta):
+    """Base class for adding openEPD export support to LCIAResults."""
+
+    @abc.abstractmethod
+    def to_openepd_impact_set(self, lang: LangDef, base_url: str | None = None) -> ImpactSet:
+        """Read as openEPD ImpactSet object."""
+        pass
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/const.py` & `ilcdlib-0.3.0/src/ilcdlib/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from enum import StrEnum
 
-ILCD_IDENTIFICATION: tuple[str] = ("ILCD",)
+ILCD_IDENTIFICATION: tuple[str] = ("ILCD_EPD",)
 
 
 class IlcdContactClass(StrEnum):
     """Enumeration of ILCD contact classes."""
 
     Person = "Persons"
     Company = "Organisations"
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-0.3.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/dto.py` & `ilcdlib-0.3.0/src/ilcdlib/dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,13 +23,20 @@
 class IlcdReference(NamedTuple):
     """A reference to an ILCD entity."""
 
     entity_type: str
     entity_id: str
     entity_version: str | None
 
+    def to_url(self, base_url: str | None) -> str:
+        """Convert the reference to a URL."""
+        prefix = base_url if base_url is not None else "https://unknown.tld"
+        if prefix.endswith("/"):
+            prefix = prefix[:-1]
+        return f"{prefix}/resource/{self.entity_type}/{self.entity_id}?version={self.entity_version}"
+
 
 class ProductClassDef(NamedTuple):
     """A product class definition."""
 
     id: str | None
     name: str | None
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/entity/__init__.py` & `ilcdlib-0.3.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/entity/contact.py` & `ilcdlib-0.3.0/src/ilcdlib/entity/contact.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,33 +13,37 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from openepd.model.common import ExternalIdentification
 from openepd.model.org import Contact, Org
 
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdContactSupportReader
 from ilcdlib.const import IlcdContactClass
+from ilcdlib.dto import IlcdReference
 from ilcdlib.sanitizing.domain import domain_from_url
 from ilcdlib.sanitizing.phone import cleanup_phone
 from ilcdlib.type import LangDef
-from ilcdlib.utils import create_openepd_identification, none_throws
+from ilcdlib.utils import create_openepd_attachments, none_throws
 from ilcdlib.xml_parser import T_ET
 
 
 class IlcdContactReader(OpenEpdContactSupportReader, IlcdXmlReader):
     """Reader for ILCD contact data sets."""
 
     def __init__(self, element: T_ET.Element, data_provider: BaseIlcdMediumSpecificReader):
         super().__init__(data_provider)
         self._entity = element
 
+    def get_own_reference(self) -> IlcdReference | None:
+        """Get the reference to this data set."""
+        return IlcdReference(entity_type="contacts", entity_id=self.get_uuid(), entity_version=self.get_version())
+
     def get_uuid(self) -> str:
         """Get the UUID of the entity described by this data set."""
         return none_throws(
             self._get_text(self._entity, ("contact:contactInformation", "contact:dataSetInformation", "common:UUID"))
         )
 
     def get_version(self) -> str | None:
@@ -100,24 +104,20 @@
 
     def get_address(self) -> str | None:
         """Get the address of the contact described by this data set."""
         return self._get_text(
             self._entity, ("contact:contactInformation", "contact:dataSetInformation", "contact:contactAddress")
         )
 
-    def to_openepd_org(self, lang: LangDef) -> Org:
+    def to_openepd_org(self, lang: LangDef, base_url: str | None = None) -> Org:
         """Convert this data set to an OpenEPD org object."""
         open_epd_contact = Contact.construct(
             email=self.get_email(),
             phone=cleanup_phone(self.get_phone()),
             website=self.get_website(),
         )
-        identification = ExternalIdentification.construct(
-            id=self.get_uuid(),
-            version=self.get_version(),
-        )
         return Org.construct(
             name=self.get_name(lang),
             web_domain=domain_from_url(self.get_website()),
             contacts=open_epd_contact if open_epd_contact.has_values() else None,
-            identified=create_openepd_identification(identification),
+            attachments=create_openepd_attachments(self.get_own_reference(), base_url),
         )
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/entity/flow.py` & `ilcdlib-0.3.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/entity/material.py` & `ilcdlib-0.3.0/src/ilcdlib/entity/material.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,28 +14,51 @@
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import dataclasses
+from enum import StrEnum
 from typing import IO, Literal
 
 from ilcdlib.xml_parser import T_ET, XmlParser
 
 
+class IlcdStandardMatProperties(StrEnum):
+    """Represent ILCD standard material properties."""
+
+    GrossDensity = "gross density"
+    BulkDensity = "bulk density"
+    LinearDensity = "linear density"
+    ConversionToKgFactor = "conversion factor to 1 kg"
+    Grammage = "grammage"
+    LayerThickness = "layer thickness"
+    Productiveness = "productiveness"
+
+
 @dataclasses.dataclass
 class MatMlMaterialProperty:
     """Represent MatML Material Property."""
 
     value: str | int | float | None
     data_format: Literal["float", "integer", "string", "exponential", "mixed"]
     unit: str | None = None
     internal_id: str | None = None
 
+    def to_unit_string(self) -> str | None:
+        """Get unit string."""
+        if self.value is not None and self.unit is not None:
+            return f"{self.value} {self.unit}"
+        if self.unit is None and self.value is not None:
+            return str(self.value)
+        if self.data_format == "string" and self.value is not None:
+            return str(self.value)
+        return None
+
 
 @dataclasses.dataclass
 class MatMlMaterial:
     """Represent MatML Material."""
 
     name: str
     properties: dict[str, MatMlMaterialProperty] = dataclasses.field(default_factory=dict)
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/entity/pcr.py` & `ilcdlib-0.3.0/src/ilcdlib/entity/pcr.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from typing import Type
 
-from openepd.model.common import ExternalIdentification
 from openepd.model.pcr import Pcr
 
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdPcrSupportReader
+from ilcdlib.dto import IlcdReference
 from ilcdlib.entity.contact import IlcdContactReader
 from ilcdlib.type import LangDef
-from ilcdlib.utils import create_openepd_identification, none_throws
+from ilcdlib.utils import create_openepd_attachments, none_throws
 from ilcdlib.xml_parser import T_ET
 
 
 class IlcdPcrReader(OpenEpdPcrSupportReader, IlcdXmlReader):
     """Read an ILCD PCR XML file."""
 
     def __init__(
@@ -39,14 +39,18 @@
         *,
         contact_reader_cls: Type[IlcdContactReader] = IlcdContactReader,
     ):
         super().__init__(data_provider)
         self.contact_reader_cls = contact_reader_cls
         self._entity = element
 
+    def get_own_reference(self) -> IlcdReference | None:
+        """Get the reference to this data set."""
+        return IlcdReference(entity_type="sources", entity_id=self.get_uuid(), entity_version=self.get_version())
+
     def get_uuid(self) -> str:
         """Get the UUID of the entity described by this data set."""
         return none_throws(
             self._get_text(self._entity, ("source:sourceInformation", "source:dataSetInformation", "common:UUID"))
         )
 
     def get_version(self) -> str | None:
@@ -70,20 +74,16 @@
                 "source:sourceInformation",
                 "source:dataSetInformation",
                 "source:referenceToContact",
             ),
         )
         return self.contact_reader_cls(element, self.data_provider) if element is not None else None
 
-    def to_openepd_pcr(self, lang: LangDef) -> Pcr:
+    def to_openepd_pcr(self, lang: LangDef, base_url: str | None = None) -> Pcr:
         """Read as OpenEPD Pcr object."""
-        identification = ExternalIdentification.construct(
-            id=self.get_uuid(),
-            version=self.get_version(),
-        )
         issuer_reader = self.get_reference_to_contact_reader()
         issuer = issuer_reader.to_openepd_org(lang) if issuer_reader is not None else None
         return Pcr.construct(
             name=self.get_name(lang),
             issuer=issuer,
-            identified=create_openepd_identification(identification),
+            attachments=create_openepd_attachments(self.get_own_reference(), base_url),
         )
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/entity/unit.py` & `ilcdlib-0.3.0/src/ilcdlib/entity/unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from dataclasses import dataclass
 
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader
+from ilcdlib.mapping.common import SimpleDataMapper
+from ilcdlib.mapping.units import default_units_uuid_mapper
 from ilcdlib.type import LangDef
 from ilcdlib.utils import none_throws
 from ilcdlib.xml_parser import T_ET
 
 
 @dataclass(kw_only=True)
 class UnitDto:
@@ -32,17 +34,24 @@
     name: str
     mean_value: float
 
 
 class IlcdUnitGroupReader(IlcdXmlReader):
     """Read an ILCD Unit Group XML file."""
 
-    def __init__(self, element: T_ET.Element, data_provider: BaseIlcdMediumSpecificReader):
+    def __init__(
+        self,
+        element: T_ET.Element,
+        data_provider: BaseIlcdMediumSpecificReader,
+        *,
+        unit_mapper: SimpleDataMapper[str] = default_units_uuid_mapper,
+    ):
         super().__init__(data_provider)
         self._entity = element
+        self.unit_mapper = unit_mapper
 
     def get_uuid(self) -> str:
         """Get the UUID of the entity described by this data set."""
         return none_throws(
             self._get_text(self._entity, ("ug:unitGroupInformation", "ug:dataSetInformation", "common:UUID"))
         )
 
@@ -61,29 +70,33 @@
 
     def get_ref_to_reference_unit(self) -> int | None:
         """Get the internal id of the reference flow property."""
         return self._get_int(
             self._entity, ("ug:unitGroupInformation", "ug:quantitativeReference", "ug:referenceToReferenceUnit")
         )
 
-    def get_reference_unit(
-        self,
-    ) -> UnitDto | None:
+    def get_reference_unit(self, allow_mapping: bool = True) -> UnitDto | None:
         """Get the reader for the reference flow property with the given id."""
         reference_unit_id = self.get_ref_to_reference_unit()
         if reference_unit_id is None:
             return None
         element = self._get_el(
             self._entity,
             (
                 "ug:units",
                 f"ug:unit[@dataSetInternalID='{reference_unit_id}']",
             ),
         )
+        if element is None:
+            return None
+        unit_name = none_throws(self._get_text(element, "ug:name"))
+        unit_uuid = self.get_uuid()
+        if allow_mapping and unit_uuid is not None:
+            unit_name = self.unit_mapper.map(unit_uuid, unit_name)
         return (
             UnitDto(
-                name=none_throws(self._get_text(element, "ug:name")),
+                name=unit_name,
                 mean_value=none_throws(self._get_float(element, "ug:meanValue")),
             )
             if element is not None
             else None
         )
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/epd/__init__.py` & `ilcdlib-0.3.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-0.3.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-0.3.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-0.3.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-0.3.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/epd/factory.py` & `ilcdlib-0.3.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/epd/reader.py` & `ilcdlib-0.3.0/src/ilcdlib/epd/reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,55 +14,59 @@
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import datetime
-from typing import Sequence, Type
+from typing import IO, Sequence, Type
 
-from openepd.model.common import Amount, ExternalIdentification
+from openepd.model.common import Amount
 from openepd.model.epd import Epd
+from openepd.model.lcia import ImpactSet
+from openepd.model.specs import Specs
 
+from ilcdlib import const
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdEdpSupportReader
 from ilcdlib.const import IlcdDatasetType
 from ilcdlib.dto import IlcdReference, ProductClassDef
 from ilcdlib.entity.contact import IlcdContactReader
 from ilcdlib.entity.flow import IlcdExchangeDto, IlcdFlowReader
+from ilcdlib.entity.lcia import IlcdLciaResultsReader
 from ilcdlib.entity.material import MatMlMaterial
 from ilcdlib.entity.pcr import IlcdPcrReader
 from ilcdlib.type import LangDef
-from ilcdlib.utils import create_openepd_identification, none_throws
+from ilcdlib.utils import create_ext, create_openepd_attachments, none_throws
 
 
 class IlcdEpdReader(OpenEpdEdpSupportReader, IlcdXmlReader):
     """Reader for ILCD+EPD datasets."""
 
     def __init__(
         self,
         epd_process_id: str | None,
         epd_version: str | None,
         data_provider: BaseIlcdMediumSpecificReader,
         *,
         contact_reader_cls: Type[IlcdContactReader] = IlcdContactReader,
         pcr_reader_cls: Type[IlcdPcrReader] = IlcdPcrReader,
         flow_reader_cls: Type[IlcdFlowReader] = IlcdFlowReader,
+        lcia_results_reader_cls: Type[IlcdLciaResultsReader] = IlcdLciaResultsReader,
     ):
         super().__init__(data_provider)
         self.contact_reader_cls = contact_reader_cls
         self.pcr_reader_cls = pcr_reader_cls
         self.flow_reader_cls = flow_reader_cls
+        self.lcia_results_reader_cls = lcia_results_reader_cls
         if epd_process_id is None:
             entities = data_provider.list_entities(IlcdDatasetType.Processes)
             self.__epd_entity_ref = entities[0]
         else:
             self.__epd_entity_ref = IlcdReference(IlcdDatasetType.Processes, epd_process_id, epd_version)
         self.epd_el_tree = self.get_xml_tree(*self.__epd_entity_ref, allow_static_datasets=False)
-        self.xml_parser.xml_ns["epd2013"] = "http://www.iai.kit.edu/EPD/2013"
-        self.xml_parser.xml_ns["epd2019"] = "http://www.iai.kit.edu/EPD/2019"
         self.post_init()
 
     def post_init(self):
         """
         Post-initialization actions, will be executed as a last step in constructor.
 
         It could be overriden by subclasses to perform additional initialization actions.
@@ -77,14 +81,18 @@
             ("process:processInformation", "process:dataSetInformation", "process:name", "process:baseName"),
         )
         for x in elements:
             if x.attrib and x.attrib.get(self._LANG_ATTRIB_NAME):
                 result.append(none_throws(x.attrib.get(self._LANG_ATTRIB_NAME)))
         return result
 
+    def get_own_reference(self) -> IlcdReference | None:
+        """Get the reference to this data set."""
+        return IlcdReference(entity_type="processes", entity_id=self.get_uuid(), entity_version=self.get_version())
+
     def get_uuid(self) -> str:
         """Get the UUID of the entity described by this data set."""
         return none_throws(
             self._get_text(
                 self.epd_el_tree, ("process:processInformation", "process:dataSetInformation", "common:UUID")
             )
         )
@@ -112,14 +120,26 @@
             self._get_text(
                 self.epd_el_tree,
                 ("process:modellingAndValidation", "process:LCIMethodAndAllocation", "common:other", "epd2013:subType"),
             )
             == "average dataset"
         )
 
+    def get_epd_document_stream(self) -> IO[bytes] | None:
+        """Extract the EPD document."""
+        return self._get_external_binary(
+            self.epd_el_tree,
+            (
+                "process:modellingAndValidation",
+                "process:dataSourcesTreatmentAndRepresentativeness",
+                "common:other",
+                "epd2019:referenceToOriginalEPD",
+            ),
+        )
+
     def get_product_name(self, lang: LangDef) -> str | None:
         """Return the product name in the given language."""
         return self._get_localized_text(
             self.epd_el_tree,
             ("process:processInformation", "process:dataSetInformation", "process:name", "process:baseName"),
             lang,
         )
@@ -318,55 +338,76 @@
     def get_program_operator_id(self) -> str | None:
         """Get document identifier assigned by program operator."""
         return self._get_text(
             self.epd_el_tree,
             ("process:administrativeInformation", "process:publicationAndOwnership", "common:registrationNumber"),
         )
 
-    def _product_classes_to_openepd_org(self, classes: dict[str, list[ProductClassDef]]) -> dict[str, str]:
+    def get_lcia_results_reader(self) -> IlcdLciaResultsReader | None:
+        """Return the LCIA results reader."""
+        element = self._get_el(
+            self.epd_el_tree,
+            ("process:LCIAResults",),
+        )
+        return self.lcia_results_reader_cls(element, self.data_provider) if element is not None else None
+
+    def get_lcia_results(self) -> ImpactSet | None:
+        """Return the LCIA results."""
+        reader = self.get_lcia_results_reader()
+        if reader is None:
+            return None
+        return reader.get_impacts()
+
+    def _product_classes_to_openepd(self, classes: dict[str, list[ProductClassDef]]) -> dict[str, str]:
         result: dict[str, str] = {}
         for classification_name, class_defs in classes.items():
             if classification_name.lower() == "oekobau.dat":
                 result["oekobau.dat"] = none_throws(class_defs[-1].id)
             elif classification_name.lower() == "ibucategories":
                 result["IBU"] = " >> ".join([none_throws(x.name) for x in class_defs])
+            if len(class_defs) > 0:
+                result[const.ILCD_IDENTIFICATION[0]] = (
+                    (class_defs[-1].id or "") + " " + " / ".join([none_throws(x.name) for x in class_defs])
+                ).strip()
         return result
 
-    def to_openepd_epd(self, lang: LangDef) -> Epd:
+    def to_openepd_epd(self, lang: LangDef, base_url: str | None = None) -> Epd:
         """Return the EPD as OpenEPD object."""
         lang_code = lang if isinstance(lang, str) else None
         if isinstance(lang, Sequence):
             lang_code = lang[0] if len(lang) > 0 else None
-        identification = ExternalIdentification.construct(
-            id=self.get_uuid(),
-            version=self.get_version(),
-        )
         manufacturer_reader = self.get_manufacturer_reader()
         manufacturer = manufacturer_reader.to_openepd_org(lang) if manufacturer_reader else None
         program_operator_reader = self.get_program_operator_reader()
         program_operator = program_operator_reader.to_openepd_org(lang) if program_operator_reader else None
         external_verifier_reader = self.get_external_verifier_reader()
         external_verifier = external_verifier_reader.to_openepd_org(lang) if external_verifier_reader else None
         pcr_reader = self.get_pcr_reader()
         pcr = pcr_reader.to_openepd_pcr(lang) if pcr_reader else None
         declared_unit = self.get_declared_unit()
         quantitative_props = self.get_quantitative_product_props_str(lang)
         product_name = self.get_product_name(lang)
         if product_name and quantitative_props:
             product_name += "; " + quantitative_props
-        # material_properties = self.get_material_properties()
+        material_properties = self.get_material_properties()
+        if material_properties:
+            specs = Specs(ext=create_ext({n: v.to_unit_string() for n, v in material_properties.properties.items()}))
+        else:
+            specs = Specs()
         return Epd.construct(
-            doctype="ILCD_EPD",
+            doctype="openEPD",
             language=lang_code,
-            identified=create_openepd_identification(identification),
+            attachments=create_openepd_attachments(self.get_own_reference(), base_url),
             name=product_name,
             description=self.get_product_description(lang),
             date_published=self.get_date_published(),
             valid_until=self.get_validity_ends_date(),
             program_operator_doc_id=self.get_program_operator_id(),
             manufacturer=manufacturer,
             program_operator=program_operator,
-            product_class=self._product_classes_to_openepd_org(self.get_product_classes()),
+            product_class=self._product_classes_to_openepd(self.get_product_classes()),
             third_party_verifier=external_verifier,
             pcr=pcr,
             declared_unit=declared_unit,
+            impacts=self.get_lcia_results(),
+            specs=specs,
         )
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/medium/__init__.py` & `ilcdlib-0.3.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/medium/archive.py` & `ilcdlib-0.3.0/src/ilcdlib/medium/archive.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         IlcdDatasetType.Processes: "processes",
         IlcdDatasetType.FlowProperty: "flowproperties",
     }
 
     def __init__(self, zip_file: PathLike | IO[bytes]):
         try:
             self._zip_file = ZipFile(zip_file, "r")
+            self._zip_file
         except Exception:
             raise ValueError("Could not open zip file. Please check if this is a valid zip file.")
         self.__ilcd_dir = ZipPath(self._zip_file) / "ILCD"
         if not self.__ilcd_dir.is_dir():
             raise ValueError("Could not find ILCD directory in the archive root. Is it really an ILCD archive?")
 
     @overload
@@ -154,7 +155,15 @@
     def close(self):
         """
         Close the reader and release any resources.
 
         This method is called automatically when used in a context manager.
         """
         self._zip_file.close()
+
+    def save_to(self, p: PathLike):
+        """Save underling the zip file to the given path."""
+        if self._zip_file.fp is None:
+            raise ValueError("Cannot save closed zip file.")
+        with open(p, "wb") as f:
+            self._zip_file.fp.seek(0)
+            f.write(self._zip_file.fp.read())
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-0.3.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/reference_data.py` & `ilcdlib-0.3.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-0.3.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-0.3.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-0.3.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/type.py` & `ilcdlib-0.3.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.2.2/src/ilcdlib/utils.py` & `ilcdlib-0.3.0/src/ilcdlib/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,30 +13,34 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import TypeVar
-
-from openepd.model.common import ExternalIdentification
+from typing import Any, TypeVar
 
 from ilcdlib import const
+from ilcdlib.dto import IlcdReference
 
 T = TypeVar("T")
 
 
 def none_throws(optional: T | None, message: str = "Unexpected `None`") -> T:
     """Convert an optional to its value. Raises an `AssertionError` if the value is `None`."""
     if optional is None:
         raise AssertionError(message)
     return optional
 
 
-def create_openepd_identification(
-    identification: ExternalIdentification | None,
-) -> dict[str, ExternalIdentification] | None:
-    """Create a dictionary of OpenEPD identification objects."""
-    if identification is None or not identification.has_values():
+def create_openepd_attachments(reference: IlcdReference | None, base_url: str | None = None) -> dict[str, str] | None:
+    """Create a dictionary of OpenEPD attachments."""
+    if reference is None:
+        return None
+    return {x: reference.to_url(base_url) for x in const.ILCD_IDENTIFICATION}
+
+
+def create_ext(data: Any) -> dict[str, Any] | None:
+    """Create a dictionary of OpenEPD ext field."""
+    if data is None:
         return None
-    return {x: identification for x in const.ILCD_IDENTIFICATION}
+    return {x: data for x in const.ILCD_IDENTIFICATION}
```

### Comparing `ilcdlib-0.2.2/src/ilcdlib/xml_parser.py` & `ilcdlib-0.3.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

