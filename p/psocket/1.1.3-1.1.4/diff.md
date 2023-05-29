# Comparing `tmp/psocket-1.1.3.tar.gz` & `tmp/psocket-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psocket-1.1.3.tar", last modified: Fri May 26 10:54:05 2023, max compression
+gzip compressed data, was "psocket-1.1.4.tar", last modified: Mon May 29 16:57:57 2023, max compression
```

## Comparing `psocket-1.1.3.tar` & `psocket-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-26 10:54:05.919239 psocket-1.1.3/
--rw-r--r--   0 c-pher     (502) staff       (20)     1074 2023-05-25 16:06:10.000000 psocket-1.1.3/LICENSE
--rw-r--r--   0 c-pher     (502) staff       (20)     3912 2023-05-26 10:54:05.919114 psocket-1.1.3/PKG-INFO
--rw-r--r--   0 c-pher     (502) staff       (20)     3109 2023-05-26 10:43:49.000000 psocket-1.1.3/README.md
-drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-26 10:54:05.918117 psocket-1.1.3/psocket/
--rw-r--r--   0 c-pher     (502) staff       (20)     6455 2023-05-26 10:44:07.000000 psocket-1.1.3/psocket/__init__.py
-drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-26 10:54:05.918929 psocket-1.1.3/psocket.egg-info/
--rw-r--r--   0 c-pher     (502) staff       (20)     3912 2023-05-26 10:54:05.000000 psocket-1.1.3/psocket.egg-info/PKG-INFO
--rw-r--r--   0 c-pher     (502) staff       (20)      200 2023-05-26 10:54:05.000000 psocket-1.1.3/psocket.egg-info/SOURCES.txt
--rw-r--r--   0 c-pher     (502) staff       (20)        1 2023-05-26 10:54:05.000000 psocket-1.1.3/psocket.egg-info/dependency_links.txt
--rw-r--r--   0 c-pher     (502) staff       (20)       15 2023-05-26 10:54:05.000000 psocket-1.1.3/psocket.egg-info/requires.txt
--rw-r--r--   0 c-pher     (502) staff       (20)        8 2023-05-26 10:54:05.000000 psocket-1.1.3/psocket.egg-info/top_level.txt
--rw-r--r--   0 c-pher     (502) staff       (20)       38 2023-05-26 10:54:05.919282 psocket-1.1.3/setup.cfg
--rw-r--r--   0 c-pher     (502) staff       (20)     1194 2023-05-26 10:25:33.000000 psocket-1.1.3/setup.py
+drwxr-xr-x   0 c-pher     (501) staff       (20)        0 2023-05-29 16:57:57.430652 psocket-1.1.4/
+-rw-r--r--   0 c-pher     (501) staff       (20)     1074 2023-05-29 16:39:26.000000 psocket-1.1.4/LICENSE
+-rw-r--r--   0 c-pher     (501) staff       (20)     4032 2023-05-29 16:57:57.430539 psocket-1.1.4/PKG-INFO
+-rw-r--r--   0 c-pher     (501) staff       (20)     3229 2023-05-29 16:57:34.000000 psocket-1.1.4/README.md
+drwxr-xr-x   0 c-pher     (501) staff       (20)        0 2023-05-29 16:57:57.429664 psocket-1.1.4/psocket/
+-rw-r--r--   0 c-pher     (501) staff       (20)     6818 2023-05-29 16:56:50.000000 psocket-1.1.4/psocket/__init__.py
+drwxr-xr-x   0 c-pher     (501) staff       (20)        0 2023-05-29 16:57:57.430388 psocket-1.1.4/psocket.egg-info/
+-rw-r--r--   0 c-pher     (501) staff       (20)     4032 2023-05-29 16:57:57.000000 psocket-1.1.4/psocket.egg-info/PKG-INFO
+-rw-r--r--   0 c-pher     (501) staff       (20)      200 2023-05-29 16:57:57.000000 psocket-1.1.4/psocket.egg-info/SOURCES.txt
+-rw-r--r--   0 c-pher     (501) staff       (20)        1 2023-05-29 16:57:57.000000 psocket-1.1.4/psocket.egg-info/dependency_links.txt
+-rw-r--r--   0 c-pher     (501) staff       (20)       15 2023-05-29 16:57:57.000000 psocket-1.1.4/psocket.egg-info/requires.txt
+-rw-r--r--   0 c-pher     (501) staff       (20)        8 2023-05-29 16:57:57.000000 psocket-1.1.4/psocket.egg-info/top_level.txt
+-rw-r--r--   0 c-pher     (501) staff       (20)       38 2023-05-29 16:57:57.430688 psocket-1.1.4/setup.cfg
+-rw-r--r--   0 c-pher     (501) staff       (20)     1194 2023-05-29 16:41:24.000000 psocket-1.1.4/setup.py
```

### Comparing `psocket-1.1.3/LICENSE` & `psocket-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psocket-1.1.3/PKG-INFO` & `psocket-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psocket
-Version: 1.1.3
+Version: 1.1.4
 Summary: The cross-platform tool to work with remote connection using sockets
 Home-page: https://github.com/c-pher/PSocket.git
 Author: Andrey Komissarov
 Author-email: a.komisssarov@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -52,29 +52,36 @@
 
 client = SocketClient(host='172.16.0.48', port=3261)
 print(client)
 ```
 ```python
 from psocket import SocketClient
 
-client = SocketClient(host='172.16.0.48', port=3261)
+client = SocketClient(host='172.16.0.48', port=3261, initialize=True)
 print(client.send_command('<commands>'))
 ```
 
 ---
 
 ## Changelog
 
+##### 1.1.4 (29.05.2023)
+
+- debug log extended with timeout error
+- global timeout management added
+
 ##### 1.1.3 (26.05.2023)
+
 - Reading completion from the socket fixed
 - buffer size reduced to 4k
 - Logger extended
 - Refactoring
 
 ##### 1.1.2 (25.05.2023)
+
 - buffer size increased to 8k
 - debug log added
 
 ##### 1.1.1 (04.08.2022)
 
 - Detect command is completed by \n\n
```

### Comparing `psocket-1.1.3/README.md` & `psocket-1.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,29 +31,36 @@
 
 client = SocketClient(host='172.16.0.48', port=3261)
 print(client)
 ```
 ```python
 from psocket import SocketClient
 
-client = SocketClient(host='172.16.0.48', port=3261)
+client = SocketClient(host='172.16.0.48', port=3261, initialize=True)
 print(client.send_command('<commands>'))
 ```
 
 ---
 
 ## Changelog
 
+##### 1.1.4 (29.05.2023)
+
+- debug log extended with timeout error
+- global timeout management added
+
 ##### 1.1.3 (26.05.2023)
+
 - Reading completion from the socket fixed
 - buffer size reduced to 4k
 - Logger extended
 - Refactoring
 
 ##### 1.1.2 (25.05.2023)
+
 - buffer size increased to 8k
 - debug log added
 
 ##### 1.1.1 (04.08.2022)
 
 - Detect command is completed by \n\n
```

### Comparing `psocket-1.1.3/psocket/__init__.py` & `psocket-1.1.4/psocket/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,53 +11,54 @@
     def __init__(self,
                  host: str,
                  port: int = 0,
                  buffer_size: int = 4096,
                  initialize: bool = False,
                  logger_enabled: bool = True,
                  log_level: str = 'INFO',
-                 connection_timeout: int = None):
+                 timeout: int = None):
         """Create and connect client to a remote host.
 
         :param host: Host IP
         :param port: Port
         :param logger_enabled: Enable/disable module logger
         :param log_level: INFO
         :param initialize: Establish connection during init
+        :param timeout: Read and connection timeout
         """
 
         self.host = host
         self.port = port
         self.buffer_size = buffer_size
         self.logger = logger('SocketClient', enabled=logger_enabled, level=log_level)
-        self.connection_timeout = connection_timeout
+        self.timeout = timeout
 
         if initialize:
             try:
-                self.client = self.connect(timeout=self.connection_timeout)
+                self.client = self.connect(timeout=self.timeout)
             except ConnectionRefusedError as err:
                 self.logger.error(f'Cannot establish socket connection to {self.host}:{self.port}. {err}')
                 raise err
             except socket.gaierror as err:
                 self.logger.error(f'Check host and port format. {self.host}:{self.port}. {err}')
                 raise err
             except socket.timeout as err:
-                self.logger.error(f'{self.host}:{self.port} is unavailable within {self.connection_timeout} sec. {err}')
+                self.logger.error(f'{self.host}:{self.port} is unavailable within {self.timeout} sec. {err}')
                 raise err
 
     def __getattr__(self, attr):
         self.logger.error(f'No such attribute ({attr}) error. Perhaps, object is not initialized.')
         raise AttributeError(f'SocketClient does not have specific attribute "{attr}"')
 
     def __str__(self):
         msg = (f'Host: {self.host}\n'
                f'Port: {self.port}\n'
                f'Reading buffer size: {self.buffer_size}\n'
                f'Logger name: {self.logger.name}\n'
-               f'Connection timeout: {self.connection_timeout}')
+               f'Timeout: {self.timeout}')
         return msg
 
     def connect(self, timeout: int = None):
         """Create connection
 
         :param timeout:
         :return:
@@ -145,28 +146,35 @@
             self.logger.error(f'{self.host:<14} | {err}')
             raise err
 
     def receive_all(self, stop_signs: str = '\r\n\r\n'):
         """Get and decode socket response
 
         Args:
-            buffer_size: 4096 by default
             stop_signs: Symbols which will stop socket reading
         """
 
         self.logger.debug(f'Start reading from socket.\n\t'
-                          f'{self.buffer_size = }\n\t'
-                          f'{stop_signs = }')
+                          f'Timeout:     {self.timeout} seconds\n\t'
+                          f'Buffer size: {self.buffer_size} bytes\n\t'
+                          f'Stop signs:  {stop_signs.__repr__()}')
+
+        self.logger.debug(f'Set socket global timeout to {self.timeout}')
+        self.client.settimeout(self.timeout)
+        self.logger.debug('Completed')
 
         data = bytearray()
-
         self.logger.debug(f'Initial data: {data}')
 
         while True:
-            chunk = self.client.recv(self.buffer_size)
+            try:
+                chunk = self.client.recv(self.buffer_size)
+            except TimeoutError as err:
+                self.logger.exception(f'Read timeout ({self.timeout}) error')
+                raise err
             self.logger.debug(f'Chunk ({len(chunk)}): {chunk}')
 
             data.extend(chunk)
 
             if data.endswith(stop_signs.encode()):
                 self.logger.debug(f'Reading response ran to completion. <{stop_signs = }> received.')
                 break
```

### Comparing `psocket-1.1.3/psocket.egg-info/PKG-INFO` & `psocket-1.1.4/psocket.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psocket
-Version: 1.1.3
+Version: 1.1.4
 Summary: The cross-platform tool to work with remote connection using sockets
 Home-page: https://github.com/c-pher/PSocket.git
 Author: Andrey Komissarov
 Author-email: a.komisssarov@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -52,29 +52,36 @@
 
 client = SocketClient(host='172.16.0.48', port=3261)
 print(client)
 ```
 ```python
 from psocket import SocketClient
 
-client = SocketClient(host='172.16.0.48', port=3261)
+client = SocketClient(host='172.16.0.48', port=3261, initialize=True)
 print(client.send_command('<commands>'))
 ```
 
 ---
 
 ## Changelog
 
+##### 1.1.4 (29.05.2023)
+
+- debug log extended with timeout error
+- global timeout management added
+
 ##### 1.1.3 (26.05.2023)
+
 - Reading completion from the socket fixed
 - buffer size reduced to 4k
 - Logger extended
 - Refactoring
 
 ##### 1.1.2 (25.05.2023)
+
 - buffer size increased to 8k
 - debug log added
 
 ##### 1.1.1 (04.08.2022)
 
 - Detect command is completed by \n\n
```

### Comparing `psocket-1.1.3/setup.py` & `psocket-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='psocket',
-    version='1.1.3',
+    version='1.1.4',
     packages=['psocket'],
     url='https://github.com/c-pher/PSocket.git',
     license='MIT',
     author='Andrey Komissarov',
     author_email='a.komisssarov@gmail.com',
     description='The cross-platform tool to work with remote connection using sockets',
     long_description=long_description,
```

