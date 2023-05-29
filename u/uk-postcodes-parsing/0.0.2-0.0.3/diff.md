# Comparing `tmp/uk_postcodes_parsing-0.0.2.tar.gz` & `tmp/uk_postcodes_parsing-0.0.3.tar.gz`

## Comparing `uk_postcodes_parsing-0.0.2.tar` & `uk_postcodes_parsing-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/__init__.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/fix.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/postcode_utils.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/ukpostcode.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/tests/tests.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/LICENSE
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/__init__.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/fix.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/postcode_utils.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/ukpostcode.py
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/tests/test_all.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/tests/data/postcode_parse_test.csv
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/README.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/PKG-INFO
```

### Comparing `uk_postcodes_parsing-0.0.2/.github/workflows/python-publish.yml` & `uk_postcodes_parsing-0.0.3/.github/workflows/python-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,15 @@
   workflow_dispatch:
 
 permissions:
   contents: read
 
 jobs:
   deploy:
-
     runs-on: ubuntu-latest
-
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
     - name: Install dependencies
```

### Comparing `uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/fix.py` & `uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/fix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 import re
 
-FIXABLE_REGEX = re.compile(r"^\s*[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}\s*$", re.I)
+FIXABLE_REGEX = re.compile(
+    r"^\s*[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}\s*$", re.I
+)
+
 
 def fix(s: str) -> str:
     match = FIXABLE_REGEX.match(s)
     if match is None:
         return s
     s = s.upper().strip().replace(r"\s+", "")
     inward = s[-3:].strip()
     outward = s[:-3].strip()
     return f"{coerce_outcode(outward)} {coerce_incode(inward)}"
 
+
 def to_letter(c: str) -> str:
     return {
         "0": "O",
         "1": "I",
     }.get(c, c)
 
+
 def to_number(c: str) -> str:
     return {
         "O": "0",
         "I": "1",
     }.get(c, c)
 
 
 def coerce(pattern: str, input: str) -> str:
     """
-    Coerce a given input into a pattern. For e.g. 
+    Coerce a given input into a pattern. For e.g.
             pattern: "LN" => signifies a letter followed by a number
-            input: "01" => changes to "O1". Where the first 0 should be a letter so it 
+            input: "01" => changes to "O1". Where the first 0 should be a letter so it
                 is coverted from 0 to O. The Second 1 is already correct so no change.
     """
     return "".join(
-            to_number(c) if target == "N" else to_letter(c) if target == "L" else c
-            for c, target in zip(input, pattern)
+        to_number(c) if target == "N" else to_letter(c) if target == "L" else c
+        for c, target in zip(input, pattern)
     )
 
+
 def coerce_outcode(i: str) -> str:
     """Coerce outcode based on length of outcode"""
     if len(i) == 2:
         return coerce("LN", i)
     elif len(i) == 3:
         return coerce("L??", i)
     elif len(i) == 4:
         return coerce("LLN?", i)
     else:
         return i
 
-def coerce_incode(i :str) -> str:
+
+def coerce_incode(i: str) -> str:
     """Coerce incode"""
-    return coerce('NLL', i)
+    return coerce("NLL", i)
```

### Comparing `uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/postcode_utils.py` & `uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/postcode_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,91 @@
 import re
 from typing import Union
 
-# Tests for district 
-DISTRICT_SPLIT_REGEX = re.compile(r'^([a-z]{1,2}\d)([a-z])$', re.I)
+# Tests for district
+DISTRICT_SPLIT_REGEX = re.compile(r"^([a-z]{1,2}\d)([a-z])$", re.I)
 
 # Tests for the unit section of a postcode
-UNIT_REGEX = re.compile(r'[a-z]{2}$', re.I)
+UNIT_REGEX = re.compile(r"[a-z]{2}$", re.I)
 
 # Tests for the inward code section of a postcode
-INCODE_REGEX = re.compile(r'\d[a-z]{2}$', re.I)
+INCODE_REGEX = re.compile(r"\d[a-z]{2}$", re.I)
 
 # Tests for the outward code section of a postcode
-OUTCODE_REGEX = re.compile(r'^[a-z]{1,2}\d[a-z\d]?$', re.I)
+OUTCODE_REGEX = re.compile(r"^[a-z]{1,2}\d[a-z\d]?$", re.I)
 
 # Tests for a valid postcode
-POSTCODE_REGEX = re.compile(r'^[a-z]{1,2}\d[a-z\d]?\s*\d[a-z]{2}$', re.I)
+POSTCODE_REGEX = re.compile(r"^[a-z]{1,2}\d[a-z\d]?\s*\d[a-z]{2}$", re.I)
 
 # Tests for the area section of a postcode
-AREA_REGEX = re.compile(r'^[a-z]{1,2}', re.I)
+AREA_REGEX = re.compile(r"^[a-z]{1,2}", re.I)
+
 
 def sanitize(s: str) -> str:
-    return s.replace(' ', '').upper()
+    return s.replace(" ", "").upper()
+
 
 def is_valid(postcode: str) -> bool:
     return re.match(POSTCODE_REGEX, postcode) is not None
 
+
 def is_valid_outcode(outcode: str) -> bool:
     return re.match(OUTCODE_REGEX, outcode) is not None
 
+
 def to_normalised(postcode: str) -> Union[str, None]:
     outcode = to_outcode(postcode)
     if outcode is None:
         return None
     incode = to_incode(postcode)
-    return None if incode is None else f'{outcode} {incode}'
+    return None if incode is None else f"{outcode} {incode}"
+
 
 def to_outcode(postcode: str) -> Union[str, None]:
     if not is_valid(postcode):
         return None
-    return re.sub(INCODE_REGEX, '', sanitize(postcode))
+    return re.sub(INCODE_REGEX, "", sanitize(postcode))
+
 
 def to_incode(postcode: str) -> Union[str, None]:
     if not is_valid(postcode):
         return
     incode = re.findall(INCODE_REGEX, sanitize(postcode))
     return incode[0] if incode else None
 
+
 def to_area(postcode: str) -> Union[str, None]:
     if not is_valid(postcode):
         return None
     area = re.findall(AREA_REGEX, sanitize(postcode))
     return area[0] if area else None
 
+
 def to_sector(postcode: str) -> Union[str, None]:
     outcode = to_outcode(postcode)
     if outcode is None:
         return None
     incode = to_incode(postcode)
-    return None if incode is None else f'{outcode} {incode[0]}'
+    return None if incode is None else f"{outcode} {incode[0]}"
+
 
 def to_unit(postcode: str) -> Union[str, None]:
     if not is_valid(postcode):
         return None
     unit = re.findall(UNIT_REGEX, sanitize(postcode))
     return unit[0] if unit else None
 
+
 def to_district(postcode):
     outcode = to_outcode(postcode)
     if outcode is None:
         return None
     district = re.match(DISTRICT_SPLIT_REGEX, outcode)
     return district[1] if district else outcode
 
+
 def to_sub_district(postcode):
     outcode = to_outcode(postcode)
     if outcode is None:
         return None
     split = re.match(DISTRICT_SPLIT_REGEX, outcode)
-    return None if split is None else outcode
+    return None if split is None else outcode
```

### Comparing `uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/ukpostcode.py` & `uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/ukpostcode.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,58 +3,64 @@
 from dataclasses import dataclass
 from typing import Union, List
 
 from uk_postcodes_parsing.postcode_utils import *
 from uk_postcodes_parsing.fix import fix
 
 logging.basicConfig(level=logging.DEBUG)
-logger = logging.getLogger('uk-postcodes-parsing')
+logger = logging.getLogger("uk-postcodes-parsing")
 
 # Test for a valid postcode embedded in text
-POSTCODE_CORPUS_REGEX = re.compile(r'[a-z]{1,2}\d[a-z\d]?\s*\d[a-z]{2}', re.I)
-FIXABLE_POSTCODE_CORPUS_REGEX = re.compile("[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}")
+POSTCODE_CORPUS_REGEX = re.compile(r"[a-z]{1,2}\d[a-z\d]?\s*\d[a-z]{2}", re.I)
+FIXABLE_POSTCODE_CORPUS_REGEX = re.compile(
+    r"[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}"
+)
+
 
 def _parse(postcode: str) -> dict:
     if not is_valid(postcode):
         return None
     return {
-        "postcode":  to_normalised(postcode),
-        "incode":  to_incode(postcode),
-        "outcode" :  to_outcode(postcode),
-        "area":  to_area(postcode),
-        "district":  to_district(postcode),
-        "sub_district":  to_sub_district(postcode),
-        "sector":  to_sector(postcode),
-        "unit":  to_unit(postcode),
+        "postcode": to_normalised(postcode),
+        "incode": to_incode(postcode),
+        "outcode": to_outcode(postcode),
+        "area": to_area(postcode),
+        "district": to_district(postcode),
+        "sub_district": to_sub_district(postcode),
+        "sector": to_sector(postcode),
+        "unit": to_unit(postcode),
     }
 
+
 def parse(postcode, attempt_fix=True):
     if is_valid(postcode):
         return Postcode(**_parse(postcode), original=postcode)
     if attempt_fix:
         fixed = fix(postcode)
         if is_valid(fixed):
             logger.info("Postcode Fixed: '%s' => '%s'", postcode, fixed)
             return Postcode(**_parse(fixed), original=postcode)
         logger.error("Unable to fix postcode")
     logger.error("Failed to parse postcode")
     return None
 
+
 def parse_from_corpus(text: str, attempt_fix=False) -> List[str]:
     if attempt_fix:
-         postcodes = re.findall(FIXABLE_POSTCODE_CORPUS_REGEX, text)
+        postcodes = re.findall(FIXABLE_POSTCODE_CORPUS_REGEX, text)
     else:
         postcodes = re.findall(POSTCODE_CORPUS_REGEX, text)
     logger.info("Found %d postcodes in corpus", len(postcodes))
     return list(map(parse, postcodes))
 
+
 @dataclass
-class Postcode():
+class Postcode:
     original: str
     postcode: str
     incode: str
     outcode: str
     area: str
     district: str
-    sub_district: Union[str,None]
+    sub_district: Union[str, None]
     sector: str
-    unit: str
+    unit: str
```

### Comparing `uk_postcodes_parsing-0.0.2/.gitignore` & `uk_postcodes_parsing-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.2/LICENSE` & `uk_postcodes_parsing-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.2/PKG-INFO` & `uk_postcodes_parsing-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-Metadata-Version: 2.1
-Name: uk_postcodes_parsing
-Version: 0.0.2
-Summary: A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP.
-Project-URL: Homepage, https://github.com/anirudhgangwal/ukpostcodes
-Project-URL: Bug Tracker, https://github.com/anirudhgangwal/ukpostcodes/issues
-Author-email: Anirudh Gangwal <angangwa@amazon.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # uk-postcodes-parsing
 
+[![Test](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/test.yml/badge.svg)](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/test.yml) 
+[![Upload Python Package](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/python-publish.yml/badge.svg)](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/python-publish.yml)
+
 A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP.
 
 Install:
 
 ```bash
 pip install uk-postcodes-parsing
 ``` 
 
 ## Usage
 
 - Parsing text to get a list of postcodes.
 
 ```python
->>> from uk_postcodes_parsing.ukpostcode import parse_from_corpus, Postcode
+>>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
->>> postcodes = parse_from_corpus(corpus)
+>>> postcodes = ukpostcode.parse_from_corpus(corpus)
 INFO:uk-postcodes-parsing:Found 2 postcodes in corpus
 >>> print(postcodes)
 [Postcode(original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'), Postcode(original='e34ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS')]
 ```
 
 - Optional auto-correct: Attempt correcting common mistakes in postcodes such as reading "O" and "0" and vice-versa.
 
 ```python
->>> from uk_postcodes_parsing.ukpostcode import parse_from_corpus, Postcode
+>>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
->>> postcodes = parse_from_corpus(corpus, attempt_fix=True)
+>>> postcodes = ukpostcode.parse_from_corpus(corpus, attempt_fix=True)
 INFO:uk-postcodes-parsing:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
 INFO:uk-postcodes-parsing:Found 3 postcodes in corpus
 ```
 
 - Parsing
 
 ```python
->>> parse("EC1r 1ub")
+>>> from uk_postcodes_parsing import ukpostcode
+>>> ukpostcode.parse("EC1r 1ub")
 Postcode(original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
->>> parse("EH16 50Y", attempt_fix=True)
+>>> ukpostcode.parse("EH16 50Y", attempt_fix=True)
 INFO:ukpostcode:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
 Postcode(original='eh16 50y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')
+>>> ukpostcode.parse("0W1") 
+ERROR:ukpostcode:Unable to fix postcode
+ERROR:ukpostcode:Failed to parse postcode
+```
+
+- Validity check
+
+```python
+>>> from uk_postcodes_parsing import postcode_utils
+>>> postcode_utils.is_valid("0W1 0AA")
+False
+>>> postcode_utils.is_valid("OW1 0AA")
+True
 ```
 
 - Fixing
 
 ```python
 >>> from uk_postcodes_parsing.fix import fix
 >>> fix("0W1 OAA") 
-OW1 0AA
+'OW1 0AA'
 ```
```

