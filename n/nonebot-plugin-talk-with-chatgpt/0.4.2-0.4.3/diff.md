# Comparing `tmp/nonebot_plugin_talk_with_chatgpt-0.4.2.tar.gz` & `tmp/nonebot_plugin_talk_with_chatgpt-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.4.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.4.3.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_chatgpt-0.4.2.tar` & `nonebot_plugin_talk_with_chatgpt-0.4.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8454 2023-04-22 14:28:18.532815 nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/__init__.py
--rw-r--r--   0        0        0    13518 2023-04-22 14:27:21.436142 nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/config.py
--rw-r--r--   0        0        0     5281 2023-05-18 02:26:25.865457 nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/data_handle.py
--rw-r--r--   0        0        0      974 2023-05-18 02:26:39.929502 nonebot_plugin_talk_with_chatgpt-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4902 2023-05-18 02:26:59.624892 nonebot_plugin_talk_with_chatgpt-0.4.2/README.md
--rw-r--r--   0        0        0     5831 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     8694 2023-05-29 01:52:17.318389 nonebot_plugin_talk_with_chatgpt-0.4.3/nonebot_plugin_talk_with_chatgpt/__init__.py
+-rw-r--r--   0        0        0    13686 2023-05-29 01:47:06.923464 nonebot_plugin_talk_with_chatgpt-0.4.3/nonebot_plugin_talk_with_chatgpt/config.py
+-rw-r--r--   0        0        0     5281 2023-05-18 02:26:25.865457 nonebot_plugin_talk_with_chatgpt-0.4.3/nonebot_plugin_talk_with_chatgpt/data_handle.py
+-rw-r--r--   0        0        0      974 2023-05-29 01:54:22.900923 nonebot_plugin_talk_with_chatgpt-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     5180 2023-05-29 01:54:55.279379 nonebot_plugin_talk_with_chatgpt-0.4.3/README.md
+-rw-r--r--   0        0        0     6105 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.4.3/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/__init__.py` & `nonebot_plugin_talk_with_chatgpt-0.4.3/nonebot_plugin_talk_with_chatgpt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         var.session_data[id] = ["", "", "默认"]
     return id
 
 
 async def rule_check(event: MessageEvent, bot: Bot) -> bool:
     """对话响应判断"""
     # bot判断
-    if bot != var.handle_bot:
+    if pc.talk_with_chatgpt_bot_qqnum_list != ["all"] and bot != var.handle_bot:
         return False
     # 获取纯文本
     text = event.get_plaintext().strip()
 
     if isinstance(event, GroupMessageEvent):
         # 仅艾特但没发内容
         if event.is_tome() and pc.talk_with_chatgpt_talk_at:
@@ -69,27 +69,35 @@
         return text[: len(talk_cmd)] == talk_cmd
 
     return False
 
 
 async def rule_check2(event: MessageEvent, bot: Bot) -> bool:
     """其他命令判断"""
-    return bot == var.handle_bot and (
+    if not (
         isinstance(event, GroupMessageEvent) or isinstance(event, PrivateMessageEvent)
-    )
+    ):
+        return False
+
+    if pc.talk_with_chatgpt_bot_qqnum_list == ["all"]:
+        return True
+    else:
+        return bot == var.handle_bot
 
 
 async def rule_check3(event: MessageEvent, bot: Bot) -> bool:
     """预设权限判断"""
     if not (
-        bot == var.handle_bot
-        and isinstance(event, GroupMessageEvent)
-        or isinstance(event, PrivateMessageEvent)
+        isinstance(event, GroupMessageEvent) or isinstance(event, PrivateMessageEvent)
     ):
         return False
+
+    if pc.talk_with_chatgpt_bot_qqnum_list != ["all"] and bot != var.handle_bot:
+        return False
+
     if pc.talk_with_chatgpt_prompt_admin_only and not await SUPERUSER(bot, event):
         return False
     else:
         return True
 
 
 #################
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/config.py` & `nonebot_plugin_talk_with_chatgpt-0.4.3/nonebot_plugin_talk_with_chatgpt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     talk_with_chatgpt_prompt_cmd: str = "/prompt"
 
     # 请求超时时间
     talk_with_chatgpt_timeout: int = 60
     # chatgpt模型
     talk_with_chatgpt_api_model: str = "text-davinci-002-render-sha"
 
-    # 机器人的QQ号（如果写了就按优先级响应，否则就第一个连上的响应） [1234, 5678, 6666]
+    # 机器人的QQ号（如果写了就按优先级响应，否则就第一个连上的响应） [1234, 5678, 6666]  ["all"]则全部响应
     talk_with_chatgpt_bot_qqnum_list: List[str] = []  # 可选
     # 插件数据文件名
     talk_with_chatgpt_data: str = "talk_with_chatgpt.json"
 
 
 driver = get_driver()
 global_config = driver.config
@@ -130,14 +130,16 @@
             ensure_ascii=False,
         )
 
 
 # qq机器人连接时执行
 @driver.on_bot_connect
 async def _(bot: Bot):
+    if pc.talk_with_chatgpt_bot_qqnum_list == ["all"]:
+        return
     # 是否有写bot qq，如果写了只处理bot qq在列表里的
     if (
         pc.talk_with_chatgpt_bot_qqnum_list
         and bot.self_id in pc.talk_with_chatgpt_bot_qqnum_list
     ):
         # 如果已经有bot连了
         if var.handle_bot:
@@ -159,14 +161,16 @@
     elif not pc.talk_with_chatgpt_bot_qqnum_list and not var.handle_bot:
         var.handle_bot = bot
 
 
 # qq机器人断开时执行
 @driver.on_bot_disconnect
 async def _(bot: Bot):
+    if pc.talk_with_chatgpt_bot_qqnum_list == ["all"]:
+        return
     # 判断掉线的是否为handle bot
     if bot == var.handle_bot:
         # 如果有写bot qq列表
         if pc.talk_with_chatgpt_bot_qqnum_list:
             # 获取当前连着的bot列表(需要bot是在bot qq列表里)
             available_bot_id_list = [
                 bot_id
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/data_handle.py` & `nonebot_plugin_talk_with_chatgpt-0.4.3/nonebot_plugin_talk_with_chatgpt/data_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.2/pyproject.toml` & `nonebot_plugin_talk_with_chatgpt-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_chatgpt"
-version = "0.4.2"
+version = "0.4.3"
 description = "Nonebot2 基于accessToken登录的ChatGPT聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_chatgpt"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.2/README.md` & `nonebot_plugin_talk_with_chatgpt-0.4.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -83,36 +83,40 @@
 # 请求超时时间，回答生成的时间也要算在这里面的，所以不能太短，默认60秒
 talk_with_chatgpt_timeout = 60
 # chatgpt模型，默认 text-davinci-002-render-sha，更多模型请参考 https://platform.openai.com/docs/models
 talk_with_chatgpt_api_model = text-davinci-002-render-sha
 
 # 机器人的QQ号列表，选填
 # 如果有多个bot连接，会按照填写的list，左边的机器人QQ优先级最高 1234 > 5678 > 6666，会自动切换
-# 如果不填该配置则由第一个连上的bot响应，所以单bot连可以不填
+# 如果不填该配置则由第一个连上的bot响应，所以单bot连可以不填，写 ["all"]则所有机器人均响应
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666]
 # 插件数据文件名，默认./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json
 ```
 
 ## 插件命令（均可修改！） 
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，默认群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
-| /clear | 重置对话（不会重置预设） |
+| /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
+### 2023/5/29 \[v0.4.3]
+
+* [支持所有机器人响应命令](https://github.com/nikissXI/nonebot_plugins/issues/22)
+
 ### 2023/5/18 \[v0.4.2]
 
-* 修复会话丢失不重置的问题
+* [修复会话丢失不重置的问题](https://github.com/nikissXI/nonebot_plugins/issues/21)
 
 ### 2023/4/22 \[v0.4.1]
 
-* 增加群聊at触发开关
+* [增加群聊at触发开关](https://github.com/nikissXI/nonebot_plugins/issues/21)
 
 ### 2023/4/21 \[v0.4.0]
 
 * 更换了默认API，暂时能用，建议还是自己搭建API
 * 新增多预设功能，内置三个预设：猫娘、魅魔、开发者模式
 * 增加私聊沉浸式对话
 * 优化大量细节
```

#### html2text {}

```diff
@@ -41,22 +41,26 @@
 è¯·æ±è¶æ¶æ¶é´ï¼åç­çæçæ¶é´ä¹è¦ç®å¨è¿éé¢çï¼æä»¥ä¸è½å¤ªç­ï¼é»è®¤60ç§
 talk_with_chatgpt_timeout = 60 # chatgptæ¨¡åï¼é»è®¤ text-davinci-002-
 render-shaï¼æ´å¤æ¨¡åè¯·åè https://platform.openai.com/docs/models
 talk_with_chatgpt_api_model = text-davinci-002-render-sha #
 æºå¨äººçQQå·åè¡¨ï¼éå¡« #
 å¦ææå¤ä¸ªbotè¿æ¥ï¼ä¼æç§å¡«åçlistï¼å·¦è¾¹çæºå¨äººQQä¼åçº§æé«
 1234 > 5678 > 6666ï¼ä¼èªå¨åæ¢ #
-å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååºï¼æä»¥åbotè¿å¯ä»¥ä¸å¡«
-talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666] #
-æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
+å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååºï¼æä»¥åbotè¿å¯ä»¥ä¸å¡«ï¼å
+["all"]åæææºå¨äººåååº talk_with_chatgpt_bot_qqnum_list = [1234,
+5678, 6666] # æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
-æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /clear |
+æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-5/18 \[v0.4.2] * ä¿®å¤ä¼è¯ä¸¢å¤±ä¸éç½®çé®é¢ ### 2023/4/22 \[v0.4.1] *
-å¢å ç¾¤èatè§¦åå¼å³ ### 2023/4/21 \[v0.4.0] *
+5/29 \[v0.4.3] * [æ¯ææææºå¨äººååºå½ä»¤](https://github.com/
+nikissXI/nonebot_plugins/issues/22) ### 2023/5/18 \[v0.4.2] *
+[ä¿®å¤ä¼è¯ä¸¢å¤±ä¸éç½®çé®é¢](https://github.com/nikissXI/
+nonebot_plugins/issues/21) ### 2023/4/22 \[v0.4.1] *
+[å¢å ç¾¤èatè§¦åå¼å³](https://github.com/nikissXI/nonebot_plugins/
+issues/21) ### 2023/4/21 \[v0.4.0] *
 æ´æ¢äºé»è®¤APIï¼ææ¶è½ç¨ï¼å»ºè®®è¿æ¯èªå·±æ­å»ºAPI *
 æ°å¢å¤é¢è®¾åè½ï¼åç½®ä¸ä¸ªé¢è®¾ï¼ç«å¨ãé­é­ãå¼åèæ¨¡å¼
 * å¢å ç§èæ²æµ¸å¼å¯¹è¯ * ä¼åå¤§éç»è ### 2023/4/11 \[v0.2.3] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.2/PKG-INFO` & `nonebot_plugin_talk_with_chatgpt-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-chatgpt
-Version: 0.4.2
+Version: 0.4.3
 Summary: Nonebot2 基于accessToken登录的ChatGPT聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -106,36 +106,40 @@
 # 请求超时时间，回答生成的时间也要算在这里面的，所以不能太短，默认60秒
 talk_with_chatgpt_timeout = 60
 # chatgpt模型，默认 text-davinci-002-render-sha，更多模型请参考 https://platform.openai.com/docs/models
 talk_with_chatgpt_api_model = text-davinci-002-render-sha
 
 # 机器人的QQ号列表，选填
 # 如果有多个bot连接，会按照填写的list，左边的机器人QQ优先级最高 1234 > 5678 > 6666，会自动切换
-# 如果不填该配置则由第一个连上的bot响应，所以单bot连可以不填
+# 如果不填该配置则由第一个连上的bot响应，所以单bot连可以不填，写 ["all"]则所有机器人均响应
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666]
 # 插件数据文件名，默认./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json
 ```
 
 ## 插件命令（均可修改！） 
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，默认群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
-| /clear | 重置对话（不会重置预设） |
+| /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
+### 2023/5/29 \[v0.4.3]
+
+* [支持所有机器人响应命令](https://github.com/nikissXI/nonebot_plugins/issues/22)
+
 ### 2023/5/18 \[v0.4.2]
 
-* 修复会话丢失不重置的问题
+* [修复会话丢失不重置的问题](https://github.com/nikissXI/nonebot_plugins/issues/21)
 
 ### 2023/4/22 \[v0.4.1]
 
-* 增加群聊at触发开关
+* [增加群聊at触发开关](https://github.com/nikissXI/nonebot_plugins/issues/21)
 
 ### 2023/4/21 \[v0.4.0]
 
 * 更换了默认API，暂时能用，建议还是自己搭建API
 * 新增多预设功能，内置三个预设：猫娘、魅魔、开发者模式
 * 增加私聊沉浸式对话
 * 优化大量细节
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.4.2
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.4.3
 Summary: Nonebot2 åºäºaccessTokenç»å½çChatGPTèå¤©æä»¶ Home-page:
 https://github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt License: MIT Author: nikissXI Author-email:
 1299577815@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -56,22 +56,26 @@
 è¯·æ±è¶æ¶æ¶é´ï¼åç­çæçæ¶é´ä¹è¦ç®å¨è¿éé¢çï¼æä»¥ä¸è½å¤ªç­ï¼é»è®¤60ç§
 talk_with_chatgpt_timeout = 60 # chatgptæ¨¡åï¼é»è®¤ text-davinci-002-
 render-shaï¼æ´å¤æ¨¡åè¯·åè https://platform.openai.com/docs/models
 talk_with_chatgpt_api_model = text-davinci-002-render-sha #
 æºå¨äººçQQå·åè¡¨ï¼éå¡« #
 å¦ææå¤ä¸ªbotè¿æ¥ï¼ä¼æç§å¡«åçlistï¼å·¦è¾¹çæºå¨äººQQä¼åçº§æé«
 1234 > 5678 > 6666ï¼ä¼èªå¨åæ¢ #
-å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååºï¼æä»¥åbotè¿å¯ä»¥ä¸å¡«
-talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666] #
-æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
+å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååºï¼æä»¥åbotè¿å¯ä»¥ä¸å¡«ï¼å
+["all"]åæææºå¨äººåååº talk_with_chatgpt_bot_qqnum_list = [1234,
+5678, 6666] # æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
-æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /clear |
+æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-5/18 \[v0.4.2] * ä¿®å¤ä¼è¯ä¸¢å¤±ä¸éç½®çé®é¢ ### 2023/4/22 \[v0.4.1] *
-å¢å ç¾¤èatè§¦åå¼å³ ### 2023/4/21 \[v0.4.0] *
+5/29 \[v0.4.3] * [æ¯ææææºå¨äººååºå½ä»¤](https://github.com/
+nikissXI/nonebot_plugins/issues/22) ### 2023/5/18 \[v0.4.2] *
+[ä¿®å¤ä¼è¯ä¸¢å¤±ä¸éç½®çé®é¢](https://github.com/nikissXI/
+nonebot_plugins/issues/21) ### 2023/4/22 \[v0.4.1] *
+[å¢å ç¾¤èatè§¦åå¼å³](https://github.com/nikissXI/nonebot_plugins/
+issues/21) ### 2023/4/21 \[v0.4.0] *
 æ´æ¢äºé»è®¤APIï¼ææ¶è½ç¨ï¼å»ºè®®è¿æ¯èªå·±æ­å»ºAPI *
 æ°å¢å¤é¢è®¾åè½ï¼åç½®ä¸ä¸ªé¢è®¾ï¼ç«å¨ãé­é­ãå¼åèæ¨¡å¼
 * å¢å ç§èæ²æµ¸å¼å¯¹è¯ * ä¼åå¤§éç»è ### 2023/4/11 \[v0.2.3] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

