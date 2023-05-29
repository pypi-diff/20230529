# Comparing `tmp/nonebot_plugin_multincm-0.3.1.tar.gz` & `tmp/nonebot_plugin_multincm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.3.1.tar", last modified: Sat May 27 22:18:39 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.3.2.tar", last modified: Mon May 29 16:49:23 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.3.1.tar` & `nonebot_plugin_multincm-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/LICENSE
--rw-r--r--   0        0        0     7380 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/README.md
--rw-r--r--   0        0        0     1646 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0    11552 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      512 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0      134 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/const.py
--rw-r--r--   0        0        0     5500 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0    11669 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2957 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0     2228 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/msg_cache.py
--rw-r--r--   0        0        0   212591 2023-05-27 22:18:17.117726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     3007 2023-05-27 22:18:17.117726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      851 2023-05-27 22:18:17.117726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      867 2023-05-27 22:18:39.233830 nonebot_plugin_multincm-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8330 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8147 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/README.md
+-rw-r--r--   0        0        0     1646 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0    12064 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      582 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0      134 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/const.py
+-rw-r--r--   0        0        0     5556 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0    11669 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2957 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0     2279 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/msg_cache.py
+-rw-r--r--   0        0        0   212591 2023-05-29 16:49:10.291833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0     3007 2023-05-29 16:49:10.291833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      851 2023-05-29 16:49:10.291833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      867 2023-05-29 16:49:23.299930 nonebot_plugin_multincm-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9097 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.2/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.3.1/LICENSE` & `nonebot_plugin_multincm-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.1/README.md` & `nonebot_plugin_multincm-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 </div>
 
 ## 📖 介绍
 
 一个网易云多选点歌插件，可以翻页，可以登录网易云账号点 vip 歌曲听（插件发送的是自定义音乐卡片），没了
 
+插件获取的是音乐播放链接，不会消耗会员每月下载次数
+
 ### 效果图
 
 <details>
 <summary>歌曲列表效果图（点击展开）</summary>
 
 ![pic](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/QQ图片20230515025601.jpg)
 
@@ -130,25 +132,27 @@
 
 如果你安装了 [nonebot-plugin-ncm](https://github.com/kitUIN/nonebot-plugin-ncm)，本插件会与其共用同一个 Session，就可以不用填下面的账号密码了
 
 下面配置中，手机号登录 和 邮箱登录、明文密码 和 MD5 密码哈希 各选其一填写即可
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|        配置项        | 必填 | 默认值 |                  说明                   |
-| :------------------: | :--: | :----: | :-------------------------------------: |
-|     `NCM_CTCODE`     |  否  |  `86`  |       手机号登录用，登录手机区号        |
-|     `NCM_PHONE`      |  否  |   无   |        手机号登录用，登录手机号         |
-|     `NCM_EMAIL`      |  否  |   无   |          邮箱登录用，登录邮箱           |
-|    `NCM_PASSWORD`    |  否  |   无   |   帐号明文密码，邮箱登录时为邮箱密码    |
-| `NCM_PASSWORD_HASH`  |  否  |   无   | 帐号密码 MD5 哈希，邮箱登录时为邮箱密码 |
-|   `NCM_LIST_LIMIT`   |  否  |  `20`  |         歌曲列表每页的最大数量          |
-|   `NCM_LIST_FONT`    |  否  |   无   |         渲染歌曲列表使用的字体          |
-|  `NCM_MAX_NAME_LEN`  |  否  | `600`  | 歌曲列表中歌名列的最大文本宽度（像素）  |
-| `NCM_MAX_ARTIST_LEN` |  否  | `400`  | 歌曲列表中歌手列的最大文本宽度（像素）  |
+|        配置项        | 必填 | 默认值  |                               说明                                |
+| :------------------: | :--: | :-----: | :---------------------------------------------------------------: |
+|     `NCM_CTCODE`     |  否  |  `86`   |                    手机号登录用，登录手机区号                     |
+|     `NCM_PHONE`      |  否  |   无    |                     手机号登录用，登录手机号                      |
+|     `NCM_EMAIL`      |  否  |   无    |                       邮箱登录用，登录邮箱                        |
+|    `NCM_PASSWORD`    |  否  |   无    |                帐号明文密码，邮箱登录时为邮箱密码                 |
+| `NCM_PASSWORD_HASH`  |  否  |   无    |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
+|   `NCM_LIST_LIMIT`   |  否  |  `20`   |                      歌曲列表每页的最大数量                       |
+|   `NCM_LIST_FONT`    |  否  |   无    |                      渲染歌曲列表使用的字体                       |
+|  `NCM_MAX_NAME_LEN`  |  否  |  `600`  |              歌曲列表中歌名列的最大文本宽度（像素）               |
+| `NCM_MAX_ARTIST_LEN` |  否  |  `400`  |              歌曲列表中歌手列的最大文本宽度（像素）               |
+| `NCM_MSG_CACHE_TIME` |  否  | `3600`  | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
+|  `NCM_AUTO_RESOLVE`  |  否  | `False` |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
 
 ## 🎉 使用
 
 ### 指令
 
 - 点歌 [歌曲名 / 音乐 ID]
   - 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐
@@ -208,14 +212,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.2
+
+- 新增配置项 `NCM_MSG_CACHE_TIME`、`NCM_AUTO_RESOLVE`
+- 调整登录流程到 `driver.on_startup` 中
+
 ### 0.3.1
 
 - 修复电台相关 bug
 
 ### 0.3.0
 
 - 支持电台节目的解析与点播
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
    # NoneBot-Plugin-MultiNCM _â¨ ç½æäºå¤éç¹æ­ â¨_ [python] [pdm-
                              managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç»
 ä¸ä¸ªç½æäºå¤éç¹æ­æä»¶ï¼å¯ä»¥ç¿»é¡µï¼å¯ä»¥ç»å½ç½æäºè´¦å·ç¹
-vip æ­æ²å¬ï¼æä»¶åéçæ¯èªå®ä¹é³ä¹å¡çï¼ï¼æ²¡äº ###
+vip æ­æ²å¬ï¼æä»¶åéçæ¯èªå®ä¹é³ä¹å¡çï¼ï¼æ²¡äº
+æä»¶è·åçæ¯é³ä¹æ­æ¾é¾æ¥ï¼ä¸ä¼æ¶èä¼åæ¯æä¸è½½æ¬¡æ° ###
 ææå¾  æ­æ²åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
 QQå¾ç20230515025601.jpg)   çµå°åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic]
 (https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
 QQå¾ç20230519034438.jpg)   æ­è¯ææå¾ï¼ç¹å»å±å¼ï¼ ![pic](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
 QQå¾ç20230519034757.png)  ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³
@@ -26,28 +27,32 @@
 "nonebot_plugin_multincm" ] ```  ## âï¸ éç½® å¦æä½ å®è£äº [nonebot-
 plugin-ncm](https://github.com/kitUIN/nonebot-plugin-
 ncm)ï¼æ¬æä»¶ä¼ä¸å¶å±ç¨åä¸ä¸ª
 Sessionï¼å°±å¯ä»¥ä¸ç¨å¡«ä¸é¢çè´¦å·å¯ç äº
 ä¸é¢éç½®ä¸­ï¼ææºå·ç»å½ å é®ç®±ç»å½ãææå¯ç  å MD5
 å¯ç åå¸ åéå¶ä¸å¡«åå³å¯ å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | | :------------------: | :--: | :----: | :----------------------------
----------: | | `NCM_CTCODE` | å¦ | `86` |
+è¯´æ | | :------------------: | :--: | :-----: | :---------------------------
+------------------------------------: | | `NCM_CTCODE` | å¦ | `86` |
 ææºå·ç»å½ç¨ï¼ç»å½ææºåºå· | | `NCM_PHONE` | å¦ | æ  |
 ææºå·ç»å½ç¨ï¼ç»å½ææºå· | | `NCM_EMAIL` | å¦ | æ  |
 é®ç®±ç»å½ç¨ï¼ç»å½é®ç®± | | `NCM_PASSWORD` | å¦ | æ  |
 å¸å·ææå¯ç ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | | `NCM_PASSWORD_HASH` |
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
-æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | ## ð ä½¿ç¨ ###
-æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
+æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
+`NCM_MSG_CACHE_TIME` | å¦ | `3600` | ç¼å­ Bot å·²åéé³ä¹å¡ççé³ä¹
+ID å ç¨æ·æè¿ä¸æ¬¡æä½ çæ¶é¿ï¼ç§ï¼ | | `NCM_AUTO_RESOLVE` | å¦
+| `False` |
+å½ç¨æ·åéé³ä¹é¾æ¥æ¶ï¼æ¯å¦èªå¨è§£æå¹¶åéé³ä¹å¡ç | ##
+ð ä½¿ç¨ ### æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
 ä»ç»ï¼æç´¢æ­æ²ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
 å«åï¼`ç½æäº`ã`wyy` - çµå° [æ­æ²å / èç® ID] -
 ä»ç»ï¼æç´¢çµå°èç®ãå½è¾å¥çµå° ID æ¶ä¼ç´æ¥åéå¯¹åºèç®
 - å«åï¼`å£°é³`ã`ç½æçµå°`ã`wydt`ã`wydj` - è§£æ [åå¤
 é³ä¹å¡ç / é¾æ¥] - ä»ç»ï¼è·åè¯¥ é³ä¹ / çµå°èç®
 çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
 å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ [åå¤ é³ä¹å¡ç / é¾æ¥] -
@@ -66,17 +71,18 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ###
-0.3.0 - æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 -
-`è§£æ`ã`æ­è¯`ã`é¾æ¥` æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot
-åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.2 - æ°å¢éç½®é¡¹
+`NCM_MSG_CACHE_TIME`ã`NCM_AUTO_RESOLVE` - è°æ´ç»å½æµç¨å°
+`driver.on_startup` ä¸­ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ### 0.3.0 -
+æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
+æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
 æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
 ç°å¨æä»¶ä¼å®æ¶æ¸çèªèº«åå­ä¸­çç¼å­äº ### 0.2.4 -
 ä¿®å¤ä¸ä¸ªæ­è¯è§£æ bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
 å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
 å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
 `è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

### Comparing `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/__init__.py` & `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nonebot.plugin import PluginMetadata, require
 
 require("nonebot_plugin_apscheduler")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 __plugin_meta__ = PluginMetadata(
     "MultiNCM",
     "网易云多选点歌",
     (
         "指令列表：\n"
         "▶ 点歌 [歌曲名 / 音乐 ID]\n"
         "    ▷ 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐\n"
```

### Comparing `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Optional,
     Tuple,
     Union,
     cast,
     overload,
 )
 
-from nonebot import logger, on_command
+from nonebot import logger, on_command, on_regex
 from nonebot.adapters.onebot.v11 import (
     Bot,
     Event,
     GroupMessageEvent,
     Message,
     MessageEvent,
     MessageSegment,
@@ -61,16 +61,16 @@
     "voice": ("dj", "program"),
 }
 
 link_types: List[str] = []
 [link_types.extend(x) for x in LINK_TYPE_MAP.values()]
 link_type_reg = "|".join(link_types)
 
-SONG_ID_REGEX = re.compile(
-    rf"music\.163\.com(.*?)(?P<type>{link_type_reg})/?\?id=(?P<id>[0-9]+)(|&)",
+SONG_ID_REGEX = (
+    rf"music\.163\.com(.*?)(?P<type>{link_type_reg})/?\?id=(?P<id>[0-9]+)(|&)"
 )
 
 
 def get_chat_cache_key(event: MessageEvent) -> str:
     g = event.group_id if isinstance(event, GroupMessageEvent) else 0
     return f"{g}.{event.user_id}"
 
@@ -89,51 +89,57 @@
     type_name = type_name.lower()
     for k, v in LINK_TYPE_MAP.items():
         if type_name in v:
             return cast(Any, k)
     raise ValueError(f"invalid type {type_name}")
 
 
-async def reply_music_rule(event: MessageEvent, state: T_State) -> bool:
-    if reply := event.reply:
-        res = re.search(SONG_ID_REGEX, str(reply.message))
-        if res:
-            type_name = None
-            with suppress(ValueError):
-                type_name = get_type_from_url_type(res["type"])
+async def msg_or_reply_music_rule(event: MessageEvent, state: T_State) -> bool:
+    check_reply: bool = state.get("check_reply", True)
+    message = event.reply.message if (check_reply and event.reply) else event.message
+
+    res = re.search(SONG_ID_REGEX, str(message))
+    if res:
+        type_name = None
+        with suppress(ValueError):
+            type_name = get_type_from_url_type(res["type"])
 
-            if type_name:
-                state["song_cache"] = SongCache(id=int(res["id"]), type=type_name)
-                return True
+        if type_name:
+            state["song_cache"] = SongCache(id=int(res["id"]), type=type_name)
+            return True
 
     return False
 
 
 async def chat_last_music_rule(event: MessageEvent, state: T_State) -> bool:
     if song_cache := chat_last_song_cache.get(get_chat_cache_key(event)):
         state["song_cache"] = song_cache
         return True
 
     return False
 
 
+async def auto_resolve_rule():
+    return config.ncm_auto_resolve
+
+
 def any_rule(*rules: Union[T_RuleChecker, Rule]) -> Callable[..., Awaitable[bool]]:
     async def rule(bot: Bot, event: Event, state: T_State):
         # 要按顺序执行，所以不能用 asyncio.gather
         for x in rules:  # noqa: SIM110
             if await Rule(x)(bot, event, state):
                 return True
         return False
 
     return rule
 
 
 music_msg_matcher_rule = any_rule(
     cache_music_msg_rule,
-    reply_music_rule,
+    msg_or_reply_music_rule,
     chat_last_music_rule,
 )
 
 
 async def send_music(matcher: Matcher, song: SongInfo):
     is_song = isinstance(song, Song)
     calling = CALLING_MAP["song" if is_song else "voice"]
@@ -337,21 +343,31 @@
 
 
 cmd_get_song = on_command(
     "解析",
     aliases={"resolve", "parse", "get"},
     rule=music_msg_matcher_rule,
 )
+reg_song_url = on_regex(
+    SONG_ID_REGEX,
+    rule=Rule(auto_resolve_rule) & msg_or_reply_music_rule,
+    state={"check_reply": False, "tip_user": True},
+)
 
 
 @cmd_get_song.handle()
+@reg_song_url.handle()
 async def _(matcher: Matcher, state: T_State):
     song_cache: SongCache = state["song_cache"]
     calling = CALLING_MAP[song_cache.type]
 
+    tip_user = state.get("tip_user", False)
+    if tip_user:
+        await matcher.send("检测到您发送了网易云音乐卡片/链接，正在为您解析播放链接")
+
     try:
         if song_cache.type == "voice":
             song = await get_voice_info(song_cache.id)
         else:
             song = await get_track_info([song_cache.id])
             song = song[0] if song else None
     except:
```

### Comparing `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/data_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from typing import Any, Callable, Dict, List, cast
 
 import anyio
 from nonebot import get_available_plugin_names, logger, require
 from pyncm import (
     DumpSessionAsString,
     GetCurrentSession,
@@ -91,15 +90,15 @@
     privileges = {y.id: y for y in [Privilege(**x) for x in res["privileges"]]}
     return [
         Song(
             **x,
             privilege=(
                 privileges[song_id]
                 if (song_id := x["id"]) in privileges
-                else Privilege(id=song_id, pl=128000, plLevel="standard")
+                else Privilege(id=song_id, pl=128000)  # , plLevel="standard")
             ),
         )
         for x in res["songs"]
     ]
 
 
 async def get_track_lrc(song_id: int) -> LyricData:
@@ -114,15 +113,15 @@
 
     res = await ncm_request(GetProgramDetail)
     return VoiceBaseInfo(**res["program"])
 
 
 async def login(retry=True):
     if SESSION_FILE.exists():
-        logger.info(f"使用缓存登录态 ({str(SESSION_FILE)})")
+        logger.info(f"使用缓存登录态 ({SESSION_FILE})")
         SetCurrentSession(
             LoadSessionFromString(
                 (await anyio.Path(SESSION_FILE).read_text(encoding="u8")),
             ),
         )
 
     elif (config.ncm_phone or config.ncm_email) and (
@@ -175,9 +174,16 @@
     session = GetCurrentSession()
     logger.info(f"登录成功，欢迎您，{session.nickname} [{session.uid}]")
 
 
 if "nonebot-plugin-ncm" in get_available_plugin_names():
     logger.info("nonebot-plugin-ncm 已安装，本插件将依赖其全局 Session")
     require("nonebot-plugin-ncm")
+
 else:
-    asyncio.get_event_loop().run_until_complete(login())
+    from nonebot import get_driver
+
+    driver = get_driver()
+
+    @driver.on_startup
+    async def _():
+        await login()
```

### Comparing `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/lrc_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/msg_cache.py` & `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/msg_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import time
 from dataclasses import dataclass
 from typing import Dict, Generic, Iterable, Literal, Optional, Tuple, TypeVar, overload
 
 from nonebot_plugin_apscheduler import scheduler
 
+from .config import config
+
 KT = TypeVar("KT")
 VT = TypeVar("VT")
 
 SongType = Literal["song", "voice"]
 
 CALLING_MAP: Dict[SongType, str] = {
     "song": "歌曲",
@@ -20,15 +22,15 @@
     id: int  # noqa: A003
     type: SongType  # noqa: A003
 
 
 # “优雅”
 class CacheManager(Generic[KT, VT], Dict[KT, Tuple[float, VT]]):
     def __init__(self, *args, **kwargs):
-        self._job = scheduler.add_job(self.clear_expired, "interval", hours=1)
+        self._job = scheduler.add_job(self.clear_expired, "interval", minutes=1)
         super().__init__(*args, **kwargs)
 
     def __del__(self):
         scheduler.remove_job(self._job)
 
     def __getitem__(self, __key: KT) -> VT:
         return super().__getitem__(__key)[1]
@@ -72,13 +74,13 @@
             return super().pop(__key)[1]
         except KeyError:
             return __default
 
     def clear_expired(self):
         now_t = time.time()
         for k, (create_t, _) in self.copy().items():
-            if now_t - create_t >= 3600:
+            if now_t - create_t >= config.ncm_msg_cache_time:
                 del self[k]
 
 
 song_msg_id_cache: CacheManager[int, SongCache] = CacheManager()
 chat_last_song_cache: CacheManager[str, SongCache] = CacheManager()
```

### Comparing `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Literal, Optional, Union
 
 from pydantic import BaseModel
 
-BrLevel = Literal["hires", "lossless", "exhigh", "higher", "standard"]
+BrLevel = Literal["hires", "lossless", "exhigh", "higher", "standard", "none"]
 
 SearchResult = Union["SongSearchResult", "VoiceSearchResult"]
 SongInfo = Union["Song", "VoiceBaseInfo"]
 
 
 class Artist(BaseModel):
     id: int  # noqa: A003
@@ -21,15 +21,15 @@
     picUrl: str  # noqa: N815
     tns: List[str]
 
 
 class Privilege(BaseModel):
     id: int  # noqa: A003
     pl: int
-    plLevel: Optional[BrLevel]  # noqa: N815
+    # plLevel: BrLevel  # noqa: N815
 
 
 class Song(BaseModel):
     name: str
     id: int  # noqa: A003
     ar: List[Artist]
     alia: List[str]
```

### Comparing `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.1/pyproject.toml` & `nonebot_plugin_multincm-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.3.1"
+version = "0.3.2"
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot_plugin_multincm-0.3.1/PKG-INFO` & `nonebot_plugin_multincm-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.3.1
+Version: 0.3.2
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0-rc.1
@@ -62,14 +62,16 @@
 
 </div>
 
 ## 📖 介绍
 
 一个网易云多选点歌插件，可以翻页，可以登录网易云账号点 vip 歌曲听（插件发送的是自定义音乐卡片），没了
 
+插件获取的是音乐播放链接，不会消耗会员每月下载次数
+
 ### 效果图
 
 <details>
 <summary>歌曲列表效果图（点击展开）</summary>
 
 ![pic](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/QQ图片20230515025601.jpg)
 
@@ -156,25 +158,27 @@
 
 如果你安装了 [nonebot-plugin-ncm](https://github.com/kitUIN/nonebot-plugin-ncm)，本插件会与其共用同一个 Session，就可以不用填下面的账号密码了
 
 下面配置中，手机号登录 和 邮箱登录、明文密码 和 MD5 密码哈希 各选其一填写即可
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|        配置项        | 必填 | 默认值 |                  说明                   |
-| :------------------: | :--: | :----: | :-------------------------------------: |
-|     `NCM_CTCODE`     |  否  |  `86`  |       手机号登录用，登录手机区号        |
-|     `NCM_PHONE`      |  否  |   无   |        手机号登录用，登录手机号         |
-|     `NCM_EMAIL`      |  否  |   无   |          邮箱登录用，登录邮箱           |
-|    `NCM_PASSWORD`    |  否  |   无   |   帐号明文密码，邮箱登录时为邮箱密码    |
-| `NCM_PASSWORD_HASH`  |  否  |   无   | 帐号密码 MD5 哈希，邮箱登录时为邮箱密码 |
-|   `NCM_LIST_LIMIT`   |  否  |  `20`  |         歌曲列表每页的最大数量          |
-|   `NCM_LIST_FONT`    |  否  |   无   |         渲染歌曲列表使用的字体          |
-|  `NCM_MAX_NAME_LEN`  |  否  | `600`  | 歌曲列表中歌名列的最大文本宽度（像素）  |
-| `NCM_MAX_ARTIST_LEN` |  否  | `400`  | 歌曲列表中歌手列的最大文本宽度（像素）  |
+|        配置项        | 必填 | 默认值  |                               说明                                |
+| :------------------: | :--: | :-----: | :---------------------------------------------------------------: |
+|     `NCM_CTCODE`     |  否  |  `86`   |                    手机号登录用，登录手机区号                     |
+|     `NCM_PHONE`      |  否  |   无    |                     手机号登录用，登录手机号                      |
+|     `NCM_EMAIL`      |  否  |   无    |                       邮箱登录用，登录邮箱                        |
+|    `NCM_PASSWORD`    |  否  |   无    |                帐号明文密码，邮箱登录时为邮箱密码                 |
+| `NCM_PASSWORD_HASH`  |  否  |   无    |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
+|   `NCM_LIST_LIMIT`   |  否  |  `20`   |                      歌曲列表每页的最大数量                       |
+|   `NCM_LIST_FONT`    |  否  |   无    |                      渲染歌曲列表使用的字体                       |
+|  `NCM_MAX_NAME_LEN`  |  否  |  `600`  |              歌曲列表中歌名列的最大文本宽度（像素）               |
+| `NCM_MAX_ARTIST_LEN` |  否  |  `400`  |              歌曲列表中歌手列的最大文本宽度（像素）               |
+| `NCM_MSG_CACHE_TIME` |  否  | `3600`  | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
+|  `NCM_AUTO_RESOLVE`  |  否  | `False` |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
 
 ## 🎉 使用
 
 ### 指令
 
 - 点歌 [歌曲名 / 音乐 ID]
   - 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐
@@ -234,14 +238,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.2
+
+- 新增配置项 `NCM_MSG_CACHE_TIME`、`NCM_AUTO_RESOLVE`
+- 调整登录流程到 `driver.on_startup` 中
+
 ### 0.3.1
 
 - 修复电台相关 bug
 
 ### 0.3.0
 
 - 支持电台节目的解析与点播
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.1 Summary: NCM
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.2 Summary: NCM
 Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
 Dist: pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
@@ -15,15 +15,16 @@
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
    # NoneBot-Plugin-MultiNCM _â¨ ç½æäºå¤éç¹æ­ â¨_ [python] [pdm-
                              managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç»
 ä¸ä¸ªç½æäºå¤éç¹æ­æä»¶ï¼å¯ä»¥ç¿»é¡µï¼å¯ä»¥ç»å½ç½æäºè´¦å·ç¹
-vip æ­æ²å¬ï¼æä»¶åéçæ¯èªå®ä¹é³ä¹å¡çï¼ï¼æ²¡äº ###
+vip æ­æ²å¬ï¼æä»¶åéçæ¯èªå®ä¹é³ä¹å¡çï¼ï¼æ²¡äº
+æä»¶è·åçæ¯é³ä¹æ­æ¾é¾æ¥ï¼ä¸ä¼æ¶èä¼åæ¯æä¸è½½æ¬¡æ° ###
 ææå¾  æ­æ²åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
 QQå¾ç20230515025601.jpg)   çµå°åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic]
 (https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
 QQå¾ç20230519034438.jpg)   æ­è¯ææå¾ï¼ç¹å»å±å¼ï¼ ![pic](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
 QQå¾ç20230519034757.png)  ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³
@@ -40,28 +41,32 @@
 "nonebot_plugin_multincm" ] ```  ## âï¸ éç½® å¦æä½ å®è£äº [nonebot-
 plugin-ncm](https://github.com/kitUIN/nonebot-plugin-
 ncm)ï¼æ¬æä»¶ä¼ä¸å¶å±ç¨åä¸ä¸ª
 Sessionï¼å°±å¯ä»¥ä¸ç¨å¡«ä¸é¢çè´¦å·å¯ç äº
 ä¸é¢éç½®ä¸­ï¼ææºå·ç»å½ å é®ç®±ç»å½ãææå¯ç  å MD5
 å¯ç åå¸ åéå¶ä¸å¡«åå³å¯ å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | | :------------------: | :--: | :----: | :----------------------------
----------: | | `NCM_CTCODE` | å¦ | `86` |
+è¯´æ | | :------------------: | :--: | :-----: | :---------------------------
+------------------------------------: | | `NCM_CTCODE` | å¦ | `86` |
 ææºå·ç»å½ç¨ï¼ç»å½ææºåºå· | | `NCM_PHONE` | å¦ | æ  |
 ææºå·ç»å½ç¨ï¼ç»å½ææºå· | | `NCM_EMAIL` | å¦ | æ  |
 é®ç®±ç»å½ç¨ï¼ç»å½é®ç®± | | `NCM_PASSWORD` | å¦ | æ  |
 å¸å·ææå¯ç ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | | `NCM_PASSWORD_HASH` |
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
-æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | ## ð ä½¿ç¨ ###
-æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
+æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
+`NCM_MSG_CACHE_TIME` | å¦ | `3600` | ç¼å­ Bot å·²åéé³ä¹å¡ççé³ä¹
+ID å ç¨æ·æè¿ä¸æ¬¡æä½ çæ¶é¿ï¼ç§ï¼ | | `NCM_AUTO_RESOLVE` | å¦
+| `False` |
+å½ç¨æ·åéé³ä¹é¾æ¥æ¶ï¼æ¯å¦èªå¨è§£æå¹¶åéé³ä¹å¡ç | ##
+ð ä½¿ç¨ ### æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
 ä»ç»ï¼æç´¢æ­æ²ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
 å«åï¼`ç½æäº`ã`wyy` - çµå° [æ­æ²å / èç® ID] -
 ä»ç»ï¼æç´¢çµå°èç®ãå½è¾å¥çµå° ID æ¶ä¼ç´æ¥åéå¯¹åºèç®
 - å«åï¼`å£°é³`ã`ç½æçµå°`ã`wydt`ã`wydj` - è§£æ [åå¤
 é³ä¹å¡ç / é¾æ¥] - ä»ç»ï¼è·åè¯¥ é³ä¹ / çµå°èç®
 çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
 å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ [åå¤ é³ä¹å¡ç / é¾æ¥] -
@@ -80,17 +85,18 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ###
-0.3.0 - æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 -
-`è§£æ`ã`æ­è¯`ã`é¾æ¥` æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot
-åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.2 - æ°å¢éç½®é¡¹
+`NCM_MSG_CACHE_TIME`ã`NCM_AUTO_RESOLVE` - è°æ´ç»å½æµç¨å°
+`driver.on_startup` ä¸­ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ### 0.3.0 -
+æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
+æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
 æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
 ç°å¨æä»¶ä¼å®æ¶æ¸çèªèº«åå­ä¸­çç¼å­äº ### 0.2.4 -
 ä¿®å¤ä¸ä¸ªæ­è¯è§£æ bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
 å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
 å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
 `è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

