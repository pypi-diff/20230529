# Comparing `tmp/agenta-0.1.0.tar.gz` & `tmp/agenta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agenta-0.1.0.tar", max compression
+gzip compressed data, was "agenta-0.1.1.tar", max compression
```

## Comparing `agenta-0.1.0.tar` & `agenta-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2844 2023-05-15 14:38:07.049766 agenta-0.1.0/README.md
--rw-r--r--   0        0        0       53 2023-05-20 06:49:49.205423 agenta-0.1.0/agenta/__init__.py
--rw-r--r--   0        0        0     3016 2023-05-27 19:36:21.673488 agenta-0.1.0/agenta/agenta.py
--rw-r--r--   0        0        0     5902 2023-05-27 11:34:19.594433 agenta-0.1.0/agenta/cli.py
--rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.0/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.0/agenta/client/__init__.py
--rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.0/agenta/client/api_models.py
--rw-r--r--   0        0        0     1479 2023-05-26 07:44:13.475577 agenta-0.1.0/agenta/client/client.py
--rw-r--r--   0        0        0      550 2023-05-11 14:46:01.166162 agenta-0.1.0/agenta/config.py
--rw-r--r--   0        0        0       91 2023-05-12 12:52:29.405049 agenta-0.1.0/agenta/config.toml
--rw-r--r--   0        0        0      337 2023-05-24 09:05:58.092867 agenta-0.1.0/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.0/agenta/docker/docker-assets/README.md
--rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.0/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     2585 2023-05-27 10:11:21.981693 agenta-0.1.0/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0      407 2023-05-22 17:58:10.352282 agenta-0.1.0/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0      642 2023-05-24 09:05:58.093598 agenta-0.1.0/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.0/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.0/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0      512 2023-05-24 09:05:58.094733 agenta-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 agenta-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2844 2023-05-15 14:38:07.049766 agenta-0.1.1/README.md
+-rw-r--r--   0        0        0       53 2023-05-20 06:49:49.205423 agenta-0.1.1/agenta/__init__.py
+-rw-r--r--   0        0        0     3016 2023-05-27 19:36:21.673488 agenta-0.1.1/agenta/agenta.py
+-rw-r--r--   0        0        0     5924 2023-05-29 13:26:47.815435 agenta-0.1.1/agenta/cli.py
+-rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.1/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.1/agenta/client/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.1/agenta/client/api_models.py
+-rw-r--r--   0        0        0     1479 2023-05-26 07:44:13.475577 agenta-0.1.1/agenta/client/client.py
+-rw-r--r--   0        0        0      550 2023-05-11 14:46:01.166162 agenta-0.1.1/agenta/config.py
+-rw-r--r--   0        0        0       91 2023-05-12 12:52:29.405049 agenta-0.1.1/agenta/config.toml
+-rw-r--r--   0        0        0      337 2023-05-24 09:05:58.092867 agenta-0.1.1/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.1/agenta/docker/docker-assets/README.md
+-rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.1/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     2585 2023-05-27 10:11:21.981693 agenta-0.1.1/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0      407 2023-05-22 17:58:10.352282 agenta-0.1.1/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0      642 2023-05-24 09:05:58.093598 agenta-0.1.1/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.1/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.1/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0      513 2023-05-29 13:29:06.958141 agenta-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 agenta-0.1.1/PKG-INFO
```

### Comparing `agenta-0.1.0/README.md` & `agenta-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `agenta-0.1.0/agenta/agenta.py` & `agenta-0.1.1/agenta/agenta.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.0/agenta/cli.py` & `agenta-0.1.1/agenta/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             choices=[questionary.Choice(title=f"{template} - {template_desc}", value=template)
                      for template, template_desc in zip(templates, template_desc)]
         ).ask()
 
         # Copy the template files to the current directory
         chosen_template_dir = template_dir / template
         for file in chosen_template_dir.glob("*"):
-            if file.name != 'template.toml':
+            if file.name != 'template.toml' and not file.is_dir():
                 shutil.copy(file, current_dir / file.name)
     click.echo("App initialized successfully")
 
 
 @click.command(name='start')
 @click.option('--variant_name', default=None)
 @click.argument('app_folder', default=".")
```

### Comparing `agenta-0.1.0/agenta/client/client.py` & `agenta-0.1.1/agenta/client/client.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.0/agenta/config.py` & `agenta-0.1.1/agenta/config.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.0/agenta/docker/docker_utils.py` & `agenta-0.1.1/agenta/docker/docker_utils.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.0/agenta/templates/simple_prompt/app.py` & `agenta-0.1.1/agenta/templates/simple_prompt/app.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.0/pyproject.toml` & `agenta-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agenta"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Mahmoud Mabrouk <mahmoudmabrouk.mail@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docker = "^6.1.1"
@@ -19,8 +19,8 @@
 pytest = "^6.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-agenta = "agenta.cli:cli"
+agenta = "agenta.cli:cli"
```

### Comparing `agenta-0.1.0/PKG-INFO` & `agenta-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agenta
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Mahmoud Mabrouk
 Author-email: mahmoudmabrouk.mail@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

