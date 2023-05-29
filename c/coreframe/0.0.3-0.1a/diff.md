# Comparing `tmp/coreframe-0.0.3.tar.gz` & `tmp/coreframe-0.1a.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coreframe-0.0.3.tar", last modified: Mon May 29 18:06:53 2023, max compression
+gzip compressed data, was "dist/coreframe-0.1a.tar", last modified: Mon Jun 29 22:19:17 2020, max compression
```

## Comparing `coreframe-0.0.3.tar` & `coreframe-0.1a.tar`

### file list

```diff
@@ -1,22 +1,4 @@
-drwxrwxrwx   0 azamat    (1000) azamat    (1000)        0 2023-05-29 18:06:53.376233 coreframe-0.0.3/
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)     1088 2023-05-29 17:58:57.000000 coreframe-0.0.3/LICENSE
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      712 2023-05-29 18:06:53.375229 coreframe-0.0.3/PKG-INFO
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       88 2023-02-27 05:49:39.000000 coreframe-0.0.3/README.md
-drwxrwxrwx   0 azamat    (1000) azamat    (1000)        0 2023-05-29 18:06:53.352231 coreframe-0.0.3/coreframe/
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      194 2023-05-29 17:59:07.000000 coreframe-0.0.3/coreframe/__init__.py
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      177 2023-05-29 17:59:07.000000 coreframe-0.0.3/coreframe/config.py
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)    18637 2023-05-29 17:59:07.000000 coreframe-0.0.3/coreframe/coreframe.py
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      690 2023-02-27 05:27:46.000000 coreframe-0.0.3/coreframe/from_csv.py
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)     1318 2023-05-29 17:59:07.000000 coreframe-0.0.3/coreframe/from_nc.py
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)     5096 2023-05-29 17:59:07.000000 coreframe-0.0.3/coreframe/parallelize.py
-drwxrwxrwx   0 azamat    (1000) azamat    (1000)        0 2023-05-29 18:06:53.372231 coreframe-0.0.3/coreframe.egg-info/
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      712 2023-05-29 18:06:53.000000 coreframe-0.0.3/coreframe.egg-info/PKG-INFO
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      362 2023-05-29 18:06:53.000000 coreframe-0.0.3/coreframe.egg-info/SOURCES.txt
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)        1 2023-05-29 18:06:53.000000 coreframe-0.0.3/coreframe.egg-info/dependency_links.txt
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       11 2023-05-29 18:06:53.000000 coreframe-0.0.3/coreframe.egg-info/requires.txt
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       10 2023-05-29 18:06:53.000000 coreframe-0.0.3/coreframe.egg-info/top_level.txt
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       82 2023-02-03 14:00:45.000000 coreframe-0.0.3/pyproject.toml
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       38 2023-05-29 18:06:53.376233 coreframe-0.0.3/setup.cfg
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      966 2023-05-29 18:05:15.000000 coreframe-0.0.3/setup.py
-drwxrwxrwx   0 azamat    (1000) azamat    (1000)        0 2023-05-29 18:06:53.374230 coreframe-0.0.3/tests/
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)    11554 2023-05-29 17:59:07.000000 coreframe-0.0.3/tests/test_coreframe.py
+drwxr-xr-x   0 hjkim     (2122) hydrolab  (1000)        0 2020-06-29 22:19:17.000000 coreframe-0.1a/
+-rw-r--r--   0 hjkim     (2122) hydrolab  (1000)      479 2020-06-29 22:19:17.000000 coreframe-0.1a/PKG-INFO
+-rw-r--r--   0 hjkim     (2122) hydrolab  (1000)      959 2015-07-12 00:38:03.000000 coreframe-0.1a/__init__.py
+-rwxr-xr-x   0 hjkim     (2122) hydrolab  (1000)      964 2020-06-29 22:19:01.000000 coreframe-0.1a/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

