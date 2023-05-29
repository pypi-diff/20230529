# Comparing `tmp/EdgeGPT-0.6.8.tar.gz` & `tmp/EdgeGPT-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.6.8.tar", last modified: Sun May 28 11:40:43 2023, max compression
+gzip compressed data, was "EdgeGPT-0.6.9.tar", last modified: Mon May 29 02:18:30 2023, max compression
```

## Comparing `EdgeGPT-0.6.8.tar` & `EdgeGPT-0.6.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:40:43.556187 EdgeGPT-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-28 11:39:02.000000 EdgeGPT-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-28 11:40:43.556187 EdgeGPT-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-28 11:40:43.000000 EdgeGPT-0.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 11:40:43.556187 EdgeGPT-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-28 11:39:02.000000 EdgeGPT-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:40:43.556187 EdgeGPT-0.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:40:43.556187 EdgeGPT-0.6.8/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-28 11:40:43.000000 EdgeGPT-0.6.8/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-28 11:40:43.000000 EdgeGPT-0.6.8/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:40:43.000000 EdgeGPT-0.6.8/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-28 11:40:43.000000 EdgeGPT-0.6.8/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-28 11:40:43.000000 EdgeGPT-0.6.8/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-28 11:40:43.000000 EdgeGPT-0.6.8/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39135 2023-05-28 11:39:02.000000 EdgeGPT-0.6.8/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-28 11:39:02.000000 EdgeGPT-0.6.8/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:18:30.036017 EdgeGPT-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-29 02:17:53.000000 EdgeGPT-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-29 02:18:30.036017 EdgeGPT-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-29 02:18:29.000000 EdgeGPT-0.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 02:18:30.036017 EdgeGPT-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-29 02:17:53.000000 EdgeGPT-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:18:30.036017 EdgeGPT-0.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:18:30.036017 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39337 2023-05-29 02:17:53.000000 EdgeGPT-0.6.9/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-29 02:17:53.000000 EdgeGPT-0.6.9/src/ImageGen.py
```

### Comparing `EdgeGPT-0.6.8/LICENSE` & `EdgeGPT-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.8/PKG-INFO` & `EdgeGPT-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.8
+Version: 0.6.9
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.8 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.9 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.6.8/README.md` & `EdgeGPT-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.8/setup.py` & `EdgeGPT-0.6.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.6.8",
+    version="0.6.9",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.6.8/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.6.9/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.8
+Version: 0.6.9
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.8 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.9 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.6.8/src/EdgeGPT.py` & `EdgeGPT-0.6.9/src/EdgeGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -737,22 +737,25 @@
 
     return PromptSession(key_bindings=kb, history=InMemoryHistory())
 
 
 def _create_completer(commands: list, pattern_str: str = "$"):
     return WordCompleter(words=commands, pattern=re.compile(pattern_str))
 
+
 def _create_history_logger(f):
     def logger(*args, **kwargs):
         tmp = sys.stdout
         sys.stdout = f
         print(*args, **kwargs, flush=True)
         sys.stdout = tmp
+
     return logger
 
+
 async def async_main(args: argparse.Namespace) -> None:
     """
     Main function
     """
     print("Initializing...")
     print("Enter `alt+enter` or `escape+enter` to send a message")
     # Read and parse cookies
@@ -763,16 +766,17 @@
     session = _create_session()
     completer = _create_completer(["!help", "!exit", "!reset"])
     initial_prompt = args.prompt
 
     # Log chat history
     def p_hist(*args, **kwargs):
         pass
+
     if args.history_file:
-        f = open(args.history_file, 'a+',encoding="utf-8")
+        f = open(args.history_file, "a+", encoding="utf-8")
         p_hist = _create_history_logger(f)
 
     while True:
         print("\nYou:")
         p_hist("\nYou:")
         if initial_prompt:
             question = initial_prompt
@@ -799,21 +803,21 @@
             continue
         if question == "!reset":
             await bot.reset()
             continue
         print("Bot:")
         p_hist("Bot:")
         if args.no_stream:
-            response=(
-                    await bot.ask(
-                        prompt=question,
-                        conversation_style=args.style,
-                        wss_link=args.wss_link,
-                    )
-                )["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"]
+            response = (
+                await bot.ask(
+                    prompt=question,
+                    conversation_style=args.style,
+                    wss_link=args.wss_link,
+                )
+            )["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"]
             print(response)
             p_hist(response)
         else:
             wrote = 0
             if args.rich:
                 md = Markdown("")
                 with Live(md, auto_refresh=False) as live:
@@ -969,14 +973,15 @@
             )
             return
         print(f"> Importing cookies from: {cls.current_filepath.name}")
         with open(cls.current_filepath, encoding="utf-8") as file:
             cls.current_data = json.load(file)
         cls.image_token = [x for x in cls.current_data if x.get("name") == "_U"]
         cls.image_token = cls.image_token[0].get("value")
+        return cls.current_data
 
     @classmethod
     def import_next(cls):
         """
         Cycle through to the next cookies file.  Import it.  Mark the previous
         file to be ignored for the remainder of the current session.
         """
@@ -996,40 +1001,42 @@
         self,
         prompt,
         style="precise",
         content_type="text",
         cookie_file=0,
         echo=True,
         echo_prompt=False,
+        proxy: str | None = None,
     ):
         """
         Arguments:
 
         prompt: Text to enter into Bing Chat
         style: creative, balanced, or precise
         content_type: "text" for Bing Chat; "image" for Dall-e
         cookie_file: Path, filepath string, or index (int) to list of cookie paths
         echo: Print something to confirm request made
         echo_prompt: Print confirmation of the evaluated prompt
         """
+        self.proxy = proxy
         self.index = []
         self.request_count = {}
         self.image_dirpath = Path("./").resolve()
         Cookie.import_data()
         self.index += [self]
         self.prompt = prompt
         files = Cookie.files()
         if isinstance(cookie_file, int):
             index = cookie_file if cookie_file < len(files) else 0
         else:
             if not isinstance(cookie_file, (str, Path)):
                 message = "'cookie_file' must be an int, str, or Path object"
                 raise TypeError(message)
             cookie_file = Path(cookie_file)
-            if cookie_file in files():  # Supplied filepath IS in Cookie.dirpath
+            if cookie_file in files:  # Supplied filepath IS in Cookie.dirpath
                 index = files.index(cookie_file)
             else:  # Supplied filepath is NOT in Cookie.dirpath
                 if cookie_file.is_file():
                     Cookie.dirpath = cookie_file.parent.resolve()
                 if cookie_file.is_dir():
                     Cookie.dirpath = cookie_file.resolve()
                 index = 0
@@ -1056,15 +1063,17 @@
         )
 
     async def send_to_bing(self, echo=True, echo_prompt=False):
         """Creat, submit, then close a Chatbot instance.  Return the response"""
         retries = len(Cookie.files())
         while retries:
             try:
-                bot = await Chatbot.create()
+                # Read the cookies file
+                cookie_data = Cookie.import_data()
+                bot = await Chatbot.create(proxy=self.proxy, cookies=cookie_data)
                 if echo_prompt:
                     print(f"> {self.prompt}=")
                 if echo:
                     print("> Waiting for response...")
                 if self.style.lower() not in "creative balanced precise".split():
                     self.style = "precise"
                 response = await bot.ask(
```

