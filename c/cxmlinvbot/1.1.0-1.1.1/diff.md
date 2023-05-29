# Comparing `tmp/cxmlinvbot-1.1.0.tar.gz` & `tmp/cxmlinvbot-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxmlinvbot-1.1.0.tar", last modified: Sat May 13 13:34:52 2023, max compression
+gzip compressed data, was "cxmlinvbot-1.1.1.tar", last modified: Mon May 29 15:40:35 2023, max compression
```

## Comparing `cxmlinvbot-1.1.0.tar` & `cxmlinvbot-1.1.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:52.284175 cxmlinvbot-1.1.0/
--rw-rw-rw-   0        0        0      166 2023-05-13 13:34:52.283160 cxmlinvbot-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:51.942665 cxmlinvbot-1.1.0/cxmlinvbot/
--rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.1.0/cxmlinvbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:51.962613 cxmlinvbot-1.1.0/cxmlinvbot/config/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.1.0/cxmlinvbot/config/__init__.py
--rw-rw-rw-   0        0        0     1641 2023-05-13 13:29:31.000000 cxmlinvbot-1.1.0/cxmlinvbot/config/base.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:51.970595 cxmlinvbot-1.1.0/cxmlinvbot/errors/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.1.0/cxmlinvbot/errors/__init__.py
--rw-rw-rw-   0        0        0      445 2023-05-13 12:28:57.000000 cxmlinvbot-1.1.0/cxmlinvbot/errors/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:51.979603 cxmlinvbot-1.1.0/cxmlinvbot/filing/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.1.0/cxmlinvbot/filing/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-05-13 13:12:19.000000 cxmlinvbot-1.1.0/cxmlinvbot/filing/filing.py
--rw-rw-rw-   0        0        0      246 2023-05-06 11:05:58.000000 cxmlinvbot-1.1.0/cxmlinvbot/kill.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:51.988543 cxmlinvbot-1.1.0/cxmlinvbot/mail/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.1.0/cxmlinvbot/mail/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-05-10 18:39:23.000000 cxmlinvbot-1.1.0/cxmlinvbot/mail/mail.py
--rw-rw-rw-   0        0        0     9021 2023-05-13 12:46:13.000000 cxmlinvbot-1.1.0/cxmlinvbot/main.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:52.013478 cxmlinvbot-1.1.0/cxmlinvbot/mapping/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.1.0/cxmlinvbot/mapping/__init__.py
--rw-rw-rw-   0        0        0     1925 2023-05-06 13:49:41.000000 cxmlinvbot-1.1.0/cxmlinvbot/mapping/action.py
--rw-rw-rw-   0        0        0     4712 2023-05-10 12:55:16.000000 cxmlinvbot-1.1.0/cxmlinvbot/mapping/headermapping.py
--rw-rw-rw-   0        0        0    12894 2023-05-10 12:56:37.000000 cxmlinvbot-1.1.0/cxmlinvbot/mapping/invoicedetailrequestmapping.py
--rw-rw-rw-   0        0        0     1046 2023-05-13 12:27:38.000000 cxmlinvbot-1.1.0/cxmlinvbot/mapping/mapping.py
--rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.1.0/cxmlinvbot/mapping/profilerequestmapping.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:52.191813 cxmlinvbot-1.1.0/cxmlinvbot/objects/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.1.0/cxmlinvbot/objects/__init__.py
--rw-rw-rw-   0        0        0     5144 2023-05-06 09:08:47.000000 cxmlinvbot-1.1.0/cxmlinvbot/objects/cxmlobject.py
--rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.1.0/cxmlinvbot/objects/profileresponse.py
--rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.1.0/cxmlinvbot/objects/response.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:52.279170 cxmlinvbot-1.1.0/cxmlinvbot/unittests/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.1.0/cxmlinvbot/unittests/__init__.py
--rw-rw-rw-   0        0        0     2231 2023-05-06 13:49:56.000000 cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_action.py
--rw-rw-rw-   0        0        0     2947 2023-05-06 09:06:03.000000 cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_cxmlobject.py
--rw-rw-rw-   0        0        0     1218 2023-05-13 12:30:12.000000 cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_errors.py
--rw-rw-rw-   0        0        0     2950 2023-05-13 13:26:20.000000 cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_filing.py
--rw-rw-rw-   0        0        0    24304 2023-05-13 12:46:25.000000 cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_main.py
--rw-rw-rw-   0        0        0     2183 2023-05-13 12:30:54.000000 cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_mapping.py
--rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_profileresponse.py
--rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_response.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:51.955633 cxmlinvbot-1.1.0/cxmlinvbot.egg-info/
--rw-rw-rw-   0        0        0      166 2023-05-13 13:34:51.000000 cxmlinvbot-1.1.0/cxmlinvbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2023-05-13 13:34:51.000000 cxmlinvbot-1.1.0/cxmlinvbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 13:34:51.000000 cxmlinvbot-1.1.0/cxmlinvbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-13 13:34:51.000000 cxmlinvbot-1.1.0/cxmlinvbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-13 13:34:51.000000 cxmlinvbot-1.1.0/cxmlinvbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 13:34:52.284175 cxmlinvbot-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-05-13 13:33:59.000000 cxmlinvbot-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:40:35.209355 cxmlinvbot-1.1.1/
+-rw-rw-rw-   0        0        0      166 2023-05-29 15:40:35.208362 cxmlinvbot-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.586148 cxmlinvbot-1.1.1/cxmlinvbot/
+-rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.1.1/cxmlinvbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.606093 cxmlinvbot-1.1.1/cxmlinvbot/config/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.1.1/cxmlinvbot/config/__init__.py
+-rw-rw-rw-   0        0        0     1641 2023-05-29 13:29:14.000000 cxmlinvbot-1.1.1/cxmlinvbot/config/base.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.649975 cxmlinvbot-1.1.1/cxmlinvbot/errors/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.1.1/cxmlinvbot/errors/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-05-13 12:28:57.000000 cxmlinvbot-1.1.1/cxmlinvbot/errors/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.744329 cxmlinvbot-1.1.1/cxmlinvbot/filing/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.1.1/cxmlinvbot/filing/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-05-13 13:12:19.000000 cxmlinvbot-1.1.1/cxmlinvbot/filing/filing.py
+-rw-rw-rw-   0        0        0      246 2023-05-06 11:05:58.000000 cxmlinvbot-1.1.1/cxmlinvbot/kill.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.803489 cxmlinvbot-1.1.1/cxmlinvbot/mail/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.1.1/cxmlinvbot/mail/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-05-10 18:39:23.000000 cxmlinvbot-1.1.1/cxmlinvbot/mail/mail.py
+-rw-rw-rw-   0        0        0     9291 2023-05-29 15:04:38.000000 cxmlinvbot-1.1.1/cxmlinvbot/main.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.937710 cxmlinvbot-1.1.1/cxmlinvbot/mapping/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/__init__.py
+-rw-rw-rw-   0        0        0     2142 2023-05-29 13:24:41.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/action.py
+-rw-rw-rw-   0        0        0     4712 2023-05-10 12:55:16.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/headermapping.py
+-rw-rw-rw-   0        0        0    14134 2023-05-29 15:13:38.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/invoicedetailrequestmapping.py
+-rw-rw-rw-   0        0        0    13884 2023-05-29 15:15:10.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py
+-rw-rw-rw-   0        0        0     1046 2023-05-13 12:27:38.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/mapping.py
+-rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/profilerequestmapping.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:40:35.105129 cxmlinvbot-1.1.1/cxmlinvbot/objects/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.1.1/cxmlinvbot/objects/__init__.py
+-rw-rw-rw-   0        0        0     5144 2023-05-06 09:08:47.000000 cxmlinvbot-1.1.1/cxmlinvbot/objects/cxmlobject.py
+-rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.1.1/cxmlinvbot/objects/profileresponse.py
+-rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.1.1/cxmlinvbot/objects/response.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:40:35.203371 cxmlinvbot-1.1.1/cxmlinvbot/unittests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/__init__.py
+-rw-rw-rw-   0        0        0     2231 2023-05-06 13:49:56.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_action.py
+-rw-rw-rw-   0        0        0     2947 2023-05-06 09:06:03.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_cxmlobject.py
+-rw-rw-rw-   0        0        0     1218 2023-05-13 12:30:12.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_errors.py
+-rw-rw-rw-   0        0        0     2950 2023-05-13 13:26:20.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_filing.py
+-rw-rw-rw-   0        0        0    24937 2023-05-29 15:37:28.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_main.py
+-rw-rw-rw-   0        0        0     2183 2023-05-13 12:30:54.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_mapping.py
+-rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_profileresponse.py
+-rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_response.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.599111 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-05-29 15:40:34.000000 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1207 2023-05-29 15:40:34.000000 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 15:40:34.000000 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-29 15:40:34.000000 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-29 15:40:34.000000 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 15:40:35.210352 cxmlinvbot-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-05-13 13:33:59.000000 cxmlinvbot-1.1.1/setup.py
```

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/config/base.py` & `cxmlinvbot-1.1.1/cxmlinvbot/config/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     PROD_COUPA_END_POINT    = 'https://cbre.coupahost.com/cxml/'
     TEST_COUPA_END_POINT    = 'https://cbre-test.coupahost.com/cxml/'
     PROD_INVOICE_END_POINT  = '%sinvoices/' % PROD_COUPA_END_POINT
     TEST_INVOICE_END_POINT  = '%sinvoices/' % TEST_COUPA_END_POINT
 
     # Miscellania...
     MAIL_PREAMBLE           = 'Pro Door Invoice Bot - '
-    VERSION                 = '1.1.0'
+    VERSION                 = '1.1.1'
 
     # Testing widgets...
     SAMPLE_PATH             = '%sResources\\cXML\\1.2.057\\Samples\\' % EnvConfig.PROJECT_ROOT
     XML_SAMPLES             = {
         'ProfileResponse'           : '%sprofileresponse.xml' % SAMPLE_PATH,
         'ProfileResponseNoDTD'      : '%sprofileresponsenodtd.xml' % SAMPLE_PATH,
         'ProfileResponseInvalidXML' : '%sprofileresponseinvalidxml.xml' % SAMPLE_PATH,
```

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/filing/filing.py` & `cxmlinvbot-1.1.1/cxmlinvbot/filing/filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/mail/mail.py` & `cxmlinvbot-1.1.1/cxmlinvbot/mail/mail.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/main.py` & `cxmlinvbot-1.1.1/cxmlinvbot/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import traceback
 
 from   cxmlinvbot.config.base import BaseConfig
 from   cxmlinvbot.errors.errors import LockedFileError, MapActionError
 from   cxmlinvbot.filing.filing import Archive
 from   cxmlinvbot.mail.mail import Mail
 from   cxmlinvbot.mapping.action import MapActionError
+from   cxmlinvbot.mapping.invoicedetailrequestservicemapping import InvoiceDetailRequestServiceMapping
 from   cxmlinvbot.mapping.invoicedetailrequestmapping import InvoiceDetailRequestMapping
 from   cxmlinvbot.objects.cxmlobject import CXMLObject, CXML_DTDError
 from   cxmlinvbot.objects.response import Response
 from   local.config.env import EnvConfig
 from   local.config.mail import MailConfig
 
 
@@ -29,14 +30,17 @@
     for gf in graceFiles:
         os.remove(gf)
 
 def postCXML(invoice, cxml):
     endPoint = BaseConfig.PROD_INVOICE_END_POINT \
         if EnvConfig.TGT_ENDPOINT == 'production' else BaseConfig.TEST_INVOICE_END_POINT
     
+    if EnvConfig.LOG_CXML_B4_SEND:
+        logger.info(cxml.asXMLString(prettyPrint=True))
+
     # Can raise ConnectionError
     headers = {'Content-Type':'text/xml'}
     r = requests.post(endPoint, headers=headers, data=cxml.asXMLString())
 
     logger.info('Response for cxml from endpoint - %s : %s' % (r.status_code, r.text))
     if r.status_code == 200:
         cxmlResp = Response()
@@ -56,15 +60,15 @@
     invoice = row.get('InvoiceNumber', '')
     if not (type(invoice) == str and len(invoice)):
         return {'UNKNOWN' : 'There are rows in the CSV file without an InvoiceNumber field.'}
     
     logger.info('Processing invoice - %s' % invoice)
     if not cxmlArchive.exists(invoice):
         cxml = CXMLObject()
-        req = InvoiceDetailRequestMapping()
+        req = InvoiceDetailRequestMapping() if row.get('Quantity', True) else InvoiceDetailRequestServiceMapping()
         try:
             cxml.fromPathValueMap(req.perform(row, catchAll=True))
             cxml.validate(req.getDTD_URL())
         except MapActionError as e1:
             logger.error('CSV mapping failed, please correct CSV for missing fields below...')
             logger.error(e1)
             return {invoice : e1}
```

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/mapping/action.py` & `cxmlinvbot-1.1.1/cxmlinvbot/mapping/action.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import datetime
 import logging
+import re
 
 from   cxmlinvbot.errors.errors import MapActionError
 
 logger = logging.getLogger(__name__)
 
+FLOAT_RE = re.compile('[0-9]*\.[0-9]*')
+INT_RE = re.compile('[0-9]*')
+DATE_RE = re.compile('(?P<day>[0-3]?[0-9])/(?P<month>[0-1][0-9])/(?P<year>[0-9]{4})')
 
 class MapAction(object):
     
     def __init__(self, paths=None):
         self._paths = paths if type(paths) == type(()) or type(paths) == list else [paths]
 
     def perform(self, key, nvPairs):
@@ -45,20 +49,20 @@
         for p in self._paths:
 
             args = []
             for k in self._keys:
                 arg = nvPairs.get(k, '')
                 if not len(arg):
                     raise MapActionError('Lambda field %s is missing from invoice CSV.' % k)
-                if '.' in arg:
+                if FLOAT_RE.fullmatch(arg):
                     arg = float(arg)
-                elif '/' in arg:
-                    arg = datetime.datetime.strptime(arg, '%d/%m/%Y')
-                else:
+                elif INT_RE.fullmatch(arg):
                     arg = int(arg)
+                elif DATE_RE.fullmatch(arg):
+                    arg = datetime.datetime.strptime(arg, '%d/%m/%Y')
                 args.append(arg)
             m[p] = str(self._op(*args))
         return m 
 
 
 class Required(MapAction):
```

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/mapping/headermapping.py` & `cxmlinvbot-1.1.1/cxmlinvbot/mapping/headermapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/mapping/invoicedetailrequestmapping.py` & `cxmlinvbot-1.1.1/cxmlinvbot/mapping/invoicedetailrequestmapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import datetime
+import re
 import cxmlinvbot.mapping.action
 
 from   cxmlinvbot.config.base import BaseConfig
 from   cxmlinvbot.mapping.headermapping import HeaderMapping
 from   cxmlinvbot.mapping.mapping import Mapping
 from   local.config.env import EnvConfig
 
 class InvoiceDetailRequestMapping(Mapping):
   
+  VAT_RE = re.compile('(?P<rate>[0-9]*)%.*')
+
   DTD_URL = BaseConfig.INVOICE_DETAIL_DTD_URL
 
   STRUCTURE = HeaderMapping.STRUCTURE + [
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailHeaderIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailLineIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name',
@@ -53,24 +55,29 @@
     #                                'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic'),
     #                                '775685765'),
     InvoiceNumber=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceID'),
     Reference=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference@payloadID'),      
     InvoiceDate=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceDate', lambda d : d.isoformat(), ('InvoiceDate',)),
     #DueDate=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm/Extrinsic'),
     PlannedDate=cxmlinvbot.mapping.action.Ignore(),
-    TaxableAmount=cxmlinvbot.mapping.action.Ignore(),
-    Total=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/GrossAmount/Money'),
+    TaxableAmount=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
+                                          'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
+                                          'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
+                                          'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
+                                          'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money')),
+    Total=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/GrossAmount/Money',
+                                              'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money')),
     TaxTotal=cxmlinvbot.mapping.action.Ignore(),
     InvoiceAmountPaid=cxmlinvbot.mapping.action.Ignore(),
     InvoiceAmountDue=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money'),
     InventoryItemCode=cxmlinvbot.mapping.action.Ignore(),
     Description=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference/Description'),      
     Quantity=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem@quantity'),
     UnitAmount=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitPrice/Money'),
-    UoM=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitOfMeasure', 'Each'),      
+    UoM=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitOfMeasure', lambda m : {'Each':'EA'}.get(m, 'M4'), ('UoM',)),      
     Discount=cxmlinvbot.mapping.action.Ignore(),
     LineAmount=cxmlinvbot.mapping.action.Ignore(),
     TaxType=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Description',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description')),
     #TaxCode=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxRegime',
     #                                'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxRegime'),
     #                                'Standard'),
@@ -114,18 +121,21 @@
     IPRole=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@role', 'remitTo'),
     Language=cxmlinvbot.mapping.action.Default(( 'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference/Description@xml:lang',
                                       'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Description@xml:lang',
                                       'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description@xml:lang',
                                       'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name@xml:lang'), 
                                       'en'), # Standard xmlLangCode
     PayInNumDays=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm@payInNumberOfDays', lambda d1, d2 : str((d1-d2).days), ('DueDate', 'InvoiceDate')),
-    SubTotalAmount=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
-                                          'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
-                                          'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
-                                          'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
-                                          'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money'),
-                                            lambda x, y : str(x * y), ('UnitAmount', 'Quantity')), # we never expect a Quantity > 1 currently            
+    #SubTotalAmount=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
+    #                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
+    #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
+    #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
+    #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money'),
+    #                                        lambda x, y : str(x * y), ('UnitAmount', 'Quantity')), # we never expect a Quantity > 1 currently            
     TaxCat=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail@category',
-                                  'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail@category'),
-                                  'vat'),
+                                              'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail@category'),
+                                              'vat'),
     TaxInline=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailLineIndicator@isTaxInLine', 'yes'),
+    TaxRate=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail@percentageRate',
+                                              'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail@percentageRate'),
+                                              lambda s : InvoiceDetailRequestMapping.VAT_RE.fullmatch(s).group('rate'), ('TaxType',)),
 )]
```

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/mapping/mapping.py` & `cxmlinvbot-1.1.1/cxmlinvbot/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/objects/cxmlobject.py` & `cxmlinvbot-1.1.1/cxmlinvbot/objects/cxmlobject.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/objects/profileresponse.py` & `cxmlinvbot-1.1.1/cxmlinvbot/objects/profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/objects/response.py` & `cxmlinvbot-1.1.1/cxmlinvbot/objects/response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_action.py` & `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_action.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_cxmlobject.py` & `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_cxmlobject.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_errors.py` & `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_errors.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_filing.py` & `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_main.py` & `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -285,22 +285,25 @@
         expectedInvoice = 'inv12345'
         expectedRespCode = 200
         expectedRespText = '<xml %s>OK</xml>'
         expectedEPRespCode = 200
         expectedEPRespText = 'ALL GOOD'
         expectedEPRespData = 'SOME DATA'
         expectedHdrs = {'Content-Type':'text/xml'}
+        mockCXML = MagicMock()
+        mockCXML.asXMLString.return_value = 'CXML'
         expectedLogs = [
+            call.info('CXML'),
             call.info('Response for cxml from endpoint - %s : %s' % (expectedRespCode, expectedRespText%'encoding="UTF-8"'))
         ]
         expectedCXML = [
+            call.asXMLString(prettyPrint=True),
             call.asXMLString(),
             call.asXMLString(prettyPrint=True),
         ]
-        mockCXML = MagicMock()
         mockResp = MagicMock()
         mockResp.status_code = expectedRespCode
         mockResp.text = expectedRespText%'encoding="UTF-8"'
         self.mockPost.side_effect = lambda e, **kwargs : mockResp
         self.mockEPResponse().status = MagicMock()
         self.mockEPResponse().status.code = expectedEPRespCode
         self.mockEPResponse().status.text = expectedEPRespText
@@ -325,59 +328,73 @@
         origEP = EnvConfig.TGT_ENDPOINT
         EnvConfig.TGT_ENDPOINT = 'production'
         expectedInvoice = 'inv12345'
         expectedEx = requests.HTTPError('BAD HTTP')
         expectedRespCode = 999
         expectedRespText = 'FAILED'
         expectedHdrs = {'Content-Type':'text/xml'}
+        mockCXML = MagicMock()
+        mockCXML.asXMLString.return_value = 'CXML'
         expectedLogs = [
+            call.info('CXML'),
             call.info('Response for cxml from endpoint - %s : %s' % (expectedRespCode, expectedRespText))
         ]
-        mockCXML = MagicMock()
+        expectedCXML = [
+            call.asXMLString(prettyPrint=True),
+            call.asXMLString(),
+        ]
         mockResp = MagicMock()
         mockResp.status_code = expectedRespCode
         mockResp.text = expectedRespText
         mockResp.raise_for_status.side_effect = expectedEx
         self.mockPost.side_effect = lambda e, **kwargs : mockResp
         self.assertRaises(requests.HTTPError, postCXML, expectedInvoice, mockCXML)
         EnvConfig.TGT_ENDPOINT = origEP
         self.mockPost.assert_called_once_with(BaseConfig.PROD_INVOICE_END_POINT, headers = expectedHdrs, data=mockCXML.asXMLString.return_value)
-        mockCXML.asXMLString.assert_called_once_with()
+        for c, exc in zip(mockCXML.method_calls, expectedCXML):
+            self.assertEqual(c, exc)
         for c, exc in zip(self.mockLogger.method_calls, expectedLogs):
             self.assertEqual(c, exc)
 
     def testPostCXMLErrorDoc(self):
         self.resetFn('postCXML') 
         origEP = EnvConfig.TGT_ENDPOINT
         EnvConfig.TGT_ENDPOINT = 'test'
         expectedInvoice = 'inv12345'
         expectedRespCode = 200
         expectedRespText = '<xml %s>OK</xml>'
         expectedEPRespCode = 999
         expectedEPRespText = 'BAD DOC'
         expectedEPRespData = 'SOME DATA'
         expectedHdrs = {'Content-Type':'text/xml'}
+        mockCXML = MagicMock()
+        mockCXML.asXMLString.return_value = 'CXML'
         expectedLogs = [
+            call.info('CXML'),
             call.info('Response for cxml from endpoint - %s : %s' % (expectedRespCode, expectedRespText%'encoding="UTF-8"'))
         ]
-        mockCXML = MagicMock()
+        expectedCXML = [
+            call.asXMLString(prettyPrint=True),
+            call.asXMLString(),
+        ]
         mockResp = MagicMock()
         mockResp.status_code = expectedRespCode
         mockResp.text = expectedRespText%'encoding="UTF-8"'
         self.mockPost.side_effect = lambda e, **kwargs : mockResp
         self.mockEPResponse().status = MagicMock()
         self.mockEPResponse().status.code = expectedEPRespCode
         self.mockEPResponse().status.text = expectedEPRespText
         self.mockEPResponse().status.data = expectedEPRespData
         res = postCXML(expectedInvoice, mockCXML)
         EnvConfig.TGT_ENDPOINT = origEP
         self.mockEPResponse.assert_called()
         self.mockEPResponse().fromXMLString.assert_called_once_with(expectedRespText%'')
         self.mockPost.assert_called_once_with(BaseConfig.TEST_INVOICE_END_POINT, headers = expectedHdrs, data=mockCXML.asXMLString.return_value)
-        mockCXML.asXMLString.assert_called_once_with()
+        for c, exc in zip(mockCXML.method_calls, expectedCXML):
+            self.assertEqual(c, exc)
         for c, exc in zip(self.mockLogger.method_calls, expectedLogs):
             self.assertEqual(c, exc)
         self.assertEqual(res, {expectedInvoice : '%s : %s : %s' % (expectedEPRespCode, expectedEPRespText, expectedEPRespData)})
 
     def testMain(self):
         self.resetFn('main')
         expectedFile = 'a_file'
```

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_mapping.py` & `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_profileresponse.py` & `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot/unittests/test_response.py` & `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.0/cxmlinvbot.egg-info/SOURCES.txt` & `cxmlinvbot-1.1.1/cxmlinvbot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 cxmlinvbot/filing/filing.py
 cxmlinvbot/mail/__init__.py
 cxmlinvbot/mail/mail.py
 cxmlinvbot/mapping/__init__.py
 cxmlinvbot/mapping/action.py
 cxmlinvbot/mapping/headermapping.py
 cxmlinvbot/mapping/invoicedetailrequestmapping.py
+cxmlinvbot/mapping/invoicedetailrequestservicemapping.py
 cxmlinvbot/mapping/mapping.py
 cxmlinvbot/mapping/profilerequestmapping.py
 cxmlinvbot/objects/__init__.py
 cxmlinvbot/objects/cxmlobject.py
 cxmlinvbot/objects/profileresponse.py
 cxmlinvbot/objects/response.py
 cxmlinvbot/unittests/__init__.py
```

### Comparing `cxmlinvbot-1.1.0/setup.py` & `cxmlinvbot-1.1.1/setup.py`

 * *Files identical despite different names*

