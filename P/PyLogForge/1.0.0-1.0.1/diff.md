# Comparing `tmp/PyLogForge-1.0.0.tar.gz` & `tmp/PyLogForge-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLogForge-1.0.0.tar", last modified: Mon May 29 13:16:13 2023, max compression
+gzip compressed data, was "PyLogForge-1.0.1.tar", last modified: Mon May 29 14:20:40 2023, max compression
```

## Comparing `PyLogForge-1.0.0.tar` & `PyLogForge-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 scuevas    (501) staff       (20)        0 2023-05-29 13:16:13.177572 PyLogForge-1.0.0/
--rw-r--r--   0 scuevas    (501) staff       (20)      557 2023-05-29 13:16:13.177475 PyLogForge-1.0.0/PKG-INFO
-drwxr-xr-x   0 scuevas    (501) staff       (20)        0 2023-05-29 13:16:13.177349 PyLogForge-1.0.0/PyLogForge.egg-info/
--rw-r--r--   0 scuevas    (501) staff       (20)      557 2023-05-29 13:16:13.000000 PyLogForge-1.0.0/PyLogForge.egg-info/PKG-INFO
--rw-r--r--   0 scuevas    (501) staff       (20)      158 2023-05-29 13:16:13.000000 PyLogForge-1.0.0/PyLogForge.egg-info/SOURCES.txt
--rw-r--r--   0 scuevas    (501) staff       (20)        1 2023-05-29 13:16:13.000000 PyLogForge-1.0.0/PyLogForge.egg-info/dependency_links.txt
--rw-r--r--   0 scuevas    (501) staff       (20)       11 2023-05-29 13:16:13.000000 PyLogForge-1.0.0/PyLogForge.egg-info/top_level.txt
--rw-r--r--   0 scuevas    (501) staff       (20)     4468 2023-05-29 13:04:08.000000 PyLogForge-1.0.0/pylogforge.py
--rw-r--r--   0 scuevas    (501) staff       (20)       38 2023-05-29 13:16:13.177607 PyLogForge-1.0.0/setup.cfg
--rw-r--r--   0 scuevas    (501) staff       (20)      710 2023-05-29 13:15:41.000000 PyLogForge-1.0.0/setup.py
+drwxr-xr-x   0 scuevas    (501) staff       (20)        0 2023-05-29 14:20:40.750363 PyLogForge-1.0.1/
+-rw-r--r--   0 scuevas    (501) staff       (20)     3162 2023-05-29 14:20:40.750202 PyLogForge-1.0.1/PKG-INFO
+drwxr-xr-x   0 scuevas    (501) staff       (20)        0 2023-05-29 14:20:40.749920 PyLogForge-1.0.1/PyLogForge.egg-info/
+-rw-r--r--   0 scuevas    (501) staff       (20)     3162 2023-05-29 14:20:40.000000 PyLogForge-1.0.1/PyLogForge.egg-info/PKG-INFO
+-rw-r--r--   0 scuevas    (501) staff       (20)      168 2023-05-29 14:20:40.000000 PyLogForge-1.0.1/PyLogForge.egg-info/SOURCES.txt
+-rw-r--r--   0 scuevas    (501) staff       (20)        1 2023-05-29 14:20:40.000000 PyLogForge-1.0.1/PyLogForge.egg-info/dependency_links.txt
+-rw-r--r--   0 scuevas    (501) staff       (20)       11 2023-05-29 14:20:40.000000 PyLogForge-1.0.1/PyLogForge.egg-info/top_level.txt
+-rw-r--r--   0 scuevas    (501) staff       (20)     2564 2023-05-29 13:57:45.000000 PyLogForge-1.0.1/README.md
+-rw-r--r--   0 scuevas    (501) staff       (20)     4501 2023-05-29 13:48:31.000000 PyLogForge-1.0.1/pylogforge.py
+-rw-r--r--   0 scuevas    (501) staff       (20)       38 2023-05-29 14:20:40.750434 PyLogForge-1.0.1/setup.cfg
+-rw-r--r--   0 scuevas    (501) staff       (20)      809 2023-05-29 14:17:09.000000 PyLogForge-1.0.1/setup.py
```

### Comparing `PyLogForge-1.0.0/pylogforge.py` & `PyLogForge-1.0.1/pylogforge.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,39 +79,39 @@
         file_level = getattr(logging, os.environ.get('LOG_FILE_LEVEL', ''), file_level)
 
         self.logger.setLevel(min(console_level, file_level))
 
         for handler in self.logger.handlers:
             self.logger.removeHandler(handler)
 
-        console_formatter = CustomFormatter('[%(asctime)s] %(levelname)s - %(message)s')
+        console_formatter = CustomFormatter('[%(asctime)s] %(name)s - %(levelname)s - %(message)s')
         console_handler = logging.StreamHandler()
         console_handler.setLevel(console_level)
         console_handler.setFormatter(console_formatter)
         self.logger.addHandler(console_handler)
 
         log_dir = os.environ.get('LOG_DIR')
         if log_dir:
             os.makedirs(log_dir, exist_ok=True)
 
             if os.environ.get('LOG_SINGLE_FILE', '').lower() == 'true':
                 file_handler = logging.FileHandler(os.path.join(log_dir, "app.log"))
                 file_handler.setLevel(file_level)
-                file_formatter = CleanLevelFormatter('[%(asctime)s] %(levelname)s - %(message)s')
+                file_formatter = CleanLevelFormatter('[%(asctime)s] %(name)s - %(levelname)s - %(message)s')
                 file_handler.setFormatter(file_formatter)
                 self.logger.addHandler(file_handler)
             else:
                 for level in (logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR, logging.CRITICAL):
                     if level >= file_level:
                         level_name = logging.getLevelName(level)
                         log_file = os.path.join(log_dir, f"{level_name.lower()}.log")
                         file_handler = logging.FileHandler(log_file)
                         file_handler.setLevel(level)
                         file_handler.addFilter(LevelFilter(level))  # Only log records at the specific level
-                        file_formatter = CleanLevelFormatter('[%(asctime)s] %(levelname)s - %(message)s')
+                        file_formatter = CleanLevelFormatter('[%(asctime)s] %(name)s - %(levelname)s - %(message)s')
                         file_handler.setFormatter(file_formatter)
                         self.logger.addHandler(file_handler)
 
 
 class CleanLevelFormatter(logging.Formatter):
     color_pattern = re.compile(r'\x1b\[\d{1,2}(;\d{1,2})?m')
```

### Comparing `PyLogForge-1.0.0/setup.py` & `PyLogForge-1.0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup
 
 setup(
     name='PyLogForge',
-    version='1.0.0',
+    version='1.0.1',
     description='Custom Logger Module',
     author='Sebastián M. Cuevas',
     author_email='sebastian.cuevas@greatgeek.net',
     url='https://github.com/krash0n/pylogforge',
     py_modules=['pylogforge'],
+    long_description= open('README.md').read(),
+    long_description_content_type='text/markdown',
     install_requires=[],  # Add any dependencies here
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

