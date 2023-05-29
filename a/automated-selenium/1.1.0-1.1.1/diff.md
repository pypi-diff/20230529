# Comparing `tmp/automated_selenium-1.1.0.tar.gz` & `tmp/automated_selenium-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automated_selenium-1.1.0.tar", max compression
+gzip compressed data, was "automated_selenium-1.1.1.tar", max compression
```

## Comparing `automated_selenium-1.1.0.tar` & `automated_selenium-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      143 2023-05-22 11:20:22.645610 automated_selenium-1.1.0/automated_selenium/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:49.528226 automated_selenium-1.1.0/automated_selenium/drivers/__init__.py
--rw-r--r--   0        0        0     1009 2023-05-22 11:20:41.941751 automated_selenium-1.1.0/automated_selenium/drivers/undetected_driver.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:49.528226 automated_selenium-1.1.0/automated_selenium/pages/__init__.py
--rw-r--r--   0        0        0    15383 2023-05-22 11:21:18.542924 automated_selenium-1.1.0/automated_selenium/pages/base_page.py
--rw-r--r--   0        0        0     1175 2023-05-22 10:40:23.715165 automated_selenium-1.1.0/automated_selenium/resources/resources.py
--rw-r--r--   0        0        0     1121 2023-05-22 10:02:06.511333 automated_selenium-1.1.0/LICENSE
--rw-r--r--   0        0        0      667 2023-05-22 12:08:15.790370 automated_selenium-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9041 2023-05-22 12:03:21.271803 automated_selenium-1.1.0/README.md
--rw-r--r--   0        0        0     9766 1970-01-01 00:00:00.000000 automated_selenium-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      204 2023-05-29 08:01:38.722352 automated_selenium-1.1.1/automated_selenium/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:02:49.528226 automated_selenium-1.1.1/automated_selenium/drivers/__init__.py
+-rw-r--r--   0        0        0     1009 2023-05-22 11:20:41.941751 automated_selenium-1.1.1/automated_selenium/drivers/undetected_driver.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:02:49.528226 automated_selenium-1.1.1/automated_selenium/pages/__init__.py
+-rw-r--r--   0        0        0    15383 2023-05-22 11:21:18.542924 automated_selenium-1.1.1/automated_selenium/pages/base_page.py
+-rw-r--r--   0        0        0     1175 2023-05-22 10:40:23.715165 automated_selenium-1.1.1/automated_selenium/resources/resources.py
+-rw-r--r--   0        0        0     1121 2023-05-22 10:02:06.511333 automated_selenium-1.1.1/LICENSE
+-rw-r--r--   0        0        0      667 2023-05-29 08:02:55.653885 automated_selenium-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9767 2023-05-29 08:15:57.609791 automated_selenium-1.1.1/README.md
+-rw-r--r--   0        0        0    10472 1970-01-01 00:00:00.000000 automated_selenium-1.1.1/PKG-INFO
```

### Comparing `automated_selenium-1.1.0/automated_selenium/drivers/undetected_driver.py` & `automated_selenium-1.1.1/automated_selenium/drivers/undetected_driver.py`

 * *Files identical despite different names*

### Comparing `automated_selenium-1.1.0/automated_selenium/pages/base_page.py` & `automated_selenium-1.1.1/automated_selenium/pages/base_page.py`

 * *Files identical despite different names*

### Comparing `automated_selenium-1.1.0/automated_selenium/resources/resources.py` & `automated_selenium-1.1.1/automated_selenium/resources/resources.py`

 * *Files identical despite different names*

### Comparing `automated_selenium-1.1.0/LICENSE` & `automated_selenium-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `automated_selenium-1.1.0/pyproject.toml` & `automated_selenium-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "automated-selenium"
-version = "1.1.0"
+version = "1.1.1"
 description = "Automated-Selenium is a Python library that provides a base page class designed to facilitate the implementation of the Page Object Model (POM) structure in Selenium-based test automation projects."
 authors = ["Waqar Khan <waqarkhan1252617@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "automated_selenium"}]
 
 [tool.poetry.dependencies]
```

### Comparing `automated_selenium-1.1.0/README.md` & `automated_selenium-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,49 +57,69 @@
    from .resources import LoginResources
    ```
 
 3. Create a new class for your page object, inherit from `BasePage` and add your own methods:
 
    ```python
    class MyPage(BasePage):
+       logged_in = False
+       url = 'https://example.com'
+
+       def __init__(self, *args, **kwargs):
+         super().__init__(*args, **kwargs)
+         # call your web url here
+         self.driver.get(self.url)
+         
        # Add your custom methods and properties here
+       def check_login(self):
+         # check if the user is logged in
+         # perform some task to check login
+         # if user is logged in make self.logged_in = True
+         self.logged_in = True
+
        def login(self, username: str, password: str):
-         # Find username field
-         username_field = self.find(LoginResources.username_field)
-         # Type username like human
-         self.send_keys(username_field, username)
-
-         # Find password field
-         password_field = self.find(LoginResources.password_field)
-         # Type password like human
-         self.send_keys(password_field, password)
-
-         # Find submit button
-         submit_button = self.find(LoginResources.submit_button)
-         # click on submit button
-         self.click(submit_button)
-
-         # Return self if you want to chain your actions as follow.
-         # login_page = LoginPage(driver)
-         # login_page.check_login()\
-         #           .login()\
-         return self
-   ```
+         # check if user is already logged in
+         self.check_login()
+         if self.logged_in:
+            # Find username field
+            username_field = self.find(LoginResources.username_field)
+            # Type username like human
+            self.send_keys(username_field, username)
+
+            # Find password field
+            password_field = self.find(LoginResources.password_field)
+            # Type password like human
+            self.send_keys(password_field, password)
+
+            # Find submit button
+            submit_button = self.find(LoginResources.submit_button)
+            # click on submit button
+            self.click(submit_button)
+            # check if you are logged in successfully
+            self.check_login()
+            # Return self if you want to chain your actions as follow.
+            # login_page = LoginPage(driver)
+            # login_page.check_login()\
+            #           .login()\
+            return self
+      ```
 4. Now use this page object to login in your `main.py`.
    ```python
    from automated_selenium import get_undetected_chrome_browser
    from your_pages import MyPage
 
    def main():
       # A profile to use by browser it will create new one if it do not have already
       # the profile will store cookies and other user data for the next run.
       profile_name = 'my_profile'
       # Create a new driver instance
       driver = get_undetected_chrome_browser(profile_name)
       my_page = MyPage(driver)
+      # Perform some task here
+
       my_page.login(username='admin', password='automated_selenium')
 
    if __name__ == '__main__':
       main()
    ```
    
 5. Implement your page-specific methods and use the provided base methods to interact with web elements, handle navigation, and perform other automation tasks.
```

### Comparing `automated_selenium-1.1.0/PKG-INFO` & `automated_selenium-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automated-selenium
-Version: 1.1.0
+Version: 1.1.1
 Summary: Automated-Selenium is a Python library that provides a base page class designed to facilitate the implementation of the Page Object Model (POM) structure in Selenium-based test automation projects.
 License: MIT
 Author: Waqar Khan
 Author-email: waqarkhan1252617@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -77,49 +77,69 @@
    from .resources import LoginResources
    ```
 
 3. Create a new class for your page object, inherit from `BasePage` and add your own methods:
 
    ```python
    class MyPage(BasePage):
+       logged_in = False
+       url = 'https://example.com'
+
+       def __init__(self, *args, **kwargs):
+         super().__init__(*args, **kwargs)
+         # call your web url here
+         self.driver.get(self.url)
+         
        # Add your custom methods and properties here
+       def check_login(self):
+         # check if the user is logged in
+         # perform some task to check login
+         # if user is logged in make self.logged_in = True
+         self.logged_in = True
+
        def login(self, username: str, password: str):
-         # Find username field
-         username_field = self.find(LoginResources.username_field)
-         # Type username like human
-         self.send_keys(username_field, username)
-
-         # Find password field
-         password_field = self.find(LoginResources.password_field)
-         # Type password like human
-         self.send_keys(password_field, password)
-
-         # Find submit button
-         submit_button = self.find(LoginResources.submit_button)
-         # click on submit button
-         self.click(submit_button)
-
-         # Return self if you want to chain your actions as follow.
-         # login_page = LoginPage(driver)
-         # login_page.check_login()\
-         #           .login()\
-         return self
-   ```
+         # check if user is already logged in
+         self.check_login()
+         if self.logged_in:
+            # Find username field
+            username_field = self.find(LoginResources.username_field)
+            # Type username like human
+            self.send_keys(username_field, username)
+
+            # Find password field
+            password_field = self.find(LoginResources.password_field)
+            # Type password like human
+            self.send_keys(password_field, password)
+
+            # Find submit button
+            submit_button = self.find(LoginResources.submit_button)
+            # click on submit button
+            self.click(submit_button)
+            # check if you are logged in successfully
+            self.check_login()
+            # Return self if you want to chain your actions as follow.
+            # login_page = LoginPage(driver)
+            # login_page.check_login()\
+            #           .login()\
+            return self
+      ```
 4. Now use this page object to login in your `main.py`.
    ```python
    from automated_selenium import get_undetected_chrome_browser
    from your_pages import MyPage
 
    def main():
       # A profile to use by browser it will create new one if it do not have already
       # the profile will store cookies and other user data for the next run.
       profile_name = 'my_profile'
       # Create a new driver instance
       driver = get_undetected_chrome_browser(profile_name)
       my_page = MyPage(driver)
+      # Perform some task here
+
       my_page.login(username='admin', password='automated_selenium')
 
    if __name__ == '__main__':
       main()
    ```
    
 5. Implement your page-specific methods and use the provided base methods to interact with web elements, handle navigation, and perform other automation tasks.
```

