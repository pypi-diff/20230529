# Comparing `tmp/nonebot_plugin_bilichat-2.0.2.tar.gz` & `tmp/nonebot_plugin_bilichat-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.0.2.tar", last modified: Wed May 17 03:49:46 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.0.3.tar", last modified: Mon May 29 06:08:08 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.0.2.tar` & `nonebot_plugin_bilichat-2.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-05-17 03:49:36.881691 nonebot_plugin_bilichat-2.0.2/LICENSE
--rw-r--r--   0        0        0    11827 2023-05-17 03:49:36.881691 nonebot_plugin_bilichat-2.0.2/README.md
--rw-r--r--   0        0        0     7999 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4805 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1045 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5825 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2343 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1447 2023-05-17 03:49:46.589766 nonebot_plugin_bilichat-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    13164 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-29 06:07:56.779661 nonebot_plugin_bilichat-2.0.3/LICENSE
+-rw-r--r--   0        0        0    11827 2023-05-29 06:07:56.779661 nonebot_plugin_bilichat-2.0.3/README.md
+-rw-r--r--   0        0        0     8102 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4805 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5825 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2343 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-05-29 06:07:56.787661 nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1447 2023-05-29 06:08:08.159655 nonebot_plugin_bilichat-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    13164 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.0.2/LICENSE` & `nonebot_plugin_bilichat-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/README.md` & `nonebot_plugin_bilichat-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 async def video_info(
     bot: BOT,
     event: MESSAGE_EVENT,
     state: T_State,
     matcher: Matcher,
     options: Options = Depends(get_args),
 ):
+    # sourcery skip: hoist-similar-statement-from-if, swap-nested-ifs, use-fstring-for-concatenation
     DISABLE_REPLY = isinstance(bot, Mirai_Bot)  # 部分平台Reply暂不可用
     DISABLE_LINK = isinstance(bot, QG_Bot)  # 部分平台发送链接都要审核
     SEND_IMAGE_SEPARATELY = isinstance(bot, QG_Bot)  # 部分平台无法一次性发送多张图片，或无法与其他消息组合发出
     reply = "" if DISABLE_REPLY else await SegmentBuilder.reply()
     # basic info
     bili_number, uid = state["bili_number"], state["_uid_"]
     if bili_number[:2] in ["BV", "bv", "av"]:
@@ -182,36 +183,36 @@
         raise FinishedException
 
     # get video cache
     try:
         cache = await get_content_cache(info, options)
     except AbortError as e:
         logger.exception(e)
-        await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
+        await matcher.finish(reply + f"视频字幕获取失败: {str(e)}")
     except Exception as e:
         capture_exception()
         logger.exception(e)
-        await matcher.finish(f"{reply}未知错误: {e}")
+        await matcher.finish(reply + f"未知错误: {e}")
 
     # wordcloud
     wc_image = ""
     if plugin_config.bilichat_word_cloud:
         if image := await wordcloud(cache=cache, cid=str(info.cid)):
             wc_image = await SegmentBuilder.image(image=image)
         else:
-            await matcher.finish(f"{reply}视频无有效字幕")
+            await matcher.finish(reply + "视频无有效字幕")
 
     # summary
     summary = ""
     if ENABLE_SUMMARY:
         if summary := await summarization(cache=cache, cid=str(info.cid)):
             if isinstance(summary, bytes):
                 summary = await SegmentBuilder.image(image=summary)
         else:
-            await matcher.finish(f"{reply}视频无有效字幕")
+            await matcher.finish(reply + "视频无有效字幕")
 
     if wc_image:
         if SEND_IMAGE_SEPARATELY:
             await matcher.send(wc_image)
             if summary:
                 await matcher.finish(summary)
         await matcher.finish(reply + wc_image + summary)  # type: ignore
```

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.0.3/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.2/pyproject.toml` & `nonebot_plugin_bilichat-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.0.2"
+version = "2.0.3"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-2.0.2/PKG-INFO` & `nonebot_plugin_bilichat-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.0.2
+Version: 2.0.3
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.0.3 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-segbuilder>=0.2.0 Requires-Dist: nonebot-plugin-
```

