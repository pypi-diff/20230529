# Comparing `tmp/openepd-0.2.0.tar.gz` & `tmp/openepd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-0.2.0.tar", max compression
+gzip compressed data, was "openepd-0.3.0.tar", max compression
```

## Comparing `openepd-0.2.0.tar` & `openepd-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-05-26 15:18:34.913564 openepd-0.2.0/LICENSE
--rw-r--r--   0        0        0     2841 2023-05-26 15:18:34.913564 openepd-0.2.0/README.md
--rw-r--r--   0        0        0     3051 2023-05-26 15:18:34.913564 openepd-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     1987 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     2178 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/common.py
--rw-r--r--   0        0        0     5838 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0     9496 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3690 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     2855 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0        0 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/py.typed
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-29 12:59:31.650074 openepd-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2841 2023-05-29 12:59:31.650074 openepd-0.3.0/README.md
+-rw-r--r--   0        0        0     3051 2023-05-29 12:59:31.650074 openepd-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     2155 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     2178 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0     7763 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     8887 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     3690 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     2855 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0     1137 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3342 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0     1519 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:59:31.650074 openepd-0.3.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.3.0/PKG-INFO
```

### Comparing `openepd-0.2.0/LICENSE` & `openepd-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-0.2.0/README.md` & `openepd-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `openepd-0.2.0/pyproject.toml` & `openepd-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "0.2.0"
+version = "0.3.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
@@ -52,15 +52,15 @@
 types-deprecated = ">=1.2.9"
 
 [tool.poetry.extras]
 #xml = ["lxml"]
 
 
 [tool.commitizen]
-version = "0.2.0"
+version = "0.3.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/openepd/__version__.py",
 ]
```

### Comparing `openepd-0.2.0/src/openepd/__init__.py` & `openepd-0.3.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.2.0/src/openepd/__version__.py` & `openepd-0.3.0/src/openepd/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.2.0"
+VERSION = "0.3.0"
```

### Comparing `openepd-0.2.0/src/openepd/model/__init__.py` & `openepd-0.3.0/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.2.0/src/openepd/model/base.py` & `openepd-0.3.0/src/openepd/model/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,19 +22,21 @@
 
 AnySerializable = int | str | bool | float | list | dict | pydantic.BaseModel | None
 
 
 class BaseOpenEpdSchema(pydantic.BaseModel):
     """Base class for all OpenEPD models."""
 
-    extensions: dict[str, AnySerializable] | None = pydantic.Field(alias="ext", default=None)
+    ext: dict[str, AnySerializable] | None = pydantic.Field(alias="ext", default=None)
 
     class Config:
         allow_mutation = True
         validate_assignment = False
+        allow_population_by_field_name = True
+        use_enum_values = True
 
     def has_values(self) -> bool:
         """Return True if the model has any values."""
         return len(self.dict(exclude_unset=True, exclude_none=True)) > 0
 
     @classmethod
     def is_allowed_field_name(cls, field_name: str) -> bool:
@@ -52,7 +54,13 @@
         return False
 
 
 class BaseOpenEpdGenericSchema(GenericModel, BaseOpenEpdSchema):
     """Base class for all OpenEPD generic models."""
 
     pass
+
+
+class BaseOpenEpdSpec(BaseOpenEpdSchema):
+    """Base class for all OpenEPD specs."""
+
+    pass
```

### Comparing `openepd-0.2.0/src/openepd/model/common.py` & `openepd-0.3.0/src/openepd/model/common.py`

 * *Files identical despite different names*

### Comparing `openepd-0.2.0/src/openepd/model/epd.py` & `openepd-0.3.0/src/openepd/model/epd.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 import datetime
 from typing import Literal
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import Amount
-from openepd.model.lcia import ImpactSet, OutputFlowSet, ResourceUseSet, Standard
+from openepd.model.lcia import ImpactSet, OutputFlowSet, ResourceUseSet
 from openepd.model.org import Org, Plant
+from openepd.model.specs import Specs
+from openepd.model.standard import Standard
 
 
 class Epd(BaseOpenEpdSchema):
     """Represent an EPD."""
 
     # TODO: Add validator for open-xpd-uuid on this field
     id: str = pyd.Field(
@@ -119,7 +121,38 @@
     output_flows: OutputFlowSet | None = pyd.Field(
         description="Set of Waste and Output Flow indicators which describe the waste categories "
         "and other material output flows derived from the LCI."
     )
     compliance: list[Standard] = pyd.Field(
         description="Standard(s) to which this declaration is compliant.", default_factory=list
     )
+    specs: Specs = pyd.Field(
+        default_factory=Specs,
+        description="Data structure(s) describing performance specs of product. Unique for each material type.",
+    )
+    lca_discussion: str | None = pyd.Field(
+        max_length=20000,
+        description="""A rich text description containing information for experts reviewing the EPD contents. 
+    Text descriptions required by ISO 14025, ISO 21930, EN 15804,, relevant PCRs, or program instructions and which do not 
+    have specific openEPD fields should be entered here.  This field may be large, and may contain multiple sections 
+    separated by github flavored markdown formatting.""",
+        example="""# Packaging
+
+    Information on product-specific packaging: type, composition and possible reuse of packaging materials (paper, 
+    strapping, pallets, foils, drums, etc.) shall be included in this Section. The EPD shall describe specific packaging 
+    scenario assumptions, including disposition pathways for each packaging material by reuse, recycling, or landfill 
+    disposal based on packaging type.*
+
+    # Product Installation
+
+    A description of the type of processing, machinery, tools, dust extraction equipment, auxiliary materials, etc. 
+    to be used during installation shall be included. Information on industrial and environmental protection may be 
+    included in this section. Any waste treatment included within the system boundary of installation waste should be 
+    specified.
+
+    # Use Conditions
+
+    Use-stage environmental impacts of flooring products during building operations depend on product cleaning assumptions. 
+    Information on cleaning frequency and cleaning products shall be provided based on the manufacturer’s recommendations. 
+    In the absence of primary data, cleaning assumptions shall be documented.
+    """,
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openepd-0.2.0/src/openepd/model/lcia.py` & `openepd-0.3.0/src/openepd/model/lcia.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import Measurement
-from openepd.model.org import Org
 
 
 class EolScenario(BaseOpenEpdSchema):
     """
     A scenario for end-of-life.
 
     If a particular implementation commits to a specific scenario, then that value can be used;
@@ -164,18 +163,7 @@
     )
 
 
 class OutputFlowSet(BaseOpenEpdSchema):
     """A set of output flows, such as waste, emissions, etc."""
 
     hwd: ScopeSet | None = pyd.Field(description="Hazardous waste disposed")
-
-
-class Standard(BaseOpenEpdSchema):
-    """A standard, such as EN 15804, ISO 14044, ISO 14024:2018, etc."""
-
-    short_name: str = pyd.Field(description="Short-form of name of standard.  Must be unique. Case-insensitive")
-    name: str | None = pyd.Field(description="Full document name.  Must be unique. Case-insensitive", default=None)
-    link: pyd.AnyUrl | None = pyd.Field(
-        description="Link to the exact standard (including version) referred to", default=None
-    )
-    issuer: Org | None = pyd.Field(description="Org that issued this standard", default=None)
```

### Comparing `openepd-0.2.0/src/openepd/model/org.py` & `openepd-0.3.0/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-0.2.0/src/openepd/model/pcr.py` & `openepd-0.3.0/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-0.2.0/PKG-INFO` & `openepd-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 0.2.0 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 0.3.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: support@c-change-labs.com
 Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

