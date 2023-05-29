# Comparing `tmp/UnlimitedGPT-0.0.9.tar.gz` & `tmp/UnlimitedGPT-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.0.9.tar", last modified: Sun May 28 15:55:56 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.1.0.tar", last modified: Mon May 29 16:25:03 2023, max compression
```

## Comparing `UnlimitedGPT-0.0.9.tar` & `UnlimitedGPT-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-28 15:55:56.646984 UnlimitedGPT-0.0.9/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     5974 2023-05-28 15:55:56.642984 UnlimitedGPT-0.0.9/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-28 15:55:56.606984 UnlimitedGPT-0.0.9/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    20332 2023-05-28 14:23:24.000000 UnlimitedGPT-0.0.9/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.0.9/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-28 15:55:56.630984 UnlimitedGPT-0.0.9/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2036 2023-05-28 13:36:32.000000 UnlimitedGPT-0.0.9/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-28 11:02:47.000000 UnlimitedGPT-0.0.9/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-28 11:29:18.000000 UnlimitedGPT-0.0.9/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-28 15:55:56.610984 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     5974 2023-05-28 15:55:54.000000 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      344 2023-05-28 15:55:54.000000 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-28 15:55:54.000000 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-28 15:55:54.000000 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-05-28 15:55:54.000000 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-28 15:55:56.646984 UnlimitedGPT-0.0.9/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1686 2023-05-28 14:37:21.000000 UnlimitedGPT-0.0.9/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-29 16:25:02.984886 UnlimitedGPT-0.1.0/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4181 2023-05-29 16:25:02.984886 UnlimitedGPT-0.1.0/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-29 16:25:02.976886 UnlimitedGPT-0.1.0/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    25484 2023-05-29 16:14:45.000000 UnlimitedGPT-0.1.0/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.0/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-29 16:25:02.980886 UnlimitedGPT-0.1.0/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2188 2023-05-29 14:53:34.000000 UnlimitedGPT-0.1.0/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-28 11:02:47.000000 UnlimitedGPT-0.1.0/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-28 11:29:18.000000 UnlimitedGPT-0.1.0/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-29 16:25:02.980886 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4181 2023-05-29 16:25:02.000000 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      344 2023-05-29 16:25:02.000000 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-29 16:25:02.000000 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-29 16:25:02.000000 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-05-29 16:25:02.000000 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-29 16:25:02.988886 UnlimitedGPT-0.1.0/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1686 2023-05-29 16:20:08.000000 UnlimitedGPT-0.1.0/setup.py
```

### Comparing `UnlimitedGPT-0.0.9/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.1.0/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from json import loads
 from logging import getLogger, DEBUG, Formatter, StreamHandler
 from weakref import finalize
 
 from markdownify import markdownify
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.common.exceptions import TimeoutException, NoSuchElementException
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.action_chains import ActionChains
 from undetected_chromedriver import ChromeOptions
 
 from .internal.driver import ChatGPTDriver
@@ -84,15 +85,15 @@
         if hasattr(self, 'driver'):
             self.logger.debug('Closing browser...')
             self.driver.quit()
         if hasattr(self, 'display'):
             self.logger.debug('Closing display...')
             self.display.stop()
 
-    def get_out_of_menu(self) -> None:
+    def _get_out_of_menu(self) -> None:
         """
         Get out of any menu present.
         """
         for i in range(5):
             # First escape click is to remove the options menu
             # Second escape click is to get out of the settings menu
             # The rest are just to be safe
@@ -277,21 +278,22 @@
             raise ValueError('Invalid session token')
         self.logger.debug('Authorization is valid')
 
         self.logger.debug('Closing tab...')
         self.driver.close()
         self.driver.switch_to.window(original_window)
 
-    def send_message(self, message: str) -> ChatGPTResponse:
+    def send_message(self, message: str, timeout: int = 240) -> ChatGPTResponse:
         """
         Send a message to ChatGPT.
 
         Args:
         ----------
             message (str): Message to send.
+            timeout (int, optional): Timeout in seconds. Defaults to 240.
 
         Returns:
         ----------
             ChatGPTResponse: Response from ChatGPT.
 
         Raises:
         ----------
@@ -310,15 +312,15 @@
             for char in message:
                 textbox.send_keys(char)
                 sleep(self._input_delay)
 
         textbox.send_keys(Keys.ENTER)
 
         self.logger.debug('Waiting for completion...')
-        WebDriverWait(self.driver, 240).until_not(
+        WebDriverWait(self.driver, timeout).until_not(
             EC.presence_of_element_located(CGPTV.chatgpt_streaming)
         )
 
         self.logger.debug('Getting response...')
         responses = self.driver.find_elements(*CGPTV.chatgpt_big_response)
         if responses:
             response = responses[-1]
@@ -399,49 +401,49 @@
             - `SYSTEM`: Switch to the system theme.
         """
         self.logger.debug(f'Switching theme to {theme}...')
         try:
             menu_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_button)
             if not menu_button_clicked:
                 self.logger.debug('Could not click menu button')
-                return self.get_out_of_menu()
+                return self._get_out_of_menu()
 
             self.logger.debug('Clicked menu button')
             
             settings_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_settings_button)
             if not settings_button_clicked:
                 self.logger.debug('Could not click settings button')
-                return self.get_out_of_menu()
+                return self._get_out_of_menu()
 
             self.logger.debug('Clicked settings button')
             
             current_theme_value = self.driver.find_element(*CGPTV.chatgpt_outer_html).get_attribute('class')
             current_theme = 'LIGHT' if 'light' in current_theme_value else 'DARK'
             if theme == current_theme:
                 self.logger.debug('Theme is already set to the desired theme')
-                return self.get_out_of_menu()
+                return self._get_out_of_menu()
 
             select_element = self.driver.find_element(By.CSS_SELECTOR, 'select.rounded')
             ActionChains(self.driver).move_to_element(select_element).click().perform()
 
             if theme == 'OPPOSITE':
                 if current_theme == 'SYSTEM':
                     self.logger.debug('Theme cannot be set to opposite of system theme')
-                    return self.get_out_of_menu()
+                    return self._get_out_of_menu()
                     
                 opposite_theme = 'dark' if current_theme == 'LIGHT' else 'light'
                 option = self.driver.find_element(By.CSS_SELECTOR, f'select.rounded option[value={opposite_theme}]')
                 option.click()
                 self.logger.debug(f'Selected opposite theme of {current_theme}')
             else:
                 option = self.driver.find_element(By.CSS_SELECTOR, f'select.rounded option[value={theme.lower()}]')
                 option.click()
                 self.logger.debug(f'Selected theme {theme}')
             
-            self.get_out_of_menu()
+            self._get_out_of_menu()
         except NoSuchElementException:
             self.logger.debug('Could not find theme buttons')
             self.driver.save_screenshot('theme_switch_failed.png')
 
     def switch_account(self, session_token: str):
         """
         Switch the account.
@@ -522,7 +524,119 @@
         response = self.driver.page_source
         if response[0] != '{':
             response = self.driver.find_element(By.TAG_NAME, 'pre').text
         response = loads(response)
         if response == {}:
             self.logger.debug('Logout successful')
             return
+
+    def toggle_chat_history(self, state: bool = False) -> None:
+        """
+        Toggle chat history.
+
+        Args:
+        ----------
+            state (bool, optional): The state to set the chat history toggle to. Defaults to False.
+        """
+        self.logger.debug('Disabling chat history...')
+        try:
+            menu_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_button)
+            if not menu_button_clicked:
+                self.logger.debug('Could not click menu button')
+                return self._get_out_of_menu()
+
+            self.logger.debug('Clicked menu button')
+            
+            settings_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_settings_button)
+            if not settings_button_clicked:
+                self.logger.debug('Could not click settings button')
+                return self._get_out_of_menu()
+
+            self.logger.debug('Clicked settings button')
+
+            wait = WebDriverWait(self.driver, 20)
+
+            # Click "Data controls" button
+            data_controls_button: WebElement = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-state="inactive"][id^="radix-"][id$="-trigger-DataControls"]')))
+            data_controls_button.click()
+
+            # Click "Disable chat history" button
+            chat_history_toggle = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Chat History & Training"]')))
+            current_state = True if chat_history_toggle.get_attribute('aria-checked') == 'true' else False
+            if current_state == state:
+                self.logger.debug('Chat history is already set to the desired state')
+                return self._get_out_of_menu()
+            
+            chat_history_toggle.click()
+            self.logger.debug(f'Chat history is now {"enabled" if state else "disabled"}')
+            self._get_out_of_menu()
+        except:
+            self.logger.debug(f'Could not {"enable" if state else "disable"} chat history')
+            self.driver.save_screenshot('disable_chat_history_failed.png')
+    
+    def regenerate_response(self, message_timeout: int = 240, click_timeout: int = 20) -> ChatGPTResponse:
+        """
+        Regenerate the response.
+
+        Returns:
+        ----------
+            response (ChatGPTResponse): The newly regenerated response data.
+            message_timeout (int, optional): Time to wait for the message to regenerate before timing out. Defaults to 240.
+            click_timeout (int, optional): Time to wait for the click to succeed before timing out. Defaults to 20.
+
+        Raises:
+        ----------
+            TimeoutException: If the message fails to send.
+            TimeoutException: If the click fails to succeed.
+            ValueError: If the response is invalid.
+            ValueError: If the response is not found.
+        """
+        self.logger.debug('Regenerating response...')
+
+        # Click "Regenerate response" button
+        regenerate_response_button = WebDriverWait(self.driver, click_timeout).until(
+            EC.element_to_be_clickable(CGPTV.chatgpt_regenerate_response_button)
+        )
+        regenerate_response_button.click()
+
+        # Get the response, same way as send_message without the part of sending the message
+        self.logger.debug('Waiting for completion...')
+        WebDriverWait(self.driver, message_timeout).until_not(
+            EC.presence_of_element_located(CGPTV.chatgpt_streaming)
+        )
+
+        self.logger.debug('Getting response...')
+        responses = self.driver.find_elements(*CGPTV.chatgpt_big_response)
+        if responses:
+            response = responses[-1]
+            if 'text-red' in response.get_attribute('class'):
+                self.logger.debug('Response is an error')
+                raise ValueError(response.text)
+        response = self.driver.find_elements(*CGPTV.chatgpt_small_response)
+        try:
+            response = response[-1]
+        except IndexError:
+            self.logger.debug('Response not found, resetting conversation...')
+            self.reset_conversation()
+            raise ValueError('Response not found')
+
+        content = markdownify(response.get_attribute('innerHTML')).replace(
+            'Copy code`', '`'
+        )
+        
+        pattern = re.compile(
+            r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
+        )
+        matches = pattern.search(self.driver.current_url)
+        if not matches:
+            self.reset_conversation()
+            WebDriverWait(self.driver, 60).until(
+                EC.element_to_be_clickable(CGPTV.chatgpt_chats_list_first_node)
+            ).click()
+            sleep(0.5)
+            matches = pattern.search(self.driver.current_url)
+        try:
+            conversation_id = matches.group() # type: ignore
+        except:
+            conversation_id = None
+        self.logger.debug('Regenerated response')
+        return ChatGPTResponse(content, conversation_id)
```

### Comparing `UnlimitedGPT-0.0.9/UnlimitedGPT/internal/chatgpt_data.py` & `UnlimitedGPT-0.1.0/UnlimitedGPT/internal/chatgpt_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,9 +59,13 @@
         By.XPATH,
         "/html/body/div[1]/div[2]/div[1]/div/div/div/nav/div[3]/div/div/nav/a[3]"
     )
     chatgpt_theme_selector = (
         By.XPATH,
         "/html/body/div[5]/div/div/div/div[2]/div/div[2]/div/div[1]/div/select"
     )
+    chatgpt_regenerate_response_button = (
+        By.XPATH,
+        "/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div[1]/div/button"
+    )
 
     chatgpt_chat_url = 'https://chat.openai.com/chat'
```

### Comparing `UnlimitedGPT-0.0.9/UnlimitedGPT/internal/driver.py` & `UnlimitedGPT-0.1.0/UnlimitedGPT/internal/driver.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.0.9/UnlimitedGPT/internal/objects.py` & `UnlimitedGPT-0.1.0/UnlimitedGPT/internal/objects.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.0.9/setup.py` & `UnlimitedGPT-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     name='UnlimitedGPT',
     author='Sxvxge',
     url='https://github.com/Sxvxgee/UnlimitedGPT',
     project_urls={
         'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
         'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
     },
-    version="0.0.9",
+    version="0.1.0",
     packages=['UnlimitedGPT', 'UnlimitedGPT/internal'],
     py_modules=['UnlimitedGPT'],
     license='GPL-3.0 license',
     description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
```

