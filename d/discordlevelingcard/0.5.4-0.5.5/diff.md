# Comparing `tmp/discordlevelingcard-0.5.4.tar.gz` & `tmp/discordlevelingcard-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordlevelingcard-0.5.4.tar", max compression
+gzip compressed data, was "discordlevelingcard-0.5.5.tar", max compression
```

## Comparing `discordlevelingcard-0.5.4.tar` & `discordlevelingcard-0.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      129 2023-05-29 17:20:09.194905 discordlevelingcard-0.5.4/DiscordLevelingCard/__init__.py
--rw-r--r--   0        0        0      842 2023-04-25 08:29:49.129344 discordlevelingcard-0.5.4/DiscordLevelingCard/assets/curveborder.png
--rw-r--r--   0        0        0     2596 2023-04-25 08:29:49.129826 discordlevelingcard-0.5.4/DiscordLevelingCard/assets/curvedoverlay.png
--rw-r--r--   0        0        0    60288 2023-04-25 08:29:49.131350 discordlevelingcard-0.5.4/DiscordLevelingCard/assets/levelfont.otf
--rw-r--r--   0        0        0     9742 2023-04-25 08:29:49.132354 discordlevelingcard-0.5.4/DiscordLevelingCard/assets/mask_circle.jpg
--rw-r--r--   0        0        0     4775 2023-05-29 17:05:04.175407 discordlevelingcard-0.5.4/DiscordLevelingCard/assets/overlay1.png
--rw-r--r--   0        0        0     2590 2023-04-25 08:29:49.133788 discordlevelingcard-0.5.4/DiscordLevelingCard/card_settings.py
--rw-r--r--   0        0        0    12505 2023-05-29 17:39:37.772268 discordlevelingcard-0.5.4/DiscordLevelingCard/discord_card.py
--rw-r--r--   0        0        0      531 2023-04-25 08:29:49.134664 discordlevelingcard-0.5.4/DiscordLevelingCard/error.py
--rw-r--r--   0        0        0     7459 2023-05-29 17:17:30.123452 discordlevelingcard-0.5.4/DiscordLevelingCard/sandbox.py
--rw-r--r--   0        0        0     6247 2023-05-29 17:54:43.984970 discordlevelingcard-0.5.4/DiscordLevelingCard/tester.py
--rw-r--r--   0        0        0   124130 2023-05-29 17:13:57.444261 discordlevelingcard-0.5.4/Examples/custom card examples/black_card1.png
--rw-r--r--   0        0        0   125492 2023-05-29 17:15:51.029764 discordlevelingcard-0.5.4/Examples/custom card examples/blue_card1.png
--rw-r--r--   0        0        0   125447 2023-05-29 17:15:25.624219 discordlevelingcard-0.5.4/Examples/custom card examples/white_card1.png
--rw-r--r--   0        0        0     1511 2023-05-29 17:56:46.850193 discordlevelingcard-0.5.4/Examples/tester_example.py
--rw-r--r--   0        0        0     1083 2023-04-25 08:29:49.135173 discordlevelingcard-0.5.4/LICENSE
--rw-r--r--   0        0        0      943 2023-05-29 18:36:02.030392 discordlevelingcard-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     6592 2023-05-29 18:36:17.228987 discordlevelingcard-0.5.4/README.md
--rw-r--r--   0        0        0     7394 2023-05-29 18:36:48.491545 discordlevelingcard-0.5.4/setup.py
--rw-r--r--   0        0        0     7265 2023-05-29 18:36:48.491545 discordlevelingcard-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      129 2023-05-29 17:20:09.194905 discordlevelingcard-0.5.5/DiscordLevelingCard/__init__.py
+-rw-r--r--   0        0        0      842 2023-04-25 08:29:49.129344 discordlevelingcard-0.5.5/DiscordLevelingCard/assets/curveborder.png
+-rw-r--r--   0        0        0     2596 2023-04-25 08:29:49.129826 discordlevelingcard-0.5.5/DiscordLevelingCard/assets/curvedoverlay.png
+-rw-r--r--   0        0        0    60288 2023-04-25 08:29:49.131350 discordlevelingcard-0.5.5/DiscordLevelingCard/assets/levelfont.otf
+-rw-r--r--   0        0        0     9742 2023-04-25 08:29:49.132354 discordlevelingcard-0.5.5/DiscordLevelingCard/assets/mask_circle.jpg
+-rw-r--r--   0        0        0     4775 2023-05-29 17:05:04.175407 discordlevelingcard-0.5.5/DiscordLevelingCard/assets/overlay1.png
+-rw-r--r--   0        0        0     2590 2023-04-25 08:29:49.133788 discordlevelingcard-0.5.5/DiscordLevelingCard/card_settings.py
+-rw-r--r--   0        0        0    12505 2023-05-29 17:39:37.772268 discordlevelingcard-0.5.5/DiscordLevelingCard/discord_card.py
+-rw-r--r--   0        0        0      531 2023-04-25 08:29:49.134664 discordlevelingcard-0.5.5/DiscordLevelingCard/error.py
+-rw-r--r--   0        0        0     7459 2023-05-29 17:17:30.123452 discordlevelingcard-0.5.5/DiscordLevelingCard/sandbox.py
+-rw-r--r--   0        0        0     6247 2023-05-29 17:54:43.984970 discordlevelingcard-0.5.5/DiscordLevelingCard/tester.py
+-rw-r--r--   0        0        0   124130 2023-05-29 17:13:57.444261 discordlevelingcard-0.5.5/Examples/custom card examples/black_card1.png
+-rw-r--r--   0        0        0   125492 2023-05-29 17:15:51.029764 discordlevelingcard-0.5.5/Examples/custom card examples/blue_card1.png
+-rw-r--r--   0        0        0   125447 2023-05-29 17:15:25.624219 discordlevelingcard-0.5.5/Examples/custom card examples/white_card1.png
+-rw-r--r--   0        0        0     1511 2023-05-29 17:56:46.850193 discordlevelingcard-0.5.5/Examples/tester_example.py
+-rw-r--r--   0        0        0     1083 2023-04-25 08:29:49.135173 discordlevelingcard-0.5.5/LICENSE
+-rw-r--r--   0        0        0      943 2023-05-29 18:37:53.626251 discordlevelingcard-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     6686 2023-05-29 18:40:04.718748 discordlevelingcard-0.5.5/README.md
+-rw-r--r--   0        0        0     7488 2023-05-29 18:40:59.176058 discordlevelingcard-0.5.5/setup.py
+-rw-r--r--   0        0        0     7348 2023-05-29 18:40:59.176058 discordlevelingcard-0.5.5/PKG-INFO
```

### Comparing `discordlevelingcard-0.5.4/DiscordLevelingCard/assets/curveborder.png` & `discordlevelingcard-0.5.5/DiscordLevelingCard/assets/curveborder.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/DiscordLevelingCard/assets/curvedoverlay.png` & `discordlevelingcard-0.5.5/DiscordLevelingCard/assets/curvedoverlay.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/DiscordLevelingCard/assets/levelfont.otf` & `discordlevelingcard-0.5.5/DiscordLevelingCard/assets/levelfont.otf`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/DiscordLevelingCard/assets/mask_circle.jpg` & `discordlevelingcard-0.5.5/DiscordLevelingCard/assets/mask_circle.jpg`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/DiscordLevelingCard/assets/overlay1.png` & `discordlevelingcard-0.5.5/DiscordLevelingCard/assets/overlay1.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/DiscordLevelingCard/card_settings.py` & `discordlevelingcard-0.5.5/DiscordLevelingCard/card_settings.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/DiscordLevelingCard/discord_card.py` & `discordlevelingcard-0.5.5/DiscordLevelingCard/discord_card.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/DiscordLevelingCard/error.py` & `discordlevelingcard-0.5.5/DiscordLevelingCard/error.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/DiscordLevelingCard/sandbox.py` & `discordlevelingcard-0.5.5/DiscordLevelingCard/sandbox.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/DiscordLevelingCard/tester.py` & `discordlevelingcard-0.5.5/DiscordLevelingCard/tester.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/Examples/custom card examples/black_card1.png` & `discordlevelingcard-0.5.5/Examples/custom card examples/black_card1.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/Examples/custom card examples/blue_card1.png` & `discordlevelingcard-0.5.5/Examples/custom card examples/blue_card1.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/Examples/custom card examples/white_card1.png` & `discordlevelingcard-0.5.5/Examples/custom card examples/white_card1.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/Examples/tester_example.py` & `discordlevelingcard-0.5.5/Examples/tester_example.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/LICENSE` & `discordlevelingcard-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.4/pyproject.toml` & `discordlevelingcard-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discordlevelingcard"
-version = "0.5.4"
+version = "0.5.5"
 readme = "README.md"
 description = "A library with leveling cards for your discord bot."
 repository = "https://github.com/krishsharma0413/DiscordLevelingCard"
 authors = ["Reset <krishsharma0413@gmail.com>"]
 license = "MIT"
 keywords = [
     "discord", "leveling", "card",
```

### Comparing `discordlevelingcard-0.5.4/README.md` & `discordlevelingcard-0.5.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,24 @@
 
 - `max_exp` - max exp of the user.
 
 - `username` - username of the user.
 
 - `rank` - rank of the user. (optional)
 
+## methods
+
+- `card1`
+- `card2`
+- `card3`
+
 </details>
 
+<details>
+
 <summary> <span style="color:yellow">Sandbox</span> class</summary>
 
 <br>
 
 `__init__` method
 
 ```py
@@ -148,14 +156,17 @@
 
 - `username` - username of the user.
 
 - `rank` - rank of the user. (optional)
 
 - `cacheing` - if set to `True` then it will cache the image and will not regenerate it again. (default is `True`)
   
+
+## methods
+- `custom_card1`
   
 </details>
 
 
 
 
 <details>
```

### Comparing `discordlevelingcard-0.5.4/setup.py` & `discordlevelingcard-0.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'DiscordLevelingCard': ['assets/*']}
 
 install_requires = \
 ['Pillow>=9.2.0,<10.0.0', 'aiohttp>=3.8.1,<4.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'discordlevelingcard',
-    'version': '0.5.4',
+    'version': '0.5.5',
     'description': 'A library with leveling cards for your discord bot.',
-    'long_description': '# DiscordLevelingCard\nA library with Rank cards for your discord bot.\n\n<h3 style="color:yellow;"> now create your own custom rank cards!</h3>\n\n<br>\n\n[![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)\n\n# card preview\n\n`card1`\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n\n`card2`\n![card2](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n\n`card3` *same as card2 but with background*\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n# installation\n\n`for pypi version`\n```sh\npip install discordlevelingcard\n```\n\n`for github developement version`\n```sh\npip install git+https://github.com/krishsharma0413/DiscordLevelingCard\n```\n\n# How To Use\n\nIf you don\'t provide `path` then the method will return `bytes` which can directly be used in discord.py/disnake/pycord/nextcord \'s `File class`.\n\n\n<br>\n\n\n# Example\n\n`since no path was provided, it returns bytes which can directly be used in discord.py and its fork\'s File class.`\n\n```py\nfrom disnake.ext import commands\nfrom DiscordLevelingCard import RankCard, Settings\nimport disnake\n\nclient = commands.Bot()\n# define background, bar_color, text_color at one place\ncard_settings = Settings(\n    background="url or path to background image",\n    text_color="white",\n    bar_color="#000000"\n)\n\n@client.slash_command(name="rank")\nasync def user_rank_card(ctx, user:disnake.Member):\n    await ctx.response.defer()\n    a = RankCard(\n        settings=card_settings,\n        avatar=user.display_avatar.url,\n        level=1,\n        current_exp=1,\n        max_exp=1,\n        username="cool username"\n    )\n    image = await a.card1()\n    await ctx.edit_original_message(file=disnake.File(image, filename="rank.png")) # providing filename is very important\n\n```\n\n<br>\n\n## Documentation\n\n\n<details>\n\n<summary> <span style="color:yellow">RankCard</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n</details>\n\n<summary> <span style="color:yellow">Sandbox</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    cacheing:bool = True,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n- `cacheing` - if set to `True` then it will cache the image and will not regenerate it again. (default is `True`)\n  \n  \n</details>\n\n\n\n\n<details>\n\n<summary> <span style="color:yellow">Settings</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nSettings(\n    background: Union[PathLike, BufferedIOBase, str],\n    bar_color: Optional[str] = \'white\',\n    text_color: Optional[str] = \'white\',\n    background_color: Optional[str]= "#36393f"\n\n)\n```\n\n- `background` - background image url or file-object in `rb` mode.\n  - `4:1` aspect ratio recommended.\n\n- `bar_color` - color of the bar [example: "white" or "#000000"]\n\n- `text_color` - color of the text [example: "white" or "#000000"]\n\n- `background_color` - color of the background [example: "white" or "#000000"]\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card1</span> method</summary>\n\n\n```py\nRankCard.card1(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card2</span> method</summary>\n\n\n```py\nRankCard.card2(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card3</span> method</summary>\n\n\n```py\nRankCard.card3(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">custom_card1</span> method</summary>\n\n\n```py\nSandbox.custom_card1(card_colour:str = "black", resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n- `card_colour` : color of the card. (default is black)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n## examples\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/blue_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/white_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/black_card1.png)\n\n<br>\n\n</details>\n\n\n<br><br>\n\nif you want to see changelog then click [here](https://github.com/krishsharma0413/DiscordLevelingCard/blob/main/CHANGELOG.md)\n\n<br><br>\nplease star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D\n',
+    'long_description': '# DiscordLevelingCard\nA library with Rank cards for your discord bot.\n\n<h3 style="color:yellow;"> now create your own custom rank cards!</h3>\n\n<br>\n\n[![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)\n\n# card preview\n\n`card1`\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n\n`card2`\n![card2](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n\n`card3` *same as card2 but with background*\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n# installation\n\n`for pypi version`\n```sh\npip install discordlevelingcard\n```\n\n`for github developement version`\n```sh\npip install git+https://github.com/krishsharma0413/DiscordLevelingCard\n```\n\n# How To Use\n\nIf you don\'t provide `path` then the method will return `bytes` which can directly be used in discord.py/disnake/pycord/nextcord \'s `File class`.\n\n\n<br>\n\n\n# Example\n\n`since no path was provided, it returns bytes which can directly be used in discord.py and its fork\'s File class.`\n\n```py\nfrom disnake.ext import commands\nfrom DiscordLevelingCard import RankCard, Settings\nimport disnake\n\nclient = commands.Bot()\n# define background, bar_color, text_color at one place\ncard_settings = Settings(\n    background="url or path to background image",\n    text_color="white",\n    bar_color="#000000"\n)\n\n@client.slash_command(name="rank")\nasync def user_rank_card(ctx, user:disnake.Member):\n    await ctx.response.defer()\n    a = RankCard(\n        settings=card_settings,\n        avatar=user.display_avatar.url,\n        level=1,\n        current_exp=1,\n        max_exp=1,\n        username="cool username"\n    )\n    image = await a.card1()\n    await ctx.edit_original_message(file=disnake.File(image, filename="rank.png")) # providing filename is very important\n\n```\n\n<br>\n\n## Documentation\n\n\n<details>\n\n<summary> <span style="color:yellow">RankCard</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n## methods\n\n- `card1`\n- `card2`\n- `card3`\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">Sandbox</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    cacheing:bool = True,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n- `cacheing` - if set to `True` then it will cache the image and will not regenerate it again. (default is `True`)\n  \n\n## methods\n- `custom_card1`\n  \n</details>\n\n\n\n\n<details>\n\n<summary> <span style="color:yellow">Settings</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nSettings(\n    background: Union[PathLike, BufferedIOBase, str],\n    bar_color: Optional[str] = \'white\',\n    text_color: Optional[str] = \'white\',\n    background_color: Optional[str]= "#36393f"\n\n)\n```\n\n- `background` - background image url or file-object in `rb` mode.\n  - `4:1` aspect ratio recommended.\n\n- `bar_color` - color of the bar [example: "white" or "#000000"]\n\n- `text_color` - color of the text [example: "white" or "#000000"]\n\n- `background_color` - color of the background [example: "white" or "#000000"]\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card1</span> method</summary>\n\n\n```py\nRankCard.card1(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card2</span> method</summary>\n\n\n```py\nRankCard.card2(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card3</span> method</summary>\n\n\n```py\nRankCard.card3(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">custom_card1</span> method</summary>\n\n\n```py\nSandbox.custom_card1(card_colour:str = "black", resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n- `card_colour` : color of the card. (default is black)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n## examples\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/blue_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/white_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/black_card1.png)\n\n<br>\n\n</details>\n\n\n<br><br>\n\nif you want to see changelog then click [here](https://github.com/krishsharma0413/DiscordLevelingCard/blob/main/CHANGELOG.md)\n\n<br><br>\nplease star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D\n',
     'author': 'Reset',
     'author_email': 'krishsharma0413@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/krishsharma0413/DiscordLevelingCard',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `discordlevelingcard-0.5.4/PKG-INFO` & `discordlevelingcard-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordlevelingcard
-Version: 0.5.4
+Version: 0.5.5
 Summary: A library with leveling cards for your discord bot.
 Home-page: https://github.com/krishsharma0413/DiscordLevelingCard
 License: MIT
 Keywords: discord,leveling,card,image,discord.py,disnake,nextcord,rank,ranking,level,discord-bot,bot,discord-leveling,level-card,discord-leveling-card,discord-rank-card,sandbox,custom,custom-card
 Author: Reset
 Author-email: krishsharma0413@gmail.com
 Requires-Python: >=3.8,<4
@@ -132,16 +132,24 @@
 
 - `max_exp` - max exp of the user.
 
 - `username` - username of the user.
 
 - `rank` - rank of the user. (optional)
 
+## methods
+
+- `card1`
+- `card2`
+- `card3`
+
 </details>
 
+<details>
+
 <summary> <span style="color:yellow">Sandbox</span> class</summary>
 
 <br>
 
 `__init__` method
 
 ```py
@@ -169,14 +177,17 @@
 
 - `username` - username of the user.
 
 - `rank` - rank of the user. (optional)
 
 - `cacheing` - if set to `True` then it will cache the image and will not regenerate it again. (default is `True`)
   
+
+## methods
+- `custom_card1`
   
 </details>
 
 
 
 
 <details>
```

