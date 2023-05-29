# Comparing `tmp/distgen-1.8.tar.gz` & `tmp/distgen-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/distgen-1.8.tar", last modified: Tue Jun  8 14:06:07 2021, max compression
+gzip compressed data, was "distgen-1.9.tar", last modified: Wed Jan 26 12:55:50 2022, max compression
```

## Comparing `distgen-1.8.tar` & `distgen-1.9.tar`

### file list

```diff
@@ -1,249 +1,254 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)      354 2021-06-08 14:05:01.000000 distgen-1.8/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2021-06-08 14:05:01.000000 distgen-1.8/docs/spec_expansion.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5809 2021-06-08 14:05:01.000000 distgen-1.8/docs/intro.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4676 2021-06-08 14:05:01.000000 distgen-1.8/docs/config.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      607 2021-06-08 14:05:01.000000 distgen-1.8/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     5255 2021-06-08 14:05:01.000000 distgen-1.8/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7135 2021-06-08 14:05:01.000000 distgen-1.8/docs/spec_multispec.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1509 2021-06-08 14:05:01.000000 distgen-1.8/docs/usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      523 2021-06-08 14:05:01.000000 distgen-1.8/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1108 2021-06-08 14:05:01.000000 distgen-1.8/docs/builtins.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      895 2021-06-08 14:05:01.000000 distgen-1.8/docs/macros.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)      196 2021-06-08 14:05:01.000000 distgen-1.8/dg
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2021-06-08 14:05:01.000000 distgen-1.8/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      371 2021-06-08 14:06:07.000000 distgen-1.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3342 2021-06-08 14:05:01.000000 distgen-1.8/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      911 2021-06-08 14:05:01.000000 distgen-1.8/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/distgen/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1690 2021-06-08 14:05:01.000000 distgen-1.8/distgen/pathmanager.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/distgen/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/distgen/templates/container/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/distgen/templates/container/docker/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3420 2021-06-08 14:05:01.000000 distgen-1.8/distgen/templates/container/docker/parts.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2021-06-08 14:05:01.000000 distgen-1.8/distgen/templates/makefile-macros.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2021-06-08 14:05:01.000000 distgen-1.8/distgen/templates/general.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      464 2021-06-08 14:05:01.000000 distgen-1.8/distgen/templates/docker.tpl
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/distgen/distconf/
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-24-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-29-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/rhel-7.3-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-22-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-28-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-28-x86_64.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/distgen/distconf/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)       86 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/lib/rpmsystems.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/lib/centos.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      283 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/lib/fedora.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      409 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/lib/general.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      126 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/lib/rhel.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      215 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/centos-7-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-35-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-27-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-33-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-25-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-30-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-31-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-27-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-21-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-34-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-20-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-20-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-rawhide-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-29-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-26-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-32-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-35-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/rhel-7.2-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      204 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/rhel-7-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/centos-6-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-30-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-34-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-23-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-26-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-31-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-25-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-24-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-32-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/rhel-8-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      121 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-rawhide-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-33-i686.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-23-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-22-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/fedora-21-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      215 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distconf/centos-8-x86_64.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2021-06-08 14:05:01.000000 distgen-1.8/distgen/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10651 2021-06-08 14:05:01.000000 distgen-1.8/distgen/multispec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10449 2021-06-08 14:05:01.000000 distgen-1.8/distgen/generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1587 2021-06-08 14:05:01.000000 distgen-1.8/distgen/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2021-06-08 14:05:01.000000 distgen-1.8/distgen/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2420 2021-06-08 14:05:01.000000 distgen-1.8/distgen/commands.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       83 2021-06-08 14:05:01.000000 distgen-1.8/distgen/err.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:01.000000 distgen-1.8/distgen/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      526 2021-06-08 14:05:01.000000 distgen-1.8/distgen/distro_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5809 2021-06-08 14:05:01.000000 distgen-1.8/bin/dg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/unittests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/unittests/test_examples.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/examples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/examples/copr/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/examples/copr/copr_cli/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1067 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/copr_cli/build_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1067 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/copr_cli/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49047 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/copr_cli/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/copr_cli/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/examples/copr/fake-deps/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/examples/copr/fake-deps/copr/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/fake-deps/copr/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/examples/copr/fake-deps/copr/client/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/fake-deps/copr/client/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       29 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/fake-deps/copr/client/responses.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/fake-deps/copr/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/fake-deps/jinja2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/fake-deps/simplejson.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1070 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/copr/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/examples/old_format/
--rw-rw-r--   0 travis    (2000) travis    (2000)      519 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/old_format/example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      823 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/old_format/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/examples/raw-description/
--rw-rw-r--   0 travis    (2000) travis    (2000)      982 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/examples/raw-description/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/build_manpages/build_manpages/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3172 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/build_manpages/build_manpages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8899 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/build_manpages/build_manpage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5527 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/build_manpages/manpage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/build_manpages/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      319 2021-06-08 14:05:02.000000 distgen-1.8/build_manpages/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/distgen.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      371 2021-06-08 14:06:06.000000 distgen-1.8/distgen.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-08 14:06:06.000000 distgen-1.8/distgen.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2021-06-08 14:06:06.000000 distgen-1.8/distgen.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6636 2021-06-08 14:06:06.000000 distgen-1.8/distgen.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2021-06-08 14:06:06.000000 distgen-1.8/distgen.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2021-06-08 14:06:07.000000 distgen-1.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    18092 2021-06-08 14:05:01.000000 distgen-1.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1720 2021-06-08 14:05:01.000000 distgen-1.8/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3821 2021-06-08 14:05:01.000000 distgen-1.8/NEWS
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/macros-cmdline/
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-cmdline/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-cmdline/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-cmdline/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-cmdline/dg-opts
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-cmdline/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/minimal-dockerfile/
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-06-08 14:05:01.000000 distgen-1.8/tests/minimal-dockerfile/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      624 2021-06-08 14:05:01.000000 distgen-1.8/tests/minimal-dockerfile/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)       62 2021-06-08 14:05:01.000000 distgen-1.8/tests/minimal-dockerfile/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:01.000000 distgen-1.8/tests/minimal-dockerfile/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/unittests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/unittests/fixtures/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/unittests/fixtures/generator/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/unittests/fixtures/generator/simple_with_projectfile/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1387 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/generator/simple_with_projectfile/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)      253 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/generator/simple_with_projectfile/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1369 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/generator/simple_with_projectfile/expected_output
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/generator/simple_with_projectfile/common.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      816 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/generator/simple_with_projectfile/complex.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/unittests/fixtures/generator/projectfile/
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/generator/projectfile/project.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/unittests/fixtures/generator/simple/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1354 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/generator/simple/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/generator/simple/expected_output
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/generator/simple/common.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      930 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/generator/simple/complex.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/unittests/fixtures/multispec/
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/multispec/simplest.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1090 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/multispec/complex.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/unittests/fixtures/load_config/
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/load_config/level3.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/load_config/simple.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       36 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/fixtures/load_config/level2.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2264 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/test_pathmanager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2288 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/test_commands.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1018 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/test_distro_detection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7462 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/test_multispec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      315 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/test_error.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3025 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/test_generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1063 2021-06-08 14:05:01.000000 distgen-1.8/tests/unittests/test_config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/macros/
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)     2832 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros/test.yaml
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3695 2021-06-08 14:05:01.000000 distgen-1.8/tests/testsuite
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/keep-block-whitespaces/
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2021-06-08 14:05:01.000000 distgen-1.8/tests/keep-block-whitespaces/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)       42 2021-06-08 14:05:01.000000 distgen-1.8/tests/keep-block-whitespaces/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2021-06-08 14:05:01.000000 distgen-1.8/tests/keep-block-whitespaces/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2021-06-08 14:05:01.000000 distgen-1.8/tests/keep-block-whitespaces/dg-opts
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/docker-labels/
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-labels/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      913 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-labels/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2310 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-labels/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-labels/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)      167 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-labels/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/dockerfile/
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-06-08 14:05:01.000000 distgen-1.8/tests/dockerfile/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      891 2021-06-08 14:05:01.000000 distgen-1.8/tests/dockerfile/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4293 2021-06-08 14:05:01.000000 distgen-1.8/tests/dockerfile/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2021-06-08 14:05:01.000000 distgen-1.8/tests/dockerfile/container_opt
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2021-06-08 14:05:01.000000 distgen-1.8/tests/dockerfile/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2021-06-08 14:05:01.000000 distgen-1.8/tests/dockerfile/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/SAMPLE/
--rw-rw-r--   0 travis    (2000) travis    (2000)       29 2021-06-08 14:05:01.000000 distgen-1.8/tests/SAMPLE/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-08 14:05:01.000000 distgen-1.8/tests/SAMPLE/test.exp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/SAMPLE/subdir/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:01.000000 distgen-1.8/tests/SAMPLE/subdir/.gitkeep
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2021-06-08 14:05:01.000000 distgen-1.8/tests/SAMPLE/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:01.000000 distgen-1.8/tests/SAMPLE/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/macros-from/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/macros-from/some-other-dir/
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-from/some-other-dir/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-from/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      186 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-from/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3679 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-from/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-from/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-from/dg-opts
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-from/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/macros-from/some-dir/
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-from/some-dir/project.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/pkginstaller/
--rw-rw-r--   0 travis    (2000) travis    (2000)      608 2021-06-08 14:05:01.000000 distgen-1.8/tests/pkginstaller/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)     2208 2021-06-08 14:05:01.000000 distgen-1.8/tests/pkginstaller/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2021-06-08 14:05:01.000000 distgen-1.8/tests/pkginstaller/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:01.000000 distgen-1.8/tests/pkginstaller/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/macros-short/
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-short/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)     2832 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-short/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-short/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-08 14:05:01.000000 distgen-1.8/tests/macros-short/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/multispec/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1268 2021-06-08 14:05:01.000000 distgen-1.8/tests/multispec/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      877 2021-06-08 14:05:01.000000 distgen-1.8/tests/multispec/multispec.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     3675 2021-06-08 14:05:01.000000 distgen-1.8/tests/multispec/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2021-06-08 14:05:01.000000 distgen-1.8/tests/multispec/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2021-06-08 14:05:01.000000 distgen-1.8/tests/multispec/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/docker-cmd/
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-cmd/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      190 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-cmd/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-cmd/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)       88 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-cmd/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/docker-entrypoint/
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-entrypoint/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-entrypoint/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-entrypoint/container_opt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-entrypoint/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)      676 2021-06-08 14:05:01.000000 distgen-1.8/tests/docker-entrypoint/test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/no-spec/
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2021-06-08 14:05:01.000000 distgen-1.8/tests/no-spec/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-06-08 14:05:01.000000 distgen-1.8/tests/no-spec/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2021-06-08 14:05:01.000000 distgen-1.8/tests/no-spec/distros
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-08 14:06:07.000000 distgen-1.8/tests/non-ascii-chars/
--rw-rw-r--   0 travis    (2000) travis    (2000)       90 2021-06-08 14:05:01.000000 distgen-1.8/tests/non-ascii-chars/test.tpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      181 2021-06-08 14:05:01.000000 distgen-1.8/tests/non-ascii-chars/test.exp
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2021-06-08 14:05:01.000000 distgen-1.8/tests/non-ascii-chars/distros
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2021-06-08 14:05:01.000000 distgen-1.8/tests/non-ascii-chars/test.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      216 2021-06-08 14:05:01.000000 distgen-1.8/AUTHORS
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.318197 distgen-1.9/
+-rw-r--r--   0 twine    (17125) twine    (17125)      216 2021-02-19 08:47:04.000000 distgen-1.9/AUTHORS
+-rw-r--r--   0 twine    (17125) twine    (17125)    18092 2021-02-19 08:47:04.000000 distgen-1.9/LICENSE
+-rw-r--r--   0 twine    (17125) twine    (17125)      354 2021-02-19 08:47:04.000000 distgen-1.9/MANIFEST.in
+-rw-r--r--   0 twine    (17125) twine    (17125)      911 2021-02-19 08:47:04.000000 distgen-1.9/Makefile
+-rw-r--r--   0 twine    (17125) twine    (17125)     4038 2022-01-26 12:55:36.000000 distgen-1.9/NEWS
+-rw-r--r--   0 twine    (17125) twine    (17125)      371 2022-01-26 12:55:50.318197 distgen-1.9/PKG-INFO
+-rw-r--r--   0 twine    (17125) twine    (17125)     3342 2021-02-19 08:47:04.000000 distgen-1.9/README.md
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.284196 distgen-1.9/bin/
+-rwxr-xr-x   0 twine    (17125) twine    (17125)     5809 2021-02-19 08:47:04.000000 distgen-1.9/bin/dg
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.284196 distgen-1.9/build_manpages/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.285197 distgen-1.9/build_manpages/build_manpages/
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/build_manpages/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     8899 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/build_manpages/build_manpage.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     3172 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/build_manpages/build_manpages.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     5527 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/build_manpages/manpage.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.280197 distgen-1.9/build_manpages/examples/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.285197 distgen-1.9/build_manpages/examples/copr/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.285197 distgen-1.9/build_manpages/examples/copr/copr_cli/
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/copr_cli/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1067 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/copr_cli/build_config.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    49047 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/copr_cli/main.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1067 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/copr_cli/util.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.286197 distgen-1.9/build_manpages/examples/copr/fake-deps/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.286197 distgen-1.9/build_manpages/examples/copr/fake-deps/copr/
+-rw-r--r--   0 twine    (17125) twine    (17125)       43 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/fake-deps/copr/__init__.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.286197 distgen-1.9/build_manpages/examples/copr/fake-deps/copr/client/
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/fake-deps/copr/client/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)       29 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/fake-deps/copr/client/responses.py
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/fake-deps/copr/exceptions.py
+-rw-r--r--   0 twine    (17125) twine    (17125)       28 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/fake-deps/jinja2.py
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/fake-deps/simplejson.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1070 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/copr/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.287196 distgen-1.9/build_manpages/examples/old_format/
+-rw-r--r--   0 twine    (17125) twine    (17125)      519 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/old_format/example.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      823 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/old_format/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.287196 distgen-1.9/build_manpages/examples/raw-description/
+-rw-r--r--   0 twine    (17125) twine    (17125)      982 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/examples/raw-description/setup.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      319 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.287196 distgen-1.9/build_manpages/unittests/
+-rw-r--r--   0 twine    (17125) twine    (17125)     3041 2021-06-08 14:02:12.000000 distgen-1.9/build_manpages/unittests/test_examples.py
+-rwxr-xr-x   0 twine    (17125) twine    (17125)      196 2021-02-19 08:47:04.000000 distgen-1.9/dg
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.289197 distgen-1.9/distgen/
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-02-19 08:47:04.000000 distgen-1.9/distgen/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     2420 2021-02-19 08:47:04.000000 distgen-1.9/distgen/commands.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1587 2021-02-19 08:47:04.000000 distgen-1.9/distgen/config.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.298197 distgen-1.9/distgen/distconf/
+-rw-r--r--   0 twine    (17125) twine    (17125)       92 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/centos-6-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      215 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/centos-7-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      215 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/centos-8-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      264 2022-01-26 12:55:36.000000 distgen-1.9/distgen/distconf/centos-stream-9-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       46 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-20-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-20-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       46 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-21-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-21-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-22-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-22-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-23-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-23-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-24-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-24-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-25-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-25-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-26-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-26-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-27-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-27-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-28-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-28-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-29-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-29-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-30-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-30-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-31-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-31-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-32-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-32-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-33-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-33-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-06-08 14:01:49.000000 distgen-1.9/distgen/distconf/fedora-34-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-06-08 14:01:49.000000 distgen-1.9/distgen/distconf/fedora-34-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2021-06-08 14:01:49.000000 distgen-1.9/distgen/distconf/fedora-35-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2021-06-08 14:01:49.000000 distgen-1.9/distgen/distconf/fedora-35-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2022-01-26 12:55:36.000000 distgen-1.9/distgen/distconf/fedora-36-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2022-01-26 12:55:36.000000 distgen-1.9/distgen/distconf/fedora-36-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2022-01-26 12:55:36.000000 distgen-1.9/distgen/distconf/fedora-37-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      111 2022-01-26 12:55:36.000000 distgen-1.9/distgen/distconf/fedora-37-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       78 2022-01-26 12:55:36.000000 distgen-1.9/distgen/distconf/fedora-rawhide-i686.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      121 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/fedora-rawhide-x86_64.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.299197 distgen-1.9/distgen/distconf/lib/
+-rw-r--r--   0 twine    (17125) twine    (17125)      124 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/lib/centos.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      283 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/lib/fedora.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      409 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/lib/general.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      126 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/lib/rhel.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       86 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/lib/rpmsystems.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      204 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/rhel-7-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       50 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/rhel-7.2-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       50 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/rhel-7.3-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       71 2021-02-19 08:47:04.000000 distgen-1.9/distgen/distconf/rhel-8-x86_64.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      856 2022-01-26 12:55:36.000000 distgen-1.9/distgen/distro_version.py
+-rw-r--r--   0 twine    (17125) twine    (17125)       83 2021-02-19 08:47:04.000000 distgen-1.9/distgen/err.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    10449 2021-02-19 08:47:04.000000 distgen-1.9/distgen/generator.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    10651 2021-02-19 08:47:04.000000 distgen-1.9/distgen/multispec.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1690 2021-02-19 08:47:04.000000 distgen-1.9/distgen/pathmanager.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1632 2021-02-19 08:47:04.000000 distgen-1.9/distgen/project.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.299197 distgen-1.9/distgen/templates/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.280197 distgen-1.9/distgen/templates/container/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.300197 distgen-1.9/distgen/templates/container/docker/
+-rw-r--r--   0 twine    (17125) twine    (17125)     3420 2021-02-19 08:47:04.000000 distgen-1.9/distgen/templates/container/docker/parts.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)      464 2021-02-19 08:47:04.000000 distgen-1.9/distgen/templates/docker.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)      469 2021-02-19 08:47:04.000000 distgen-1.9/distgen/templates/general.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)       53 2021-02-19 08:47:04.000000 distgen-1.9/distgen/templates/makefile-macros.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)       19 2022-01-26 12:55:36.000000 distgen-1.9/distgen/version.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.290197 distgen-1.9/distgen.egg-info/
+-rw-r--r--   0 twine    (17125) twine    (17125)      371 2022-01-26 12:55:50.000000 distgen-1.9/distgen.egg-info/PKG-INFO
+-rw-r--r--   0 twine    (17125) twine    (17125)     6833 2022-01-26 12:55:50.000000 distgen-1.9/distgen.egg-info/SOURCES.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)        1 2022-01-26 12:55:50.000000 distgen-1.9/distgen.egg-info/dependency_links.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)       25 2022-01-26 12:55:50.000000 distgen-1.9/distgen.egg-info/requires.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)        8 2022-01-26 12:55:50.000000 distgen-1.9/distgen.egg-info/top_level.txt
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.301197 distgen-1.9/docs/
+-rw-r--r--   0 twine    (17125) twine    (17125)      607 2021-02-19 08:47:04.000000 distgen-1.9/docs/Makefile
+-rw-r--r--   0 twine    (17125) twine    (17125)     1108 2021-02-19 08:47:04.000000 distgen-1.9/docs/builtins.rst
+-rw-r--r--   0 twine    (17125) twine    (17125)     5255 2021-02-19 08:47:04.000000 distgen-1.9/docs/conf.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     4676 2021-02-19 08:47:04.000000 distgen-1.9/docs/config.rst
+-rw-r--r--   0 twine    (17125) twine    (17125)      523 2021-02-19 08:47:04.000000 distgen-1.9/docs/index.rst
+-rw-r--r--   0 twine    (17125) twine    (17125)     5809 2021-02-19 08:47:04.000000 distgen-1.9/docs/intro.rst
+-rw-r--r--   0 twine    (17125) twine    (17125)      895 2021-02-19 08:47:04.000000 distgen-1.9/docs/macros.rst
+-rw-r--r--   0 twine    (17125) twine    (17125)     1499 2021-02-19 08:47:04.000000 distgen-1.9/docs/spec_expansion.rst
+-rw-r--r--   0 twine    (17125) twine    (17125)     7135 2021-02-19 08:47:04.000000 distgen-1.9/docs/spec_multispec.rst
+-rw-r--r--   0 twine    (17125) twine    (17125)     1509 2021-02-19 08:47:04.000000 distgen-1.9/docs/usage.rst
+-rw-r--r--   0 twine    (17125) twine    (17125)       25 2021-02-19 08:47:04.000000 distgen-1.9/requirements.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)      152 2022-01-26 12:55:50.318197 distgen-1.9/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)     1720 2021-02-19 08:47:04.000000 distgen-1.9/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.301197 distgen-1.9/tests/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.302197 distgen-1.9/tests/SAMPLE/
+-rw-r--r--   0 twine    (17125) twine    (17125)      110 2021-02-19 08:47:04.000000 distgen-1.9/tests/SAMPLE/distros
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.302197 distgen-1.9/tests/SAMPLE/subdir/
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-02-19 08:47:04.000000 distgen-1.9/tests/SAMPLE/subdir/.gitkeep
+-rw-r--r--   0 twine    (17125) twine    (17125)        1 2021-02-19 08:47:04.000000 distgen-1.9/tests/SAMPLE/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       29 2021-02-19 08:47:04.000000 distgen-1.9/tests/SAMPLE/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-02-19 08:47:04.000000 distgen-1.9/tests/SAMPLE/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.303197 distgen-1.9/tests/docker-cmd/
+-rw-r--r--   0 twine    (17125) twine    (17125)       14 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-cmd/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)      190 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-cmd/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       27 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-cmd/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)       88 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-cmd/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.304197 distgen-1.9/tests/docker-entrypoint/
+-rw-r--r--   0 twine    (17125) twine    (17125)        7 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-entrypoint/container_opt
+-rw-r--r--   0 twine    (17125) twine    (17125)       14 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-entrypoint/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)      534 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-entrypoint/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       27 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-entrypoint/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)      676 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-entrypoint/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.305197 distgen-1.9/tests/docker-labels/
+-rw-r--r--   0 twine    (17125) twine    (17125)       48 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-labels/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)      913 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-labels/project.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     2310 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-labels/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       27 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-labels/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)      167 2021-02-19 08:47:04.000000 distgen-1.9/tests/docker-labels/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.306197 distgen-1.9/tests/dockerfile/
+-rw-r--r--   0 twine    (17125) twine    (17125)        7 2021-02-19 08:47:04.000000 distgen-1.9/tests/dockerfile/container_opt
+-rw-r--r--   0 twine    (17125) twine    (17125)       89 2021-02-19 08:47:04.000000 distgen-1.9/tests/dockerfile/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)      891 2021-02-19 08:47:04.000000 distgen-1.9/tests/dockerfile/project.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     4293 2022-01-26 12:55:36.000000 distgen-1.9/tests/dockerfile/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       27 2021-02-19 08:47:04.000000 distgen-1.9/tests/dockerfile/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)     1238 2021-02-19 08:47:04.000000 distgen-1.9/tests/dockerfile/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.306197 distgen-1.9/tests/keep-block-whitespaces/
+-rw-r--r--   0 twine    (17125) twine    (17125)       25 2021-02-19 08:47:04.000000 distgen-1.9/tests/keep-block-whitespaces/dg-opts
+-rw-r--r--   0 twine    (17125) twine    (17125)       22 2021-02-19 08:47:04.000000 distgen-1.9/tests/keep-block-whitespaces/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)       42 2021-02-19 08:47:04.000000 distgen-1.9/tests/keep-block-whitespaces/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       73 2021-02-19 08:47:04.000000 distgen-1.9/tests/keep-block-whitespaces/test.tpl
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.307197 distgen-1.9/tests/macros/
+-rw-r--r--   0 twine    (17125) twine    (17125)      110 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)     2832 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       24 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.308197 distgen-1.9/tests/macros-cmdline/
+-rw-r--r--   0 twine    (17125) twine    (17125)       30 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-cmdline/dg-opts
+-rw-r--r--   0 twine    (17125) twine    (17125)      110 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-cmdline/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)      262 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-cmdline/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       17 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-cmdline/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-cmdline/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.309197 distgen-1.9/tests/macros-from/
+-rw-r--r--   0 twine    (17125) twine    (17125)       60 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-from/dg-opts
+-rw-r--r--   0 twine    (17125) twine    (17125)      110 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-from/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)      186 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-from/project.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.309197 distgen-1.9/tests/macros-from/some-dir/
+-rw-r--r--   0 twine    (17125) twine    (17125)      208 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-from/some-dir/project.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.309197 distgen-1.9/tests/macros-from/some-other-dir/
+-rw-r--r--   0 twine    (17125) twine    (17125)      159 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-from/some-other-dir/project.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     3679 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-from/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       73 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-from/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-from/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.310197 distgen-1.9/tests/macros-short/
+-rw-r--r--   0 twine    (17125) twine    (17125)      110 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-short/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)     2832 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-short/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       19 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-short/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-02-19 08:47:04.000000 distgen-1.9/tests/macros-short/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.310197 distgen-1.9/tests/minimal-dockerfile/
+-rw-r--r--   0 twine    (17125) twine    (17125)       62 2021-02-19 08:47:04.000000 distgen-1.9/tests/minimal-dockerfile/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)      624 2021-02-19 08:47:04.000000 distgen-1.9/tests/minimal-dockerfile/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       27 2021-02-19 08:47:04.000000 distgen-1.9/tests/minimal-dockerfile/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-02-19 08:47:04.000000 distgen-1.9/tests/minimal-dockerfile/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.311197 distgen-1.9/tests/multispec/
+-rw-r--r--   0 twine    (17125) twine    (17125)       49 2021-02-19 08:47:04.000000 distgen-1.9/tests/multispec/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)      877 2021-02-19 08:47:04.000000 distgen-1.9/tests/multispec/multispec.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)     3675 2021-02-19 08:47:04.000000 distgen-1.9/tests/multispec/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)     1268 2021-02-19 08:47:04.000000 distgen-1.9/tests/multispec/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)      113 2021-02-19 08:47:04.000000 distgen-1.9/tests/multispec/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.312197 distgen-1.9/tests/no-spec/
+-rw-r--r--   0 twine    (17125) twine    (17125)       14 2021-02-19 08:47:04.000000 distgen-1.9/tests/no-spec/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)       28 2021-02-19 08:47:04.000000 distgen-1.9/tests/no-spec/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       19 2021-02-19 08:47:04.000000 distgen-1.9/tests/no-spec/test.tpl
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.313197 distgen-1.9/tests/non-ascii-chars/
+-rw-r--r--   0 twine    (17125) twine    (17125)       33 2021-02-19 08:47:04.000000 distgen-1.9/tests/non-ascii-chars/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)      181 2021-02-19 08:47:04.000000 distgen-1.9/tests/non-ascii-chars/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)       90 2021-02-19 08:47:04.000000 distgen-1.9/tests/non-ascii-chars/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)       12 2021-02-19 08:47:04.000000 distgen-1.9/tests/non-ascii-chars/test.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.313197 distgen-1.9/tests/pkginstaller/
+-rw-r--r--   0 twine    (17125) twine    (17125)      110 2021-02-19 08:47:04.000000 distgen-1.9/tests/pkginstaller/distros
+-rw-r--r--   0 twine    (17125) twine    (17125)     2208 2021-02-19 08:47:04.000000 distgen-1.9/tests/pkginstaller/test.exp
+-rw-r--r--   0 twine    (17125) twine    (17125)      608 2021-02-19 08:47:04.000000 distgen-1.9/tests/pkginstaller/test.tpl
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-02-19 08:47:04.000000 distgen-1.9/tests/pkginstaller/test.yaml
+-rwxr-xr-x   0 twine    (17125) twine    (17125)     3695 2021-02-19 08:47:04.000000 distgen-1.9/tests/testsuite
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.315197 distgen-1.9/tests/unittests/
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/__init__.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.282197 distgen-1.9/tests/unittests/fixtures/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.282197 distgen-1.9/tests/unittests/fixtures/generator/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.315197 distgen-1.9/tests/unittests/fixtures/generator/projectfile/
+-rw-r--r--   0 twine    (17125) twine    (17125)      239 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/generator/projectfile/project.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.315197 distgen-1.9/tests/unittests/fixtures/generator/simple/
+-rw-r--r--   0 twine    (17125) twine    (17125)     1354 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/generator/simple/Dockerfile
+-rw-r--r--   0 twine    (17125) twine    (17125)      113 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/generator/simple/common.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      930 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/generator/simple/complex.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)     1359 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/generator/simple/expected_output
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.316197 distgen-1.9/tests/unittests/fixtures/generator/simple_with_projectfile/
+-rw-r--r--   0 twine    (17125) twine    (17125)     1387 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/generator/simple_with_projectfile/Dockerfile
+-rw-r--r--   0 twine    (17125) twine    (17125)      113 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/generator/simple_with_projectfile/common.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)      816 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/generator/simple_with_projectfile/complex.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)     1369 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/generator/simple_with_projectfile/expected_output
+-rw-r--r--   0 twine    (17125) twine    (17125)      253 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/generator/simple_with_projectfile/project.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.317197 distgen-1.9/tests/unittests/fixtures/load_config/
+-rw-r--r--   0 twine    (17125) twine    (17125)       36 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/load_config/level2.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       38 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/load_config/level3.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       26 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/load_config/simple.yaml
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-01-26 12:55:50.317197 distgen-1.9/tests/unittests/fixtures/multispec/
+-rw-r--r--   0 twine    (17125) twine    (17125)     1090 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/multispec/complex.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)       89 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/fixtures/multispec/simplest.yaml
+-rw-r--r--   0 twine    (17125) twine    (17125)     2288 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/test_commands.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1063 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/test_config.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1018 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/test_distro_detection.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      315 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/test_error.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     3025 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/test_generator.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     7462 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/test_multispec.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     2264 2021-02-19 08:47:04.000000 distgen-1.9/tests/unittests/test_pathmanager.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `distgen-1.8/docs/spec_expansion.rst` & `distgen-1.9/docs/spec_expansion.rst`

 * *Files identical despite different names*

### Comparing `distgen-1.8/docs/intro.rst` & `distgen-1.9/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `distgen-1.8/docs/config.rst` & `distgen-1.9/docs/config.rst`

 * *Files identical despite different names*

### Comparing `distgen-1.8/docs/Makefile` & `distgen-1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `distgen-1.8/docs/conf.py` & `distgen-1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/docs/spec_multispec.rst` & `distgen-1.9/docs/spec_multispec.rst`

 * *Files identical despite different names*

### Comparing `distgen-1.8/docs/usage.rst` & `distgen-1.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `distgen-1.8/docs/index.rst` & `distgen-1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `distgen-1.8/docs/builtins.rst` & `distgen-1.9/docs/builtins.rst`

 * *Files identical despite different names*

### Comparing `distgen-1.8/docs/macros.rst` & `distgen-1.9/docs/macros.rst`

 * *Files identical despite different names*

### Comparing `distgen-1.8/README.md` & `distgen-1.9/README.md`

 * *Files identical despite different names*

### Comparing `distgen-1.8/Makefile` & `distgen-1.9/Makefile`

 * *Files identical despite different names*

### Comparing `distgen-1.8/distgen/pathmanager.py` & `distgen-1.9/distgen/pathmanager.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/distgen/templates/container/docker/parts.tpl` & `distgen-1.9/distgen/templates/container/docker/parts.tpl`

 * *Files identical despite different names*

### Comparing `distgen-1.8/distgen/project.py` & `distgen-1.9/distgen/project.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/distgen/multispec.py` & `distgen-1.9/distgen/multispec.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/distgen/generator.py` & `distgen-1.9/distgen/generator.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/distgen/config.py` & `distgen-1.9/distgen/config.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/distgen/commands.py` & `distgen-1.9/distgen/commands.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/bin/dg` & `distgen-1.9/bin/dg`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/unittests/test_examples.py` & `distgen-1.9/build_manpages/unittests/test_examples.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/examples/copr/copr_cli/build_config.py` & `distgen-1.9/build_manpages/examples/copr/copr_cli/build_config.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/examples/copr/copr_cli/util.py` & `distgen-1.9/build_manpages/examples/copr/copr_cli/util.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/examples/copr/copr_cli/main.py` & `distgen-1.9/build_manpages/examples/copr/copr_cli/main.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/examples/copr/setup.py` & `distgen-1.9/build_manpages/examples/copr/setup.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/examples/old_format/example.py` & `distgen-1.9/build_manpages/examples/old_format/example.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/examples/old_format/setup.py` & `distgen-1.9/build_manpages/examples/old_format/setup.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/examples/raw-description/setup.py` & `distgen-1.9/build_manpages/examples/raw-description/setup.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/build_manpages/build_manpages.py` & `distgen-1.9/build_manpages/build_manpages/build_manpages.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/build_manpages/build_manpage.py` & `distgen-1.9/build_manpages/build_manpages/build_manpage.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/build_manpages/build_manpages/manpage.py` & `distgen-1.9/build_manpages/build_manpages/manpage.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/distgen.egg-info/SOURCES.txt` & `distgen-1.9/distgen.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 distgen.egg-info/SOURCES.txt
 distgen.egg-info/dependency_links.txt
 distgen.egg-info/requires.txt
 distgen.egg-info/top_level.txt
 distgen/distconf/centos-6-x86_64.yaml
 distgen/distconf/centos-7-x86_64.yaml
 distgen/distconf/centos-8-x86_64.yaml
+distgen/distconf/centos-stream-9-x86_64.yaml
 distgen/distconf/fedora-20-i686.yaml
 distgen/distconf/fedora-20-x86_64.yaml
 distgen/distconf/fedora-21-i686.yaml
 distgen/distconf/fedora-21-x86_64.yaml
 distgen/distconf/fedora-22-i686.yaml
 distgen/distconf/fedora-22-x86_64.yaml
 distgen/distconf/fedora-23-i686.yaml
@@ -75,14 +76,18 @@
 distgen/distconf/fedora-32-x86_64.yaml
 distgen/distconf/fedora-33-i686.yaml
 distgen/distconf/fedora-33-x86_64.yaml
 distgen/distconf/fedora-34-i686.yaml
 distgen/distconf/fedora-34-x86_64.yaml
 distgen/distconf/fedora-35-i686.yaml
 distgen/distconf/fedora-35-x86_64.yaml
+distgen/distconf/fedora-36-i686.yaml
+distgen/distconf/fedora-36-x86_64.yaml
+distgen/distconf/fedora-37-i686.yaml
+distgen/distconf/fedora-37-x86_64.yaml
 distgen/distconf/fedora-rawhide-i686.yaml
 distgen/distconf/fedora-rawhide-x86_64.yaml
 distgen/distconf/rhel-7-x86_64.yaml
 distgen/distconf/rhel-7.2-x86_64.yaml
 distgen/distconf/rhel-7.3-x86_64.yaml
 distgen/distconf/rhel-8-x86_64.yaml
 distgen/distconf/lib/centos.yaml
```

### Comparing `distgen-1.8/LICENSE` & `distgen-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `distgen-1.8/setup.py` & `distgen-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/NEWS` & `distgen-1.9/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+New in 1.9:
+
+* Fixed detection of OS/RELEASE on Fedora 35+
+
+* Added Fedora 36 and 35 configuration
+
+* Added CentOS Stream 9 configuration
+
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 New in 1.8:
 
 * Spec file fix for FTBFS issue on Fedora.
 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 New in 1.7:
```

### Comparing `distgen-1.8/tests/minimal-dockerfile/test.exp` & `distgen-1.9/tests/minimal-dockerfile/test.exp`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/fixtures/generator/simple_with_projectfile/Dockerfile` & `distgen-1.9/tests/unittests/fixtures/generator/simple_with_projectfile/Dockerfile`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/fixtures/generator/simple_with_projectfile/expected_output` & `distgen-1.9/tests/unittests/fixtures/generator/simple_with_projectfile/expected_output`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/fixtures/generator/simple_with_projectfile/complex.yaml` & `distgen-1.9/tests/unittests/fixtures/generator/simple_with_projectfile/complex.yaml`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/fixtures/generator/simple/Dockerfile` & `distgen-1.9/tests/unittests/fixtures/generator/simple/Dockerfile`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/fixtures/generator/simple/expected_output` & `distgen-1.9/tests/unittests/fixtures/generator/simple/expected_output`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/fixtures/generator/simple/complex.yaml` & `distgen-1.9/tests/unittests/fixtures/generator/simple/complex.yaml`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/fixtures/multispec/complex.yaml` & `distgen-1.9/tests/unittests/fixtures/multispec/complex.yaml`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/test_pathmanager.py` & `distgen-1.9/tests/unittests/test_pathmanager.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/test_commands.py` & `distgen-1.9/tests/unittests/test_commands.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/test_distro_detection.py` & `distgen-1.9/tests/unittests/test_distro_detection.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/test_multispec.py` & `distgen-1.9/tests/unittests/test_multispec.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/test_generator.py` & `distgen-1.9/tests/unittests/test_generator.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/unittests/test_config.py` & `distgen-1.9/tests/unittests/test_config.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/macros/test.exp` & `distgen-1.9/tests/macros/test.exp`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/testsuite` & `distgen-1.9/tests/testsuite`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/docker-labels/project.py` & `distgen-1.9/tests/docker-labels/project.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/docker-labels/test.exp` & `distgen-1.9/tests/docker-labels/test.exp`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/dockerfile/project.py` & `distgen-1.9/tests/dockerfile/project.py`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/dockerfile/test.exp` & `distgen-1.9/tests/dockerfile/test.exp`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 === fedora-rawhide-x86_64 ===
 
 FROM registry.fedoraproject.org/fedora:rawhide
 MAINTAINER Pavel Raiskup <praiskup@redhat.com>
 
 ENV container="docker" \
     PGDATA="/var/lib/pgsql/data" \
-    TEST_VAR="build_for fedora-35-x86_64"
+    TEST_VAR="build_for fedora-37-x86_64"
 
 RUN dnf -y --setopt=tsflags=nodocs install postgresql-server \
     && dnf -y --setopt=tsflags=nodocs reinstall glibc-common \
     && dnf -y --setopt=tsflags=nodocs install fedpkg \
     && dnf -y --setopt=tsflags=nodocs clean all --enablerepo='*'
 
 ADD "./scripts/rh-cont-pg-initdb" \
```

### Comparing `distgen-1.8/tests/dockerfile/test.yaml` & `distgen-1.9/tests/dockerfile/test.yaml`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/macros-from/test.exp` & `distgen-1.9/tests/macros-from/test.exp`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/pkginstaller/test.tpl` & `distgen-1.9/tests/pkginstaller/test.tpl`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/pkginstaller/test.exp` & `distgen-1.9/tests/pkginstaller/test.exp`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/macros-short/test.exp` & `distgen-1.9/tests/macros-short/test.exp`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/multispec/test.tpl` & `distgen-1.9/tests/multispec/test.tpl`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/multispec/multispec.yaml` & `distgen-1.9/tests/multispec/multispec.yaml`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/multispec/test.exp` & `distgen-1.9/tests/multispec/test.exp`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/docker-entrypoint/test.exp` & `distgen-1.9/tests/docker-entrypoint/test.exp`

 * *Files identical despite different names*

### Comparing `distgen-1.8/tests/docker-entrypoint/test.yaml` & `distgen-1.9/tests/docker-entrypoint/test.yaml`

 * *Files identical despite different names*

