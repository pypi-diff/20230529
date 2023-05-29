# Comparing `tmp/usepy-0.2.3.tar.gz` & `tmp/usepy-0.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usepy-0.2.3.tar", max compression
+gzip compressed data, was "usepy-0.2.3a0.tar", max compression
```

## Comparing `usepy-0.2.3.tar` & `usepy-0.2.3a0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1756 2023-05-17 15:53:32.220015 usepy-0.2.3/README.md
--rw-r--r--   0        0        0      619 2023-05-17 15:53:32.232015 usepy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      129 2023-05-17 15:53:32.232015 usepy-0.2.3/src/usepy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 15:53:32.232015 usepy-0.2.3/src/usepy/contrib/__init__.py
--rw-r--r--   0        0        0     1295 2023-05-17 15:53:32.232015 usepy-0.2.3/src/usepy/contrib/pydantic_.py
--rw-r--r--   0        0        0     2039 2023-05-17 15:53:32.232015 usepy-0.2.3/src/usepy/contrib/tenacity_.py
--rw-r--r--   0        0        0     1290 2023-05-17 15:53:32.232015 usepy-0.2.3/src/usepy/core/__init__.py
--rw-r--r--   0        0        0     5214 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useAddict.py
--rw-r--r--   0        0        0     2075 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useBloomFilter.py
--rw-r--r--   0        0        0      467 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useCachedProperty.py
--rw-r--r--   0        0        0      417 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useCatchError.py
--rw-r--r--   0        0        0      883 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useCleanHtml.py
--rw-r--r--   0        0        0     1059 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useCounter.py
--rw-r--r--   0        0        0     6468 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useDateTime.py
--rw-r--r--   0        0        0     8828 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useDict.py
--rw-r--r--   0        0        0     1529 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useImport.py
--rw-r--r--   0        0        0      692 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useIs.py
--rw-r--r--   0        0        0     9024 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useList.py
--rw-r--r--   0        0        0      419 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useListify.py
--rw-r--r--   0        0        0     2909 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/usePath.py
--rw-r--r--   0        0        0      596 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useRandom.py
--rw-r--r--   0        0        0     1814 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useRetry.py
--rw-r--r--   0        0        0      379 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useRunInThread.py
--rw-r--r--   0        0        0      522 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useSingleton.py
--rw-r--r--   0        0        0     3146 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useString.py
--rw-r--r--   0        0        0      552 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useStringDecode.py
--rw-r--r--   0        0        0      534 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useStringEncode.py
--rw-r--r--   0        0        0      229 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useStringReverse.py
--rw-r--r--   0        0        0     1158 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useThread.py
--rw-r--r--   0        0        0      352 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useTimeIt.py
--rw-r--r--   0        0        0      840 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useTimeout.py
--rw-r--r--   0        0        0     4748 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useTimer.py
--rw-r--r--   0        0        0     1971 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/core/useTo.py
--rw-r--r--   0        0        0      226 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/crawl/__init__.py
--rw-r--r--   0        0        0      221 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/crawl/useCookieToDict.py
--rw-r--r--   0        0        0     3405 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/crawl/useCurl.py
--rw-r--r--   0        0        0      239 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/crawl/useDataToDict.py
--rw-r--r--   0        0        0      267 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/crawl/useHeaderToDict.py
--rw-r--r--   0        0        0     1382 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/crawl/useUrl.py
--rw-r--r--   0        0        0   711543 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/crawl/useUserAgent.py
--rw-r--r--   0        0        0        9 2023-05-17 15:53:32.236015 usepy-0.2.3/src/usepy/integrations/__init__.py
--rw-r--r--   0        0        0      266 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useLogger/__init__.py
--rw-r--r--   0        0        0     2042 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useLogger/formatters.py
--rw-r--r--   0        0        0     1149 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useLogger/handlers.py
--rw-r--r--   0        0        0     2791 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useLogger/intercept.py
--rw-r--r--   0        0        0     2087 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useLogger/logger.py
--rw-r--r--   0        0        0       84 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/__init__.py
--rw-r--r--   0        0        0      219 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/channels/__init__.py
--rw-r--r--   0        0        0      508 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/channels/bark.py
--rw-r--r--   0        0        0      271 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/channels/base.py
--rw-r--r--   0        0        0      597 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/channels/chanify.py
--rw-r--r--   0        0        0      897 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/channels/ding.py
--rw-r--r--   0        0        0     1027 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/channels/email.py
--rw-r--r--   0        0        0      578 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/channels/pushdeer.py
--rw-r--r--   0        0        0      688 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/channels/pushover.py
--rw-r--r--   0        0        0      675 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/channels/wechat.py
--rw-r--r--   0        0        0      534 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/integrations/useNotify/notification.py
--rw-r--r--   0        0        0       82 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/utils/__init__.py
--rw-r--r--   0        0        0      410 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/utils/useFormatSizeof.py
--rw-r--r--   0        0        0      306 2023-05-17 15:53:32.240015 usepy-0.2.3/src/usepy/utils/useFuncName.py
--rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 usepy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1756 2023-05-17 15:00:50.344299 usepy-0.2.3a0/README.md
+-rw-r--r--   0        0        0      530 2023-05-17 15:40:08.683330 usepy-0.2.3a0/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-05-04 13:23:33.839971 usepy-0.2.3a0/src/usepy/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 13:11:06.758012 usepy-0.2.3a0/src/usepy/contrib/__init__.py
+-rw-r--r--   0        0        0     1295 2023-05-04 13:23:33.840151 usepy-0.2.3a0/src/usepy/contrib/pydantic_.py
+-rw-r--r--   0        0        0     2039 2023-03-23 13:11:06.758312 usepy-0.2.3a0/src/usepy/contrib/tenacity_.py
+-rw-r--r--   0        0        0     1290 2023-05-09 15:43:08.433827 usepy-0.2.3a0/src/usepy/core/__init__.py
+-rw-r--r--   0        0        0     5214 2023-05-09 15:43:08.433946 usepy-0.2.3a0/src/usepy/core/useAddict.py
+-rw-r--r--   0        0        0     2075 2023-05-09 15:43:08.434056 usepy-0.2.3a0/src/usepy/core/useBloomFilter.py
+-rw-r--r--   0        0        0      467 2023-05-09 15:43:08.434161 usepy-0.2.3a0/src/usepy/core/useCachedProperty.py
+-rw-r--r--   0        0        0      417 2023-05-09 15:43:08.434259 usepy-0.2.3a0/src/usepy/core/useCatchError.py
+-rw-r--r--   0        0        0      883 2023-05-09 15:43:08.434372 usepy-0.2.3a0/src/usepy/core/useCleanHtml.py
+-rw-r--r--   0        0        0     1059 2023-05-09 15:43:08.434475 usepy-0.2.3a0/src/usepy/core/useCounter.py
+-rw-r--r--   0        0        0     6468 2023-05-17 15:00:50.445229 usepy-0.2.3a0/src/usepy/core/useDateTime.py
+-rw-r--r--   0        0        0     8828 2023-05-17 15:00:50.344835 usepy-0.2.3a0/src/usepy/core/useDict.py
+-rw-r--r--   0        0        0     1529 2023-05-09 15:43:08.435074 usepy-0.2.3a0/src/usepy/core/useImport.py
+-rw-r--r--   0        0        0      692 2023-05-09 15:43:08.435205 usepy-0.2.3a0/src/usepy/core/useIs.py
+-rw-r--r--   0        0        0     9024 2023-05-17 15:00:50.455771 usepy-0.2.3a0/src/usepy/core/useList.py
+-rw-r--r--   0        0        0      419 2023-05-09 15:43:08.435516 usepy-0.2.3a0/src/usepy/core/useListify.py
+-rw-r--r--   0        0        0     2909 2023-05-09 15:43:08.435624 usepy-0.2.3a0/src/usepy/core/usePath.py
+-rw-r--r--   0        0        0      596 2023-05-09 15:43:08.435747 usepy-0.2.3a0/src/usepy/core/useRandom.py
+-rw-r--r--   0        0        0     1814 2023-05-09 15:43:08.436045 usepy-0.2.3a0/src/usepy/core/useRetry.py
+-rw-r--r--   0        0        0      379 2023-05-09 15:43:08.436178 usepy-0.2.3a0/src/usepy/core/useRunInThread.py
+-rw-r--r--   0        0        0      522 2023-05-09 15:43:08.436280 usepy-0.2.3a0/src/usepy/core/useSingleton.py
+-rw-r--r--   0        0        0     3146 2023-05-09 15:43:08.436385 usepy-0.2.3a0/src/usepy/core/useString.py
+-rw-r--r--   0        0        0      552 2023-05-09 15:43:08.436492 usepy-0.2.3a0/src/usepy/core/useStringDecode.py
+-rw-r--r--   0        0        0      534 2023-05-09 15:43:08.436605 usepy-0.2.3a0/src/usepy/core/useStringEncode.py
+-rw-r--r--   0        0        0      229 2023-05-09 15:43:08.436715 usepy-0.2.3a0/src/usepy/core/useStringReverse.py
+-rw-r--r--   0        0        0     1158 2023-05-09 15:43:08.436819 usepy-0.2.3a0/src/usepy/core/useThread.py
+-rw-r--r--   0        0        0      352 2023-05-17 15:00:50.345280 usepy-0.2.3a0/src/usepy/core/useTimeIt.py
+-rw-r--r--   0        0        0      840 2023-05-09 15:43:08.437121 usepy-0.2.3a0/src/usepy/core/useTimeout.py
+-rw-r--r--   0        0        0     4748 2023-05-09 15:43:08.437258 usepy-0.2.3a0/src/usepy/core/useTimer.py
+-rw-r--r--   0        0        0     1971 2023-05-09 15:43:08.437374 usepy-0.2.3a0/src/usepy/core/useTo.py
+-rw-r--r--   0        0        0      226 2023-05-04 13:23:33.843667 usepy-0.2.3a0/src/usepy/crawl/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-09 15:43:08.437484 usepy-0.2.3a0/src/usepy/crawl/useCookieToDict.py
+-rw-r--r--   0        0        0     3405 2023-05-09 15:43:08.437594 usepy-0.2.3a0/src/usepy/crawl/useCurl.py
+-rw-r--r--   0        0        0      239 2023-05-09 15:43:08.437737 usepy-0.2.3a0/src/usepy/crawl/useDataToDict.py
+-rw-r--r--   0        0        0      267 2023-05-09 15:43:08.437925 usepy-0.2.3a0/src/usepy/crawl/useHeaderToDict.py
+-rw-r--r--   0        0        0     1382 2023-05-09 15:43:08.438047 usepy-0.2.3a0/src/usepy/crawl/useUrl.py
+-rw-r--r--   0        0        0   711543 2023-05-09 15:43:08.440768 usepy-0.2.3a0/src/usepy/crawl/useUserAgent.py
+-rw-r--r--   0        0        0        9 2023-05-04 13:23:33.846741 usepy-0.2.3a0/src/usepy/integrations/__init__.py
+-rw-r--r--   0        0        0      266 2023-05-04 13:23:33.846987 usepy-0.2.3a0/src/usepy/integrations/useLogger/__init__.py
+-rw-r--r--   0        0        0     2042 2023-05-04 13:23:33.847128 usepy-0.2.3a0/src/usepy/integrations/useLogger/formatters.py
+-rw-r--r--   0        0        0     1149 2023-05-04 13:23:33.847246 usepy-0.2.3a0/src/usepy/integrations/useLogger/handlers.py
+-rw-r--r--   0        0        0     2791 2023-05-04 13:23:33.847414 usepy-0.2.3a0/src/usepy/integrations/useLogger/intercept.py
+-rw-r--r--   0        0        0     2087 2023-05-04 13:23:33.847571 usepy-0.2.3a0/src/usepy/integrations/useLogger/logger.py
+-rw-r--r--   0        0        0       84 2023-05-04 13:23:33.847813 usepy-0.2.3a0/src/usepy/integrations/useNotify/__init__.py
+-rw-r--r--   0        0        0      219 2023-05-04 13:23:33.848052 usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/__init__.py
+-rw-r--r--   0        0        0      508 2023-05-04 13:23:33.848237 usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/bark.py
+-rw-r--r--   0        0        0      271 2023-05-04 13:23:33.848361 usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/base.py
+-rw-r--r--   0        0        0      597 2023-05-04 13:23:33.848476 usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/chanify.py
+-rw-r--r--   0        0        0      897 2023-05-04 13:23:33.848593 usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/ding.py
+-rw-r--r--   0        0        0     1027 2023-05-04 13:23:33.848715 usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/email.py
+-rw-r--r--   0        0        0      578 2023-05-04 13:23:33.848823 usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/pushdeer.py
+-rw-r--r--   0        0        0      688 2023-05-04 13:23:33.849017 usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/pushover.py
+-rw-r--r--   0        0        0      675 2023-05-04 13:23:33.849148 usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/wechat.py
+-rw-r--r--   0        0        0      534 2023-05-04 13:23:33.849253 usepy-0.2.3a0/src/usepy/integrations/useNotify/notification.py
+-rw-r--r--   0        0        0       82 2023-05-09 15:43:08.441262 usepy-0.2.3a0/src/usepy/utils/__init__.py
+-rw-r--r--   0        0        0      410 2023-05-09 15:43:08.441504 usepy-0.2.3a0/src/usepy/utils/useFormatSizeof.py
+-rw-r--r--   0        0        0      306 2023-05-09 15:43:08.441728 usepy-0.2.3a0/src/usepy/utils/useFuncName.py
+-rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 usepy-0.2.3a0/PKG-INFO
```

### Comparing `usepy-0.2.3/README.md` & `usepy-0.2.3a0/README.md`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/pyproject.toml` & `usepy-0.2.3a0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usepy"
-version = "0.2.3"
+version = "0.2.3a0"
 description = "usepy"
 homepage = "https://usepy.code05.com/"
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'usepy', from = 'src' }
 ]
@@ -15,15 +15,12 @@
     { version = "^4.0.0", python = ">=3.6,<3.7" },
     { version = "^4.5.0", python = ">=3.7" }
 ]
 
 
 
 [tool.poetry.group.test.dependencies]
-pytest = [
-    { version = "^7.0.0", python = ">=3.6,<3.7" },
-    { version = "^7.3.1", python = ">=3.7" }
-]
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `usepy-0.2.3/src/usepy/contrib/pydantic_.py` & `usepy-0.2.3a0/src/usepy/contrib/pydantic_.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/contrib/tenacity_.py` & `usepy-0.2.3a0/src/usepy/contrib/tenacity_.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/__init__.py` & `usepy-0.2.3a0/src/usepy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useAddict.py` & `usepy-0.2.3a0/src/usepy/core/useAddict.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useBloomFilter.py` & `usepy-0.2.3a0/src/usepy/core/useBloomFilter.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useCleanHtml.py` & `usepy-0.2.3a0/src/usepy/core/useCleanHtml.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useCounter.py` & `usepy-0.2.3a0/src/usepy/core/useCounter.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useDateTime.py` & `usepy-0.2.3a0/src/usepy/core/useDateTime.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useDict.py` & `usepy-0.2.3a0/src/usepy/core/useDict.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useImport.py` & `usepy-0.2.3a0/src/usepy/core/useImport.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useIs.py` & `usepy-0.2.3a0/src/usepy/core/useIs.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useList.py` & `usepy-0.2.3a0/src/usepy/core/useList.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/usePath.py` & `usepy-0.2.3a0/src/usepy/core/usePath.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useRandom.py` & `usepy-0.2.3a0/src/usepy/core/useRandom.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useRetry.py` & `usepy-0.2.3a0/src/usepy/core/useRetry.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useSingleton.py` & `usepy-0.2.3a0/src/usepy/core/useSingleton.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useString.py` & `usepy-0.2.3a0/src/usepy/core/useString.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useStringDecode.py` & `usepy-0.2.3a0/src/usepy/core/useStringDecode.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useStringEncode.py` & `usepy-0.2.3a0/src/usepy/core/useStringEncode.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useThread.py` & `usepy-0.2.3a0/src/usepy/core/useThread.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useTimeout.py` & `usepy-0.2.3a0/src/usepy/core/useTimeout.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useTimer.py` & `usepy-0.2.3a0/src/usepy/core/useTimer.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/core/useTo.py` & `usepy-0.2.3a0/src/usepy/core/useTo.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/crawl/useCurl.py` & `usepy-0.2.3a0/src/usepy/crawl/useCurl.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/crawl/useUrl.py` & `usepy-0.2.3a0/src/usepy/crawl/useUrl.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/crawl/useUserAgent.py` & `usepy-0.2.3a0/src/usepy/crawl/useUserAgent.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useLogger/formatters.py` & `usepy-0.2.3a0/src/usepy/integrations/useLogger/formatters.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useLogger/handlers.py` & `usepy-0.2.3a0/src/usepy/integrations/useLogger/handlers.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useLogger/intercept.py` & `usepy-0.2.3a0/src/usepy/integrations/useLogger/intercept.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useLogger/logger.py` & `usepy-0.2.3a0/src/usepy/integrations/useLogger/logger.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useNotify/channels/chanify.py` & `usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/chanify.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useNotify/channels/ding.py` & `usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/ding.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useNotify/channels/email.py` & `usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/email.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useNotify/channels/pushdeer.py` & `usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/pushdeer.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useNotify/channels/pushover.py` & `usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/pushover.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useNotify/channels/wechat.py` & `usepy-0.2.3a0/src/usepy/integrations/useNotify/channels/wechat.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/src/usepy/integrations/useNotify/notification.py` & `usepy-0.2.3a0/src/usepy/integrations/useNotify/notification.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.3/PKG-INFO` & `usepy-0.2.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usepy
-Version: 0.2.3
+Version: 0.2.3a0
 Summary: usepy
 Home-page: https://usepy.code05.com/
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usepy Version: 0.2.3 Summary: usepy Home-page:
+Metadata-Version: 2.1 Name: usepy Version: 0.2.3a0 Summary: usepy Home-page:
 https://usepy.code05.com/ Author: miclon Author-email: jcnd@163.com Requires-
 Python: >=3.6,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: typing-extensions (>=4.0.0,<5.0.0) ; python_version >= "3.6" and
```

