# Comparing `tmp/libretranslate-1.3.8.tar.gz` & `tmp/libretranslate-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretranslate-1.3.8.tar", last modified: Fri Jan  6 14:39:27 2023, max compression
+gzip compressed data, was "libretranslate-1.3.9.tar", last modified: Wed Feb  1 22:48:53 2023, max compression
```

## Comparing `libretranslate-1.3.8.tar` & `libretranslate-1.3.9.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:39:27.924631 libretranslate-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-01-06 14:39:18.000000 libretranslate-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30055 2023-01-06 14:39:27.924631 libretranslate-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24764 2023-01-06 14:39:18.000000 libretranslate-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:39:27.920631 libretranslate-1.3.8/libretranslate/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    33520 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/default_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/flood.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/no_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/remove_translated_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/security.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/suggestions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:39:27.924631 libretranslate-1.3.8/libretranslate/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:39:27.924631 libretranslate-1.3.8/libretranslate/tests/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/tests/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/tests/test_api/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/tests/test_api/test_api_detect_language.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/tests/test_api/test_api_frontend_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/tests/test_api/test_api_get_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/tests/test_api/test_api_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/tests/test_api/test_api_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-01-06 14:39:18.000000 libretranslate-1.3.8/libretranslate/tests/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:39:27.924631 libretranslate-1.3.8/libretranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30055 2023-01-06 14:39:27.000000 libretranslate-1.3.8/libretranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-06 14:39:27.000000 libretranslate-1.3.8/libretranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 14:39:27.000000 libretranslate-1.3.8/libretranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-06 14:39:27.000000 libretranslate-1.3.8/libretranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-01-06 14:39:27.000000 libretranslate-1.3.8/libretranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-06 14:39:27.000000 libretranslate-1.3.8/libretranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-06 14:39:27.924631 libretranslate-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-06 14:39:18.000000 libretranslate-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:48:53.976047 libretranslate-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-01 22:48:38.000000 libretranslate-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-02-01 22:48:53.976047 libretranslate-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28315 2023-02-01 22:48:38.000000 libretranslate-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:48:53.976047 libretranslate-1.3.9/libretranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35719 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/default_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/flood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/locales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/no_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/remove_translated_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/suggestions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:48:53.976047 libretranslate-1.3.9/libretranslate/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:48:53.976047 libretranslate-1.3.9/libretranslate/tests/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/tests/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/tests/test_api/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/tests/test_api/test_api_detect_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/tests/test_api/test_api_frontend_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/tests/test_api/test_api_get_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/tests/test_api/test_api_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/tests/test_api/test_api_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-01 22:48:38.000000 libretranslate-1.3.9/libretranslate/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:48:53.976047 libretranslate-1.3.9/libretranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-02-01 22:48:53.000000 libretranslate-1.3.9/libretranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-01 22:48:53.000000 libretranslate-1.3.9/libretranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 22:48:53.000000 libretranslate-1.3.9/libretranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-01 22:48:53.000000 libretranslate-1.3.9/libretranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-01 22:48:53.000000 libretranslate-1.3.9/libretranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-01 22:48:53.000000 libretranslate-1.3.9/libretranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-01 22:48:53.976047 libretranslate-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-02-01 22:48:38.000000 libretranslate-1.3.9/setup.py
```

### Comparing `libretranslate-1.3.8/LICENSE` & `libretranslate-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/PKG-INFO` & `libretranslate-1.3.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,587 +1,619 @@
-Metadata-Version: 2.1
-Name: libretranslate
-Version: 1.3.8
-Summary: Free and Open Source Machine Translation API. Self-hosted, no limits, no ties to proprietary services.
-Home-page: https://libretranslate.com
-Author: LibreTranslate Authors
-Author-email: pt@uav4geo.com
-License: GNU Affero General Public License v3.0
-Description: # LibreTranslate
-        
-        [Try it online!](https://libretranslate.com) | [API Docs](https://libretranslate.com/docs) | [Community Forum](https://community.libretranslate.com/)
-        
-        [![Python versions](https://img.shields.io/pypi/pyversions/libretranslate)](https://pypi.org/project/libretranslate) [![Run tests](https://github.com/LibreTranslate/LibreTranslate/workflows/Run%20tests/badge.svg)](https://github.com/LibreTranslate/LibreTranslate/actions?query=workflow%3A%22Run+tests%22) [![Build and Publish Docker Image](https://github.com/LibreTranslate/LibreTranslate/actions/workflows/publish-docker.yml/badge.svg)](https://github.com/LibreTranslate/LibreTranslate/actions/workflows/publish-docker.yml) [![Publish package](https://github.com/LibreTranslate/LibreTranslate/actions/workflows/publish-package.yml/badge.svg)](https://github.com/LibreTranslate/LibreTranslate/actions/workflows/publish-package.yml) [![Awesome Humane Tech](https://raw.githubusercontent.com/humanetech-community/awesome-humane-tech/main/humane-tech-badge.svg?sanitize=true)](https://github.com/humanetech-community/awesome-humane-tech)
-        
-        Free and Open Source Machine Translation API, entirely self-hosted. Unlike other APIs, it doesn't rely on proprietary providers such as Google or Azure to perform translations. Instead, its translation engine is powered by the open source [Argos Translate](https://github.com/argosopentech/argos-translate) library.
-        
-        ![image](https://user-images.githubusercontent.com/64697405/139015751-279f31ac-36f1-4950-9ea7-87e76bf65f51.png)
-        
-        
-        [Try it online!](https://libretranslate.com) | [API Docs](https://libretranslate.com/docs)
-        
-        ## API Examples
-        
-        
-        ### Simple
-        
-        Request:
-        
-        ```javascript
-        const res = await fetch("https://libretranslate.com/translate", {
-        	method: "POST",
-        	body: JSON.stringify({
-        		q: "Hello!",
-        		source: "en",
-        		target: "es"
-        	}),
-        	headers: { "Content-Type": "application/json" }
-        });
-        
-        console.log(await res.json());
-        ```
-        
-        Response:
-        
-        ```javascript
-        {
-            "translatedText": "¡Hola!"
-        }
-        ```
-        
-        ### Auto Detect Language
-        
-        Request:
-        
-        ```javascript
-        const res = await fetch("https://libretranslate.com/translate", {
-        	method: "POST",
-        	body: JSON.stringify({
-        		q: "Ciao!",
-        		source: "auto",
-        		target: "en"
-        	}),
-        	headers: { "Content-Type": "application/json" }
-        });
-        
-        console.log(await res.json());
-        ```
-        
-        Response:
-        
-        ```javascript
-        {
-            "detectedLanguage": {
-                "confidence": 83,
-                "language": "it"
-            },
-            "translatedText": "Bye!"
-        }
-        ```
-        
-        ### HTML (beta)
-        
-        Request:
-        
-        ```javascript
-        const res = await fetch("https://libretranslate.com/translate", {
-        	method: "POST",
-        	body: JSON.stringify({
-        		q: '<p class="green">Hello!</p>',
-        		source: "en",
-        		target: "es",
-        		format: "html"
-        	}),
-        	headers: { "Content-Type": "application/json" }
-        });
-        
-        console.log(await res.json());
-        ```
-        
-        Response:
-        
-        ```javascript
-        {
-            "translatedText": "<p class=\"green\">¡Hola!</p>"
-        }
-        ```
-        
-        ## Install and Run
-        
-        You can run your own API server with just a few lines of setup!
-        
-        Make sure you have Python installed (3.8 or higher is recommended), then simply run:
-        
-        ```bash
-        pip install libretranslate
-        libretranslate [args]
-        ```
-        
-        Then open a web browser to http://localhost:5000
-        
-        On Ubuntu 20.04 you can also use the install script available at https://github.com/argosopentech/LibreTranslate-init
-        
-        ## Build and Run
-        
-        If you want to make changes to the code, you can build from source, and run the API:
-        
-        ```bash
-        git clone https://github.com/LibreTranslate/LibreTranslate
-        cd LibreTranslate
-        pip install -e .
-        libretranslate [args]
-        
-        # Or
-        python main.py [args]
-        ```
-        
-        Then open a web browser to http://localhost:5000
-        
-        ### Run with Docker
-        
-        Linux/MacOS: `./run.sh [args]`
-        Windows: `run.bat [args]`
-        
-        Then open a web browser to http://localhost:5000
-        
-        
-        ### Build with Docker
-        
-        ```bash
-        docker build [--build-arg with_models=true] -t libretranslate .
-        ```
-        
-        If you want to run the Docker image in a complete offline environment, you need to add the `--build-arg with_models=true` parameter. Then the language models are downloaded during the build process of the image. Otherwise these models get downloaded on the first run of the image/container.
-        
-        Run the built image:
-        
-        ```bash
-        docker run -it -p 5000:5000 libretranslate [args]
-        ```
-        
-        Or build and run using `docker-compose`:
-        
-        ```bash
-        docker-compose up -d --build
-        ```
-        
-        > Feel free to change the [`docker-compose.yml`](https://github.com/LibreTranslate/LibreTranslate/blob/main/docker-compose.yml) file to adapt it to your deployment needs, or use an extra `docker-compose.prod.yml` file for your deployment configuration.
-        
-        > The models are stored inside the container under `/home/libretranslate/.local/share` and `/home/libretranslate/.local/cache`. Feel free to use volumes if you do not want to redownload the models when the container is destroyed. To update the models, use the `--update-models` argument.
-        
-        ### CUDA
-        
-        You can use hardware acceleration to speed up translations on a GPU machine with CUDA 11.2 and [nvidia-docker](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html) installed.
-        
-        Run this version with:
-        
-        ```bash
-        docker-compose -f docker-compose.cuda.yml up -d --build
-        ```
-        
-        ## Arguments
-        
-        | Argument                    | Description                                                                                                 | Default              | Env. name                    |
-        |-----------------------------|-------------------------------------------------------------------------------------------------------------| -------------------- |------------------------------|
-        | --host                      | Set host to bind the server to                                                                              | `127.0.0.1`          | LT_HOST                      |
-        | --port                      | Set port to bind the server to                                                                              | `5000`               | LT_PORT                      |
-        | --char-limit                | Set character limit                                                                                         | `No limit`               | LT_CHAR_LIMIT                |
-        | --req-limit                 | Set maximum number of requests per minute per client                                                        | `No limit`               | LT_REQ_LIMIT                 |
-        | --req-limit-storage         | Storage URI to use for request limit data storage. See [Flask Limiter](https://flask-limiter.readthedocs.io/en/stable/configuration.html) | `memory://` | LT_REQ_LIMIT_STORAGE |
-        | --batch-limit               | Set maximum number of texts to translate in a batch request                                                 | `No limit`               | LT_BATCH_LIMIT               |
-        | --ga-id                     | Enable Google Analytics on the API client page by providing an ID                                           | `No tracking`               | LT_GA_ID                     |
-        | --debug                     | Enable debug environment                                                                                    | `False`           | LT_DEBUG                     |
-        | --ssl                       | Whether to enable SSL                                                                                       | `False`               | LT_SSL                       |
-        | --frontend-language-source  | Set frontend default language - source                                                                      | `en`          | LT_FRONTEND_LANGUAGE_SOURCE  |
-        | --frontend-language-target  | Set frontend default language - target                                                                      | `es`          | LT_FRONTEND_LANGUAGE_TARGET  |
-        | --frontend-timeout          | Set frontend translation timeout                                                                            | `500`         | LT_FRONTEND_TIMEOUT          |
-        | --api-keys                  | Enable API keys database for per-user rate limits lookup                                                    | `Don't use API keys` | LT_API_KEYS                  |
-        | --api-keys-db-path          | Use a specific path inside the container for the local database. Can be absolute or relative                | `db/api_keys.db`                      | LT_API_KEYS_DB_PATH          |
-        | --api-keys-remote           | Use this remote endpoint to query for valid API keys instead of using the local database                    | `Use local API key database` | LT_API_KEYS_REMOTE                  |
-        | --get-api-key-link          | Show a link in the UI where to direct users to get an API key                                               | `Don't show a link` | LT_GET_API_KEY_LINK                  |
-        | --require-api-key-origin    | Require use of an API key for programmatic access to the API, unless the request origin matches this domain | `No restrictions on domain origin` | LT_REQUIRE_API_KEY_ORIGIN    |
-        | --load-only                 | Set available languages                                                                                     | `all from argostranslate`    | LT_LOAD_ONLY                 |
-        | --threads                   | Set number of threads                                                                                       | `4`    | LT_THREADS                 |
-        | --suggestions               | Allow user suggestions                                                                                      | `False`    | LT_SUGGESTIONS               |
-        | --disable-files-translation | Disable files translation                                                                                   | `False`    | LT_DISABLE_FILES_TRANSLATION |
-        | --disable-web-ui            | Disable web ui                                                                                              | `False`    | LT_DISABLE_WEB_UI            |
-        | --update-models             | Update language models at startup                                                                           | `False`    | LT_UPDATE_MODELS            |
-        | --metrics                   | Enable the /metrics endpoint for exporting [Prometheus](https://prometheus.io/) usage metrics               | `Disabled`    | LT_METRICS            |
-        | --metrics-auth-token        | Protect the /metrics endpoint by allowing only clients that have a valid Authorization Bearer token         | `No auth`    | LT_METRICS_AUTH_TOKEN            |
-        
-        Note that each argument has an equivalent environment variable that can be used instead. The env. variables overwrite the default values but have lower priority than the command arguments and are particularly useful if used with Docker. The environment variable names are the upper-snake-case of the equivalent command argument's name with a `LT` prefix.
-        
-        ## Update
-        
-        ### Software
-        
-        If you installed with pip:
-        
-        `pip install -U libretranslate`
-        
-        If you're using docker:
-        
-        `docker pull libretranslate/libretranslate`
-        
-        ### Language Models
-        
-        Start the program with the `--update-models` argument. For example: `libretranslate --update-models` or `./run.sh --update-models`.
-        
-        Alternatively you can also run the `install_models.py` script.
-        
-        ## Run with WSGI and Gunicorn
-        
-        ```
-        pip install gunicorn
-        gunicorn --bind 0.0.0.0:5000 'wsgi:app'
-        ```
-        
-        You can pass application arguments directly to Gunicorn via:
-        
-        
-        ```
-        gunicorn --bind 0.0.0.0:5000 'wsgi:app(api_keys=True)'
-        ```
-        
-        ## Run with Kubernetes
-        
-        See ["LibreTranslate: your own translation service on Kubernetes" by JM Robles](https://jmrobles.medium.com/libretranslate-your-own-translation-service-on-kubernetes-b46c3e1af630)
-        
-        ## Manage API Keys
-        
-        LibreTranslate supports per-user limit quotas, e.g. you can issue API keys to users so that they can enjoy higher requests limits per minute (if you also set `--req-limit`). By default all users are rate-limited based on `--req-limit`, but passing an optional `api_key` parameter to the REST endpoints allows a user to enjoy higher request limits.
-        
-        To use API keys simply start LibreTranslate with the `--api-keys` option. If you modified the API keys database path with the option `--api-keys-db-path`, you must specify the path with the same argument flag when using the `ltmanage keys` command. 
-        
-        ### Add New Keys
-        
-        To issue a new API key with 120 requests per minute limits:
-        
-        ```bash
-        ltmanage keys add 120
-        ```
-        
-        If you changed the API keys database path:
-        ```bash
-        ltmanage keys --api-keys-db-path path/to/db/dbName.db add 120
-        ```
-        
-        ### Remove Keys
-        
-        ```bash
-        ltmanage keys remove <api-key>
-        ```
-        
-        ### View Keys
-        
-        ```bash
-        ltmanage keys
-        ```
-        
-        ## Prometheus Metrics
-        
-        LibreTranslate has Prometheus [exporter](https://prometheus.io/docs/instrumenting/exporters/) capabilities when you pass the `--metrics` argument at startup (disabled by default). When metrics are enabled, a `/metrics` endpoint is mounted on the instance:
-        
-        http://localhost:5000/metrics
-        
-        ```
-        # HELP libretranslate_http_requests_in_flight Multiprocess metric
-        # TYPE libretranslate_http_requests_in_flight gauge
-        libretranslate_http_requests_in_flight{api_key="",endpoint="/translate",request_ip="127.0.0.1"} 0.0
-        # HELP libretranslate_http_request_duration_seconds Multiprocess metric
-        # TYPE libretranslate_http_request_duration_seconds summary
-        libretranslate_http_request_duration_seconds_count{api_key="",endpoint="/translate",request_ip="127.0.0.1",status="200"} 0.0
-        libretranslate_http_request_duration_seconds_sum{api_key="",endpoint="/translate",request_ip="127.0.0.1",status="200"} 0.0
-        ```
-        
-        You can then configure `prometheus.yml` to read the metrics:
-        
-        ```
-        scrape_configs:
-          - job_name: "libretranslate"
-            
-            # Needed only if you use --metrics-auth-token
-            #authorization:
-              #credentials: "mytoken"
-            
-            static_configs:
-              - targets: ["localhost:5000"]
-        ```
-        
-        To secure the `/metrics` endpoint you can also use `--metrics-auth-token mytoken`.
-        
-        If you use Gunicorn, make sure to create a directory for storing multiprocess data metrics and set `PROMETHEUS_MULTIPROC_DIR`:
-        
-        ```
-        mkdir -p /tmp/prometheus_data
-        rm /tmp/prometheus_data/*
-        export PROMETHEUS_MULTIPROC_DIR=/tmp/prometheus_data 
-        gunicorn -c gunicorn_conf.py --bind 0.0.0.0:5000 'wsgi:app(metrics=True)' 
-        ```
-        
-        ## Language Bindings
-        
-        You can use the LibreTranslate API using the following bindings:
-        
-         - Rust: https://github.com/DefunctLizard/libretranslate-rs
-         - Node.js: https://github.com/franciscop/translate
-         - .Net: https://github.com/sigaloid/LibreTranslate.Net
-         - Go: https://github.com/SnakeSel/libretranslate
-         - Python: https://github.com/argosopentech/LibreTranslate-py
-         - PHP: https://github.com/jefs42/libretranslate
-         - C++: https://github.com/argosopentech/LibreTranslate-cpp
-         - Swift: https://github.com/wacumov/libretranslate
-         - Unix: https://github.com/argosopentech/LibreTranslate-sh
-         - Shell: https://github.com/Hayao0819/Hayao-Tools/tree/master/libretranslate-sh
-         - Java: https://github.com/suuft/libretranslate-java
-         - 
-        ## Discourse Plugin
-        
-        You can use this [discourse translator plugin](https://github.com/LibreTranslate/discourse-translator) to translate [Discourse](https://discourse.org) topics. To install it simply modify `/var/discourse/containers/app.yml`:
-        
-        ```
-        ## Plugins go here
-        ## see https://meta.discourse.org/t/19157 for details
-        hooks:
-          after_code:
-            - exec:
-                cd: $home/plugins
-                cmd:
-                  - git clone https://github.com/discourse/docker_manager.git
-                  - git clone https://github.com/LibreTranslate/discourse-translator
-        	  ...
-        ```
-        
-        Then issue `./launcher rebuild app`. From the Discourse's admin panel then select "LibreTranslate" as a translation provider and set the relevant endpoint configurations.
-        
-        ## Mobile Apps
-        
-        - [LibreTranslater](https://gitlab.com/BeowuIf/libretranslater) is an Android app [available on the Play Store](https://play.google.com/store/apps/details?id=de.beowulf.libretranslater) and [in the F-Droid store](https://f-droid.org/packages/de.beowulf.libretranslater/) that uses the LibreTranslate API.
-        - [LiTranslate](https://github.com/viktorkalyniuk/LiTranslate-iOS) is an iOS app [available on the App Store](https://apps.apple.com/us/app/litranslate/id1644385339) that uses the LibreTranslate API.
-        
-        ## Web browser
-        - [minbrowser](https://minbrowser.org/) is a web browser with [integrated LibreTranslate support](https://github.com/argosopentech/argos-translate/discussions/158#discussioncomment-1141551).
-        - A LibreTranslate Firefox addon is [currently a work in progress](https://github.com/LibreTranslate/LibreTranslate/issues/55).
-        
-        ## Mirrors
-        
-        This is a list of public LibreTranslate instances, some require an API key. If you want to add a new URL, please open a pull request.
-        
-        URL |API Key Required | Links
-        --- | --- | ---
-        [libretranslate.com](https://libretranslate.com)|:heavy_check_mark:|[Get API Key](https://portal.libretranslate.com)
-        [libretranslate.de](https://libretranslate.de)|-
-        [translate.argosopentech.com](https://translate.argosopentech.com/)|-
-        [translate.api.skitzen.com](https://translate.api.skitzen.com/)|-
-        [translate.fortytwo-it.com](https://translate.fortytwo-it.com/)|-
-        [translate.terraprint.co](https://translate.terraprint.co/)|-
-        [lt.vern.cc](https://lt.vern.cc)|-
-        
-        ## TOR/i2p Mirrors
-        
-        URL |API Key Required|Payment Link|Cost
-        --- | --- | --- | ---
-        [lt.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion](http://lt.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion/)|-|-
-        [lt.vern.i2p](http://vernf45n7mxwqnp5riaax7p67pwcl7wcefdcnqqvim7ckdx4264a.b32.i2p/)|-|-
-        
-        
-        ## Adding New Languages
-        
-        To add new languages you first need to train an Argos Translate model. See [this video](https://odysee.com/@argosopentech:7/training-an-Argos-Translate-model-tutorial-2022:2?r=DMnK7NqdPNHRCfwhmKY9LPow3PqVUUgw) for details.
-        
-        First you need to collect data, for example from [Opus](http://opus.nlpl.eu/), then you need to add the data to [data-index.json](https://github.com/argosopentech/argos-train/blob/master/data-index.json) in the [Argos Train](https://github.com/argosopentech/argos-train) repo.
-        
-        ## Roadmap
-        
-        Help us by opening a pull request!
-        
-        - [x] A docker image (thanks [@vemonet](https://github.com/vemonet) !)
-        - [x] Auto-detect input language (thanks [@vemonet](https://github.com/vemonet) !)
-        - [X] User authentication / tokens
-        - [ ] Language bindings for every computer language
-        - [ ] [Improved translations](https://community.libretranslate.com/t/the-best-way-to-train-models/172)
-        
-        ## FAQ
-        
-        ### Can I use your API server at libretranslate.com for my application in production?
-        
-        In short, no. [You need to buy an API key](https://portal.libretranslate.com). You can always run LibreTranslate for free on your own server of course.
-        
-        ### Can I use LibreTranslate behind a reverse proxy, like Apache2 or Caddy?
-        
-        Yes, here are config examples for Apache2 and Caddy that redirect a subdomain (with HTTPS certificate) to LibreTranslate running on a docker at localhost. 
-        ```
-        sudo docker run -ti --rm -p 127.0.0.1:5000:5000 libretranslate/libretranslate
-        ```
-        You can remove `127.0.0.1` on the above command if you want to be able to access it from `domain.tld:5000`, in addition to `subdomain.domain.tld` (this can be helpful to determine if there is an issue with Apache2 or the docker container). 
-        
-        Add `--restart unless-stopped` if you want this docker to start on boot, unless manually stopped.
-        
-        <details>
-        <summary>Apache config</summary>
-        <br>
-        
-        Replace [YOUR_DOMAIN] with your full domain; for example, `translate.domain.tld` or `libretranslate.domain.tld`. 
-        
-        Remove `#` on the ErrorLog and CustomLog lines to log requests.
-        
-        ```ApacheConf
-        #Libretranslate
-        
-        #Redirect http to https
-        <VirtualHost *:80>
-            ServerName http://[YOUR_DOMAIN]
-            Redirect / https://[YOUR_DOMAIN]
-            # ErrorLog ${APACHE_LOG_DIR}/error.log
-            # CustomLog ${APACHE_LOG_DIR}/tr-access.log combined
-         </VirtualHost>
-        
-        #https
-        <VirtualHost *:443>
-            ServerName https://[YOUR_DOMAIN]
-            
-            ProxyPass / http://127.0.0.1:5000/
-            ProxyPassReverse / http://127.0.0.1:5000/
-            ProxyPreserveHost On
-           
-            SSLEngine on
-            SSLCertificateFile /etc/letsencrypt/live/[YOUR_DOMAIN]/fullchain.pem
-            SSLCertificateKeyFile /etc/letsencrypt/live/[YOUR_DOMAIN]/privkey.pem
-            SSLCertificateChainFile /etc/letsencrypt/live/[YOUR_DOMAIN]/fullchain.pem
-            
-            # ErrorLog ${APACHE_LOG_DIR}/tr-error.log
-            # CustomLog ${APACHE_LOG_DIR}/tr-access.log combined
-        </VirtualHost>
-        ```
-        
-        Add this to an existing site config, or a new file in `/etc/apache2/sites-available/new-site.conf` and run `sudo a2ensite new-site.conf`. 
-        
-        To get a HTTPS subdomain certificate, install `certbot` (snap), run `sudo certbot certonly --manual --preferred-challenges dns` and enter your information (with `subdomain.domain.tld` as the domain). Add a DNS TXT record with your domain registrar when asked. This will save your certificate and key to `/etc/letsencrypt/live/{subdomain.domain.tld}/`. Alternatively, comment the SSL lines out if you don't want to use HTTPS.
-        </details>
-        
-        <details>
-        <summary>Caddy config</summary>
-        <br>
-        
-        Replace [YOUR_DOMAIN] with your full domain; for example, `translate.domain.tld` or `libretranslate.domain.tld`.
-        
-        ```Caddyfile
-        #Libretranslate
-        [YOUR_DOMAIN] {
-          reverse_proxy localhost:5000
-        }
-        ```
-        
-        Add this to an existing Caddyfile or save it as `Caddyfile` in any directory and run `sudo caddy reload` in that same directory.
-        
-        </details>
-        
-        <details>
-        <summary>NGINX config</summary>
-        <br>
-        
-        Replace [YOUR_DOMAIN] with your full domain; for example, `translate.domain.tld` or `libretranslate.domain.tld`.
-          
-        Remove `#` on the `access_log` and `error_log` lines to disable logging.
-        
-        ```NginxConf
-        server {
-          listen 80;
-          server_name [YOUR_DOMAIN];
-          return 301 https://$server_name$request_uri;
-        }
-        
-        server {
-          listen 443 http2 ssl;
-          server_name [YOUR_DOMAIN];
-        
-          #access_log off;
-          #error_log off;
-          
-          # SSL Section
-          ssl_certificate /etc/letsencrypt/live/[YOUR_DOMAIN]/fullchain.pem;
-          ssl_certificate_key /etc/letsencrypt/live/[YOUR_DOMAIN]/privkey.pem;
-          
-          ssl_protocols TLSv1.2 TLSv1.3;
-        
-          # Using the recommended cipher suite from: https://wiki.mozilla.org/Security/Server_Side_TLS
-          ssl_ciphers 'ECDHE-ECDSA-AES128-GCM-SHA256:ECDHE-RSA-AES128-GCM-SHA256:ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384:ECDHE-ECDSA-CHACHA20-POLY1305:ECDHE-RSA-CHACHA20-POLY1305:DHE-RSA-AES128-GCM-SHA256:DHE-RSA-AES256-GCM-SHA384';
-        
-          ssl_session_timeout 10m;
-          ssl_session_cache shared:MozSSL:10m;  # about 40000 sessions
-          ssl_session_tickets off;
-        
-          # Specifies a curve for ECDHE ciphers.
-          ssl_ecdh_curve prime256v1;
-          # Server should determine the ciphers, not the client
-          ssl_prefer_server_ciphers on;
-        
-          
-          # Header section
-          add_header Strict-Transport-Security  "max-age=31536000; includeSubDomains; preload" always;
-          add_header Referrer-Policy            "strict-origin" always;
-        
-          add_header X-Frame-Options            "SAMEORIGIN"    always;
-          add_header X-XSS-Protection           "1; mode=block" always;
-          add_header X-Content-Type-Options     "nosniff"       always;
-          add_header X-Download-Options         "noopen"        always;
-          add_header X-Robots-Tag               "none"          always;
-        
-          add_header Feature-Policy             "microphone 'none'; camera 'none'; geolocation 'none';"  always;
-          # Newer header but not everywhere supported
-          add_header Permissions-Policy         "microphone=(), camera=(), geolocation=()" always;
-        
-          # Remove X-Powered-By, which is an information leak
-          fastcgi_hide_header X-Powered-By;
-        
-          # Do not send nginx server header
-          server_tokens off;
-          
-          # GZIP Section
-          gzip on;
-          gzip_disable "msie6";
-        
-          gzip_vary on;
-          gzip_proxied any;
-          gzip_comp_level 6;
-          gzip_buffers 16 8k;
-          gzip_http_version 1.1;
-          gzip_min_length 256;
-          gzip_types text/xml text/javascript font/ttf font/eot font/otf application/x-javascript application/atom+xml application/javascript application/json application/manifest+json application/rss+xml application/x-web-app-manifest+json application/xhtml+xml application/xml image/svg+xml image/x-icon text/css text/plain;
-        
-          location / {
-              proxy_pass http://127.0.0.1:5000/;
-              proxy_set_header Host $http_host;
-              proxy_set_header X-Real-IP $remote_addr;
-              proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
-              proxy_set_header X-Forwarded-Proto $scheme;
-              client_max_body_size 0;
-          }
-        }
-        
-        ```
-        
-        Add this to an existing NGINX config or save it as `libretranslate` in the `/etc/nginx/site-enabled` directory and run `sudo nginx -s reload`.
-        
-        </details>
-        
-        ## Credits
-        
-        This work is largely possible thanks to [Argos Translate](https://github.com/argosopentech/argos-translate), which powers the translation engine.
-        
-        ## License
-        
-        [GNU Affero General Public License v3](https://www.gnu.org/licenses/agpl-3.0.en.html)
-        
-        ## Trademark
-        
-        See [Trademark Guidelines](https://github.com/LibreTranslate/LibreTranslate/blob/main/TRADEMARK.md)
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
+# LibreTranslate
+
+[Try it online!](https://libretranslate.com) | [API Docs](https://libretranslate.com/docs) | [Community Forum](https://community.libretranslate.com/)
+
+[![Python versions](https://img.shields.io/pypi/pyversions/libretranslate)](https://pypi.org/project/libretranslate) [![Run tests](https://github.com/LibreTranslate/LibreTranslate/workflows/Run%20tests/badge.svg)](https://github.com/LibreTranslate/LibreTranslate/actions?query=workflow%3A%22Run+tests%22) [![Build and Publish Docker Image](https://github.com/LibreTranslate/LibreTranslate/actions/workflows/publish-docker.yml/badge.svg)](https://github.com/LibreTranslate/LibreTranslate/actions/workflows/publish-docker.yml) [![Publish package](https://github.com/LibreTranslate/LibreTranslate/actions/workflows/publish-package.yml/badge.svg)](https://github.com/LibreTranslate/LibreTranslate/actions/workflows/publish-package.yml) [![Awesome Humane Tech](https://raw.githubusercontent.com/humanetech-community/awesome-humane-tech/main/humane-tech-badge.svg?sanitize=true)](https://github.com/humanetech-community/awesome-humane-tech)
+
+Free and Open Source Machine Translation API, entirely self-hosted. Unlike other APIs, it doesn't rely on proprietary providers such as Google or Azure to perform translations. Instead, its translation engine is powered by the open source [Argos Translate](https://github.com/argosopentech/argos-translate) library.
+
+![image](https://user-images.githubusercontent.com/64697405/139015751-279f31ac-36f1-4950-9ea7-87e76bf65f51.png)
+
+
+[Try it online!](https://libretranslate.com) | [API Docs](https://libretranslate.com/docs)
+
+## API Examples
+
+
+### Simple
+
+Request:
+
+```javascript
+const res = await fetch("https://libretranslate.com/translate", {
+	method: "POST",
+	body: JSON.stringify({
+		q: "Hello!",
+		source: "en",
+		target: "es"
+	}),
+	headers: { "Content-Type": "application/json" }
+});
+
+console.log(await res.json());
+```
+
+Response:
+
+```javascript
+{
+    "translatedText": "¡Hola!"
+}
+```
+
+### Auto Detect Language
+
+Request:
+
+```javascript
+const res = await fetch("https://libretranslate.com/translate", {
+	method: "POST",
+	body: JSON.stringify({
+		q: "Ciao!",
+		source: "auto",
+		target: "en"
+	}),
+	headers: { "Content-Type": "application/json" }
+});
+
+console.log(await res.json());
+```
+
+Response:
+
+```javascript
+{
+    "detectedLanguage": {
+        "confidence": 83,
+        "language": "it"
+    },
+    "translatedText": "Bye!"
+}
+```
+
+### HTML (beta)
+
+Request:
+
+```javascript
+const res = await fetch("https://libretranslate.com/translate", {
+	method: "POST",
+	body: JSON.stringify({
+		q: '<p class="green">Hello!</p>',
+		source: "en",
+		target: "es",
+		format: "html"
+	}),
+	headers: { "Content-Type": "application/json" }
+});
+
+console.log(await res.json());
+```
+
+Response:
+
+```javascript
+{
+    "translatedText": "<p class=\"green\">¡Hola!</p>"
+}
+```
+
+## Install and Run
+
+You can run your own API server with just a few lines of setup!
+
+Make sure you have Python installed (3.8 or higher is recommended), then simply run:
+
+```bash
+pip install libretranslate
+libretranslate [args]
+```
+
+Then open a web browser to http://localhost:5000
+
+On Ubuntu 20.04 you can also use the install script available at https://github.com/argosopentech/LibreTranslate-init
+
+## Build and Run
+
+If you want to make changes to the code, you can build from source, and run the API:
+
+```bash
+git clone https://github.com/LibreTranslate/LibreTranslate
+cd LibreTranslate
+pip install -e .
+libretranslate [args]
+
+# Or
+python main.py [args]
+```
+
+Then open a web browser to http://localhost:5000
+
+### Run with Docker
+
+Linux/MacOS: `./run.sh [args]`
+Windows: `run.bat [args]`
+
+Then open a web browser to http://localhost:5000
+
+
+### Build with Docker
+
+```bash
+docker build -f docker/Dockerfile [--build-arg with_models=true] -t libretranslate .
+```
+
+If you want to run the Docker image in a complete offline environment, you need to add the `--build-arg with_models=true` parameter. Then the language models are downloaded during the build process of the image. Otherwise these models get downloaded on the first run of the image/container.
+
+Run the built image:
+
+```bash
+docker run -it -p 5000:5000 libretranslate [args]
+```
+
+Or build and run using `docker-compose`:
+
+```bash
+docker-compose up -d --build
+```
+
+> Feel free to change the [`docker-compose.yml`](https://github.com/LibreTranslate/LibreTranslate/blob/main/docker-compose.yml) file to adapt it to your deployment needs, or use an extra `docker-compose.prod.yml` file for your deployment configuration.
+
+> The models are stored inside the container under `/home/libretranslate/.local/share` and `/home/libretranslate/.local/cache`. Feel free to use volumes if you do not want to redownload the models when the container is destroyed. To update the models, use the `--update-models` argument.
+
+### CUDA
+
+You can use hardware acceleration to speed up translations on a GPU machine with CUDA 11.2 and [nvidia-docker](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html) installed.
+
+Run this version with:
+
+```bash
+docker-compose -f docker-compose.cuda.yml up -d --build
+```
+
+## Arguments
+
+| Argument                    | Description                                                                                                 | Default              | Env. name                    |
+|-----------------------------|-------------------------------------------------------------------------------------------------------------| -------------------- |------------------------------|
+| --host                      | Set host to bind the server to                                                                              | `127.0.0.1`          | LT_HOST                      |
+| --port                      | Set port to bind the server to                                                                              | `5000`               | LT_PORT                      |
+| --char-limit                | Set character limit                                                                                         | `No limit`               | LT_CHAR_LIMIT                |
+| --req-limit                 | Set maximum number of requests per minute per client                                                        | `No limit`               | LT_REQ_LIMIT                 |
+| --req-limit-storage         | Storage URI to use for request limit data storage. See [Flask Limiter](https://flask-limiter.readthedocs.io/en/stable/configuration.html) | `memory://` | LT_REQ_LIMIT_STORAGE |
+| --batch-limit               | Set maximum number of texts to translate in a batch request                                                 | `No limit`               | LT_BATCH_LIMIT               |
+| --ga-id                     | Enable Google Analytics on the API client page by providing an ID                                           | `No tracking`               | LT_GA_ID                     |
+| --debug                     | Enable debug environment                                                                                    | `False`           | LT_DEBUG                     |
+| --ssl                       | Whether to enable SSL                                                                                       | `False`               | LT_SSL                       |
+| --frontend-language-source  | Set frontend default language - source                                                                      | `auto`        | LT_FRONTEND_LANGUAGE_SOURCE  |
+| --frontend-language-target  | Set frontend default language - target                                                                      | `locale` (match site's locale)   | LT_FRONTEND_LANGUAGE_TARGET  |
+| --frontend-timeout          | Set frontend translation timeout                                                                            | `500`         | LT_FRONTEND_TIMEOUT          |
+| --api-keys                  | Enable API keys database for per-user rate limits lookup                                                    | `Don't use API keys` | LT_API_KEYS                  |
+| --api-keys-db-path          | Use a specific path inside the container for the local database. Can be absolute or relative                | `db/api_keys.db`                      | LT_API_KEYS_DB_PATH          |
+| --api-keys-remote           | Use this remote endpoint to query for valid API keys instead of using the local database                    | `Use local API key database` | LT_API_KEYS_REMOTE                  |
+| --get-api-key-link          | Show a link in the UI where to direct users to get an API key                                               | `Don't show a link` | LT_GET_API_KEY_LINK                  |
+| --require-api-key-origin    | Require use of an API key for programmatic access to the API, unless the request origin matches this domain | `No restrictions on domain origin` | LT_REQUIRE_API_KEY_ORIGIN    |
+| --load-only                 | Set available languages                                                                                     | `all from argostranslate`    | LT_LOAD_ONLY                 |
+| --threads                   | Set number of threads                                                                                       | `4`    | LT_THREADS                 |
+| --suggestions               | Allow user suggestions                                                                                      | `False`    | LT_SUGGESTIONS               |
+| --disable-files-translation | Disable files translation                                                                                   | `False`    | LT_DISABLE_FILES_TRANSLATION |
+| --disable-web-ui            | Disable web ui                                                                                              | `False`    | LT_DISABLE_WEB_UI            |
+| --update-models             | Update language models at startup                                                                           | `False`    | LT_UPDATE_MODELS            |
+| --metrics                   | Enable the /metrics endpoint for exporting [Prometheus](https://prometheus.io/) usage metrics               | `Disabled`    | LT_METRICS            |
+| --metrics-auth-token        | Protect the /metrics endpoint by allowing only clients that have a valid Authorization Bearer token         | `No auth`    | LT_METRICS_AUTH_TOKEN            |
+| --url-prefix                | Add prefix to URL: example.com:5000/url-prefix/                                                             | `/`    | LT_URL_PREFIX            |
+
+Note that each argument has an equivalent environment variable that can be used instead. The env. variables overwrite the default values but have lower priority than the command arguments and are particularly useful if used with Docker. The environment variable names are the upper-snake-case of the equivalent command argument's name with a `LT` prefix.
+
+## Update
+
+### Software
+
+If you installed with pip:
+
+`pip install -U libretranslate`
+
+If you're using docker:
+
+`docker pull libretranslate/libretranslate`
+
+### Language Models
+
+Start the program with the `--update-models` argument. For example: `libretranslate --update-models` or `./run.sh --update-models`.
+
+Alternatively you can also run the `scripts/install_models.py` script.
+
+## Run with WSGI and Gunicorn
+
+```
+pip install gunicorn
+gunicorn --bind 0.0.0.0:5000 'wsgi:app'
+```
+
+You can pass application arguments directly to Gunicorn via:
+
+
+```
+gunicorn --bind 0.0.0.0:5000 'wsgi:app(api_keys=True)'
+```
+
+## Run with Kubernetes
+
+See ["LibreTranslate: your own translation service on Kubernetes" by JM Robles](https://jmrobles.medium.com/libretranslate-your-own-translation-service-on-kubernetes-b46c3e1af630)
+
+## Manage API Keys
+
+LibreTranslate supports per-user limit quotas, e.g. you can issue API keys to users so that they can enjoy higher requests limits per minute (if you also set `--req-limit`). By default all users are rate-limited based on `--req-limit`, but passing an optional `api_key` parameter to the REST endpoints allows a user to enjoy higher request limits.
+
+To use API keys simply start LibreTranslate with the `--api-keys` option. If you modified the API keys database path with the option `--api-keys-db-path`, you must specify the path with the same argument flag when using the `ltmanage keys` command. 
+
+### Add New Keys
+
+To issue a new API key with 120 requests per minute limits:
+
+```bash
+ltmanage keys add 120
+```
+
+If you changed the API keys database path:
+```bash
+ltmanage keys --api-keys-db-path path/to/db/dbName.db add 120
+```
+
+### Remove Keys
+
+```bash
+ltmanage keys remove <api-key>
+```
+
+### View Keys
+
+```bash
+ltmanage keys
+```
+
+## Prometheus Metrics
+
+LibreTranslate has Prometheus [exporter](https://prometheus.io/docs/instrumenting/exporters/) capabilities when you pass the `--metrics` argument at startup (disabled by default). When metrics are enabled, a `/metrics` endpoint is mounted on the instance:
+
+http://localhost:5000/metrics
+
+```
+# HELP libretranslate_http_requests_in_flight Multiprocess metric
+# TYPE libretranslate_http_requests_in_flight gauge
+libretranslate_http_requests_in_flight{api_key="",endpoint="/translate",request_ip="127.0.0.1"} 0.0
+# HELP libretranslate_http_request_duration_seconds Multiprocess metric
+# TYPE libretranslate_http_request_duration_seconds summary
+libretranslate_http_request_duration_seconds_count{api_key="",endpoint="/translate",request_ip="127.0.0.1",status="200"} 0.0
+libretranslate_http_request_duration_seconds_sum{api_key="",endpoint="/translate",request_ip="127.0.0.1",status="200"} 0.0
+```
+
+You can then configure `prometheus.yml` to read the metrics:
+
+```
+scrape_configs:
+  - job_name: "libretranslate"
+    
+    # Needed only if you use --metrics-auth-token
+    #authorization:
+      #credentials: "mytoken"
+    
+    static_configs:
+      - targets: ["localhost:5000"]
+```
+
+To secure the `/metrics` endpoint you can also use `--metrics-auth-token mytoken`.
+
+If you use Gunicorn, make sure to create a directory for storing multiprocess data metrics and set `PROMETHEUS_MULTIPROC_DIR`:
+
+```
+mkdir -p /tmp/prometheus_data
+rm /tmp/prometheus_data/*
+export PROMETHEUS_MULTIPROC_DIR=/tmp/prometheus_data 
+gunicorn -c scripts/gunicorn_conf.py --bind 0.0.0.0:5000 'wsgi:app(metrics=True)' 
+```
+
+## Language Bindings
+
+You can use the LibreTranslate API using the following bindings:
+
+ - Rust: https://github.com/DefunctLizard/libretranslate-rs
+ - Node.js: https://github.com/franciscop/translate
+ - .Net: https://github.com/sigaloid/LibreTranslate.Net
+ - Go: https://github.com/SnakeSel/libretranslate
+ - Python: https://github.com/argosopentech/LibreTranslate-py
+ - PHP: https://github.com/jefs42/libretranslate
+ - C++: https://github.com/argosopentech/LibreTranslate-cpp
+ - Swift: https://github.com/wacumov/libretranslate
+ - Unix: https://github.com/argosopentech/LibreTranslate-sh
+ - Shell: https://github.com/Hayao0819/Hayao-Tools/tree/master/libretranslate-sh
+ - Java: https://github.com/suuft/libretranslate-java
+ - 
+## Discourse Plugin
+
+You can use this [discourse translator plugin](https://github.com/LibreTranslate/discourse-translator) to translate [Discourse](https://discourse.org) topics. To install it simply modify `/var/discourse/containers/app.yml`:
+
+```
+## Plugins go here
+## see https://meta.discourse.org/t/19157 for details
+hooks:
+  after_code:
+    - exec:
+        cd: $home/plugins
+        cmd:
+          - git clone https://github.com/discourse/docker_manager.git
+          - git clone https://github.com/LibreTranslate/discourse-translator
+	  ...
+```
+
+Then issue `./launcher rebuild app`. From the Discourse's admin panel then select "LibreTranslate" as a translation provider and set the relevant endpoint configurations.
+
+## Mobile Apps
+
+- [LibreTranslater](https://gitlab.com/BeowuIf/libretranslater) is an Android app [available on the Play Store](https://play.google.com/store/apps/details?id=de.beowulf.libretranslater) and [in the F-Droid store](https://f-droid.org/packages/de.beowulf.libretranslater/) that uses the LibreTranslate API.
+- [LiTranslate](https://github.com/viktorkalyniuk/LiTranslate-iOS) is an iOS app [available on the App Store](https://apps.apple.com/us/app/litranslate/id1644385339) that uses the LibreTranslate API.
+
+## Web browser
+- [minbrowser](https://minbrowser.org/) is a web browser with [integrated LibreTranslate support](https://github.com/argosopentech/argos-translate/discussions/158#discussioncomment-1141551).
+- A LibreTranslate Firefox addon is [currently a work in progress](https://github.com/LibreTranslate/LibreTranslate/issues/55).
+
+## Mirrors
+
+This is a list of public LibreTranslate instances, some require an API key. If you want to add a new URL, please open a pull request.
+
+URL |API Key Required | Links
+--- | --- | ---
+[libretranslate.com](https://libretranslate.com)|:heavy_check_mark:|[Get API Key](https://portal.libretranslate.com)
+[translate.argosopentech.com](https://translate.argosopentech.com/)|-
+[translate.terraprint.co](https://translate.terraprint.co/)|-
+[lt.vern.cc](https://lt.vern.cc)|-
+
+## TOR/i2p Mirrors
+
+URL |
+--- |
+[lt.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion](http://lt.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion/)|
+[lt.vern.i2p](http://vernf45n7mxwqnp5riaax7p67pwcl7wcefdcnqqvim7ckdx4264a.b32.i2p/)|
+
+
+## Adding New Language Models
+
+To add new languages you first need to train an Argos Translate model. See [this video](https://odysee.com/@argosopentech:7/training-an-Argos-Translate-model-tutorial-2022:2?r=DMnK7NqdPNHRCfwhmKY9LPow3PqVUUgw) for details.
+
+First you need to collect data, for example from [Opus](http://opus.nlpl.eu/), then you need to add the data to [data-index.json](https://github.com/argosopentech/argos-train/blob/master/data-index.json) in the [Argos Train](https://github.com/argosopentech/argos-train) repo.
+
+## Localization
+
+The LibreTranslate Web UI is available in all the languages for which LibreTranslate can translate to. It can also (roughly) [translate itself!](https://github.com/LibreTranslate/LibreTranslate/blob/main/scripts/update_locales.py) Some languages might not appear in the UI since they haven't been reviewed by a human yet. You can enable all languages by turning on `--debug` mode.
+
+To help improve or review the UI translations:
+ - Go to https://hosted.weblate.org/projects/libretranslate/app/#translations. All changes are automatically pushed to this repository.
+ - Once all strings have been reviewed/edited, open a pull request and change `libretranslate/locales/{code}/meta.json`:
+
+ ```json
+{
+	"name": "<Language>",
+	"reviewed": true <-- Change this from false to true
+}
+ ```
+
+### UI Languages
+
+Language | Reviewed | Weblate Link
+-------- | -------- | ------------
+Arabic |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/ar/)
+Azerbaijani |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/az/)
+Chinese |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/zh/)
+Czech |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/cs/)
+Danish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/da/)
+Dutch |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/nl/)
+English | :heavy_check_mark: | [Edit](https://hosted.weblate.org/projects/libretranslate/app/)
+Esperanto |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/eo/)
+Finnish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/fi/)
+French |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/fr/)
+German | :heavy_check_mark: | [Edit](https://hosted.weblate.org/translate/libretranslate/app/de/)
+Greek |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/el/)
+Hebrew |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/he/)
+Hindi |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/hi/)
+Hungarian |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/hu/)
+Indonesian |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/id/)
+Irish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/ga/)
+Italian | :heavy_check_mark: | [Edit](https://hosted.weblate.org/translate/libretranslate/app/it/)
+Japanese |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/ja/)
+Kabyle |  | [Edit](https://hosted.weblate.org/projects/libretranslate/app/kab/)
+Korean |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/ko/)
+Occitan |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/oc/)
+Persian |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/fa/)
+Polish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/pl/)
+Portuguese |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/pt/)
+Russian |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/ru/)
+Slovak |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/sk/)
+Spanish | :heavy_check_mark: | [Edit](https://hosted.weblate.org/translate/libretranslate/app/es/)
+Swedish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/sv/)
+Turkish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/tr/)
+Ukranian |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/uk/)
+Vietnamese |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/vi/)
+
+## Roadmap
+
+Help us by opening a pull request!
+
+- [x] A docker image (thanks [@vemonet](https://github.com/vemonet) !)
+- [x] Auto-detect input language (thanks [@vemonet](https://github.com/vemonet) !)
+- [X] User authentication / tokens
+- [ ] Language bindings for every computer language
+- [ ] [Improved translations](https://community.libretranslate.com/t/the-best-way-to-train-models/172)
+
+## FAQ
+
+### Can I use your API server at libretranslate.com for my application in production?
+
+In short, no. [You need to buy an API key](https://portal.libretranslate.com). You can always run LibreTranslate for free on your own server of course.
+
+### Can I use LibreTranslate behind a reverse proxy, like Apache2 or Caddy?
+
+Yes, here are config examples for Apache2 and Caddy that redirect a subdomain (with HTTPS certificate) to LibreTranslate running on a docker at localhost. 
+```
+sudo docker run -ti --rm -p 127.0.0.1:5000:5000 libretranslate/libretranslate
+```
+You can remove `127.0.0.1` on the above command if you want to be able to access it from `domain.tld:5000`, in addition to `subdomain.domain.tld` (this can be helpful to determine if there is an issue with Apache2 or the docker container). 
+
+Add `--restart unless-stopped` if you want this docker to start on boot, unless manually stopped.
+
+<details>
+<summary>Apache config</summary>
+<br>
+
+Replace [YOUR_DOMAIN] with your full domain; for example, `translate.domain.tld` or `libretranslate.domain.tld`. 
+
+Remove `#` on the ErrorLog and CustomLog lines to log requests.
+
+```ApacheConf
+#Libretranslate
+
+#Redirect http to https
+<VirtualHost *:80>
+    ServerName http://[YOUR_DOMAIN]
+    Redirect / https://[YOUR_DOMAIN]
+    # ErrorLog ${APACHE_LOG_DIR}/error.log
+    # CustomLog ${APACHE_LOG_DIR}/tr-access.log combined
+ </VirtualHost>
+
+#https
+<VirtualHost *:443>
+    ServerName https://[YOUR_DOMAIN]
+    
+    ProxyPass / http://127.0.0.1:5000/
+    ProxyPassReverse / http://127.0.0.1:5000/
+    ProxyPreserveHost On
+   
+    SSLEngine on
+    SSLCertificateFile /etc/letsencrypt/live/[YOUR_DOMAIN]/fullchain.pem
+    SSLCertificateKeyFile /etc/letsencrypt/live/[YOUR_DOMAIN]/privkey.pem
+    SSLCertificateChainFile /etc/letsencrypt/live/[YOUR_DOMAIN]/fullchain.pem
+    
+    # ErrorLog ${APACHE_LOG_DIR}/tr-error.log
+    # CustomLog ${APACHE_LOG_DIR}/tr-access.log combined
+</VirtualHost>
+```
+
+Add this to an existing site config, or a new file in `/etc/apache2/sites-available/new-site.conf` and run `sudo a2ensite new-site.conf`. 
+
+To get a HTTPS subdomain certificate, install `certbot` (snap), run `sudo certbot certonly --manual --preferred-challenges dns` and enter your information (with `subdomain.domain.tld` as the domain). Add a DNS TXT record with your domain registrar when asked. This will save your certificate and key to `/etc/letsencrypt/live/{subdomain.domain.tld}/`. Alternatively, comment the SSL lines out if you don't want to use HTTPS.
+</details>
+
+<details>
+<summary>Caddy config</summary>
+<br>
+
+Replace [YOUR_DOMAIN] with your full domain; for example, `translate.domain.tld` or `libretranslate.domain.tld`.
+
+```Caddyfile
+#Libretranslate
+[YOUR_DOMAIN] {
+  reverse_proxy localhost:5000
+}
+```
+
+Add this to an existing Caddyfile or save it as `Caddyfile` in any directory and run `sudo caddy reload` in that same directory.
+
+</details>
+
+<details>
+<summary>NGINX config</summary>
+<br>
+
+Replace [YOUR_DOMAIN] with your full domain; for example, `translate.domain.tld` or `libretranslate.domain.tld`.
+  
+Remove `#` on the `access_log` and `error_log` lines to disable logging.
+
+```NginxConf
+server {
+  listen 80;
+  server_name [YOUR_DOMAIN];
+  return 301 https://$server_name$request_uri;
+}
+
+server {
+  listen 443 http2 ssl;
+  server_name [YOUR_DOMAIN];
+
+  #access_log off;
+  #error_log off;
+  
+  # SSL Section
+  ssl_certificate /etc/letsencrypt/live/[YOUR_DOMAIN]/fullchain.pem;
+  ssl_certificate_key /etc/letsencrypt/live/[YOUR_DOMAIN]/privkey.pem;
+  
+  ssl_protocols TLSv1.2 TLSv1.3;
+
+  # Using the recommended cipher suite from: https://wiki.mozilla.org/Security/Server_Side_TLS
+  ssl_ciphers 'ECDHE-ECDSA-AES128-GCM-SHA256:ECDHE-RSA-AES128-GCM-SHA256:ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384:ECDHE-ECDSA-CHACHA20-POLY1305:ECDHE-RSA-CHACHA20-POLY1305:DHE-RSA-AES128-GCM-SHA256:DHE-RSA-AES256-GCM-SHA384';
+
+  ssl_session_timeout 10m;
+  ssl_session_cache shared:MozSSL:10m;  # about 40000 sessions
+  ssl_session_tickets off;
+
+  # Specifies a curve for ECDHE ciphers.
+  ssl_ecdh_curve prime256v1;
+  # Server should determine the ciphers, not the client
+  ssl_prefer_server_ciphers on;
+
+  
+  # Header section
+  add_header Strict-Transport-Security  "max-age=31536000; includeSubDomains; preload" always;
+  add_header Referrer-Policy            "strict-origin" always;
+
+  add_header X-Frame-Options            "SAMEORIGIN"    always;
+  add_header X-XSS-Protection           "1; mode=block" always;
+  add_header X-Content-Type-Options     "nosniff"       always;
+  add_header X-Download-Options         "noopen"        always;
+  add_header X-Robots-Tag               "none"          always;
+
+  add_header Feature-Policy             "microphone 'none'; camera 'none'; geolocation 'none';"  always;
+  # Newer header but not everywhere supported
+  add_header Permissions-Policy         "microphone=(), camera=(), geolocation=()" always;
+
+  # Remove X-Powered-By, which is an information leak
+  fastcgi_hide_header X-Powered-By;
+
+  # Do not send nginx server header
+  server_tokens off;
+  
+  # GZIP Section
+  gzip on;
+  gzip_disable "msie6";
+
+  gzip_vary on;
+  gzip_proxied any;
+  gzip_comp_level 6;
+  gzip_buffers 16 8k;
+  gzip_http_version 1.1;
+  gzip_min_length 256;
+  gzip_types text/xml text/javascript font/ttf font/eot font/otf application/x-javascript application/atom+xml application/javascript application/json application/manifest+json application/rss+xml application/x-web-app-manifest+json application/xhtml+xml application/xml image/svg+xml image/x-icon text/css text/plain;
+
+  location / {
+      proxy_pass http://127.0.0.1:5000/;
+      proxy_set_header Host $http_host;
+      proxy_set_header X-Real-IP $remote_addr;
+      proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
+      proxy_set_header X-Forwarded-Proto $scheme;
+      client_max_body_size 0;
+  }
+}
+
+```
+
+Add this to an existing NGINX config or save it as `libretranslate` in the `/etc/nginx/site-enabled` directory and run `sudo nginx -s reload`.
+
+</details>
+
+## Credits
+
+This work is largely possible thanks to [Argos Translate](https://github.com/argosopentech/argos-translate), which powers the translation engine.
+
+## License
+
+[GNU Affero General Public License v3](https://www.gnu.org/licenses/agpl-3.0.en.html)
+
+## Trademark
+
+See [Trademark Guidelines](https://github.com/LibreTranslate/LibreTranslate/blob/main/TRADEMARK.md)
```

### Comparing `libretranslate-1.3.8/libretranslate/api_keys.py` & `libretranslate-1.3.9/libretranslate/api_keys.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate/app.py` & `libretranslate-1.3.9/libretranslate/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import io
 import os
 import tempfile
+import re
 import uuid
 from functools import wraps
 from html import unescape
 from timeit import default_timer
 
 import argostranslatefiles
 from argostranslatefiles import get_supported_formats
 from flask import (abort, Blueprint, Flask, jsonify, render_template, request,
-                   Response, send_file, url_for)
+                   Response, send_file, url_for, session)
 from flask_swagger import swagger
 from flask_swagger_ui import get_swaggerui_blueprint
+from flask_session import Session
 from translatehtml import translate_html
 from werkzeug.utils import secure_filename
 from werkzeug.exceptions import HTTPException
+from flask_babel import Babel
 
 from libretranslate import flood, remove_translated_files, security
 from libretranslate.language import detect_languages, improve_translation_formatting
+from libretranslate.locales import (_, _lazy, get_available_locales, get_available_locale_codes, gettext_escaped, 
+        gettext_html, lazy_swag, get_alternate_locale_links)
 
 from .api_keys import Database, RemoteDatabase
 from .suggestions import Database as SuggestionsDatabase
 
 
 def get_version():
     try:
@@ -49,15 +54,15 @@
 
     return ak
 
 
 def get_json_dict(request):
     d = request.get_json()
     if not isinstance(d, dict):
-        abort(400, description="Invalid JSON format")
+        abort(400, description=_("Invalid JSON format"))
     return d
 
 
 def get_remote_address():
     if request.headers.getlist("X-Forwarded-For"):
         ip = request.headers.getlist("X-Forwarded-For")[0].split(",")[0]
     else:
@@ -117,41 +122,55 @@
     language_pairs = {}
     for lang in languages:
         language_pairs[lang.code] = sorted([l.to_lang.code for l in lang.translations_from])
 
     # Map userdefined frontend languages to argos language object.
     if args.frontend_language_source == "auto":
         frontend_argos_language_source = type(
-            "obj", (object,), {"code": "auto", "name": "Auto Detect"}
+            "obj", (object,), {"code": "auto", "name": _("Auto Detect")}
         )
     else:
         frontend_argos_language_source = next(
             iter([l for l in languages if l.code == args.frontend_language_source]),
             None,
         )
+    if frontend_argos_language_source is None:
+        frontend_argos_language_source = languages[0]
+
+    
+    if len(languages) >= 2:
+        language_target_fallback = languages[1]
+    else:
+        language_target_fallback = languages[0]
 
-    frontend_argos_language_target = next(
-        iter([l for l in languages if l.code == args.frontend_language_target]), None
-    )
+    if args.frontend_language_target == "locale":
+      def resolve_language_locale():
+          loc = get_locale()
+          language_target = next(
+              iter([l for l in languages if l.code == loc]), None
+          )
+          if language_target is None:
+            language_target = language_target_fallback
+          return language_target
+
+      frontend_argos_language_target = resolve_language_locale
+    else:
+      language_target = next(
+          iter([l for l in languages if l.code == args.frontend_language_target]), None
+      )
+      if language_target is None:
+        language_target = language_target_fallback
+      frontend_argos_language_target = lambda: language_target
 
     frontend_argos_supported_files_format = []
 
     for file_format in get_supported_formats():
         for ff in file_format.supported_file_extensions:
             frontend_argos_supported_files_format.append(ff)
 
-    # Raise AttributeError to prevent app startup if user input is not valid.
-    if frontend_argos_language_source is None:
-        frontend_argos_language_source = languages[0]
-    if frontend_argos_language_target is None:
-        if len(languages) >= 2:
-            frontend_argos_language_target = languages[1]
-        else:
-            frontend_argos_language_target = languages[0]
-
     api_keys_db = None
 
     if args.req_limit > 0 or args.api_keys or args.daily_req_limit > 0:
         api_keys_db = None
         if args.api_keys:
             if args.api_keys_remote:
                 api_keys_db = RemoteDatabase(args.api_keys_remote)
@@ -182,15 +201,15 @@
 
       @bp.route("/metrics")
       @limiter.exempt
       def prometheus_metrics():
         if args.metrics_auth_token:
           authorization = request.headers.get('Authorization')
           if authorization != "Bearer " + args.metrics_auth_token:
-            abort(401, description="Unauthorized")
+            abort(401, description=_("Unauthorized"))
 
         registry = CollectorRegistry()
         multiprocess.MultiProcessCollector(registry)
         return Response(generate_latest(registry), mimetype=CONTENT_TYPE_LATEST)
 
       measure_request = Summary('libretranslate_http_request_duration_seconds', 'Time spent on request', ['endpoint', 'status', 'request_ip', 'api_key'])
       measure_request.labels('/translate', 200, '127.0.0.1', '')
@@ -200,33 +219,33 @@
 
     def access_check(f):
         @wraps(f)
         def func(*a, **kw):
             ip = get_remote_address()
 
             if flood.is_banned(ip):
-                abort(403, description="Too many request limits violations")
+                abort(403, description=_("Too many request limits violations"))
 
             if args.api_keys:
                 ak = get_req_api_key()
                 if (
                     ak and api_keys_db.lookup(ak) is None
                 ):
                     abort(
                         403,
-                        description="Invalid API key",
+                        description=_("Invalid API key"),
                     )
                 elif (
                     args.require_api_key_origin
                     and api_keys_db.lookup(ak) is None
-                    and request.headers.get("Origin") != args.require_api_key_origin
+                    and not re.match(args.require_api_key_origin, request.headers.get("Origin"))
                 ):
-                    description = "Please contact the server operator to get an API key"
+                    description = _("Please contact the server operator to get an API key")
                     if args.get_api_key_link:
-                        description = "Visit %s to get an API key" % args.get_api_key_link
+                        description = _("Visit %(url)s to get an API key", url=args.get_api_key_link)
                     abort(
                         403,
                         description=description,
                     )
             return f(*a, **kw)
         
         if args.metrics:
@@ -258,45 +277,53 @@
     @bp.errorhandler(500)
     def server_error(e):
         return jsonify({"error": str(e.description)}), 500
 
     @bp.errorhandler(429)
     def slow_down_error(e):
         flood.report(get_remote_address())
-        return jsonify({"error": "Slowdown: " + str(e.description)}), 429
+        return jsonify({"error": _("Slowdown:") + " " + str(e.description)}), 429
 
     @bp.errorhandler(403)
     def denied(e):
         return jsonify({"error": str(e.description)}), 403
 
     @bp.route("/")
     @limiter.exempt
     def index():
         if args.disable_web_ui:
             abort(404)
 
+        langcode = request.args.get('lang')
+        if langcode and langcode in get_available_locale_codes(not args.debug):
+            session.update(preferred_lang=langcode)
+
         return render_template(
             "index.html",
             gaId=args.ga_id,
             frontendTimeout=args.frontend_timeout,
             api_keys=args.api_keys,
             get_api_key_link=args.get_api_key_link,
             web_version=os.environ.get("LT_WEB") is not None,
             version=get_version(),
             swagger_url=SWAGGER_URL,
-            url_prefix=args.url_prefix
+            available_locales=[{'code': l['code'], 'name': _lazy(l['name'])} for l in get_available_locales(not args.debug)],
+            current_locale=get_locale(),
+            alternate_locales=get_alternate_locale_links()
         )
 
-    @bp.get("/javascript-licenses")
+    @bp.route("/js/app.js")
     @limiter.exempt
-    def javascript_licenses():
-        if args.disable_web_ui:
+    def appjs():
+      if args.disable_web_ui:
             abort(404)
 
-        return render_template("javascript-licenses.html")
+      return Response(render_template("app.js.template", 
+            url_prefix=args.url_prefix,
+            get_api_key_link=args.get_api_key_link), content_type='application/javascript; charset=utf-8')
 
     @bp.get("/languages")
     @limiter.exempt
     def langs():
         """
         Retrieve list of supported languages
         ---
@@ -319,15 +346,15 @@
                     description: Human-readable language name (in English)
                   targets:
                     type: array
                     items:
                       type: string
                     description: Supported target language codes
         """
-        return jsonify([{"code": l.code, "name": l.name, "targets": language_pairs.get(l.code, [])} for l in languages])
+        return jsonify([{"code": l.code, "name": _lazy(l.name), "targets": language_pairs.get(l.code, [])} for l in languages])
 
     # Add cors
     @bp.after_request
     def after_request(response):
         response.headers.add("Access-Control-Allow-Origin", "*")
         response.headers.add(
             "Access-Control-Allow-Headers", "Authorization, Content-Type"
@@ -448,42 +475,40 @@
         else:
             q = request.values.get("q")
             source_lang = request.values.get("source")
             target_lang = request.values.get("target")
             text_format = request.values.get("format")
 
         if not q:
-            abort(400, description="Invalid request: missing q parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='q'))
         if not source_lang:
-            abort(400, description="Invalid request: missing source parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='source'))
         if not target_lang:
-            abort(400, description="Invalid request: missing target parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='target'))
 
         batch = isinstance(q, list)
 
         if batch and args.batch_limit != -1:
             batch_size = len(q)
             if args.batch_limit < batch_size:
                 abort(
                     400,
-                    description="Invalid request: Request (%d) exceeds text limit (%d)"
-                                % (batch_size, args.batch_limit),
+                    description=_("Invalid request: request (%(size)s) exceeds text limit (%(limit)s)", size=batch_size, limit=args.batch_limit),
                 )
 
         if args.char_limit != -1:
             if batch:
                 chars = sum([len(text) for text in q])
             else:
                 chars = len(q)
 
             if args.char_limit < chars:
                 abort(
                     400,
-                    description="Invalid request: Request (%d) exceeds character limit (%d)"
-                                % (chars, args.char_limit),
+                    description=_("Invalid request: request (%(size)s) exceeds text limit (%(limit)s)", size=chars, limit=args.char_limit),
                 )
 
         if source_lang == "auto":
             source_langs = []
             if batch:
                 auto_detect_texts = q
             else:
@@ -508,34 +533,34 @@
             else:
                 source_langs = [ {"confidence": 100.0, "language": source_lang} ]
 
         src_langs = [next(iter([l for l in languages if l.code == source_lang["language"]]), None) for source_lang in source_langs]
 
         for idx, lang in enumerate(src_langs):
             if lang is None:
-                abort(400, description="%s is not supported" % source_langs[idx])
+                abort(400, description=_("%(lang)s is not supported", lang=source_langs[idx]))
 
         tgt_lang = next(iter([l for l in languages if l.code == target_lang]), None)
 
         if tgt_lang is None:
-            abort(400, description="%s is not supported" % target_lang)
+            abort(400, description=_("%(lang)s is not supported",lang=target_lang))
 
         if not text_format:
             text_format = "text"
 
         if text_format not in ["text", "html"]:
-            abort(400, description="%s format is not supported" % text_format)
+            abort(400, description=_("%(format)s format is not supported", format=text_format))
 
         try:
             if batch:
                 results = []
                 for idx, text in enumerate(q):
                     translator = src_langs[idx].get_translation(tgt_lang)
                     if translator is None:
-                        abort(400, description="%s (%s) is not available as a target language from %s (%s)" % (tgt_lang.name, tgt_lang.code, src_langs[idx].name, src_langs[idx].code))
+                        abort(400, description=_("%(tname)s (%(tcode)s) is not available as a target language from %(sname)s (%(scode)s)", tname=_lazy(tgt_lang.name), tcode=tgt_lang.code, sname=_lazy(src_langs[idx].name), scode=src_langs[idx].code))
 
                     if text_format == "html":
                         translated_text = str(translate_html(translator, text))
                     else:
                         translated_text = improve_translation_formatting(text, translator.translate(text))
 
                     results.append(unescape(translated_text))
@@ -551,15 +576,15 @@
                           {
                             "translatedText": results
                           }
                     )
             else:
                 translator = src_langs[0].get_translation(tgt_lang)
                 if translator is None:
-                    abort(400, description="%s (%s) is not available as a target language from %s (%s)" % (tgt_lang.name, tgt_lang.code, src_langs[0].name, src_langs[0].code))
+                    abort(400, description=_("%(tname)s (%(tcode)s) is not available as a target language from %(sname)s (%(scode)s)", tname=_lazy(tgt_lang.name), tcode=tgt_lang.code, sname=_lazy(src_langs[0].name), scode=src_langs[0].code))
 
                 if text_format == "html":
                     translated_text = str(translate_html(translator, q))
                 else:
                     translated_text = improve_translation_formatting(q, translator.translate(q))
 
                 if source_lang == "auto":
@@ -572,15 +597,15 @@
                 else:
                     return jsonify(
                         {
                             "translatedText": unescape(translated_text)
                         }
                     )
         except Exception as e:
-            abort(500, description="Cannot translate text: %s" % str(e))
+            abort(500, description=_("Cannot translate text: %(text)s", text=str(e)))
 
     @bp.post("/translate_file")
     @access_check
     def translate_file():
         """
         Translate file from a language to another
         ---
@@ -659,44 +684,44 @@
               type: object
               properties:
                 error:
                   type: string
                   description: Error message
         """
         if args.disable_files_translation:
-            abort(403, description="Files translation are disabled on this server.")
+            abort(403, description=_("Files translation are disabled on this server."))
 
         source_lang = request.form.get("source")
         target_lang = request.form.get("target")
         file = request.files['file']
 
         if not file:
-            abort(400, description="Invalid request: missing file parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='file'))
         if not source_lang:
-            abort(400, description="Invalid request: missing source parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='source'))
         if not target_lang:
-            abort(400, description="Invalid request: missing target parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='target'))
 
         if file.filename == '':
-            abort(400, description="Invalid request: empty file")
+            abort(400, description=_("Invalid request: empty file"))
 
         if os.path.splitext(file.filename)[1] not in frontend_argos_supported_files_format:
-            abort(400, description="Invalid request: file format not supported")
+            abort(400, description=_("Invalid request: file format not supported"))
 
         source_langs = [source_lang]
         src_langs = [next(iter([l for l in languages if l.code == source_lang]), None) for source_lang in source_langs]
 
         for idx, lang in enumerate(src_langs):
             if lang is None:
-                abort(400, description="%s is not supported" % source_langs[idx])
+                abort(400, description=_("%(lang)s is not supported", lang=source_langs[idx]))
 
         tgt_lang = next(iter([l for l in languages if l.code == target_lang]), None)
 
         if tgt_lang is None:
-            abort(400, description="%s is not supported" % target_lang)
+            abort(400, description=_("%(lang)s is not supported", lang=target_lang))
 
         try:
             filename = str(uuid.uuid4()) + '.' + secure_filename(file.filename)
             filepath = os.path.join(get_upload_dir(), filename)
 
             file.save(filepath)
 
@@ -713,23 +738,23 @@
 
     @bp.get("/download_file/<string:filename>")
     def download_file(filename: str):
         """
         Download a translated file
         """
         if args.disable_files_translation:
-            abort(400, description="Files translation are disabled on this server.")
+            abort(400, description=_("Files translation are disabled on this server."))
 
         filepath = os.path.join(get_upload_dir(), filename)
         try:
             checked_filepath = security.path_traversal_check(filepath, get_upload_dir())
             if os.path.isfile(checked_filepath):
                 filepath = checked_filepath
         except security.SuspiciousFileOperation:
-            abort(400, description="Invalid filename")
+            abort(400, description=_("Invalid filename"))
 
         return_data = io.BytesIO()
         with open(filepath, 'rb') as fo:
             return_data.write(fo.read())
         return_data.seek(0)
 
         download_filename = filename.split('.')
@@ -814,25 +839,22 @@
               id: error-response
               type: object
               properties:
                 error:
                   type: string
                   description: Error message
         """
-        if flood.is_banned(get_remote_address()):
-            abort(403, description="Too many request limits violations")
-
         if request.is_json:
             json = get_json_dict(request)
             q = json.get("q")
         else:
             q = request.values.get("q")
 
         if not q:
-            abort(400, description="Invalid request: missing q parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='q'))
 
         return jsonify(detect_languages(q))
 
     @bp.route("/frontend/settings")
     @limiter.exempt
     def frontend_settings():
         """
@@ -885,31 +907,33 @@
                         code:
                           type: string
                           description: Language code
                         name:
                           type: string
                           description: Human-readable language name (in English)
         """
+        target_lang = frontend_argos_language_target()
+
         return jsonify(
             {
                 "charLimit": args.char_limit,
                 "frontendTimeout": args.frontend_timeout,
                 "apiKeys": args.api_keys,
                 "keyRequired": bool(args.api_keys and args.require_api_key_origin),
                 "suggestions": args.suggestions,
                 "filesTranslation": not args.disable_files_translation,
                 "supportedFilesFormat": [] if args.disable_files_translation else frontend_argos_supported_files_format,
                 "language": {
                     "source": {
                         "code": frontend_argos_language_source.code,
-                        "name": frontend_argos_language_source.name,
+                        "name": _lazy(frontend_argos_language_source.name),
                     },
                     "target": {
-                        "code": frontend_argos_language_target.code,
-                        "name": frontend_argos_language_target.name,
+                        "code": target_lang.code,
+                        "name": _lazy(target_lang.name),
                     },
                 },
             }
         )
 
     @bp.post("/suggest")
     @access_check
@@ -965,52 +989,67 @@
               type: object
               properties:
                 error:
                   type: string
                   description: Error message
         """
         if not args.suggestions:
-            abort(403, description="Suggestions are disabled on this server.")
+            abort(403, description=_("Suggestions are disabled on this server."))
 
         q = request.values.get("q")
         s = request.values.get("s")
         source_lang = request.values.get("source")
         target_lang = request.values.get("target")
 
         if not q:
-            abort(400, description="Invalid request: missing q parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='q'))
         if not s:
-            abort(400, description="Invalid request: missing s parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='s'))
         if not source_lang:
-            abort(400, description="Invalid request: missing source parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='source'))
         if not target_lang:
-            abort(400, description="Invalid request: missing target parameter")
+            abort(400, description=_("Invalid request: missing %(name)s parameter", name='target'))
 
         SuggestionsDatabase().add(q, s, source_lang, target_lang)
         return jsonify({"success": True})
 
     app = Flask(__name__)
+
+    app.config["SESSION_TYPE"] = "filesystem"
+    app.config["SESSION_FILE_DIR"] = os.path.join("db", "sessions")
+    Session(app)
+
     if args.debug:
         app.config["TEMPLATES_AUTO_RELOAD"] = True
     if args.url_prefix:
         app.register_blueprint(bp, url_prefix=args.url_prefix)
     else:
         app.register_blueprint(bp)
     
     limiter.init_app(app)
 
     swag = swagger(app)
     swag["info"]["version"] = get_version()
     swag["info"]["title"] = "LibreTranslate"
 
-
     @app.route(API_URL)
     @limiter.exempt
     def spec():
-        return jsonify(swag)
+        return jsonify(lazy_swag(swag))
+
+    app.config["BABEL_TRANSLATION_DIRECTORIES"] = 'locales'
+    babel = Babel(app)
+    @babel.localeselector
+    def get_locale():
+        override_lang = request.headers.get('X-Override-Accept-Language')
+        if override_lang and override_lang in get_available_locale_codes():
+            return override_lang
+        return session.get('preferred_lang', request.accept_languages.best_match(get_available_locale_codes()))
+
+    app.jinja_env.globals.update(_e=gettext_escaped, _h=gettext_html)
 
     # Call factory function to create our blueprint
     swaggerui_blueprint = get_swaggerui_blueprint(SWAGGER_URL, API_URL)
     if args.url_prefix:
         app.register_blueprint(swaggerui_blueprint, url_prefix=SWAGGER_URL)
     else:
         app.register_blueprint(swaggerui_blueprint)
```

### Comparing `libretranslate-1.3.8/libretranslate/default_values.py` & `libretranslate-1.3.9/libretranslate/default_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,20 +89,20 @@
     {
         'name': 'SSL',
         'default_value': None,
         'value_type': 'bool'
     },
     {
         'name': 'FRONTEND_LANGUAGE_SOURCE',
-        'default_value': 'en',
+        'default_value': 'auto',
         'value_type': 'str'
     },
     {
         'name': 'FRONTEND_LANGUAGE_TARGET',
-        'default_value': 'es',
+        'default_value': 'locale',
         'value_type': 'str'
     },
     {
         'name': 'FRONTEND_TIMEOUT',
         'default_value': 500,
         'value_type': 'int'
     },
```

### Comparing `libretranslate-1.3.8/libretranslate/detect.py` & `libretranslate-1.3.9/libretranslate/detect.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate/flood.py` & `libretranslate-1.3.9/libretranslate/flood.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate/init.py` & `libretranslate-1.3.9/libretranslate/init.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate/language.py` & `libretranslate-1.3.9/libretranslate/language.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate/main.py` & `libretranslate-1.3.9/libretranslate/main.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate/manage.py` & `libretranslate-1.3.9/libretranslate/manage.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate/remove_translated_files.py` & `libretranslate-1.3.9/libretranslate/remove_translated_files.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate/suggestions.py` & `libretranslate-1.3.9/libretranslate/suggestions.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate/tests/test_api/test_api_detect_language.py` & `libretranslate-1.3.9/libretranslate/tests/test_api/test_api_detect_language.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate/tests/test_api/test_api_translate.py` & `libretranslate-1.3.9/libretranslate/tests/test_api/test_api_translate.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.3.8/libretranslate.egg-info/PKG-INFO` & `libretranslate-1.3.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretranslate
-Version: 1.3.8
+Version: 1.3.9
 Summary: Free and Open Source Machine Translation API. Self-hosted, no limits, no ties to proprietary services.
 Home-page: https://libretranslate.com
 Author: LibreTranslate Authors
 Author-email: pt@uav4geo.com
 License: GNU Affero General Public License v3.0
 Description: # LibreTranslate
         
@@ -143,15 +143,15 @@
         
         Then open a web browser to http://localhost:5000
         
         
         ### Build with Docker
         
         ```bash
-        docker build [--build-arg with_models=true] -t libretranslate .
+        docker build -f docker/Dockerfile [--build-arg with_models=true] -t libretranslate .
         ```
         
         If you want to run the Docker image in a complete offline environment, you need to add the `--build-arg with_models=true` parameter. Then the language models are downloaded during the build process of the image. Otherwise these models get downloaded on the first run of the image/container.
         
         Run the built image:
         
         ```bash
@@ -187,30 +187,31 @@
         | --char-limit                | Set character limit                                                                                         | `No limit`               | LT_CHAR_LIMIT                |
         | --req-limit                 | Set maximum number of requests per minute per client                                                        | `No limit`               | LT_REQ_LIMIT                 |
         | --req-limit-storage         | Storage URI to use for request limit data storage. See [Flask Limiter](https://flask-limiter.readthedocs.io/en/stable/configuration.html) | `memory://` | LT_REQ_LIMIT_STORAGE |
         | --batch-limit               | Set maximum number of texts to translate in a batch request                                                 | `No limit`               | LT_BATCH_LIMIT               |
         | --ga-id                     | Enable Google Analytics on the API client page by providing an ID                                           | `No tracking`               | LT_GA_ID                     |
         | --debug                     | Enable debug environment                                                                                    | `False`           | LT_DEBUG                     |
         | --ssl                       | Whether to enable SSL                                                                                       | `False`               | LT_SSL                       |
-        | --frontend-language-source  | Set frontend default language - source                                                                      | `en`          | LT_FRONTEND_LANGUAGE_SOURCE  |
-        | --frontend-language-target  | Set frontend default language - target                                                                      | `es`          | LT_FRONTEND_LANGUAGE_TARGET  |
+        | --frontend-language-source  | Set frontend default language - source                                                                      | `auto`        | LT_FRONTEND_LANGUAGE_SOURCE  |
+        | --frontend-language-target  | Set frontend default language - target                                                                      | `locale` (match site's locale)   | LT_FRONTEND_LANGUAGE_TARGET  |
         | --frontend-timeout          | Set frontend translation timeout                                                                            | `500`         | LT_FRONTEND_TIMEOUT          |
         | --api-keys                  | Enable API keys database for per-user rate limits lookup                                                    | `Don't use API keys` | LT_API_KEYS                  |
         | --api-keys-db-path          | Use a specific path inside the container for the local database. Can be absolute or relative                | `db/api_keys.db`                      | LT_API_KEYS_DB_PATH          |
         | --api-keys-remote           | Use this remote endpoint to query for valid API keys instead of using the local database                    | `Use local API key database` | LT_API_KEYS_REMOTE                  |
         | --get-api-key-link          | Show a link in the UI where to direct users to get an API key                                               | `Don't show a link` | LT_GET_API_KEY_LINK                  |
         | --require-api-key-origin    | Require use of an API key for programmatic access to the API, unless the request origin matches this domain | `No restrictions on domain origin` | LT_REQUIRE_API_KEY_ORIGIN    |
         | --load-only                 | Set available languages                                                                                     | `all from argostranslate`    | LT_LOAD_ONLY                 |
         | --threads                   | Set number of threads                                                                                       | `4`    | LT_THREADS                 |
         | --suggestions               | Allow user suggestions                                                                                      | `False`    | LT_SUGGESTIONS               |
         | --disable-files-translation | Disable files translation                                                                                   | `False`    | LT_DISABLE_FILES_TRANSLATION |
         | --disable-web-ui            | Disable web ui                                                                                              | `False`    | LT_DISABLE_WEB_UI            |
         | --update-models             | Update language models at startup                                                                           | `False`    | LT_UPDATE_MODELS            |
         | --metrics                   | Enable the /metrics endpoint for exporting [Prometheus](https://prometheus.io/) usage metrics               | `Disabled`    | LT_METRICS            |
         | --metrics-auth-token        | Protect the /metrics endpoint by allowing only clients that have a valid Authorization Bearer token         | `No auth`    | LT_METRICS_AUTH_TOKEN            |
+        | --url-prefix                | Add prefix to URL: example.com:5000/url-prefix/                                                             | `/`    | LT_URL_PREFIX            |
         
         Note that each argument has an equivalent environment variable that can be used instead. The env. variables overwrite the default values but have lower priority than the command arguments and are particularly useful if used with Docker. The environment variable names are the upper-snake-case of the equivalent command argument's name with a `LT` prefix.
         
         ## Update
         
         ### Software
         
@@ -222,15 +223,15 @@
         
         `docker pull libretranslate/libretranslate`
         
         ### Language Models
         
         Start the program with the `--update-models` argument. For example: `libretranslate --update-models` or `./run.sh --update-models`.
         
-        Alternatively you can also run the `install_models.py` script.
+        Alternatively you can also run the `scripts/install_models.py` script.
         
         ## Run with WSGI and Gunicorn
         
         ```
         pip install gunicorn
         gunicorn --bind 0.0.0.0:5000 'wsgi:app'
         ```
@@ -311,15 +312,15 @@
         
         If you use Gunicorn, make sure to create a directory for storing multiprocess data metrics and set `PROMETHEUS_MULTIPROC_DIR`:
         
         ```
         mkdir -p /tmp/prometheus_data
         rm /tmp/prometheus_data/*
         export PROMETHEUS_MULTIPROC_DIR=/tmp/prometheus_data 
-        gunicorn -c gunicorn_conf.py --bind 0.0.0.0:5000 'wsgi:app(metrics=True)' 
+        gunicorn -c scripts/gunicorn_conf.py --bind 0.0.0.0:5000 'wsgi:app(metrics=True)' 
         ```
         
         ## Language Bindings
         
         You can use the LibreTranslate API using the following bindings:
         
          - Rust: https://github.com/DefunctLizard/libretranslate-rs
@@ -365,35 +366,84 @@
         ## Mirrors
         
         This is a list of public LibreTranslate instances, some require an API key. If you want to add a new URL, please open a pull request.
         
         URL |API Key Required | Links
         --- | --- | ---
         [libretranslate.com](https://libretranslate.com)|:heavy_check_mark:|[Get API Key](https://portal.libretranslate.com)
-        [libretranslate.de](https://libretranslate.de)|-
         [translate.argosopentech.com](https://translate.argosopentech.com/)|-
-        [translate.api.skitzen.com](https://translate.api.skitzen.com/)|-
-        [translate.fortytwo-it.com](https://translate.fortytwo-it.com/)|-
         [translate.terraprint.co](https://translate.terraprint.co/)|-
         [lt.vern.cc](https://lt.vern.cc)|-
         
         ## TOR/i2p Mirrors
         
-        URL |API Key Required|Payment Link|Cost
-        --- | --- | --- | ---
-        [lt.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion](http://lt.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion/)|-|-
-        [lt.vern.i2p](http://vernf45n7mxwqnp5riaax7p67pwcl7wcefdcnqqvim7ckdx4264a.b32.i2p/)|-|-
+        URL |
+        --- |
+        [lt.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion](http://lt.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion/)|
+        [lt.vern.i2p](http://vernf45n7mxwqnp5riaax7p67pwcl7wcefdcnqqvim7ckdx4264a.b32.i2p/)|
         
         
-        ## Adding New Languages
+        ## Adding New Language Models
         
         To add new languages you first need to train an Argos Translate model. See [this video](https://odysee.com/@argosopentech:7/training-an-Argos-Translate-model-tutorial-2022:2?r=DMnK7NqdPNHRCfwhmKY9LPow3PqVUUgw) for details.
         
         First you need to collect data, for example from [Opus](http://opus.nlpl.eu/), then you need to add the data to [data-index.json](https://github.com/argosopentech/argos-train/blob/master/data-index.json) in the [Argos Train](https://github.com/argosopentech/argos-train) repo.
         
+        ## Localization
+        
+        The LibreTranslate Web UI is available in all the languages for which LibreTranslate can translate to. It can also (roughly) [translate itself!](https://github.com/LibreTranslate/LibreTranslate/blob/main/scripts/update_locales.py) Some languages might not appear in the UI since they haven't been reviewed by a human yet. You can enable all languages by turning on `--debug` mode.
+        
+        To help improve or review the UI translations:
+         - Go to https://hosted.weblate.org/projects/libretranslate/app/#translations. All changes are automatically pushed to this repository.
+         - Once all strings have been reviewed/edited, open a pull request and change `libretranslate/locales/{code}/meta.json`:
+        
+         ```json
+        {
+        	"name": "<Language>",
+        	"reviewed": true <-- Change this from false to true
+        }
+         ```
+        
+        ### UI Languages
+        
+        Language | Reviewed | Weblate Link
+        -------- | -------- | ------------
+        Arabic |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/ar/)
+        Azerbaijani |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/az/)
+        Chinese |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/zh/)
+        Czech |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/cs/)
+        Danish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/da/)
+        Dutch |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/nl/)
+        English | :heavy_check_mark: | [Edit](https://hosted.weblate.org/projects/libretranslate/app/)
+        Esperanto |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/eo/)
+        Finnish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/fi/)
+        French |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/fr/)
+        German | :heavy_check_mark: | [Edit](https://hosted.weblate.org/translate/libretranslate/app/de/)
+        Greek |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/el/)
+        Hebrew |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/he/)
+        Hindi |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/hi/)
+        Hungarian |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/hu/)
+        Indonesian |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/id/)
+        Irish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/ga/)
+        Italian | :heavy_check_mark: | [Edit](https://hosted.weblate.org/translate/libretranslate/app/it/)
+        Japanese |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/ja/)
+        Kabyle |  | [Edit](https://hosted.weblate.org/projects/libretranslate/app/kab/)
+        Korean |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/ko/)
+        Occitan |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/oc/)
+        Persian |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/fa/)
+        Polish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/pl/)
+        Portuguese |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/pt/)
+        Russian |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/ru/)
+        Slovak |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/sk/)
+        Spanish | :heavy_check_mark: | [Edit](https://hosted.weblate.org/translate/libretranslate/app/es/)
+        Swedish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/sv/)
+        Turkish |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/tr/)
+        Ukranian |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/uk/)
+        Vietnamese |  | [Edit](https://hosted.weblate.org/translate/libretranslate/app/vi/)
+        
         ## Roadmap
         
         Help us by opening a pull request!
         
         - [x] A docker image (thanks [@vemonet](https://github.com/vemonet) !)
         - [x] Auto-detect input language (thanks [@vemonet](https://github.com/vemonet) !)
         - [X] User authentication / tokens
@@ -575,13 +625,12 @@
         ## Trademark
         
         See [Trademark Guidelines](https://github.com/LibreTranslate/LibreTranslate/blob/main/TRADEMARK.md)
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `libretranslate-1.3.8/libretranslate.egg-info/SOURCES.txt` & `libretranslate-1.3.9/libretranslate.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 libretranslate/api_keys.py
 libretranslate/app.py
 libretranslate/default_values.py
 libretranslate/detect.py
 libretranslate/flood.py
 libretranslate/init.py
 libretranslate/language.py
+libretranslate/locales.py
 libretranslate/main.py
 libretranslate/manage.py
 libretranslate/no_limiter.py
 libretranslate/remove_translated_files.py
 libretranslate/security.py
 libretranslate/suggestions.py
 libretranslate.egg-info/PKG-INFO
```

### Comparing `libretranslate-1.3.8/setup.py` & `libretranslate-1.3.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,31 +9,30 @@
     description='Free and Open Source Machine Translation API. Self-hosted, no limits, no ties to proprietary services.',
     author='LibreTranslate Authors',
     author_email='pt@uav4geo.com',
     url='https://libretranslate.com',
     packages=find_packages(),
     # packages=find_packages(include=['openpredict']),
     # package_dir={'openpredict': 'openpredict'},
-    package_data={'': ['static/*', 'static/**/*', 'templates/*']},
+    package_data={'': ['static/*', 'static/**/*', 'templates/*', 'locales/**/meta.json', 'locales/**/**/*.mo']},
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'libretranslate=libretranslate.main:main',
             'ltmanage=libretranslate.manage:manage'
         ],
     },
 
-    python_requires='>=3.7.0',
+    python_requires='>=3.8.0',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     install_requires=open("requirements.txt", "r").readlines(),
-    tests_require=['pytest==7.1.2'],
+    tests_require=['pytest==7.2.0'],
     setup_requires=['pytest-runner'],
     classifiers=[
         "License :: OSI Approved :: GNU Affero General Public License v3 ",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10"
     ]
 )
```

