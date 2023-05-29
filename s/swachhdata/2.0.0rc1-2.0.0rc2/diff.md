# Comparing `tmp/swachhdata-2.0.0rc1-py3-none-any.whl.zip` & `tmp/swachhdata-2.0.0rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,22 @@
-Zip file size: 26195 bytes, number of entries: 21
--rw-r--r--  2.0 unx      228 b- defN 23-May-22 04:01 swachhdata/__init__.py
+Zip file size: 22983 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      228 b- defN 23-May-22 06:02 swachhdata/__init__.py
 -rw-r--r--  2.0 unx      106 b- defN 23-May-21 04:19 swachhdata/compose/__init__.py
 -rw-r--r--  2.0 unx     1334 b- defN 23-May-21 20:59 swachhdata/compose/core.py
 -rw-r--r--  2.0 unx      131 b- defN 22-Jan-25 09:02 swachhdata/image/__init__.py
 -rw-r--r--  2.0 unx     7477 b- defN 22-Jan-25 09:02 swachhdata/image/_image.py
--rw-r--r--  2.0 unx      173 b- defN 22-Jan-25 09:02 swachhdata/legacy/__init__.py
--rw-r--r--  2.0 unx    15947 b- defN 23-Mar-10 23:37 swachhdata/legacy/_text.py
--rw-r--r--  2.0 unx      803 b- defN 23-May-22 04:00 swachhdata/text/__init__.py
--rw-r--r--  2.0 unx     2196 b- defN 23-May-21 21:30 swachhdata/text/_base.py
--rw-r--r--  2.0 unx    74326 b- defN 23-May-22 03:57 swachhdata/text/_text.py
+-rw-r--r--  2.0 unx      726 b- defN 23-May-22 06:03 swachhdata/text/__init__.py
+-rw-r--r--  2.0 unx     3822 b- defN 23-May-22 05:22 swachhdata/text/base.py
+-rw-r--r--  2.0 unx     1712 b- defN 23-May-22 05:49 swachhdata/text/pipeline.py
+-rw-r--r--  2.0 unx    63779 b- defN 23-May-22 06:02 swachhdata/text/recast.py
 -rw-r--r--  2.0 unx      642 b- defN 23-May-21 03:53 swachhdata/utils/__init__.py
 -rw-r--r--  2.0 unx     1114 b- defN 23-May-22 01:57 swachhdata/utils/exceptions.py
 -rw-r--r--  2.0 unx      377 b- defN 23-May-22 02:30 swachhdata/utils/probe.py
 -rw-r--r--  2.0 unx     1150 b- defN 23-May-21 14:42 swachhdata/utils/recast.py
 -rw-r--r--  2.0 unx      480 b- defN 23-May-21 03:06 swachhdata/utils/tools.py
 -rw-r--r--  2.0 unx     1310 b- defN 23-May-21 14:42 swachhdata/utils/verify.py
--rw-rw-rw-  2.0 unx    17096 b- defN 23-May-22 04:01 swachhdata-2.0.0rc1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2206 b- defN 23-May-22 04:01 swachhdata-2.0.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 04:01 swachhdata-2.0.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 04:01 swachhdata-2.0.0rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1749 b- defN 23-May-22 04:01 swachhdata-2.0.0rc1.dist-info/RECORD
-21 files, 128948 bytes uncompressed, 23347 bytes compressed:  81.9%
+-rw-rw-rw-  2.0 unx    17096 b- defN 23-May-22 06:04 swachhdata-2.0.0rc2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2206 b- defN 23-May-22 06:04 swachhdata-2.0.0rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 06:04 swachhdata-2.0.0rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-22 06:04 swachhdata-2.0.0rc2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1664 b- defN 23-May-22 06:04 swachhdata-2.0.0rc2.dist-info/RECORD
+20 files, 105457 bytes uncompressed, 20267 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -9,27 +9,24 @@
 
 Filename: swachhdata/image/__init__.py
 Comment: 
 
 Filename: swachhdata/image/_image.py
 Comment: 
 
-Filename: swachhdata/legacy/__init__.py
-Comment: 
-
-Filename: swachhdata/legacy/_text.py
+Filename: swachhdata/text/__init__.py
 Comment: 
 
-Filename: swachhdata/text/__init__.py
+Filename: swachhdata/text/base.py
 Comment: 
 
-Filename: swachhdata/text/_base.py
+Filename: swachhdata/text/pipeline.py
 Comment: 
 
-Filename: swachhdata/text/_text.py
+Filename: swachhdata/text/recast.py
 Comment: 
 
 Filename: swachhdata/utils/__init__.py
 Comment: 
 
 Filename: swachhdata/utils/exceptions.py
 Comment: 
@@ -42,23 +39,23 @@
 
 Filename: swachhdata/utils/tools.py
 Comment: 
 
 Filename: swachhdata/utils/verify.py
 Comment: 
 
-Filename: swachhdata-2.0.0rc1.dist-info/LICENSE.txt
+Filename: swachhdata-2.0.0rc2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: swachhdata-2.0.0rc1.dist-info/METADATA
+Filename: swachhdata-2.0.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: swachhdata-2.0.0rc1.dist-info/WHEEL
+Filename: swachhdata-2.0.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: swachhdata-2.0.0rc1.dist-info/top_level.txt
+Filename: swachhdata-2.0.0rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: swachhdata-2.0.0rc1.dist-info/RECORD
+Filename: swachhdata-2.0.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swachhdata/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = '2.0.0rc1'
+__version__ = '2.0.0rc2'
 __author__ = 'Kritik Seth'
 __maintainer__ = __author__
 __license__ = 'Mozilla Public License Version 2.0'
 __url__ = 'https://swachhdata.readthedocs.io/'
 __connect__ = 'https://www.kritikseth.com/'
```

## swachhdata/text/__init__.py

```diff
@@ -1,39 +1,35 @@
-from ._text import (
+from .recast import (
     urlRecast,
     htmlRecast,
     EscapeSequencesRecast,
     MentionsRecast,
     ContractionsRecast,
     CaseRecast,
     HashtagsRecast,
     ShortWordsRecast,
     StopWordsRecast,
-    NumberRecast,
+    NumbersRecast,
     AlphabetRecast,
-    PunctuationRecast,
+    PunctuationsRecast,
     StemmingRecast,
     LemmatizationRecast,
-    TokenisationRecast,
-    TextRecast,
-    RecastPipeline
+    TokenisationRecast
 )
 
 __all__ = [
     'urlRecast',
     'htmlRecast',
     'EscapeSequencesRecast',
     'MentionsRecast',
     'ContractionsRecast',
     'CaseRecast',
     'HashtagsRecast',
     'ShortWordsRecast',
     'StopWordsRecast',
-    'NumberRecast',
+    'NumbersRecast',
     'AlphabetRecast',
-    'PunctuationRecast',
+    'PunctuationsRecast',
     'StemmingRecast',
     'LemmatizationRecast',
-    'TokenisationRecast',
-    'TextRecast',
-    'RecastPipeline'
-]
+    'TokenisationRecast'
+]
```

## Comparing `swachhdata/text/_text.py` & `swachhdata/text/recast.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import num2words
 import unicodedata
 import string
 
 import emoji
 from emoji import EMOJI_DATA
 
-from tqdm.auto import trange, tqdm
+from tqdm.auto import tqdm
 
-from ._base import TextFormatter, BaseTextRecast
+from .base import BaseTextRecast
 from ..utils import probe_string_data
 
 class urlRecast(BaseTextRecast):
     """Recast text data by removing or extracting URLs.
 
     URLs supported:
         * HTTP address: http://www.website.com
@@ -90,14 +90,15 @@
     """
 
     def __init__(self, process='remove', verbose=0):
 
         super().__init__(process, verbose)
         self.urls = None
         self.__regex = r'\b((?:https?://)?(?:(?:www\.)?(?:[\da-z\.-]+)\.(?:[a-z]{2,6})|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)|(?:(?:[0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|(?:[0-9a-fA-F]{1,4}:){1,7}:|(?:[0-9a-fA-F]{1,4}:){1,6}:[0-9a-fA-F]{1,4}|(?:[0-9a-fA-F]{1,4}:){1,5}(?::[0-9a-fA-F]{1,4}){1,2}|(?:[0-9a-fA-F]{1,4}:){1,4}(?::[0-9a-fA-F]{1,4}){1,3}|(?:[0-9a-fA-F]{1,4}:){1,3}(?::[0-9a-fA-F]{1,4}){1,4}|(?:[0-9a-fA-F]{1,4}:){1,2}(?::[0-9a-fA-F]{1,4}){1,5}|[0-9a-fA-F]{1,4}:(?:(?::[0-9a-fA-F]{1,4}){1,6})|:(?:(?::[0-9a-fA-F]{1,4}){1,7}|:)|fe80:(?::[0-9a-fA-F]{0,4}){0,4}%[0-9a-zA-Z]{1,}|::(?:ffff(?::0{1,4}){0,1}:){0,1}(?:(?:25[0-5]|(?:2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(?:25[0-5]|(?:2[0-4]|1{0,1}[0-9]){0,1}[0-9])|(?:[0-9a-fA-F]{1,4}:){1,4}:(?:(?:25[0-5]|(?:2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(?:25[0-5]|(?:2[0-4]|1{0,1}[0-9]){0,1}[0-9])))(?::[0-9]{1,4}|[1-5][0-9]{4}|6[0-4][0-9]{3}|65[0-4][0-9]{2}|655[0-2][0-9]|6553[0-5])?(?:/[\w\.-]*)*/?)\b'
+        self._name = 'urlRecast'
 
     @property
     def regex(self):
         return self.__regex
 
     
     def __base_recast(self, text):
@@ -146,23 +147,26 @@
             data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
             data_tqdm.set_postfix({'urlRecast process': self._process})
 
         if self._process in ['remove', 'extract']:
             recast_text = [self.__base_recast(text) for text in data_tqdm]
             if self._process == 'extract':
                 self.urls = recast_text
+            else:
+                self.data = recast_text
             return recast_text
 
         elif self._process in ['extract_remove', 'remove_extract']:
             recast_text, urls = [], []
             for text in data_tqdm:
                 text, url = self.__base_recast(text)
                 recast_text.append(text)
                 urls.append(url)
             self.urls = urls
+            self.data = recast_text
             return recast_text, urls
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -182,16 +186,14 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
 class htmlRecast(BaseTextRecast):
     """Recast text data by removing HTML tags.
 
     uses lxml from BeautifulSoup to clean up html tags
     
     Parameters
@@ -211,14 +213,15 @@
     >>> rec.setup_recast(text)
     'Click Here to have a look at the menu in the services tab'
     """
 
     def __init__(self, verbose=0):
 
         super().__init__(verbose=verbose)
+        self._name = 'htmlRecast'
     
     def __base_recast(self, text):
         """Perform selected process on the setup text
 
         Returns
         -------
         ntext : string
@@ -237,14 +240,15 @@
             Processed text
         """
         super().recast()
 
         data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
         data_tqdm.set_postfix({'htmlRecast process': 'remove'})
         recast_text = [self.__base_recast(text) for text in data_tqdm]
+        self.data = recast_text
         return recast_text
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -260,18 +264,16 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
-class EscapeSequencesRecast(TextFormatter):
+class EscapeSequencesRecast(BaseTextRecast):
     """Recast text data by removing Escape Sequences.
 
     Parameters
     ----------
     verbose: int (0, 1, -1), default=0
     
 
@@ -287,76 +289,44 @@
     >>> rec.setup_recast(text)
     'To have a look at the menu Click Here'
     """
 
 
     def __init__(self, verbose=0):
 
-        TextFormatter.__init__(self)
-        self.__setup = False
-        self.__verbose_status = True
-        self.__verbose = verbose
-        if self.__verbose == -1:
-            self.__verbose_status = False
-
-        try:
-            assert(isinstance(self.__verbose, int))
-        except:
-            print(f'Expected verbose input type <class \'int\'>, input type received {type(self.__verbose)}')
+        super().__init__(verbose=verbose)
+        self._name = 'EscapeSequencesRecast'
     
     def __base_recast(self, text):
         """Perform selected process on the setup text
 
         Returns
         -------
         ntext : string
             Processed text
         """
 
         ntext = text.replace('\r', ' ').replace('\n', ' ').replace('\t', ' ').replace('\n', ' ').replace('\f', ' ')
         return ntext
 
-
     def recast(self):
         """Perform selected process on the setup text
 
         Returns
         -------
         ntext : string / list of strings 
             Processed text
         """
+        super().recast()
         
-        try:
-            assert(self.__setup)
-        except:
-            print(f'method setup needs to be called before recast')
-        
-        if self._dtype == str:
-
-            return self.__base_recast(self._text)
-
-        elif self._dtype == list:
-
-            if self.__verbose == 0:
-
-                ntext = []
-                for text in self._text:
-                    ntext.append(self.__base_recast(text))
-                return ntext
-            
-            if self.__verbose == 1 or self.__verbose == -1:
-
-                ntext = []
-                progress_bar = trange(self._count, leave=self.__verbose_status)
-                for i in progress_bar:
-                    progress_bar.set_postfix({'EscapeSequenceRecast process': 'removing'})
-                    text = self._text[i]
-                    ntext.append(self.__base_recast(text))
-                return ntext
-
+        data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
+        data_tqdm.set_postfix({'EscapeSequencesRecast process': 'remove'})
+        recast_text = [self.__base_recast(text) for text in data_tqdm]
+        self.data = recast_text
+        return recast_text
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
         Parameters
@@ -364,20 +334,20 @@
         text : string / list of strings / pandas.core.series.Series
 
         Returns
         -------
         ntext : string / list of strings (process='remove')
             Processed text
         """
+        if not self._setup_check:
+            self.setup(text)
+            return self.recast()
+        else:
+            return self.recast()
 
-        self.setup(text)
-        return self.recast()
-
-
-##############################################################################################################
 
 
 class MentionsRecast(BaseTextRecast):
     """Recast text data by removing or extracting Mentions.
 
     Mentions supported:
         * @jon_doe
@@ -440,14 +410,15 @@
     ['@jondoe']
     """
 
     def __init__(self, process='remove', verbose=0):
 
         super().__init__(process, verbose)
         self.__regex = '([@][A-Za-z0-9._:-]+)'
+        self._name = 'MentionsRecast'
 
     @property
     def regex(self):
         return self.__regex
     
     def __base_recast(self, text):
         """Perform selected process on the setup text
@@ -491,23 +462,26 @@
             data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
             data_tqdm.set_postfix({'MentionRecast process': self._process})
 
         if self._process in ['remove', 'extract']:
             recast_text = [self.__base_recast(text) for text in data_tqdm]
             if self._process == 'extract':
                 self.mentions = recast_text
+            else:
+                self.data = recast_text
             return recast_text
 
         elif self._process in ['extract_remove', 'remove_extract']:
             recast_text, mentions = [], []
             for text in data_tqdm:
                 text, mention = self.__base_recast(text)
                 recast_text.append(text)
                 mentions.append(mention)
             self.mentions = mentions
+            self.data = recast_text
             return recast_text, mentions
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -526,15 +500,14 @@
         """
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
-##############################################################################################################
 
 
 class ContractionsRecast(BaseTextRecast):
     """Recast text data by expanding Contractions
     
     Parameters
     ----------
@@ -553,14 +526,15 @@
     >>> # OR
     >>> rec.setup_recast(text)
     'They are going to wildlife sanctuary, I guess Jon is going to be there too.'
     """
     def __init__(self, verbose=0):
 
         super().__init__(verbose=verbose)
+        self._name = 'ContractionsRecast'
     
     def __base_recast(self, text):
         """Perform selected process on the setup text
 
         Returns
         -------
         text : string
@@ -578,14 +552,15 @@
             Processed text
         """
         super().recast()
 
         data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
         data_tqdm.set_postfix({'ContractionsRecast process': 'remove'})
         recast_text = [self.__base_recast(text) for text in data_tqdm]
+        self.data = recast_text
         return recast_text
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -600,15 +575,14 @@
         """
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
-##############################################################################################################
 
 
 class CaseRecast(BaseTextRecast):
     """Recast text data by case formatting the text
 
     Case formats supported:
         * UPPER case (upper)
@@ -656,14 +630,15 @@
     >>> rec.setup_recast(text)
     'You Can Have A Look At Our Catalogue In The Services Tab'
     """
 
     def __init__(self, process='lower', verbose=0):
 
         super().__init__(process, verbose)
+        self._name = 'CaseRecast'
 
     def __base_recast(self, text):
         """Perform selected process on the setup text
 
         Returns
         -------
         text : string (process='remove')
@@ -691,14 +666,15 @@
             Processed text
         """
         super().recast()
 
         data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
         data_tqdm.set_postfix({'CaseRecast process': self._process})
         recast_text = [self.__base_recast(text) for text in data_tqdm]
+        self.data = recast_text
         return recast_text
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -714,16 +690,14 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
 class EmojiRecast(BaseTextRecast):
     """Recast text data by removing, replaing or extracting Emoji(s).
     
     Parameters
     ----------
     process: string ('remove', 'replace', 'extract', 'extract_remove', 'extract_replace'), default='remove'
@@ -797,14 +771,15 @@
 
     def __init__(self, process='remove', space_out=False, verbose=0):
 
         super().__init__(process, verbose)
         self._space_out = space_out
         self.emojis = None
         self._emoji_list = list(EMOJI_DATA.keys())
+        self._name = 'EmojiRecast'
 
     def __base_recast(self, text):
         """Perform selected process on the setup text
 
         Parameters
         ----------
         text : string / pandas.core.series.Series
@@ -873,23 +848,26 @@
             data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
             data_tqdm.set_postfix({'EmojiRecast process': self._process})
 
         if self._process in ['remove', 'extract', 'replace']:
             recast_text = [self.__base_recast(text) for text in data_tqdm]
             if self._process == 'extract':
                 self.emojis = recast_text
+            else:
+                self.data = recast_text
             return recast_text
 
         elif self._process in ['extract_remove', 'remove_extract', 'extract_replace', 'replace_extract']:
             recast_text, emojis = [], []
             for text in data_tqdm:
                 text, emoji = self.__base_recast(text)
                 recast_text.append(text)
                 emojis.append(emoji)
             self.emojis = emojis
+            self.data = recast_text
             return recast_text, emojis
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -909,16 +887,14 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
 class HashtagsRecast(BaseTextRecast):
     """Recast text data by removing or extracting Hashtag(s).
 
      supported:
         * #sample_website
         * #sample_website123
@@ -977,14 +953,15 @@
     """
 
     def __init__(self, process='remove', verbose=0):
 
         super().__init__(process, verbose)
         self.hashtags = None
         self.__regex = '([#][A-Za-z0-9_]+)'
+        self._name = 'HashtagsRecast'
     
     @property
     def regex(self):
         return self.__regex
     
     def __base_recast(self, text):
         """Perform selected process on the setup text
@@ -1031,23 +1008,26 @@
             data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
             data_tqdm.set_postfix({'HashtagsRecast process': self._process})
 
         if self._process in ['remove', 'extract']:
             recast_text = [self.__base_recast(text) for text in data_tqdm]
             if self._process == 'extract':
                 self.hashtags = recast_text
+            else:
+                self.data = recast_text
             return recast_text
 
         elif self._process in ['extract_remove', 'remove_extract']:
             recast_text, hashtags = [], []
             for text in data_tqdm:
                 text, hashtag = self.__base_recast(text)
                 recast_text.append(text)
                 hashtags.append(hashtag)
             self.hashtags = hashtags
+            self.data = recast_text
             return recast_text, hashtags
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -1067,16 +1047,14 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
 class ShortWordsRecast(BaseTextRecast):
     """Recast text data by removing (short) words of specified length.
     
     Parameters
     ----------
     min_length int (>0), default=3
@@ -1097,14 +1075,15 @@
     'have look catalogue services'
     """
 
     def __init__(self, min_length=3, verbose=0):
 
         super().__init__(verbose=verbose)
         self._min_length = min_length
+        self._name = 'ShortWordsRecast'
 
     
     def __base_recast(self, text):
         """Perform selected process on the setup text
 
         Returns
         -------
@@ -1123,14 +1102,15 @@
         ntext : string / list of strings 
             Processed text
         """
         super().recast()
         data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
         data_tqdm.set_postfix({f'ShortWordsRecast [min_length = {self._min_length}] process': 'remove'})
         recast_text = [self.__base_recast(text) for text in data_tqdm]
+        self.data = recast_text
         return recast_text
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -1147,16 +1127,14 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
 class StopWordsRecast(BaseTextRecast):
     """Recast text data by removing stop words.
     
     Parameters
     ----------
     package: str ('nltk', 'spacy', 'gensim', 'custom'), default='nltk'
@@ -1181,14 +1159,15 @@
 
         if package == 'custom':
             probe_string_data(stopwords)
         
         super().__init__(verbose=verbose)
         self._package = package
         self._stopWords = stopwords
+        self._name = 'StopWordsRecast'
     
     def __setup_package(self):
 
         if self._package == 'nltk':
             from nltk.corpus import stopwords
             self._stopWords = set(stopwords.words('english'))
 
@@ -1218,14 +1197,15 @@
         """
         super().recast()
         self.__setup_package()
 
         data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
         data_tqdm.set_postfix({f'StopWordsRecast [package={self._package}] process': 'remove'})
         recast_text = [self.__base_recast(text) for text in data_tqdm]
+        self.data = recast_text
         return recast_text
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -1241,18 +1221,16 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
-class NumberRecast(BaseTextRecast):
+class NumbersRecast(BaseTextRecast):
     """Recast text data by removing, replacing or extracting numbers.
 
     Number formats supported:
     * 1234567
     * 1,234,567 (use seperator=',')
     * 12,34,567 (use seperator=',')
     * 123.4567 (if not decimal, use seperator='.')
@@ -1330,14 +1308,15 @@
     """
 
     def __init__(self, process='remove', seperator=None, verbose=0):
 
         super().__init__(process, verbose)
         self._seperator = seperator
         self.numbers = None
+        self._name = 'NumbersRecast'
     
     def __base_recast(self, text):
         """Perform selected process on the setup text
 
         Returns
         -------
         ntext : string (process='remove' / process='replace')
@@ -1391,14 +1370,16 @@
             data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
             data_tqdm.set_postfix({'NumberRecast process': self._process})
 
         if self._process in ['remove', 'extract', 'replace']:
             recast_text = [self.__base_recast(text) for text in data_tqdm]
             if self._process == 'extract':
                 self.numbers = recast_text
+            else:
+                self.data = recast_text
             return recast_text
 
         elif self._process in ['extract_remove', 'remove_extract', 'extract_replace', 'replace_extract']:
             recast_text, numbers = [], []
             for text in data_tqdm:
                 text, number = self.__base_recast(text)
                 recast_text.append(text)
@@ -1427,16 +1408,14 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
 class AlphabetRecast(BaseTextRecast):
     """Recast text data by removing all accented, non ascii characters and keeping only alphabets.
     
     Parameters
     ----------
     process: string / list ('all', 'keep_alpha', 'rem_non_ascii', 'rem_acc_char', or combination in a list), default='all'
@@ -1457,14 +1436,15 @@
     'It was past lunch time so the   of us dropped by The Main Street Cafe  for a late lunch '
     """
 
     def __init__(self, process='all', verbose=0):
 
         super().__init__(verbose=verbose)
         self._process = process
+        self._name = 'AlphabetRecast'
     
     def __base_recast(self, text, process):
         """Perform selected process on the setup text
 
         Returns
         -------
         ntext : string
@@ -1501,21 +1481,23 @@
         if isinstance(self._process, list):
 
             for process in self._process:
                 data_tqdm = tqdm(text, leave=self._verbose_status, disable=self._verbose)
                 data_tqdm.set_postfix({'AlphabetRecast process': f'{process}'})
                 text = [self.__base_recast(text, process) for text in data_tqdm]
             
+            self.data = text
             return text
         
         elif isinstance(self._process, str):
 
             data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
             data_tqdm.set_postfix({'AlphabetRecast process': f'{self._process}'})
             recast_text = [self.__base_recast(text, self._process) for text in data_tqdm]
+            self.data = recast_text
             return recast_text
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -1531,16 +1513,14 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
 class PunctuationsRecast(BaseTextRecast):
     """Recast text data by removing punctuations.
     
     Parameters
     ----------
     verbose: int (0, 1, -1), default=0
@@ -1558,14 +1538,15 @@
     >>> rec.setup_recast(text)
     'Have you fed that dog I told you Don t feed that dog'
     """
 
     def __init__(self, verbose=0):
 
         super().__init__(verbose=verbose)
+        self._name = 'PunctuationsRecast'
     
     def __base_recast(self, text):
         """Perform selected process on the setup text
 
         Returns
         -------
         ntext : string
@@ -1582,14 +1563,15 @@
             Processed text
         """
         super().recast()
 
         data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
         data_tqdm.set_postfix({'PunctuationRecast process': 'remove'})
         recast_text = [self.__base_recast(text) for text in data_tqdm]
+        self.data = recast_text
         return recast_text
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -1605,16 +1587,14 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
 class TokenisationRecast(BaseTextRecast):
     """Recast text data by tokenising it.
 
     Tokenisation supported:
         * word tokenisation
         * sentence tokenisation
@@ -1661,14 +1641,15 @@
 
             if package == 'spacy':
                 self._sp = spacy.load('en_core_web_sm')
         else:
             raise ValueError(
                 f'Expected package either nltk or spacy, {type(package)} is not a supported package.'
             )
+        self._name = 'TokenisationRecast'
 
     def __nltk_tokenize(self, text):
 
         if self._method == 'word':
             from nltk.tokenize import word_tokenize
             return word_tokenize(text)
         
@@ -1710,14 +1691,15 @@
             Processed tokens
         """
         super().recast()
 
         data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
         data_tqdm.set_postfix({f'TokenisationRecast [package={self._package}, method={self._method}] process': 'remove'})
         recast_text = [self.__base_recast(text) for text in data_tqdm]
+        self.data = recast_text
         return recast_text
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -1733,16 +1715,14 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
 class StemmingRecast(BaseTextRecast):
     """Recast text data by performing stemming on it.
     
     Parameters
     ----------
     package: string ('nltk', 'extract', 'extract_remove'), default='nltk'
@@ -1783,14 +1763,15 @@
             self._package = package
             self._method = method
 
         else:
             raise ValueError(
                 f'Expected package either nltk or spacy, {type(package)} is not a supported package.'
             )
+        self._name = 'StemmingRecast'
 
     def __base_recast(self, text):
         """Perform selected process on the setup text
 
         Returns
         -------
         ntext : string
@@ -1817,15 +1798,15 @@
             Processed text
         """
         super().recast()
 
         data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
         data_tqdm.set_postfix({f'StemmingRecast [package={self._package}, method={self._method}] process': 'stemming'})
         recast_text = [self.__base_recast(text) for text in data_tqdm]
-
+        self.data = recast_text
         return recast_text
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
 
@@ -1841,16 +1822,14 @@
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
             return self.recast()
 
 
-##############################################################################################################
-
 
 class LemmatizationRecast(BaseTextRecast):
     """Recast text data by performing lemmatization on it.
     
     Parameters
     ----------
     package: string ('nltk', 'spacy'), default='nltk'
@@ -1879,14 +1858,15 @@
 
             if package == 'spacy':
                 self._sp = spacy.load('en', disable=['parser', 'ner'])
         else:
             raise ValueError(
                 f'Expected package either nltk or spacy, {type(package)} is not a supported package.'
             )
+        self._name = 'LemmatizationRecast'
 
     def __get_wordnet_pos(self, word):
         from nltk.corpus import wordnet
 
         tag = nltk.pos_tag([word])[0][1][0].upper()
         tag_dict = {'J': wordnet.ADJ,
                     'N': wordnet.NOUN,
@@ -1924,15 +1904,15 @@
             Processed text
         """
         super().recast()
 
         data_tqdm = tqdm(self.data, leave=self._verbose_status, disable=self._verbose)
         data_tqdm.set_postfix({f'LemmatizationRecast [package={self._package}] process': 'lemmatization'})
         recast_text = [self.__base_recast(text) for text in data_tqdm]
-
+        self.data = recast_text
         return recast_text
 
 
     def setup_recast(self, text):
         """Change the input text type to supported type
         and
         Perform selected process on the setup text
@@ -1946,262 +1926,8 @@
         ntext : string / list of strings
             Processed text
         """
         if not self._setup_check:
             self.setup(text)
             return self.recast()
         else:
-            return self.recast()
-
-
-##############################################################################################################
-
-
-def TextRecast(text, **kwargs):
-    """TextRecast: wrapper function for Recast classes.
-    
-    Parameters
-    ----------
-    text : string / list of strings / pandas.core.series.Series
-    **kwargs
-
-    kwargs Template
-    ----------
-    { urlRecast = {'process': 'extract_remove'},
-      htmlRecast = True,
-      EscapeSequenceRecast = True,
-      MentionRecast = {'process': 'extract_remove'},
-      ContractionsRecast = True,
-      CaseRecast = {'process': 'lower'},
-      EmojiRecast = {'process': 'extract_remove', 'space_out': False},
-      HashtagRecast = {'process': 'extract_remove'},
-      ShortWordsRecast = {'min_length': 3},
-      StopWordsRecast = {'package': 'nltk', 'space_out': None},
-      NumberRecast = {'process': 'remove', 'seperator': None},
-      AlphabetRecast = {'process': 'all'},
-      PunctuationRecast = True,
-      StemmingRecast = {'package': 'nltk', 'method': 'porter'},
-      LemmatizationRecast = {'package':'nltk'},
-      TokenisationRecast = {'package': 'nltk', 'method': 'sentence' }
-
-    Attributes
-    ----------
-    * url
-    * mention
-    * emoji
-    * hashtag
-    * token
-    * number
-
-    Returns
-    ---------
-    ntext : string / list of strings
-            Processed text
-    """
-
-    verbose=-1
-
-    ccount = 0 # complete count
-    rcount = len(kwargs) # recast count
-    tcount = len(text) # text length count
-
-    chunk_size = rcount * tcount
-    pbar = tqdm(total=chunk_size)
-
-    if 'urlRecast' in kwargs:
-        
-        ccount +=  1
-        pbar.set_postfix({'urlRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        global url
-        if kwargs['urlRecast']['process'] == 'extract_remove':
-           text, url  = urlRecast(kwargs['urlRecast']['process'], verbose=verbose).setup_recast(text)
-
-        elif kwargs['urlRecast']['process'] == 'extract':
-            url  = urlRecast(kwargs['urlRecast']['process'], verbose=verbose).setup_recast(text)
-        
-        elif kwargs['urlRecast']['process'] == 'remove':
-           text = urlRecast(kwargs['urlRecast']['process'], verbose=verbose).setup_recast(text) 
-
-        pbar.update(tcount)
-
-    if 'htmlRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'htmlRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        text = htmlRecast(verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-    
-    if 'EscapeSequenceRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'EscapeSequenceRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        text = EscapeSequenceRecast(verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-    
-    if 'MentionRecast' in kwargs:
-        
-        ccount +=  1
-        pbar.set_postfix({'MentionRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        global mention
-        if kwargs['MentionRecast']['process'] == 'extract_remove':
-           text, mention  = MentionRecast(kwargs['MentionRecast']['process'], verbose=verbose).setup_recast(text)
-
-        elif kwargs['MentionRecast']['process'] == 'extract':
-            mention  = MentionRecast(kwargs['MentionRecast']['process'], verbose=verbose).setup_recast(text)
-        
-        elif kwargs['MentionRecast']['process'] == 'remove':
-           text = MentionRecast(kwargs['MentionRecast']['process'], verbose=verbose).setup_recast(text)
-
-        pbar.update(tcount)
-
-    if 'ContractionsRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'ContractionsRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        text = ContractionsRecast(verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-    
-    if 'CaseRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'CaseRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        text = CaseRecast(kwargs['CaseRecast']['process'], verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-    
-    # if 'EmojiRecast' in kwargs:
-
-    #     ccount +=  1
-    #     pbar.set_postfix({'EmojiRecast || TextRecast No': f'{ccount}/{rcount}'})
-        
-    #     global emoji
-    #     if kwargs['EmojiRecast']['process'] == 'extract_remove':
-    #        text, emoji  = EmojiRecast(kwargs['EmojiRecast']['process'], kwargs['EmojiRecast']['space_out'], verbose=verbose).setup_recast(text)
-
-    #     elif kwargs['EmojiRecast']['process'] == 'extract':
-    #         emoji  = EmojiRecast(kwargs['EmojiRecast']['process'], kwargs['EmojiRecast']['space_out'], verbose=verbose).setup_recast(text)
-        
-    #     elif kwargs['EmojiRecast']['process'] == 'remove':
-    #        text = EmojiRecast(kwargs['EmojiRecast']['process'], kwargs['EmojiRecast']['space_out'], verbose=verbose).setup_recast(text)
-
-    #     pbar.update(tcount)
-    
-    if 'HashtagRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'HashtagRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        global hashtag
-        if kwargs['HashtagRecast']['process'] == 'extract_remove':
-           text, hashtag  = HashtagRecast(kwargs['HashtagRecast']['process'], verbose=verbose).setup_recast(text)
-
-        elif kwargs['HashtagRecast']['process'] == 'extract':
-            hashtag  = HashtagRecast(kwargs['HashtagRecast']['process'], verbose=verbose).setup_recast(text)
-        
-        elif kwargs['HashtagRecast']['process'] == 'remove':
-           text = HashtagRecast(kwargs['HashtagRecast']['process'], verbose=verbose).setup_recast(text)
-        
-        pbar.update(tcount)
-    
-    if 'ShortWordsRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'ShortWordsRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        text = ShortWordsRecast(kwargs['ShortWordsRecast']['min_length'], verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-
-    if 'StopWordsRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'StopWordsRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        text = StopWordsRecast(kwargs['StopWordsRecast']['package'], kwargs['StopWordsRecast']['stopwords'], verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-
-    if 'NumberRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'NumberRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        global number
-        if kwargs['NumberRecast']['process'] == 'extract_remove' or kwargs['NumberRecast']['process'] == 'extract_replace':
-           text, number  = NumberRecast(kwargs['NumberRecast']['process'], kwargs['NumberRecast']['seperator'], verbose=verbose).setup_recast(text)
-
-        elif kwargs['NumberRecast']['process'] == 'extract':
-            number  = NumberRecast(kwargs['NumberRecast']['process'], kwargs['NumberRecast']['seperator'], verbose=verbose).setup_recast(text)
-        
-        elif kwargs['NumberRecast']['process'] == 'remove' or kwargs['NumberRecast']['process'] == 'replace':
-           text = NumberRecast(kwargs['NumberRecast']['process'], kwargs['NumberRecast']['seperator'], verbose=verbose).setup_recast(text)
-        
-        pbar.update(tcount)
-
-    if 'AlphabetRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'AlphabetRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        text = AlphabetRecast(kwargs['AlphabetRecast']['process'], verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-
-    if 'PunctuationRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'PunctuationRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        text = PunctuationRecast(verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-
-    if 'StemmingRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'StemmingRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        text = StemmingRecast(kwargs['StemmingRecast']['package'], kwargs['StemmingRecast']['method'], verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-
-    if 'LemmatizationRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'LemmatizationRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        text = LemmatizationRecast(kwargs['LemmatizationRecast']['package'], verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-
-    if 'TokenisationRecast' in kwargs:
-
-        ccount +=  1
-        pbar.set_postfix({'TokenisationRecast || TextRecast No': f'{ccount}/{rcount}'})
-
-        global token
-        token = TokenisationRecast(kwargs['TokenisationRecast']['package'], kwargs['TokenisationRecast']['method'], verbose=verbose).setup_recast(text)
-        pbar.update(tcount)
-
-    pbar.set_postfix({'TextRecast Complete! || TextRecast No': f'{ccount}/{rcount}'})
-    pbar.close()
-    
-    return text
-
-
-##############################################################################################################
-
-
-      
-def RecastPipeline(text, recastFuncs, **kwargs):
-
-    ccount = 0 # complete count
-    rcount = len(recastFuncs) # recast count
-    tcount = len(text) # text length count
-
-    chunk_size = rcount * tcount
-    pbar = tqdm(total=chunk_size)
-
-    for rec in recastFuncs:
-        text = rec.setup_recast(text)
-        pbar.update(tcount)
-    
-    return text
+            return self.recast()
```

## Comparing `swachhdata-2.0.0rc1.dist-info/LICENSE.txt` & `swachhdata-2.0.0rc2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `swachhdata-2.0.0rc1.dist-info/METADATA` & `swachhdata-2.0.0rc2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swachhdata
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Data cleaning made easy with swachhdata
 Home-page: https://swachhdata.readthedocs.io/
 Author: Kritik Seth
 Author-email: sethkritik@gmail.com
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 ![](https://raw.githubusercontent.com/swachhdata/swachhdata/main/logo/sd-cover.png)
 
 # swachhdata
 
 [![pypi package](https://badge.fury.io/py/swachhdata.svg)](https://pypi.org/project/swachhdata)
 [![Downloads](https://static.pepy.tech/personalized-badge/swachhdata?period=total&units=international_system&left_color=gray&right_color=blue&left_text=Downloads)](https://pepy.tech/project/swachhdata)
 ![GitHub last commit](https://img.shields.io/github/last-commit/swachhdata/swachhdata?color=green)
-[![GitHub](https://img.shields.io/github/license/kritikseth/swachhdata.svg)](https://github.com/kritikseth/swachhdata/blob/master/LICENSE)
+[![GitHub](https://img.shields.io/github/license/swachhdata/swachhdata.svg)](https://github.com/swachhdata/swachhdata/blob/master/LICENSE)
 
 * Simple and efficient tools for cleaning and transforming data
 * Accessible to everybody, and reusable in various contexts
 * Open source, commercially usable - MPL-2.0 license
 
 ## Documentation-
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swachhdata Version: 2.0.0rc1 Summary: Data cleaning
+Metadata-Version: 2.1 Name: swachhdata Version: 2.0.0rc2 Summary: Data cleaning
 made easy with swachhdata Home-page: https://swachhdata.readthedocs.io/ Author:
 Kritik Seth Author-email: sethkritik@gmail.com Classifier: Natural Language ::
 English Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL
 2.0) Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 6 - Mature Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: regex (>=2019.12.20) Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: tqdm (>=4.41.1) Requires-Dist: beautifulsoup4 (>=4.6.3)
@@ -13,16 +13,16 @@
 raw.githubusercontent.com/swachhdata/swachhdata/main/logo/sd-cover.png) #
 swachhdata [![pypi package](https://badge.fury.io/py/swachhdata.svg)](https://
 pypi.org/project/swachhdata) [![Downloads](https://static.pepy.tech/
 personalized-badge/
 swachhdata?period=total&units=international_system&left_color=gray&right_color=blue&left_text=Downloads)]
 (https://pepy.tech/project/swachhdata) ![GitHub last commit](https://
 img.shields.io/github/last-commit/swachhdata/swachhdata?color=green) [![GitHub]
-(https://img.shields.io/github/license/kritikseth/swachhdata.svg)](https://
-github.com/kritikseth/swachhdata/blob/master/LICENSE) * Simple and efficient
+(https://img.shields.io/github/license/swachhdata/swachhdata.svg)](https://
+github.com/swachhdata/swachhdata/blob/master/LICENSE) * Simple and efficient
 tools for cleaning and transforming data * Accessible to everybody, and
 reusable in various contexts * Open source, commercially usable - MPL-2.0
 license ## Documentation- * https://swachhdata.readthedocs.io/en/latest/ *
 [Examples](https://colab.research.google.com/drive/
 1IH7ve5xoQ4vLyrRP4HvTCYBlj1Ub1GGS?usp=sharing#scrollTo=3Seymy37xQk4) ## Author-
 [Kritik_Seth]
    [https://visitor-badge.glitch.me/badge?page_id=swachhdata.visitor-badge]
```

## Comparing `swachhdata-2.0.0rc1.dist-info/RECORD` & `swachhdata-2.0.0rc2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-swachhdata/__init__.py,sha256=g8MaBSKSiE0Y9g5-dolAX83pg2SasVZYnJcEBGFFpr8,228
+swachhdata/__init__.py,sha256=tVmnoP6DHSiYE4ivVFtlLnco0lsq0yNy0nT8YMtm_vs,228
 swachhdata/compose/__init__.py,sha256=9NKRJN3d38FxfExXwK8L1jfi5IMI5jKqfEtFLt97LO8,106
 swachhdata/compose/core.py,sha256=-jqnUkAcIa8A--eoLGAWyqMKEooOm36bHWvzbrArC9A,1334
 swachhdata/image/__init__.py,sha256=m6pEvV60cN9cj5G-mMsr27F41s6A-IbPNIpmSwFvSmE,131
 swachhdata/image/_image.py,sha256=9RkuFHcWZOSVXWByBfvCnO6hhB19KLwia4QErqr6SY8,7477
-swachhdata/legacy/__init__.py,sha256=MQGn-ahr-9jjg4T_hp1Btl39mSAuw7qw359evKHUnjk,173
-swachhdata/legacy/_text.py,sha256=lQqrPQunEwCeNf0hUBrxBBIp3e7iX-WRovYb0kHi1_4,15947
-swachhdata/text/__init__.py,sha256=w4DSub20tUcvJ5iommCEDw0Fu9Fvx7LQyVqO3Zs15-k,803
-swachhdata/text/_base.py,sha256=-VGYBegK3YrUazPUMNKFB2fwbciUG9KZsMfs-jTHIqo,2196
-swachhdata/text/_text.py,sha256=igBc1yP6nU-xcM9d5ma8Aa9U6EZzy11BGCgB5RaOgUE,74326
+swachhdata/text/__init__.py,sha256=0_QJOrQyMhzfJ6jK9i3lPVzXO7VrQ0Ol7-ghxuxxLmM,726
+swachhdata/text/base.py,sha256=NPrVLcGPhHLbNQuQUiD-uIvG7MEeJJpkYc8Fgk7xD2c,3822
+swachhdata/text/pipeline.py,sha256=wLQuTB_GXCuHjSdHZDUEmierv0sjxr1b5fI7oOBCpRU,1712
+swachhdata/text/recast.py,sha256=FQ3AmobPs1EXM7sSFseQXl79JlpgzwNfJiPgvnmi-nk,63779
 swachhdata/utils/__init__.py,sha256=1ZH0VgYFVYuf0jTP8ncCxPxDnHBOEQ8OZgjy-iuvYlU,642
 swachhdata/utils/exceptions.py,sha256=4_cANml56Jeev2rEq4JDjxnqdK_cE1-ZO_CcFNBBNOU,1114
 swachhdata/utils/probe.py,sha256=q1p-R9CKXnq-eBNVSl1tyADefX64KHrlmxNElzM97TU,377
 swachhdata/utils/recast.py,sha256=WGu3HXRPDyrjXD5pLKfLfjqPBHSdfQezs1Ux4UoQZNA,1150
 swachhdata/utils/tools.py,sha256=1K9ekx8Lqt15GY7RuEH5-wgL_TtMEkEYyevN9KrP03I,480
 swachhdata/utils/verify.py,sha256=GbPuizBw7-BFRPMCLnaHDF2YnsjzABiLFzZzLOmlu10,1310
-swachhdata-2.0.0rc1.dist-info/LICENSE.txt,sha256=k0P1sbYupRWlxoESvbYq2UzoMW6MXA84LltqR-4mEo4,17096
-swachhdata-2.0.0rc1.dist-info/METADATA,sha256=ENM5g6hdyqBicjj04bmvlnq_KzZ6RhFSx_2aScrBFOc,2206
-swachhdata-2.0.0rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-swachhdata-2.0.0rc1.dist-info/top_level.txt,sha256=UPLFTkg5MwIkJLZzEOsLnndE5jByl-BGbZ0_Z40oq0Y,11
-swachhdata-2.0.0rc1.dist-info/RECORD,,
+swachhdata-2.0.0rc2.dist-info/LICENSE.txt,sha256=k0P1sbYupRWlxoESvbYq2UzoMW6MXA84LltqR-4mEo4,17096
+swachhdata-2.0.0rc2.dist-info/METADATA,sha256=ezfNV_MmI_R42NX2KEXuQVfqt50Cq9BtPbZzoZhCEOM,2206
+swachhdata-2.0.0rc2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+swachhdata-2.0.0rc2.dist-info/top_level.txt,sha256=UPLFTkg5MwIkJLZzEOsLnndE5jByl-BGbZ0_Z40oq0Y,11
+swachhdata-2.0.0rc2.dist-info/RECORD,,
```

