# Comparing `tmp/aiavatar-0.1.0-py3-none-any.whl.zip` & `tmp/aiavatar-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 16743 bytes, number of entries: 19
+Zip file size: 17457 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      351 b- defN 23-May-27 12:45 aiavatar/__init__.py
 -rw-r--r--  2.0 unx     3407 b- defN 23-May-27 09:17 aiavatar/avatar.py
--rw-r--r--  2.0 unx     4575 b- defN 23-May-27 12:44 aiavatar/bot.py
+-rw-r--r--  2.0 unx     4475 b- defN 23-May-29 11:57 aiavatar/bot.py
 -rw-r--r--  2.0 unx      284 b- defN 23-May-27 03:16 aiavatar/animation/__init__.py
 -rw-r--r--  2.0 unx       31 b- defN 23-May-27 03:48 aiavatar/device/__init__.py
 -rw-r--r--  2.0 unx      836 b- defN 23-May-27 03:48 aiavatar/device/audio.py
 -rw-r--r--  2.0 unx      888 b- defN 23-May-27 09:19 aiavatar/face/__init__.py
--rw-r--r--  2.0 unx     5677 b- defN 23-May-27 09:06 aiavatar/listeners/__init__.py
+-rw-r--r--  2.0 unx     6184 b- defN 23-May-29 12:08 aiavatar/listeners/__init__.py
 -rw-r--r--  2.0 unx      788 b- defN 23-May-24 12:01 aiavatar/listeners/voicerequest.py
--rw-r--r--  2.0 unx      689 b- defN 23-May-24 12:01 aiavatar/listeners/wakeword.py
+-rw-r--r--  2.0 unx      877 b- defN 23-May-29 11:39 aiavatar/listeners/wakeword.py
 -rw-r--r--  2.0 unx      178 b- defN 23-May-27 08:55 aiavatar/processors/__init__.py
 -rw-r--r--  2.0 unx     2151 b- defN 23-May-27 08:42 aiavatar/processors/chatgpt.py
 -rw-r--r--  2.0 unx      275 b- defN 23-May-27 08:54 aiavatar/speech/__init__.py
--rw-r--r--  2.0 unx     2754 b- defN 23-May-27 08:57 aiavatar/speech/voicevox.py
--rw-r--r--  2.0 unx    11324 b- defN 23-May-27 14:07 aiavatar-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3897 b- defN 23-May-27 14:07 aiavatar-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 14:07 aiavatar-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-27 14:07 aiavatar-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1547 b- defN 23-May-27 14:07 aiavatar-0.1.0.dist-info/RECORD
-19 files, 39753 bytes uncompressed, 14213 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx     2794 b- defN 23-May-29 13:08 aiavatar/speech/voicevox.py
+-rw-r--r--  2.0 unx    11324 b- defN 23-May-29 13:10 aiavatar-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5375 b- defN 23-May-29 13:10 aiavatar-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 13:10 aiavatar-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-29 13:10 aiavatar-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1547 b- defN 23-May-29 13:10 aiavatar-0.1.1.dist-info/RECORD
+19 files, 41866 bytes uncompressed, 14927 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: aiavatar/speech/__init__.py
 Comment: 
 
 Filename: aiavatar/speech/voicevox.py
 Comment: 
 
-Filename: aiavatar-0.1.0.dist-info/LICENSE
+Filename: aiavatar-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: aiavatar-0.1.0.dist-info/METADATA
+Filename: aiavatar-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: aiavatar-0.1.0.dist-info/WHEEL
+Filename: aiavatar-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: aiavatar-0.1.0.dist-info/top_level.txt
+Filename: aiavatar-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: aiavatar-0.1.0.dist-info/RECORD
+Filename: aiavatar-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiavatar/bot.py

```diff
@@ -1,33 +1,31 @@
 import asyncio
 from logging import getLogger, NullHandler
 import traceback
-from typing import List, Callable
+from typing import Callable
 # Device
 from .device import AudioDevice
 # Processor
 from .processors.chatgpt import ChatGPTProcessor
 # Listener
-from .listeners.wakeword import WakewordListener
 from .listeners.voicerequest import VoiceRequestListener
 # Avatar
 from .speech.voicevox import VoicevoxSpeechController
 from .animation import AnimationController, AnimationControllerDummy
 from .face import FaceController, FaceControllerDummy
 from .avatar import AvatarController
 
 class AIAvatar:
     def __init__(
         self,
         google_api_key: str,
         openai_api_key: str,
         voicevox_url: str,
         voicevox_speaker_id: int=46,
-        wakewords: List[str]=None,
-        wakevoice: str="どうしたの",
+        start_voice: str="どうしたの",
         system_message_content: str=None,
         animation_controller: AnimationController=None,
         face_controller: FaceController=None,
         avatar_request_parser: Callable=None,
         input_device: int=-1,
         output_device: int=-1
     ):
@@ -58,32 +56,31 @@
         self.logger.info(f"Output device: [{output_device}] {output_device_info['name']}")
 
         # Processor
         self.chat_processor = ChatGPTProcessor(self.openai_api_key, system_message_content=system_message_content)
 
         # Listeners
         self.request_listener = VoiceRequestListener(self.google_api_key, device_index=self.input_device)
-        self.wakewords = wakewords or ["こんにちは"]
-        self.wakevoice = wakevoice
-        async def on_ww(text):
-            self.logger.info(f"Wakeword: {text}")
-            await self.chat()
-        self.wakeword_listener = WakewordListener(self.google_api_key, self.wakewords, on_ww, device_index=self.input_device)
 
         # Avatar
         speech_controller = VoicevoxSpeechController(self.voicevox_url, self.voicevox_speaker_id, device_index=self.output_device)
         animation_controller = animation_controller or AnimationControllerDummy()
         face_controller = face_controller or FaceControllerDummy()
         self.avatar_controller = AvatarController(speech_controller, animation_controller, face_controller, avatar_request_parser)
 
-    async def chat(self):
-        try:
-            await self.avatar_controller.speech_controller.speak(self.wakevoice)
-        except Exception as ex:
-            self.logger.error(f"Error at starting chat: {str(ex)}\n{traceback.format_exc()}")
+        # Chat
+        self.chat_task = None
+        self.start_voice = start_voice
+
+    async def chat(self, skip_start_voice=False):
+        if not skip_start_voice:
+            try:
+                await self.avatar_controller.speech_controller.speak(self.start_voice)
+            except Exception as ex:
+                self.logger.error(f"Error at starting chat: {str(ex)}\n{traceback.format_exc()}")
 
         while True:
             try:
                 req = await self.request_listener.get_request()
                 if not req:
                     break
 
@@ -102,11 +99,16 @@
                         self.avatar_controller.set_text(sentence)
 
                 self.avatar_controller.set_stop()
                 await avatar_task
             
             except Exception as ex:
                 self.logger.error(f"Error at chatting loop: {str(ex)}\n{traceback.format_exc()}")
-    
 
-    async def start(self):
-        await self.wakeword_listener.start_listening()
+    async def start_chat(self):
+        self.stop_chat()
+        self.chat_task = asyncio.create_task(self.chat())
+        await self.chat_task
+
+    def stop_chat(self):
+        if self.chat_task is not None:
+            self.chat_task.cancel()
```

## aiavatar/listeners/__init__.py

```diff
@@ -20,38 +20,38 @@
         self.min_duration = min_duration
         self.max_duration = max_duration
         self.lang = lang
         self.rate = rate
         self.device_index = device_index
         self.is_listening = False
 
-    def record_audio(self, device_index) -> list:
+    def record_audio(self, device_index) -> bytes:
         audio_data = []
 
         def callback(in_data, frame_count, time_info, status):
             audio_data.append(in_data)
             return (None, pyaudio.paContinue)
 
-        stream = pyaudio.PyAudio().open(
-            input_device_index=device_index,
-            format=pyaudio.paInt16,
-            channels=1,
-            rate=self.rate,
-            input=True,
-            stream_callback=callback
-        )
-
-        start_time = time.time()
-        is_recording = False
-        silence_start_time = time.time()
-        is_silent = False
-        last_detected_time = time.time()
-        stream.start_stream()
-
         try:
+            stream = pyaudio.PyAudio().open(
+                input_device_index=device_index,
+                format=pyaudio.paInt16,
+                channels=1,
+                rate=self.rate,
+                input=True,
+                stream_callback=callback
+            )
+
+            start_time = time.time()
+            is_recording = False
+            silence_start_time = time.time()
+            is_silent = False
+            last_detected_time = time.time()
+            stream.start_stream()
+
             while stream.is_active():
                 current_time = time.time()
                 volume = numpy.frombuffer(b"".join(audio_data[-10:]), dtype=numpy.int16).max() if audio_data else 0
 
                 if not is_recording:
                     if volume > self.volume_threshold:
                         audio_data = audio_data[-100:]  # Use 100ms data before start recording
@@ -98,15 +98,16 @@
         except Exception as ex:
             self.logger.error(f"Error at record_audio: {str(ex)}\n{traceback.format_exc()}")
 
         finally:
             stream.stop_stream()
             stream.close()
 
-        return []
+        # Return empty bytes
+        return b"".join([])
 
     async def transcribe(self, audio_data: list) -> str:
         audio_b64 = base64.b64encode(audio_data).decode("utf-8")
 
         request_body = {
             "config": {
                 "encoding": "LINEAR16",
@@ -120,38 +121,48 @@
 
         async with aiohttp.ClientSession() as session:
             async with session.post(
                 f"https://speech.googleapis.com/v1/speech:recognize?key={self.api_key}",
                 json=request_body
             ) as resp:
                 j = await resp.json()
+
+                if resp.status != 200:
+                    self.logger.error(f"Failed in recognition: {resp.status}\n{j}")
+                    return None
+
                 if j.get("results"):
                     if j["results"][0]["alternatives"][0].get("transcript"):
                         return j["results"][0]["alternatives"][0]["transcript"]
 
         return None
 
     async def start_listening(self):
         self.is_listening = True
 
         try:
             self.logger.info(f"Listening... ({self.__class__.__name__})")
             while self.is_listening:
                 audio_data = self.record_audio(self.device_index)
 
-                recognized_text = await self.transcribe(audio_data)
+                if audio_data:
+                    recognized_text = await self.transcribe(audio_data)
 
-                if recognized_text:
-                    await self.on_speech_recognized(recognized_text)
+                    if recognized_text:
+                        await self.on_speech_recognized(recognized_text)
+                    else:
+                        self.logger.info("No speech recognized")
+                
                 else:
-                    self.logger.info("No speech recognized")
+                    # Stop listening when no recorded data
+                    break
 
             self.logger.info(f"Stopped listening ({self.__class__.__name__})")
 
         except Exception as ex:
-            pass
+            self.logger.error(f"Error at start_listening: {str(ex)}\n{traceback.format_exc()}")
 
         finally:
             self.is_listening = False
 
     def stop_listening(self):
         self.is_listening = False
```

## aiavatar/listeners/wakeword.py

```diff
@@ -1,12 +1,19 @@
+import asyncio
+from threading import Thread
 from typing import Callable
 from . import SpeechListenerBase
 
 class WakewordListener(SpeechListenerBase):
     def __init__(self, api_key: str, wakewords: list, on_wakeword: Callable, volume_threshold: int=3000, timeout: float=0.3, min_duration: float=0.2, max_duration: float=2, lang: str="ja-JP", rate: int=44100, device_index: int=-1):
         super().__init__(api_key, self.invoke_on_wakeword, volume_threshold, timeout, 0.0, min_duration, max_duration, lang, rate, device_index)
         self.wakewords = wakewords
         self.on_wakeword = on_wakeword
     
     async def invoke_on_wakeword(self, text: str):
         if text in self.wakewords:
             await self.on_wakeword(text)
+
+    def start(self):
+        th = Thread(target=asyncio.run, args=(self.start_listening(),), daemon=True)
+        th.start()
+        return th
```

## aiavatar/speech/voicevox.py

```diff
@@ -55,14 +55,15 @@
                 data = f.readframes(frame_count)
                 return (data, pyaudio.paContinue)
 
             stream = self.pa.open(format=self.pa.get_format_from_width(width=f.getsampwidth()),
                 output_device_index=self.device_index,
                 channels=f.getnchannels(),
                 rate=f.getframerate(),
+                frames_per_buffer=1024,
                 output=True,
                 stream_callback=stream_callback,
             )
 
             try:
                 self._is_speaking = True
                 stream.start_stream()
```

## Comparing `aiavatar-0.1.0.dist-info/LICENSE` & `aiavatar-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiavatar-0.1.0.dist-info/METADATA` & `aiavatar-0.1.1.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiavatar
-Version: 0.1.0
+Version: 0.1.1
 Summary: 🥰 Building AI-based conversational avatars lightning fast ⚡️💬
 Home-page: https://github.com/uezo/aiavatar
 Author: uezo
 Author-email: uezo@uezo.net
 Maintainer: uezo
 Maintainer-email: uezo@uezo.net
 License: Apache v2
@@ -20,15 +20,15 @@
 
 🥰 Building AI-based conversational avatars lightning fast ⚡️💬
 
 ![AIAvatarKit Architecture Overview](documents/images/aiavatarkit_overview.png) 
 
 # ✨ Features
 
-* Live anywhere: VRChat, Cluster and any other metaverse platforms, and even devices in real world.
+* Live anywhere: VRChat, cluster and any other metaverse platforms, and even devices in real world.
 * Extensible: Unlimited capabilities that depends on you.
 * Easy to start: Ready to start conversation right out of the box.
 
 
 # 🍩 Requirements
 
 - VOICEVOX API in your computer or network reachable machine (Text-to-Speech)
@@ -43,20 +43,19 @@
 ```bash
 $ pip install aiavatar
 ```
 
 Make the script as  `run.py`.
 
 ```python
-import asyncio
 import logging
-from aiavatar import AIAvatar
+from aiavatar import AIAvatar, WakewordListener
 
-GOOGLE_API_KEY = "YOUR API KEY"
-OPENAI_API_KEY = "YOUR API KEY"
+GOOGLE_API_KEY = "YOUR_API_KEY"
+OPENAI_API_KEY = "YOUR_API_KEY"
 VV_URL = "http://127.0.0.1:50021"
 VV_SPEAKER = 46
 
 # Configure root logger
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 log_format = logging.Formatter("[%(levelname)s] %(asctime)s : %(message)s")
@@ -70,23 +69,38 @@
 
 例
 [face:joy]ねえ、海が見えるよ！[face:fun]早く泳ごうよ。
 """
 
 # Create AIAvatar
 app = AIAvatar(
-    GOOGLE_API_KEY,
-    OPENAI_API_KEY,
-    VV_URL,
-    VV_SPEAKER,
+    google_api_key=GOOGLE_API_KEY,
+    openai_api_key=OPENAI_API_KEY,
+    voicevox_url=VV_URL,
+    voicevox_speaker_id=VV_SPEAKER,
     system_message_content=system_message_content,
 )
 
-# Start AIAvatar
-asyncio.run(app.start())
+# Create WakewordListener
+wakewords = ["こんにちは"]
+
+async def on_wakeword(text):
+    logger.info(f"Wakeword: {text}")
+    await app.start_chat()
+
+wakeword_listener = WakewordListener(
+    api_key=GOOGLE_API_KEY,
+    wakewords=wakewords,
+    on_wakeword=on_wakeword,
+    device_index=app.input_device
+)
+
+# Start listening
+ww_thread = wakeword_listener.start()
+ww_thread.join()
 ```
 
 Start AIAvatar.
 
 ```bash
 $ python run.py
 ```
@@ -142,7 +156,51 @@
 ```bash
 $ run.py
 ```
 
 Launch VRChat as desktop mode on the machine that runs `run.py` and log in with the account for AIAvatar. Then set `VB-Cable-A` to microphone in VRChat setting window.
 
 That's all! Let's chat with the AIAvatar. Log in to VRChat on another machine (or Quest) and go to the world the AIAvatar is in.
+
+# ⚡️ Use custom listener
+
+It's very easy to add your original listeners. Just make it run on other thread and invoke `app.start_chat()` when the listener handles the event.
+
+Here the example of `FileSystemListener` that invokes chat when `test.txt` is found on the file system.
+
+```python
+import asyncio
+import os
+from threading import Thread
+from time import sleep
+
+class FileSystemListener:
+    def __init__(self, on_file_found):
+        self.on_file_found = on_file_found
+
+    def start_listening(self):
+        while True:
+            # Check file every 3 seconds
+            if os.path.isfile("test.txt"):
+                asyncio.run(self.on_file_found())
+            sleep(3)
+
+    def start(self):
+        th = Thread(target=self.start_listening, daemon=True)
+        th.start()
+        return th
+```
+
+Use this listener in `run.py` like below.
+
+```python
+# Event handler
+def on_file_found():
+    asyncio.run(app.chat())
+
+# Instantiate
+fs_listener = FileSystemListener(on_file_found)
+fs_thread = fs_listener.start()
+    :
+# Wait for finish
+fs_thread.join()
+```
```

