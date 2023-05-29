# Comparing `tmp/ietf_reviewtool-0.2.3.tar.gz` & `tmp/ietf_reviewtool-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ietf_reviewtool-0.2.3.tar", max compression
+gzip compressed data, was "ietf_reviewtool-0.3.0.tar", max compression
```

## Comparing `ietf_reviewtool-0.2.3.tar` & `ietf_reviewtool-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0    18092 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/LICENSE
--rw-r--r--   0        0        0     6700 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/README.md
--rw-r--r--   0        0        0      285 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/__init__.py
--rw-r--r--   0        0        0      146 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/__main__.py
--rw-r--r--   0        0        0     1183 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/agenda.py
--rw-r--r--   0        0        0    13722 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/boilerplate.py
--rw-r--r--   0        0        0     5715 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/doc.py
--rw-r--r--   0        0        0     3797 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/grammar.py
--rwxr-xr-x   0        0        0    25872 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/ietf_reviewtool.py
--rw-r--r--   0        0        0     2527 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/inclusive.py
--rw-r--r--   0        0        0     4532 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/metadata.py
--rw-r--r--   0        0        0    10010 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/references.py
--rw-r--r--   0        0        0    10872 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/review.py
--rw-r--r--   0        0        0        0 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/util/__init__.py
--rw-r--r--   0        0        0     2951 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/util/docposition.py
--rw-r--r--   0        0        0    11249 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/util/fetch.py
--rw-r--r--   0        0        0     2936 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/util/format.py
--rw-r--r--   0        0        0     8636 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/util/text.py
--rw-r--r--   0        0        0     2033 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/ietf_reviewtool/util/utils.py
--rw-r--r--   0        0        0     1124 2022-10-26 11:03:02.519527 ietf_reviewtool-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     8010 1970-01-01 00:00:00.000000 ietf_reviewtool-0.2.3/setup.py
--rw-r--r--   0        0        0     7848 1970-01-01 00:00:00.000000 ietf_reviewtool-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6700 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/README.md
+-rw-r--r--   0        0        0      285 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/__init__.py
+-rw-r--r--   0        0        0      146 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/__main__.py
+-rw-r--r--   0        0        0     1183 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/agenda.py
+-rw-r--r--   0        0        0    14217 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/boilerplate.py
+-rw-r--r--   0        0        0     5144 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/doc.py
+-rw-r--r--   0        0        0     4181 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/grammar.py
+-rwxr-xr-x   0        0        0    30018 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/ietf_reviewtool.py
+-rw-r--r--   0        0        0     2527 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/inclusive.py
+-rw-r--r--   0        0        0     4829 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/metadata.py
+-rw-r--r--   0        0        0    10926 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/references.py
+-rw-r--r--   0        0        0    10872 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/review.py
+-rw-r--r--   0        0        0        0 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/__init__.py
+-rw-r--r--   0        0        0     2970 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/docposition.py
+-rw-r--r--   0        0        0    11456 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/fetch.py
+-rw-r--r--   0        0        0     2936 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/format.py
+-rw-r--r--   0        0        0    10522 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/text.py
+-rw-r--r--   0        0        0     2033 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/utils.py
+-rw-r--r--   0        0        0     1376 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7698 1970-01-01 00:00:00.000000 ietf_reviewtool-0.3.0/PKG-INFO
```

### Comparing `ietf_reviewtool-0.2.3/LICENSE` & `ietf_reviewtool-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.2.3/README.md` & `ietf_reviewtool-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/agenda.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/agenda.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/boilerplate.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/boilerplate.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,28 +46,38 @@
     Check the RFC2119/RFC8174 boilerplate in the document.
 
     @param      doc     The document
     @param      review  The IETF Review document to add comments to
 
     @return     { description_of_the_return_value }
     """
-    uses_keywords = set(re.findall(KEYWORDS_PATTERN, doc.orig))
     has_8174_boilerplate = set(re.findall(BOILERPLATE_8174_PATTERN, doc.orig))
     has_2119_boilerplate = set(re.findall(BOILERPLATE_2119_PATTERN, doc.orig))
     has_boilerplate_begin = set(re.findall(BOILERPLATE_BEGIN_PATTERN, doc.orig))
 
+    doc_minus_boilerplate = re.sub(BOILERPLATE_8174_PATTERN, "", doc.orig)
+    doc_minus_boilerplate = re.sub(BOILERPLATE_2119_PATTERN, "", doc_minus_boilerplate)
+    doc_minus_boilerplate = re.sub(BOILERPLATE_2119_PATTERN, "", doc_minus_boilerplate)
+    uses_keywords = set(re.findall(KEYWORDS_PATTERN, doc_minus_boilerplate))
+
     msg = None
     if uses_keywords:
         used_keywords = []
         for word in set(uses_keywords):
             used_keywords.append(normalize_ws(word))
         used_keywords_str = word_join(used_keywords, prefix='"', suffix='"')
         kw_text = f"keyword{'s' if len(uses_keywords) > 1 else ''}"
 
-        if doc.status.lower() in ["informational", "experimental"]:
+        if doc.status.lower() == "unknown":
+            review.comment(
+                "Boilerplate",
+                "Document boilerplate does not seem to indicate the intended "
+                "RFC status.",
+            )
+        elif doc.status.lower() in ["informational", "experimental"]:
             review.comment(
                 "Boilerplate",
                 f"Document has {doc.status} status, but uses the RFC2119 "
                 f"{kw_text} {used_keywords_str}. Check if this is really "
                 f"necessary?",
             )
 
@@ -78,15 +88,15 @@
             )
             if has_2119_boilerplate:
                 msg += " (It contains a variant of the RFC2119 boilerplate.)"
             elif has_boilerplate_begin:
                 msg += " (It contains some text with a similar beginning.)"
     else:
         if has_8174_boilerplate or has_2119_boilerplate or has_boilerplate_begin:
-            msg = "This document does not use RFC2119 keywords, but contains"
+            msg = "This document does not use RFC2119 keywords, but contains "
             if has_8174_boilerplate:
                 msg += "the RFC8174 boilerplate."
             elif has_2119_boilerplate:
                 msg += "the RFC2119 boilerplate."
             elif has_boilerplate_begin:
                 msg += "text with a beginning similar to the RFC2119 boilerplate."
```

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/doc.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/doc.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import os
 import re
 import tempfile
 
 from .util.docposition import SECTION_PATTERN
 from .util.fetch import get_items, fetch_meta
-from .util.text import basename, revision, unfold, untag, extract_urls
+from .util.text import basename, revision, unfold, untag, extract_urls, doc_parts
 from .util.utils import read
 
 
 class Doc:
     "Class to handle a document to review."
     name: str
     status: str
@@ -58,15 +58,15 @@
 
         # set status
         status = re.search(
             r"^(?:[Ii]ntended )?[Ss]tatus:\s*((?:\w+\s)+)",
             self.orig,
             re.MULTILINE,
         )
-        self.status = status.group(1).strip() if status else ""
+        self.status = status.group(1).strip() if status else "unknown"
 
         # extract relationships
         self.relationships = {}
         rel_pat = {"updates": r"[Uu]pdates", "obsoletes": r"[Oo]bsoletes"}
         for rel in ["updates", "obsoletes"]:
             match = re.search(
                 r"^"
@@ -96,66 +96,49 @@
             if in_abstract:
                 abstract += line
         self.abstract = unfold(abstract).strip()
 
         self.meta = fetch_meta(datatracker, self.name, log)
         self.is_id = self.name.startswith("draft-")
 
-        parts = {"text": "", "informative": "", "normative": ""}
-        part = "text"
-        for line in self.orig_lines:
-            pot_sec = SECTION_PATTERN.search(line)
-            if pot_sec:
-                which = pot_sec.group(0)
-                if re.search(
-                    r"^(?:(\d\.?)+\s+)?(?:Non-Norm|Inform)(?:ative|ational)\s+References?\s*$",
-                    which,
-                    flags=re.IGNORECASE,
-                ):
-                    part = "informative"
-                elif re.search(
-                    r"^(?:(\d\.?)+\s+)?(Normative\s+)?References?\s*$",
-                    which,
-                    flags=re.IGNORECASE,
-                ):
-                    part = "normative"
-                else:
-                    part = "text"
-            parts[part] += line
-
+        parts = doc_parts(self.orig)
         refs = {}
         for part, content in parts.items():
             refs[part] = re.findall(
                 r"(\[(?:\d+|[a-z]+(?:[-_.]?\w+)*)\]"
-                + (r"|RFC\d+|draft-[-a-z\d_.]+" if part == "text" else r"")
+                + (r"|\bRFC\d+\b|\bdraft-[-a-z\d_.]+\b" if part == "text" else r"")
                 + r")",
                 unfold(content),
                 flags=re.IGNORECASE,
             )
             refs[part] = list({f"[{untag(ref)}]" for ref in refs[part]})
 
         self.references = {}
         for part in ["informative", "normative"]:
             self.references[part] = []
             for ref in refs[part]:
                 ref_match = re.search(
-                    r"\s*" + re.escape(ref) + r"\s+((?:[^\n][\n]?)+)\n",
+                    r"\s*" + re.escape(ref) + r"([^\[]*)",
                     parts[part],
                     re.DOTALL,
                 )
                 if ref_match:
                     ref_text = unfold(ref_match.group(0))
-                    found = False
-
-                    for pat in [r"(draft-[-a-z\d_.]+)", r"((?:RFC|rfc)\d+)"]:
-                        match = re.search(pat, ref_text)
+                    # remove the quoted title, to avoid matching in there
+                    ref_text = re.sub(r'"[^"]*"', "", ref_text)
+                    targets = set()
+
+                    for match in re.finditer(
+                        r"\b(draft-[-a-z\d_.]+|(?:RFC|rfc)\s*\d+)\b",
+                        ref_text,
+                        re.DOTALL,
+                    ):
                         if match:
-                            found = True
-                            self.references[part].append((ref, match.group(0).lower()))
-                            break
+                            target = re.sub(r"\s+", "", match.group(0).lower())
+                            targets.add(target)
 
-                    if not found:
+                    if targets:
+                        self.references[part].append((ref, targets))
+                    else:
                         urls = extract_urls(ref_text, log, True, True)
-                        self.references[part].append(
-                            (ref, urls.pop() if urls else None)
-                        )
+                        self.references[part].append((ref, urls))
         self.references["text"] = refs["text"]
```

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/grammar.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/grammar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """ietf-reviewtool grammr module"""
 
 import math
 import re
+import requests_cache
 
 import language_tool_python  # type: ignore
 
 from .review import IetfReview
 from .util.docposition import DocPosition
 from .util.text import unfold, wrap_para
+from .util.fetch import fetch_init_cache
 
 
 def check_grammar(
     text: list,
     grammar_skip_rules: str,
     review: IetfReview,
     width: int,
@@ -23,51 +25,62 @@
     @param      text                The document text (as lines)
     @param      grammar_skip_rules  The grammar rules to skip
     @param      review              The IETF review to comment upon
     @param      show_rule_id        Whether to show rule names in messages
 
     @return     { description_of_the_return_value }
     """
+    # the languagetool auto-download seems to fail if the cache is enabled
+    requests_cache.uninstall_cache()
+    lt = language_tool_python.LanguageTool("en-US")
+    fetch_init_cache()
+
     issues = [
         i
-        for i in language_tool_python.LanguageTool("en-US").check(unfold("".join(text)))
+        for i in lt.check(unfold("".join(text)))
         if i.ruleId
         not in [
             "ADVERTISEMENT_OF_FOR",
             "ALL_OF_THE",
             "ARROWS",
             "BOTH_AS_WELL_AS",
+            "COMMA_COMPOUND_SENTENCE_2",
             "COMMA_COMPOUND_SENTENCE",
             "COMMA_PARENTHESIS_WHITESPACE",
             "COPYRIGHT",
             "CURRENCY",
             "DASH_RULE",
             "DATE_FUTURE_VERB_PAST",
             "DATE_NEW_YEAR",
+            "DOUBLE_PUNCTUATION",
             "EN_QUOTES",
             "EN_UNPAIRED_BRACKETS",
             "ENGLISH_WORD_REPEAT_BEGINNING_RULE",
             "HYPOTHESIS_TYPOGRAPHY",
             "I_LOWERCASE",
             "IN_THE_INTERNET",
             "INCORRECT_POSSESSIVE_FORM_AFTER_A_NUMBER",
             "KEY_WORDS",
             "LARGE_NUMBER_OF",
             "MORFOLOGIK_RULE_EN_US",
             "MULTIPLICATION_SIGN",
             "NUMBERS_IN_WORDS",
+            "OUTSIDE_OF",
             "PLUS_MINUS",
             "PUNCTUATION_PARAGRAPH_END",
+            "R_SYMBOL",
             "RETURN_IN_THE",
             "SENTENCE_WHITESPACE",
             "SO_AS_TO",
             "SOME_OF_THE",
+            "TRADEMARK",
             "UNIT_SPACE",
             "UNLIKELY_OPENING_PUNCTUATION",
             "UPPERCASE_SENTENCE_START",
+            "WHETHER",
             "WHITESPACE_RULE",
             "WORD_CONTAINS_UNDERSCORE",
         ]
         and (not grammar_skip_rules or i.ruleId not in grammar_skip_rules.split(","))
     ]
     issues = [i for i in issues if not i.ruleId.startswith("EN_REPEATEDWORDS_")]
```

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/ietf_reviewtool.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/ietf_reviewtool.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 SPDX-License-Identifier: GPL-2.0
 """
 
 import difflib
 import html
 import ipaddress
 import json
+import json5  # type: ignore
 import logging
 import os
 import re
 import xml.etree.ElementTree
 
 from typing import Union
 
@@ -45,14 +46,17 @@
 
 from .util.fetch import fetch_url, fetch_dt, get_items
 from .util.text import (
     word_join,
     extract_ips,
     extract_urls,
     strip_pagination,
+    unfold,
+    undo_rfc8792,
+    doc_parts,
 )
 from .util.utils import read, write
 
 
 log = logging.getLogger(__name__)
 
 
@@ -143,28 +147,33 @@
     """
     Extract URLs from items.
 
     @param      items     The items to extract URLs from.
     @param      examples  Include "example" URLs (e.g., to example.com, etc.)
     @param      common    Include "common" URLs (e.g., to rfc-editor.org)
     """
-    urls = set()
+    urls: dict[str, set] = {}
     for item in items:
         if not os.path.isfile(item):
             log.warning("%s does not exist, skipping", item)
             continue
 
         log.debug("Extracting URLs from %s", item)
         text = strip_pagination(read(item, log))
 
         if text:
-            urls |= extract_urls(read(item, log), log, examples, common)
-
-    for url in urls:
-        print(url)
+            item_urls = extract_urls(read(item, log), log, examples, common)
+            for part, part_urls in item_urls.items():
+                if part not in urls:
+                    urls[part] = set()
+                urls[part] |= item_urls[part]
+
+    for part, part_urls in urls.items():
+        for url in part_urls:
+            print(url, part)
 
 
 @click.command("fetch", help="Download items (I-Ds, charters, RFCs, etc.)")
 @click.argument("items", nargs=-1)
 @click.option(
     "--strip/--no-strip",
     "strip",
@@ -327,15 +336,15 @@
 
         if not group:
             log.warning("Could not fetch ART for %s", doc.name)
             continue
 
         if art_review["id"] in thanked:
             log.warning(
-                "Already thanked %s for %s review", reviewer["name"], group["name"]
+                "Already recorded %s for %s review", reviewer["name"], group["name"]
             )
             continue
 
         if group["acronym"].lower() == thank_art.lower():
             # remember we thanked for this
             thanked.add(art_review["id"])
 
@@ -465,15 +474,17 @@
     @param      doc      The document text
     @param      review   IETF Review object
     @param      verbose  Whether to be verbose during the checks
 
     @return     None
     """
     result = []
-    urls = extract_urls(doc.orig, log)
+    urls = set()
+    for part, part_urls in extract_urls(doc.orig, log).items():
+        urls |= part_urls
 
     for url in urls:
         if re.search(r"tools\.ietf\.org", url, flags=re.IGNORECASE):
             result.append(url)
 
     if result:
         review.nit_bullets(
@@ -515,48 +526,163 @@
         review.nit_bullets(
             "URLs",
             "These URLs in the document can probably be converted to HTTPS:",
             result,
         )
 
 
+def check_expert_review(doc: Doc, review: IetfReview) -> None:
+    """
+    Check whether the document mentions "Expert Review" or "Specification Required" and
+    add a note to check whether this IANA policy seems reasonable.
+
+    @param      doc     The document text
+    @param      review  IETF Review object
+
+    @return     None
+    """
+    if re.search(
+        r"(\bExpert\s+Review\b|Specification\s+Required)",
+        unfold(doc.orig),
+        flags=re.IGNORECASE,
+    ):
+        review.comment(
+            "Note to self",
+            "Check whether Expert Review is an appropriate registration policy here.",
+        )
+
+
+def check_implementation_status(doc: Doc, review: IetfReview) -> None:
+    """
+    Check whether the "Implementation Status" section is reasonable.
+
+    @param      doc     The document text
+    @param      review  IETF Review object
+
+    @return     None
+    """
+    if re.search(r"\bImplementation\s+Status\b", unfold(doc.orig), flags=re.IGNORECASE):
+        review.comment(
+            "Note to self",
+            'Check whether the "Implementation Status" section is reasonable.',
+        )
+
+
+def check_code(doc: Doc, review: IetfReview) -> None:
+    """
+    Check any code in "CODE BEGINS/CODE ENDS" blocks.
+
+    @param      doc     The document text
+    @param      review  IETF Review object
+
+    @return     None
+    """
+    # this assumes the JSON is properly indented
+    snippets = re.finditer(r"<CODE BEGINS>(.*)<CODE ENDS>", doc.orig, flags=re.DOTALL)
+
+    for snip in snippets:
+        text = snip.group(1)
+        # try and figure out what the code is in
+        file = re.search(r"\s*file\s*['\"](.*)['\"]\s*$", text, flags=re.MULTILINE)
+        lang = None
+        if file:
+            text = "".join(text.splitlines(keepends=True)[1:])
+            lang = os.path.splitext(file.group(1))[1][1:].lower().strip()
+        # TODO: validate
+
+
+def check_json(doc: Doc, review: IetfReview) -> None:
+    """
+    Check any JSON in the document for issues.
+
+    @param      doc     The document text
+    @param      review  IETF Review object
+
+    @return     None
+    """
+    snippets = re.finditer(r"^(\s*){\s*$", doc.orig, flags=re.MULTILINE)
+    for snip in snippets:
+        # parse JSON snippet until closing brace
+        try:
+            tokens = list(json5.tokenizer.tokenize(doc.orig[snip.start() :]))
+        except json5.utils.JSON5DecodeError as err:
+            review.nit("JSON", str(err) + "\n", wrap=False)
+            return
+        stack = []
+        collected = []
+        for token in tokens:
+            collected.append(token.value)
+            if token.type in ["WHITESPACE"]:
+                continue
+            if token.type in ["LBRACE", "LBRACKET"]:
+                stack.append(token)
+            elif token.type in ["RBRACE", "RBRACKET"]:
+                stack.pop()
+            if not stack:
+                break
+
+        text = "".join(collected)
+        # fix it up a bit
+        text = undo_rfc8792(text.replace("base64url({", "{").replace("})", "}"))
+        try:
+            json.loads(text)
+        except json.decoder.JSONDecodeError as err:
+            nit = ""
+            quote = "> "
+            if review.mkd:
+                nit += "```\n"
+                quote = ""
+
+            for i, line in enumerate(text.splitlines(keepends=True)):
+                nit += f"{quote}{line}"
+                if i == err.lineno - 2:
+                    nit += f"{quote}{' ' * (err.colno - 1)}^ {err.msg}\n"
+
+            if review.mkd:
+                nit += "```\n"
+
+            review.nit("JSON", nit, wrap=False)
+
+
 def check_xml(doc: Doc, review: IetfReview) -> None:
     """
     Check any XML in the document for issues
 
     @param      doc     The document text
     @param      review  IETF Review object
 
     @return     None
     """
     snippets = re.finditer(r"^(.*)<\?xml\s", doc.orig, flags=re.MULTILINE)
     for snip in snippets:
-        start = re.search(r"<\s*([\w:]+)", doc.orig[snip.start() :])
+        start = re.search(r"<\s*([\w:-]+)", doc.orig[snip.start() :])
         if not start:
             log.warning("cannot find an XML start tag")
             continue
 
         end = re.search(
             r"</\s*" + re.escape(start.group(1)) + r"\s*>", doc.orig[snip.start() :]
         )
         if not end:
             log.warning('cannot find XML end tag "%s"', start.group(1))
             continue
 
-        text = doc.orig[snip.start() : snip.start() + end.end()]
+        text = undo_rfc8792(doc.orig[snip.start() : snip.start() + end.end()])
+
         if snip.group(1):
             prefix = snip.group(1)
             # log.debug('XML prefix "%s"', prefix)
             text = re.sub(r"^" + re.escape(prefix), r"", text, flags=re.MULTILINE)
 
         try:
             xml.etree.ElementTree.fromstring(text)
         except xml.etree.ElementTree.ParseError as err:
-            print(text[err.position[0] - 2])
-            review.nit("XML", f'XML issue: "{err}":\n> {text[err.position[0] - 2]}')
+            review.nit(
+                "XML", f'XML issue: "{err}"\n> {text[err.position[0] - 2]}\n', False
+            )
 
 
 def validate_gh_id(_ctx, _param, value):
     """
     Validate the --github-id parameter. See
     https://click.palletsprojects.com/en/8.1.x/options/#callbacks-for-validation
 
@@ -717,27 +843,31 @@
         if not os.path.exists(item):
             log.warning("%s does not exist, skipping", item)
             continue
 
         doc = Doc(item, log, state.datatracker)
         review = IetfReview(doc, gen_mkd, role.strip(), gh_id.strip(), state.width)
 
-        if chk_misc:
-            check_html_entities(doc, review)
-
         if chk_boilerpl and doc.is_id:
             check_boilerplate(doc, review)
 
-        if chk_tlp:
-            check_tlp(doc, review)
-
         if chk_meta and doc.meta:
             check_meta(doc, review, state.datatracker, log)
 
+        if chk_misc:
+            check_html_entities(doc, review)
+
+        if chk_tlp:
+            check_tlp(doc, review)
+
         check_xml(doc, review)
+        check_json(doc, review)
+        check_code(doc, review)
+        check_expert_review(doc, review)
+        check_implementation_status(doc, review)
 
         verbose = state.verbose > 0
 
         if chk_refs and doc.is_id:
             check_refs(doc, review, state.datatracker, log)
 
         if chk_urls:
```

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/inclusive.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/inclusive.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/metadata.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import num2words  # type: ignore
 
 from .doc import Doc
 from .review import IetfReview
 from .util.fetch import fetch_meta
 from .util.text import word_join
+from .references import STATUS_RANK
 
 
 def check_meta(
     doc: Doc, review: IetfReview, datatracker: str, log: logging.Logger
 ) -> None:
     """
     Check document metadata for issues.
@@ -37,14 +38,18 @@
             or doc.status.lower() != "standards track"
         ):
             review.discuss(
                 "Unclear RFC status",
                 f'Intended RFC status in datatracker is "{level}", but '
                 f'document says "{doc.status}".',
             )
+            # continue checking with the "higher" of the two statuses
+            if STATUS_RANK[level.lower()] > STATUS_RANK[doc.status.lower()]:
+                doc.status = level
+                log.info(f"Conflicting status info; checking as {doc.status}")
 
     num_authors = len(doc.meta["authors"])
     if num_authors > 5:
         review.comment(
             "Too many authors",
             f"The document has {num2words.num2words(num_authors)} "
             "authors, which exceeds the "
```

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/references.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/references.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 """ietf-reviewtool references module"""
 
+import itertools
 import logging
 import os
 import re
 
 from .doc import Doc
 from .review import IetfReview
 from .util.fetch import fetch_meta, fetch_docs_in_last_call_text, fetch_dt
 from .util.text import untag, word_join, basename
 from .util.utils import duplicates, get_latest, die
 
 
+STATUS_RANK = {
+    "internet standard": 3,
+    "full standard": 3,
+    "best current practice": 3,
+    "draft standard": 2,
+    "proposed standard": 1,
+    "standards track": 1,
+    "experimental": 0,
+    "informational": 0,
+    "unknown": 0,
+}
+
+
 def check_refs(
     doc: Doc,
     review: IetfReview,
     datatracker: str,
     log: logging.Logger,
 ) -> None:
     """
@@ -50,14 +64,15 @@
 
     # check for duplicates
     for kind in ["normative", "informative"]:
         if not doc.references[kind]:
             continue
 
         tags, tgts = zip(*doc.references[kind])
+        tgts = list(itertools.chain(*tgts))
         dupes = duplicates(tags)
         if dupes:
             review.nit(
                 "Duplicate references",
                 f"Duplicate {kind} references: "
                 f"{word_join(list(dupes), prefix=quote, suffix=quote)}.",
             )
@@ -85,137 +100,158 @@
             f"informative sections: "
             f"{word_join(list(norm & info), prefix=quote, suffix=quote)}.",
         )
 
     if in_text - both:
         ref_list = word_join(list(in_text - both), prefix=quote, suffix=quote)
         review.comment(
-            "Missing references", f"No reference entries found for: {ref_list}."
+            "Missing references",
+            (
+                "No reference entries found for these items, "
+                f"which were mentioned in the text: {ref_list}."
+            ),
         )
 
     if both - in_text:
         ref_list = word_join(list(both - in_text), prefix=quote, suffix=quote)
         review.nit("Uncited references", f"Uncited references: {ref_list}.")
 
     for rel, rel_docs in doc.relationships.items():
         for rel_doc in rel_docs:
             ref = f"rfc{rel_doc}"
-            in_normative = ref in [x[1] for x in doc.references["normative"]]
-            in_informative = ref in [x[1] for x in doc.references["informative"]]
+
+            def ref_in(ref, refs) -> bool:
+                return (
+                    filter(
+                        lambda x: re.search(ref, x),
+                        [x[1] for x in refs],
+                    )
+                    is not None
+                )
+
+            in_normative = ref_in(ref, doc.references["normative"])
+            in_informative = ref_in(ref, doc.references["informative"])
 
             if not in_normative and not in_informative:
                 review.comment(
                     "Uncited references",
                     f"Document {rel} {quote}RFC{rel_doc}{quote}, "
-                    "but does not cite it as a reference.",
+                    "but does not cite it as a reference, which is a bit odd.",
                 )
 
     level = doc.meta and (doc.meta["std_level"] or doc.meta["intended_std_level"])
     if not level:
         # if we have no level from the metadata, see if the document has one
         level = doc.status if doc.status else "unknown"
 
     for kind in ["normative", "informative"]:
-        for tag, ref_doc in doc.references[kind]:
-            if ref_doc:
-                name = re.search(r"^(rfc\d+|draft-[-a-z\d_.]+)", ref_doc)
-            if not ref_doc or not name:
-                log.debug(
-                    "No metadata available for %s reference %s",
-                    kind,
-                    tag,
-                )
-                if kind == "normative" and doc.status.lower() not in [
-                    "informational",
-                    "experimental",
-                ]:
-                    review.comment(
-                        "DOWNREFs",
-                        f"Possible DOWNREF from this {doc.status} doc "
-                        f"to {quote}{tag}{quote}. If so, the IESG needs to approve it.",
+        for tag, ref_docs in doc.references[kind]:
+            for ref_doc in ref_docs:
+                if ref_doc:
+                    name = re.search(r"^(rfc\d+|draft-[-a-z\d_.]+)", ref_doc)
+                if not ref_doc or not name:
+                    log.debug(
+                        "No metadata available for %s reference %s",
+                        kind,
+                        tag,
                     )
-                continue
-
-            draft_components = re.search(r"^(draft-.*)-(\d{2,})$", name.group(0))
-            rev = None
-            if draft_components:
-                docname = draft_components.group(1)
-                rev = basename(draft_components.group(2))
-            else:
-                docname = re.sub(r"rfc0*(\d+)", r"rfc\1", name.group(0))
-            ref_meta = fetch_meta(datatracker, docname, log)
-            display_name = re.sub(r"rfc", r"RFC", docname)
-
-            latest = ref_meta and get_latest(ref_meta["rev_history"], "published")
-            if latest and latest["rev"] and rev and latest["rev"] > rev:
-                if latest["rev"].startswith("rfc"):
-                    review.nit(
-                        "Outdated references",
-                        f"Document references {quote}{display_name}{quote}, but that "
-                        f"has been published as {quote}{latest['rev'].upper()}{quote}.",
-                    )
-                else:
-                    review.nit(
-                        "Outdated references",
-                        f"Document references {quote}{docname}-{rev}{quote}, but "
-                        f"{quote}-{latest['rev']}{quote} is the latest "
-                        f"available revision.",
-                    )
-
-            if ref_meta and doc.status.lower() not in ["informational", "experimental"]:
-                ref_level = (
-                    ref_meta["std_level"] or ref_meta["intended_std_level"] or "unknown"
-                )
-                if (
-                    is_downref(level, kind, ref_level, log)
-                    and docname not in downrefs_in_registry
-                    and docname not in docs_in_lc
-                ):
-                    if ref_level is None:
+                    if kind == "normative" and doc.status.lower() not in [
+                        "informational",
+                        "experimental",
+                    ]:
                         review.comment(
                             "DOWNREFs",
-                            f"Possible DOWNREF {quote}{tag}{quote} from this {level} "
-                            f"to {quote}{display_name}{quote}.",
+                            f"Possible DOWNREF from this {doc.status} doc "
+                            f"to {quote}{tag}{quote}. If so, the IESG needs to approve it.",
+                        )
+                    continue
+
+                draft_components = re.search(r"^(draft-.*)-(\d{2,})$", name.group(0))
+                rev = None
+                if draft_components:
+                    docname = draft_components.group(1)
+                    rev = basename(draft_components.group(2))
+                else:
+                    docname = re.sub(r"rfc0*(\d+)", r"rfc\1", name.group(0))
+                ref_meta = fetch_meta(datatracker, docname, log)
+                display_name = re.sub(r"rfc", r"RFC", docname)
+
+                latest = ref_meta and get_latest(ref_meta["rev_history"], "published")
+                if latest and latest["rev"] and rev and latest["rev"] > rev:
+                    if latest["rev"].startswith("rfc"):
+                        review.nit(
+                            "Outdated references",
+                            f"Document references {quote}{display_name}{quote}, but that "
+                            f"has been published as {quote}{latest['rev'].upper()}{quote}.",
                         )
                     else:
-                        msg = f"DOWNREF {quote}{tag}{quote} from this {level} to "
-                        if ref_level != "unknown":
-                            msg += f"{ref_level} {quote}{display_name}{quote}."
+                        review.nit(
+                            "Outdated references",
+                            f"Document references {quote}{docname}-{rev}{quote}, but "
+                            f"{quote}-{latest['rev']}{quote} is the latest "
+                            f"available revision.",
+                        )
+
+                if ref_meta and doc.status.lower() not in [
+                    "informational",
+                    "experimental",
+                ]:
+                    ref_level = (
+                        ref_meta["std_level"]
+                        or ref_meta["intended_std_level"]
+                        or "unknown"
+                    )
+                    if (
+                        is_downref(level, kind, ref_level, log)
+                        and docname not in downrefs_in_registry
+                        and docname not in docs_in_lc
+                    ):
+                        if ref_level is None:
+                            review.comment(
+                                "DOWNREFs",
+                                f"Possible DOWNREF {quote}{tag}{quote} from this {level} "
+                                f"to {quote}{display_name}{quote}.",
+                            )
                         else:
+                            msg = f"DOWNREF {quote}{tag}{quote} from this {level} to "
+                            if ref_level != "unknown":
+                                msg += f"{ref_level} {quote}{display_name}{quote}."
+                            else:
+                                msg += (
+                                    f"{quote}{display_name}{quote}"
+                                    + " of unknown standards level."
+                                )
                             msg += (
-                                f"{quote}{display_name}{quote}"
-                                + " of unknown standards level."
+                                " (For IESG discussion. "
+                                "It seems this DOWNREF was not mentioned in "
+                                "the Last Call and also seems to not appear "
+                                "in the DOWNREF registry.)"
                             )
-                        msg += (
-                            " (For IESG discussion. "
-                            "It seems this DOWNREF was not mentioned in "
-                            "the Last Call and also seems to not appear "
-                            "in the DOWNREF registry.)"
-                        )
-                        review.comment("DOWNREFs", msg)
+                            review.comment("DOWNREFs", msg)
 
-            obsoleted_by = fetch_dt(
-                datatracker,
-                "doc/relateddocument/?relationship__slug=obs&target__name=" + docname,
-                log,
-            )
-            if obsoleted_by:
-                ob_bys = []
-                for obs in obsoleted_by:
-                    obs_by = fetch_dt(datatracker, obs["source"], log)
-                    if "rfc" in obs_by:
-                        ob_bys.append(obs_by["rfc"])
-
-                ob_rfcs = word_join(ob_bys, prefix=f"{quote}RFC", suffix=quote)
-                review.nit(
-                    "Outdated references",
-                    f"Reference {quote}{tag}{quote} to {quote}{display_name}{quote}, "
-                    f"which was obsoleted by {ob_rfcs} "
-                    "(this may be on purpose).",
+                obsoleted_by = fetch_dt(
+                    datatracker,
+                    "doc/relateddocument/?relationship__slug=obs&target__name="
+                    + docname,
+                    log,
                 )
+                if obsoleted_by:
+                    ob_bys = []
+                    for obs in obsoleted_by:
+                        obs_by = fetch_dt(datatracker, obs["source"], log)
+                        if "rfc" in obs_by:
+                            ob_bys.append(obs_by["rfc"])
+
+                    ob_rfcs = word_join(ob_bys, prefix=f"{quote}RFC", suffix=quote)
+                    review.nit(
+                        "Outdated references",
+                        f"Reference {quote}{tag}{quote} to {quote}{display_name}{quote}, "
+                        f"which was obsoleted by {ob_rfcs} "
+                        "(this may be on purpose).",
+                    )
 
 
 def is_downref(level: str, kind: str, ref_level: str, log: logging.Logger) -> bool:
     """
     Check if a document reference is allowed (i.e., is not a DOWNREF) for a
     document at a given standards level.
 
@@ -226,30 +262,17 @@
     @return     True if this is a DOWNREF, True otherwise.
     """
     kind = kind.lower()
     level = level.lower()
     ref_level = ref_level.lower()
 
     if kind == "normative":
-        rank = {
-            "internet standard": 3,
-            "full standard": 3,
-            "best current practice": 3,
-            "draft standard": 2,
-            "proposed standard": 1,
-            "standards track": 1,
-            "experimental": 0,
-            "informational": 0,
-            "unknown": 0,
-        }
-
         if level == "best current practice":
-            return rank[level] < rank["proposed standard"]
-
-        return rank[level] > rank[ref_level]
+            return STATUS_RANK[level] < STATUS_RANK["proposed standard"]
+        return STATUS_RANK[level] > STATUS_RANK[ref_level]
 
     if kind == "informative":
         return False
     die(f"unknown kind {kind}", log)
     return False  # can't be reached, but makes pylint quiet
```

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/review.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/review.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/util/docposition.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/util/docposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ietf-reviewtool document position module"""
 
 import re
 
 # pattern matching section headings
 SECTION_PATTERN = re.compile(
     r"""^(?:[\- ]\s)?(Abstract|Status\sof\sThis\sMemo|Copyright\sNotice|
-        Editorial\sNote|Table\sof\sContents|
+        Editorial\sNote|Table\sof\sContents|Acknowledge?ments?|
         (?:(?:Non-)Normative\s|Informative\s)?References?|
         Author(?:'?s?'?)?\sAddress(?:es)?|
         (?:Appendix\s+)?[\dA-Z]+(?:\.\d+)*\.?\s|
         \d+(?:\.\d+)*\.?)(.*)""",
     re.VERBOSE,
 )
```

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/util/fetch.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/util/fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 import gzip
 import json
 import logging
 import os
 import re
 import urllib.request
 
-import appdirs  # type: ignore
+import appdirs
 import requests
 import requests_cache
 
+from typing import Optional
+
 from .text import basename, strip_pagination
 from .utils import get_latest, read, write
 
 
-def fetch_init_cache(log: logging.Logger) -> None:
+def fetch_init_cache(log: Optional[logging.Logger] = None) -> None:
     """
     Initialize the fetch cache.
 
     @param      log   The log to write to
     """
     cache = appdirs.user_cache_dir("ietf-reviewtool")
     if not os.path.isdir(cache):
         os.mkdir(cache)
-    log.debug("Using cache directory %s", cache)
+    if log:
+        log.debug("Using cache directory %s", cache)
     requests_cache.install_cache(
         cache_name=os.path.join(cache, "ietf-reviewtool"),
         backend="sqlite",
         allowable_codes=[200],
         stale_if_error=False,
         match_headers=True,
         expire_after=datetime.timedelta(days=30),
@@ -275,15 +278,19 @@
             )
             url = datatracker + "/doc/" + url_pattern
             # the charters in rsync don't have milestones, can't use
             # cache = os.getenv("IETF_CHARTERS")
             do_strip = False
         elif match:
             which = match[1]
-            doc = re.sub(which + r"-(.*)", r"draft-\1", item)
+            if which == "conflict-review":
+                doc = re.sub(which + r"-(.*)", r"draft-\1", item)
+            else:
+                # FIXME: figure out how to download status change text
+                continue
             text = get_writeups(datatracker, doc, log)
             # in-progress conflict-reviews/status-changes are not in the cache
             doc = basename(doc)
             slug = "conflrev" if which == "conflict-review" else "statchg"
             target = fetch_dt(
                 datatracker,
                 f"doc/relateddocument/?relationship__slug={slug}&target__name={doc}",
```

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/util/format.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/util/format.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/util/text.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/util/text.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 import re
 import urllib.parse
 import os
 
 import textwrap
 import urlextract  # type: ignore
 
+from .docposition import SECTION_PATTERN
+
+extractor = urlextract.URLExtract()
+extractor.update_when_older(7)  # update TLDs when older than 7 days
+
 
 def normalize_ws(string: str) -> str:
     """
     Replace multiple white space characters by a single space.
 
     @param      string  The string to replace in
 
@@ -104,76 +109,85 @@
 
 
 def extract_urls(
     text: str,
     log: logging.Logger,
     examples: bool = False,
     common: bool = False,
-) -> set:
+) -> dict[str, set[str]]:
     """
     Return a list of URLs in a text string.
 
     @param      text      The text to extract URLs from
     @param      log       The log
     @param      examples  Include example URLs
     @param      common    Include URLs that are common in IETF documents
 
     @return     List of URLs.
     """
 
-    # find all URLs
-    extractor = urlextract.URLExtract()
-    extractor.update_when_older(7)  # update TLDs when older than 7 days
-    text = unfold(text)
-    urls = []
-    for url in extractor.gen_urls(text):
-        url = url.rstrip(".\"]'>;,)")
-        # if not re.search(r"://", url):
-        #     url = "http://" + url
-        if re.match(r"[\d\.:a-f]+", url, flags=re.IGNORECASE):
-            # skip literal IP addresses
-            continue
-        try:
-            urllib.parse.urlparse(url).netloc
-        except ValueError as err:
-            log.warning("%s: %s", err, url)
-            continue
-        urls.append(url)
+    urls: dict[str, set] = {}
+    for part, part_text in doc_parts(text).items():
+        if part not in urls:
+            urls[part] = set()
 
-    if not examples:
-        # remove example URLs
-        urls = [
-            u
-            for u in urls
-            if not re.search(
-                r"example\.(com|net|org)|\.example",
-                urllib.parse.urlparse(u).netloc
-                if urllib.parse.urlparse(u).netloc
-                else u,
-                re.IGNORECASE,
+        # find all URLs in part
+        part_text = unfold(part_text)
+        try:
+            extracted_urls = extractor.find_urls(
+                text=part_text, with_schema_only=True, only_unique=True
             )
-        ]
+        except UnicodeDecodeError as err:
+            log.warning("Could not extract URLs: %s", err)
+            return {}
+
+        for url in extracted_urls:
+            url = url.rstrip(".\"]'>;,)")
+            if re.match(r"[\d\.:a-f]+", url, flags=re.IGNORECASE):
+                # skip literal IP addresses
+                continue
+            try:
+                urllib.parse.urlparse(url).netloc
+            except ValueError as err:
+                log.warning("%s: %s", err, url)
+                continue
+
+            urls[part].add(url)
+
+        if not examples:
+            # remove example URLs
+            urls[part] = {
+                u
+                for u in urls[part]
+                if not re.search(
+                    r"example\.(com|net|org)|\.example",
+                    urllib.parse.urlparse(u).netloc
+                    if urllib.parse.urlparse(u).netloc
+                    else u,
+                    re.IGNORECASE,
+                )
+            }
 
-    if not common:
-        # remove some common URLs
-        urls = [
-            u
-            for u in urls
-            if not re.search(
-                r"""https?://
-                    datatracker\.ietf\.org/drafts/current/|
-                    trustee\.ietf\.org/license-info|
-                    (www\.)?rfc-editor\.org/info/rfc\d+|
-                    (www\.)?ietf\.org/archive/id/draft-""",
-                u,
-                flags=re.VERBOSE | re.IGNORECASE,
-            )
-        ]
+        if not common:
+            # remove some common URLs
+            urls[part] = {
+                u
+                for u in urls[part]
+                if not re.search(
+                    r"""https?://
+                        datatracker\.ietf\.org/drafts/current/|
+                        trustee\.ietf\.org/license-info|
+                        (www\.)?rfc-editor\.org/info/rfc\d+|
+                        (www\.)?ietf\.org/archive/id/draft-""",
+                    u,
+                    flags=re.VERBOSE | re.IGNORECASE,
+                )
+            }
 
-    return set(urls)
+    return urls
 
 
 def strip_pagination(text: str) -> str:
     """
     Strip headers and footers, end-of-line whitespace and CR/LF, similar to the rfcstrip
     tool (https://trac.tools.ietf.org/tools/rfcstrip/) from which the regexs used below
     were originally adopted.
@@ -284,7 +298,51 @@
 
     @return     Wrapped version of text followed by end.
     """
     return (
         textwrap.fill(text, width=width, break_on_hyphens=False, break_long_words=False)
         + end
     )
+
+
+def undo_rfc8792(text: str) -> str:
+    """
+    Undo RFC 8792 single backslash strategy line-wrapping.
+
+    @param      text  The text to unwrap
+
+    @return     The unwrapped text.
+    """
+    # TODO: add support for double backslash strategy
+    return re.sub(r"\\$\n^\s*", "", text, flags=re.MULTILINE)
+
+
+def doc_parts(text: str) -> dict[str, str]:
+    """
+    Split document lines into body text and reference sections.
+
+    @param      text  The text to spit
+
+    @return     A dict containing the lines in different parts of the document.
+    """
+    parts = {"text": "", "informative": "", "normative": ""}
+    part = "text"
+    for line in text.splitlines(keepends=True):
+        pot_sec = SECTION_PATTERN.search(line)
+        if pot_sec:
+            which = pot_sec.group(0)
+            if re.search(
+                r"^(?:(\d\.?)+\s+)?(?:Non-Norm|Inform)(?:ative|ational)\s+References?\s*$",
+                which,
+                flags=re.IGNORECASE,
+            ):
+                part = "informative"
+            elif re.search(
+                r"^(?:(\d\.?)+\s+)?(Normative\s+)?References?\s*$",
+                which,
+                flags=re.IGNORECASE,
+            ):
+                part = "normative"
+            else:
+                part = "text"
+        parts[part] += line
+    return parts
```

### Comparing `ietf_reviewtool-0.2.3/ietf_reviewtool/util/utils.py` & `ietf_reviewtool-0.3.0/ietf_reviewtool/util/utils.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.2.3/pyproject.toml` & `ietf_reviewtool-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 [tool.poetry]
 name = "ietf-reviewtool"
-version = "0.2.3"
+version = "0.3.0"
 description = "Review tool for IETF documents"
 authors = ["Lars Eggert <lars@eggert.org>"]
 readme = "README.md"
 homepage = "https://github.com/larseggert/ietf-reviewtool"
 repository = "https://github.com/larseggert/ietf-reviewtool"
 license = "GPL-2.0-only"
 
 [tool.poetry.dependencies]
-python = "^3, >=3.6"
-requests-cache = "^0.5.2"
-appdirs = "^1.4.4"
-click = "^7.1.2"
-language-tool-python = "^2.5.3"
-PyYAML = "^5.4.1"
-charset-normalizer = "^2.0.6"
-urlextract = "^1.5.0"
-num2words = "^0.5.10"
+python = ">=3.10, <4"
+requests-cache = ">=1.0.0"
+appdirs = ">=1.4.4"
+click = ">=7.1.2"
+language-tool-python = ">=2.5.3"
+PyYAML = ">=5.4.1"
+charset-normalizer = ">=2.0.6"
+urlextract = ">=1.5.0"
+num2words = ">=0.5.10"
+json-five = ">=0.8.0"
+urllib3 = ">=1.26.15"
+requests = ">=2.28.2"
 
 [tool.poetry.dev-dependencies]
-mypy = "^0.942"
+mypy = ">=0.942"
 
 [tool.poetry.scripts]
 irt = "ietf_reviewtool.ietf_reviewtool:cli"
 ietf-reviewtool = "ietf_reviewtool.ietf_reviewtool:cli"
 
+[tool.poetry.group.types.dependencies]
+types-requests = "^2.31.0.0"
+types-appdirs = "^1.4.3.5"
+types-urllib3 = "^1.26.25.13"
+types-click = "^7.1.8"
+types-pyyaml = "^6.0.12.10"
 [tool.pylint.messages_control]
 # TODO: these are very high and should be gradually reduced during refactoring
 max-args = 15
 max-bool-expr = 10
 max-branches = 80
 max-locals = 50
 max-module-lines = 1500
```

### Comparing `ietf_reviewtool-0.2.3/setup.py` & `ietf_reviewtool-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,232 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ietf-reviewtool
+Version: 0.3.0
+Summary: Review tool for IETF documents
+Home-page: https://github.com/larseggert/ietf-reviewtool
+License: GPL-2.0-only
+Author: Lars Eggert
+Author-email: lars@eggert.org
+Requires-Python: >=3.10,<4
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=5.4.1)
+Requires-Dist: appdirs (>=1.4.4)
+Requires-Dist: charset-normalizer (>=2.0.6)
+Requires-Dist: click (>=7.1.2)
+Requires-Dist: json-five (>=0.8.0)
+Requires-Dist: language-tool-python (>=2.5.3)
+Requires-Dist: num2words (>=0.5.10)
+Requires-Dist: requests (>=2.28.2)
+Requires-Dist: requests-cache (>=1.0.0)
+Requires-Dist: urlextract (>=1.5.0)
+Requires-Dist: urllib3 (>=1.26.15)
+Project-URL: Repository, https://github.com/larseggert/ietf-reviewtool
+Description-Content-Type: text/markdown
 
-packages = \
-['ietf_reviewtool', 'ietf_reviewtool.util']
+# ietf-reviewtool
 
-package_data = \
-{'': ['*']}
+This is a simple Python 3 tool to download and review IETF documents, such as
+Internet-Drafts or RFCs, and comes packaged as a single `ietf-reviewtool`
+script.
 
-install_requires = \
-['PyYAML>=5.4.1,<6.0.0',
- 'appdirs>=1.4.4,<2.0.0',
- 'charset-normalizer>=2.0.6,<3.0.0',
- 'click>=7.1.2,<8.0.0',
- 'language-tool-python>=2.5.3,<3.0.0',
- 'num2words>=0.5.10,<0.6.0',
- 'requests-cache>=0.5.2,<0.6.0',
- 'urlextract>=1.5.0,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['ietf-reviewtool = ietf_reviewtool.ietf_reviewtool:cli',
-                     'irt = ietf_reviewtool.ietf_reviewtool:cli']}
-
-setup_kwargs = {
-    'name': 'ietf-reviewtool',
-    'version': '0.2.3',
-    'description': 'Review tool for IETF documents',
-    'long_description': '# ietf-reviewtool\n\nThis is a simple Python 3 tool to download and review IETF documents, such as\nInternet-Drafts or RFCs, and comes packaged as a single `ietf-reviewtool`\nscript.\n\n## About\n\n`ietf-reviewtool` offers several different review tools:\n\n* `fetch` downloads items (I-Ds, charters, RFCs, etc.) for review\n\n* `fetch-agenda` downloads all items on the [agenda of the next IESG\n  telechat](https://datatracker.ietf.org/iesg/agenda/) for review\n\n* `strip` strips headers, footers and pagination from items, similar to the\n  earlier [`rfcstrip`](https://tools.ietf.org/tools/rfcstrip/about) tool\n\n* `review` extracts inline reviews from the indicated items and formats them for\n  sharing by email or submission to the [IETF\n  datatracker](https://datatracker.ietf.org/), with some functionality that is\n  similar to the earlier\n  [`idcomments`](https://tools.ietf.org/tools/idcomments/about) tool\n\nThis is a work in progress. Additional functionality will be added over time, so\nthere is a chance this documentation only covers a subset of what the actual\ntool offers. You can get command line help on the various tools by passing\n`--help` to `ietf-reviewtool` and its sub-tools.\n\n## Installation\n\nYou can install this via [PyPI](https://pypi.org/project/ietf-reviewtool/):\n\n``` shell\npip install ietf-reviewtool\n```\n\n## Usage\n\nAn example workflow of the tool is as follows.\n\n### Downloading items\n\nYou first download the item for review:\n``` shell\nietf-reviewtool fetch rfc1925.txt\n```\n\nThis downloads the text version of\n[RFC1925](https://datatracker.ietf.org/doc/html/rfc1925) into a text file named\n`rfc1925.txt` and (by default) performs a `strip` operation on the file.\n\nYou will then open the stripped `rfc1925.txt` for review in your preferred text\neditor.\n\n### Reviewing\n\nYou can flag issues of three different severity levels, namely, "discuss",\n"comment" and "nit". (These levels are inspired by the [IESG review\nprocess](https://www.ietf.org/about/groups/iesg/statements/iesg-discuss-criteria/).)\n\nIn order to flag an issue of a given severity level, enter a new line at an\nappropriate location in the document that reads `DISCUSS:`, `COMMENT:` or\n`NIT:`.\n\n#### Inline issues\n\nUsing `rfc1925.txt` as an example and using `***` to indicate the added review\ncontent, you can flag an "inline" issue like this:\n```\n2. The Fundamental Truths\n\n   (1)  It Has To Work.\n\n***COMMENT: Well, duh.***\n```\n\nAfter saving the changed `rfc1925.txt`, you can then extract a formatted review\nas:\n\n```\nSection 2, paragraph 2, comment:\nWell, duh.\n```\n\nSee below for how to extract a review.\n\nUsing `DISCUSS:` or `NIT:` instead of `COMMENT:` will change the severity of the\nissue, as appropriate.\n\n#### Issues with context\n\nIt is possible quote part of the original document, to give the review some context, like this:\n\n```\n***COMMENT:***\n   (3)  With sufficient thrust, pigs fly just fine. However, this is\n***Can we stop picking on pigs or pigeons?***\n```\n\nThis will produce the following review:\n\n```\nSection 2, paragraph 5, comment:\n>    (3)  With sufficient thrust, pigs fly just fine. However, this is\n\nCan we stop picking on pigs or pigeons?\n```\n\n#### Inline nits\n\nTo quickly flag some editing nits, such as spelling errors, you can simply edit\nthe text directly, correcting the nit. For example, to flag an existing spelling error in `rfc1925.txt` (where "agglutinate" is misspelled as "aglutenate"), you would simply correct the word in the text:\n\n```\n   (5)  It is always possible to ***agglutinate*** multiple separate problems\n        into a single complex interdependent solution. In most cases\n        this is a bad idea.\n```\n\nWhen extracting the formatted review, such inline corrections are added to the "nits" section in "diff" format:\n\n```\nSection 2, paragraph 7, nit:\n-    (5)  It is always possible to aglutenate multiple separate problems\n-                                       ^\n+    (5)  It is always possible to agglutinate multiple separate problems\n+                                    +   ^\n```\n\n### Extracting the review\n\nAfter editing a source file, you can extract a formatted review with:\n``` shell\nietf-reviewtool review rfc1925.txt\n```\n\nWith the given example, this would result in the following output:\n```\n-------------------------------------------------------------------------\nCOMMENT\n-------------------------------------------------------------------------\nSection 2, paragraph 2, comment:\nWell, duh.\n\nSection 2, paragraph 5, comment:\n>    (3)  With sufficient thrust, pigs fly just fine. However, this is\n\nCan we not always pick on pigs or pigeons?\n\n-------------------------------------------------------------------------\nNIT\n-------------------------------------------------------------------------\nSection 2, paragraph 7, nit:\n-    (5)  It is always possible to aglutenate multiple separate problems\n-                                       ^\n+    (5)  It is always possible to agglutinate multiple separate problems\n+                                    +   ^\n```\n\n### Using caches\n\nIn order to speed up the process, and to operate while being offline, you can\nset various environment variables to point the tool at directories in which you\n[cache various IETF document via\n`rsync`](https://www.ietf.org/standards/ids/internet-draft-mirror-sites/).\n\nThese environment variables are named:\n\n* `IETF_CHARTERS`\n* `IETF_CONFLICT_REVIEWS`\n* `IETF_IDS`\n* `IETF_RFCS`\n* `IETF_STATUS_CHANGES`\n\nWhen the tool finds a given item to review in the cache, it will refrain from\ndownloading it from the web.\n\nNote that the tool will **not** place items into the cache directories when they are not present; you **will** need to update the cache via `rsync`.\n\n## Acknowledgments\n\nThe ideas for some of these tools came from some of Henrik Levkowetz\'s earlier\n`bash` scripts. In the case of the `strip` tool, most of the original regular\nexpressions were taken from his\n[`rfcstrip`](https://tools.ietf.org/tools/rfcstrip/about) `awk` script.\n\n\n## License\n\nCopyright (C) 2021-2022  Lars Eggert\n\nThis program is free software; you can redistribute it and/or modify it under\nthe terms of the GNU General Public License as published by the Free Software\nFoundation; either version 2 of the License, or (at your option) any later\nversion.\n\nThis program is distributed in the hope that it will be useful, but WITHOUT ANY\nWARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A\nPARTICULAR PURPOSE.  See the GNU General Public License for more details.\n\nYou should have received a copy of the GNU General Public License along with\nthis program; if not, write to the Free Software Foundation, Inc., 51 Franklin\nStreet, Fifth Floor, Boston, MA  02110-1301, USA.\n',
-    'author': 'Lars Eggert',
-    'author_email': 'lars@eggert.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/larseggert/ietf-reviewtool',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4',
-}
+## About
 
+`ietf-reviewtool` offers several different review tools:
+
+* `fetch` downloads items (I-Ds, charters, RFCs, etc.) for review
+
+* `fetch-agenda` downloads all items on the [agenda of the next IESG
+  telechat](https://datatracker.ietf.org/iesg/agenda/) for review
+
+* `strip` strips headers, footers and pagination from items, similar to the
+  earlier [`rfcstrip`](https://tools.ietf.org/tools/rfcstrip/about) tool
+
+* `review` extracts inline reviews from the indicated items and formats them for
+  sharing by email or submission to the [IETF
+  datatracker](https://datatracker.ietf.org/), with some functionality that is
+  similar to the earlier
+  [`idcomments`](https://tools.ietf.org/tools/idcomments/about) tool
+
+This is a work in progress. Additional functionality will be added over time, so
+there is a chance this documentation only covers a subset of what the actual
+tool offers. You can get command line help on the various tools by passing
+`--help` to `ietf-reviewtool` and its sub-tools.
+
+## Installation
+
+You can install this via [PyPI](https://pypi.org/project/ietf-reviewtool/):
+
+``` shell
+pip install ietf-reviewtool
+```
+
+## Usage
+
+An example workflow of the tool is as follows.
+
+### Downloading items
+
+You first download the item for review:
+``` shell
+ietf-reviewtool fetch rfc1925.txt
+```
+
+This downloads the text version of
+[RFC1925](https://datatracker.ietf.org/doc/html/rfc1925) into a text file named
+`rfc1925.txt` and (by default) performs a `strip` operation on the file.
+
+You will then open the stripped `rfc1925.txt` for review in your preferred text
+editor.
+
+### Reviewing
+
+You can flag issues of three different severity levels, namely, "discuss",
+"comment" and "nit". (These levels are inspired by the [IESG review
+process](https://www.ietf.org/about/groups/iesg/statements/iesg-discuss-criteria/).)
+
+In order to flag an issue of a given severity level, enter a new line at an
+appropriate location in the document that reads `DISCUSS:`, `COMMENT:` or
+`NIT:`.
+
+#### Inline issues
+
+Using `rfc1925.txt` as an example and using `***` to indicate the added review
+content, you can flag an "inline" issue like this:
+```
+2. The Fundamental Truths
+
+   (1)  It Has To Work.
+
+***COMMENT: Well, duh.***
+```
+
+After saving the changed `rfc1925.txt`, you can then extract a formatted review
+as:
+
+```
+Section 2, paragraph 2, comment:
+Well, duh.
+```
+
+See below for how to extract a review.
+
+Using `DISCUSS:` or `NIT:` instead of `COMMENT:` will change the severity of the
+issue, as appropriate.
+
+#### Issues with context
+
+It is possible quote part of the original document, to give the review some context, like this:
+
+```
+***COMMENT:***
+   (3)  With sufficient thrust, pigs fly just fine. However, this is
+***Can we stop picking on pigs or pigeons?***
+```
+
+This will produce the following review:
+
+```
+Section 2, paragraph 5, comment:
+>    (3)  With sufficient thrust, pigs fly just fine. However, this is
+
+Can we stop picking on pigs or pigeons?
+```
+
+#### Inline nits
+
+To quickly flag some editing nits, such as spelling errors, you can simply edit
+the text directly, correcting the nit. For example, to flag an existing spelling error in `rfc1925.txt` (where "agglutinate" is misspelled as "aglutenate"), you would simply correct the word in the text:
+
+```
+   (5)  It is always possible to ***agglutinate*** multiple separate problems
+        into a single complex interdependent solution. In most cases
+        this is a bad idea.
+```
+
+When extracting the formatted review, such inline corrections are added to the "nits" section in "diff" format:
+
+```
+Section 2, paragraph 7, nit:
+-    (5)  It is always possible to aglutenate multiple separate problems
+-                                       ^
++    (5)  It is always possible to agglutinate multiple separate problems
++                                    +   ^
+```
+
+### Extracting the review
+
+After editing a source file, you can extract a formatted review with:
+``` shell
+ietf-reviewtool review rfc1925.txt
+```
+
+With the given example, this would result in the following output:
+```
+-------------------------------------------------------------------------
+COMMENT
+-------------------------------------------------------------------------
+Section 2, paragraph 2, comment:
+Well, duh.
+
+Section 2, paragraph 5, comment:
+>    (3)  With sufficient thrust, pigs fly just fine. However, this is
+
+Can we not always pick on pigs or pigeons?
+
+-------------------------------------------------------------------------
+NIT
+-------------------------------------------------------------------------
+Section 2, paragraph 7, nit:
+-    (5)  It is always possible to aglutenate multiple separate problems
+-                                       ^
++    (5)  It is always possible to agglutinate multiple separate problems
++                                    +   ^
+```
+
+### Using caches
+
+In order to speed up the process, and to operate while being offline, you can
+set various environment variables to point the tool at directories in which you
+[cache various IETF document via
+`rsync`](https://www.ietf.org/standards/ids/internet-draft-mirror-sites/).
+
+These environment variables are named:
+
+* `IETF_CHARTERS`
+* `IETF_CONFLICT_REVIEWS`
+* `IETF_IDS`
+* `IETF_RFCS`
+* `IETF_STATUS_CHANGES`
+
+When the tool finds a given item to review in the cache, it will refrain from
+downloading it from the web.
+
+Note that the tool will **not** place items into the cache directories when they are not present; you **will** need to update the cache via `rsync`.
+
+## Acknowledgments
+
+The ideas for some of these tools came from some of Henrik Levkowetz's earlier
+`bash` scripts. In the case of the `strip` tool, most of the original regular
+expressions were taken from his
+[`rfcstrip`](https://tools.ietf.org/tools/rfcstrip/about) `awk` script.
+
+
+## License
+
+Copyright (C) 2021-2022  Lars Eggert
+
+This program is free software; you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation; either version 2 of the License, or (at your option) any later
+version.
+
+This program is distributed in the hope that it will be useful, but WITHOUT ANY
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with
+this program; if not, write to the Free Software Foundation, Inc., 51 Franklin
+Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
-setup(**setup_kwargs)
```

