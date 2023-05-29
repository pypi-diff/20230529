# Comparing `tmp/pmcyg-3.0.tar.gz` & `tmp/pmcyg-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmcyg-3.0.tar", last modified: Mon Sep 28 15:07:41 2020, max compression
+gzip compressed data, was "pmcyg-3.2.0.tar", last modified: Mon May 29 12:17:02 2023, max compression
```

## Comparing `pmcyg-3.0.tar` & `pmcyg-3.2.0.tar`

### file list

```diff
@@ -1,17 +1,29 @@
-drwxr-x--x   0 richard   (1000) richard   (1000)        0 2020-09-28 15:07:41.000000 pmcyg-3.0/
--rw-r-----   0 richard   (1000) richard   (1000)      412 2019-04-23 07:52:23.000000 pmcyg-3.0/Authors.txt
--rw-r-----   0 richard   (1000) richard   (1000)     9068 2020-09-28 15:02:08.000000 pmcyg-3.0/ChangeLog.txt
--rw-r-----   0 richard   (1000) richard   (1000)    35068 2009-04-21 20:11:53.000000 pmcyg-3.0/LICENSE.txt
--rw-r-----   0 richard   (1000) richard   (1000)      907 2020-08-08 10:13:30.000000 pmcyg-3.0/Makefile
--rw-r-----   0 richard   (1000) richard   (1000)      808 2020-09-28 15:07:41.000000 pmcyg-3.0/PKG-INFO
--rw-r-----   0 richard   (1000) richard   (1000)     8817 2020-09-28 15:01:40.000000 pmcyg-3.0/README.md
--rw-r-----   0 richard   (1000) richard   (1000)     3636 2020-08-02 07:10:54.000000 pmcyg-3.0/example.pkgs
-drwxr-x--x   0 richard   (1000) richard   (1000)        0 2020-09-28 15:07:41.000000 pmcyg-3.0/pmcyg/
--rw-r-----   0 richard   (1000) richard   (1000)     1323 2020-08-08 10:13:30.000000 pmcyg-3.0/pmcyg/__init__.py
--rw-r-----   0 richard   (1000) richard   (1000)    59949 2020-08-08 10:13:30.000000 pmcyg-3.0/pmcyg/core.py
--rw-r-----   0 richard   (1000) richard   (1000)    25573 2020-09-27 07:48:06.000000 pmcyg-3.0/pmcyg/gui.py
--rw-r-----   0 richard   (1000) richard   (1000)    10180 2020-08-08 10:13:30.000000 pmcyg-3.0/pmcyg/gui_imgs.py
--rw-r-----   0 richard   (1000) richard   (1000)       95 2020-09-27 06:23:08.000000 pmcyg-3.0/pmcyg/version.py
--rw-r-----   0 richard   (1000) richard   (1000)     1632 2020-09-27 06:22:43.000000 pmcyg-3.0/setup.py
-drwxr-x--x   0 richard   (1000) richard   (1000)        0 2020-09-28 15:07:41.000000 pmcyg-3.0/test/
--rw-r-----   0 richard   (1000) richard   (1000)    24806 2020-09-27 08:48:47.000000 pmcyg-3.0/test/testPMCyg.py
+drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-05-29 12:17:02.773532 pmcyg-3.2.0/
+-rw-r-----   0 richard   (1000) richard   (1000)      487 2023-05-29 07:50:12.000000 pmcyg-3.2.0/Authors.txt
+-rw-r-----   0 richard   (1000) richard   (1000)     9812 2023-05-29 07:37:12.000000 pmcyg-3.2.0/ChangeLog.txt
+-rw-r-----   0 richard   (1000) richard   (1000)    35068 2009-04-21 20:11:53.000000 pmcyg-3.2.0/LICENSE.txt
+-rw-r-----   0 richard   (1000) richard   (1000)      118 2020-08-08 10:13:30.000000 pmcyg-3.2.0/MANIFEST.in
+-rw-r-----   0 richard   (1000) richard   (1000)      930 2023-05-28 18:11:57.000000 pmcyg-3.2.0/Makefile
+-rw-r-----   0 richard   (1000) richard   (1000)      812 2023-05-29 12:17:02.773532 pmcyg-3.2.0/PKG-INFO
+-rw-r-----   0 richard   (1000) richard   (1000)     8820 2023-05-29 07:55:20.000000 pmcyg-3.2.0/README.md
+-rw-r-----   0 richard   (1000) richard   (1000)     3650 2023-05-29 07:42:13.000000 pmcyg-3.2.0/example.pkgs
+drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-05-29 12:17:02.773532 pmcyg-3.2.0/pmcyg/
+-rw-r-----   0 richard   (1000) richard   (1000)      907 2021-10-03 15:31:33.000000 pmcyg-3.2.0/pmcyg/__init__.py
+-rw-r-----   0 richard   (1000) richard   (1000)      987 2021-10-09 09:35:05.000000 pmcyg-3.2.0/pmcyg/apptools.py
+-rw-r-----   0 richard   (1000) richard   (1000)     5645 2021-10-03 15:38:59.000000 pmcyg-3.2.0/pmcyg/command_line.py
+-rw-r-----   0 richard   (1000) richard   (1000)    60432 2023-05-29 07:29:06.000000 pmcyg-3.2.0/pmcyg/core.py
+-rw-r-----   0 richard   (1000) richard   (1000)    25575 2023-05-28 18:24:22.000000 pmcyg-3.2.0/pmcyg/gui.py
+-rw-r-----   0 richard   (1000) richard   (1000)    10180 2020-08-08 10:13:30.000000 pmcyg-3.2.0/pmcyg/gui_imgs.py
+-rw-r-----   0 richard   (1000) richard   (1000)       97 2023-05-29 04:48:48.000000 pmcyg-3.2.0/pmcyg/version.py
+drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-05-29 12:17:02.773532 pmcyg-3.2.0/pmcyg.egg-info/
+-rw-r-----   0 richard   (1000) richard   (1000)      812 2023-05-29 12:17:02.000000 pmcyg-3.2.0/pmcyg.egg-info/PKG-INFO
+-rw-r-----   0 richard   (1000) richard   (1000)      400 2023-05-29 12:17:02.000000 pmcyg-3.2.0/pmcyg.egg-info/SOURCES.txt
+-rw-r-----   0 richard   (1000) richard   (1000)        1 2023-05-29 12:17:02.000000 pmcyg-3.2.0/pmcyg.egg-info/dependency_links.txt
+-rw-r-----   0 richard   (1000) richard   (1000)       51 2023-05-29 12:17:02.000000 pmcyg-3.2.0/pmcyg.egg-info/entry_points.txt
+-rw-r-----   0 richard   (1000) richard   (1000)        6 2023-05-29 12:17:02.000000 pmcyg-3.2.0/pmcyg.egg-info/top_level.txt
+-rwxr-x--x   0 richard   (1000) richard   (1000)      854 2023-05-28 16:17:49.000000 pmcyg-3.2.0/pmcyg.py
+-rw-r-----   0 richard   (1000) richard   (1000)       90 2021-10-03 14:52:29.000000 pmcyg-3.2.0/pyproject.toml
+-rw-r-----   0 richard   (1000) richard   (1000)       38 2023-05-29 12:17:02.773532 pmcyg-3.2.0/setup.cfg
+-rw-r-----   0 richard   (1000) richard   (1000)     1392 2021-10-03 15:19:53.000000 pmcyg-3.2.0/setup.py
+drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-05-29 12:17:02.773532 pmcyg-3.2.0/test/
+-rw-r-----   0 richard   (1000) richard   (1000)    25827 2023-05-29 04:45:42.000000 pmcyg-3.2.0/test/testPMCyg.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pmcyg-3.0/ChangeLog.txt` & `pmcyg-3.2.0/ChangeLog.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,36 @@
 ## ChangeLog for 'pmcyg' - a tool for partial mirroring of Cygwin(TM) archives
 ## https://github.com/rwpenney/pmcyg
-## (C)Copyright 2009-2020, RW Penney
+## (C)Copyright 2009-2023, RW Penney
+
+29May23 **** pmcyg-3.2 released ****
+
+29May23
+    Fixed missing line-ending on output setup.ini
+    Added explicit text encodings on textfile read/write operations
+
+28May23
+    Fixed outdated assumptions about 'requires' field in setup.ini
+    Updated fallback list of Cygwin mirror sites
+    Updated various unit-tests to escape Python-2.7 and x86 constraints
+
+12Aug22
+    Updated fallback list of Cygwin mirror sites
+    Improved parsing of official 'mirrors.lst' to support 'noshow' flag
+
+09Oct21 **** pmcyg-3.1 released ****
+
+03Oct21
+    Moved main() into new command_line submodule, following setuptools idioms
+
+21Feb21
+    Added support for reading XZ-compressed package lists
+
+20Feb21
+    Migrated setup.py from distutils to setuptools
 
 28Sep20 **** pmcyg-3.0 released ****
 
 27Sep20
     Improved setup of default download directory to avoid system paths
 
 01Aug20
```

### Comparing `pmcyg-3.0/LICENSE.txt` & `pmcyg-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pmcyg-3.0/Makefile` & `pmcyg-3.2.0/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 DISTFILES = pmcyg.py $(shell ls pmcyg/*.py) example.pkgs \
 	Authors.txt ChangeLog.txt LICENSE.txt \
 	Makefile README.md MANIFEST.in setup.py update \
 	test/testPMCyg.py test/setup-awkward.ini $(shell ls test/tree-*)
 
 FQNAME = ${PKGNAME}-${VERSION}
 
-.PHONY:	install dist-gzip dist-zip dist-dir test clean
+.PHONY:	default install dist-gzip dist-zip dist-dir test clean
+
+default:	test
 
 install:	pmcyg.py
 	install -m 755 pmcyg.py ${PREFIX}/bin/pmcyg
 
 dist-gzip:	dist-dir
 	tar -zcf ${FQNAME}.tgz ./${FQNAME}
 	rm -rf ${FQNAME}
```

### Comparing `pmcyg-3.0/PKG-INFO` & `pmcyg-3.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: pmcyg
-Version: 3.0
+Version: 3.2.0
 Summary: Utility for creating offline Cygwin installers
 Home-page: https://github.com/rwpenney/pmcyg
 Author: RW Penney
 Author-email: rwpenney@users.sourceforge.net
 License: GPL v3
-Download-URL: https://github.com/rwpenney/pmcyg/archive/pmcyg-3.0.tar.gz
+Download-URL: https://github.com/rwpenney/pmcyg/archive/pmcyg-3.2.0.tar.gz
 Description: pmcyg is a tool for creating an offline Cygwin installer containing customized collections of packages. This avoids having to download the entirety of a Cygwin release, which might occupy many GB, instead allowing installers that can be as small as 40MB. pmcyg enables Cygwin installation from a self-contained CD/DVD image or USB-flash for use on systems without internet access.
 Keywords: Cygwin
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `pmcyg-3.0/README.md` & `pmcyg-3.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 **pmcyg** is a tool for creating customized collections of
 [Cygwin](https://www.cygwin.com) packages,
 intended to support construction of a portable self-contained CDROM or DVD
 that can be used as an offline Cygwin installer on computers that
 do not have network access to a Cygwin mirror site.
 
 pmcyg avoids having to download the entirety of a Cygwin release
-(about 5GB or more), and can create a minimal Cygwin installation within 40MB.
+(about 20GB or more), and can create a minimal Cygwin installation within 40MB.
 In general, pmcyg will take a user-supplied list of cygwin package names,
 work out which other packages they depend on, and only download those packages
 from a user-selected Cygwin mirror site.  It will then assemble a set of
 configuration files that allows the Cygwin installer to operate from
 the locally created repository.
 
 
 ## Licensing
 
 All files forming part of pmcyg are released under
 the GNU General Public License (v3) (see http://www.gnu.org/licenses)
-and are Copyright 2009-2020 RW Penney
+and are Copyright 2009-2023 RW Penney
 
 
 ## Installation
 
 To run pmcyg, you will need to have a recent version of
 [Python](https://www.python.org) installed
-(note that this must be Python-3.3 or later). This should be available
+(note that this should be Python-3.6 or later). This should be available
 by default on most GNU/Linux systems, or can be obtained from
 https://www.python.org
 
 In order to use pmcyg as a graphical (GUI) application, you will need
 the 'Tkinter' toolkit for Python. This is part of the default distribution of
 Python for Windows platforms, but may be part of a separate package
 (possibly called "python3-tk") on Unix/Linux systems.
```

### Comparing `pmcyg-3.0/example.pkgs` & `pmcyg-3.2.0/example.pkgs`

 * *Files 4% similar despite different names*

```diff
@@ -21,41 +21,41 @@
 cygwin-x-doc                    # Cygwin/X-specific documentation
 editrights                      # Alter Windows user rights and privileges from command line
 findutils                       # Utilities for finding files--find, xargs, locate, updatedb
 gzip                            # The GNU compression utility
 less                            # A file pager program, similar to more(1)
 login                           # Sign on to a system
 man-db                          # Man page viewer
-patch                           # Applies diff files
+patch                           # Utility for modifying/upgrading files
 perl                            # Perl programming language interpreter
 procps-ng                       # System and process monitoring utilities
 python2                         # Python 2 language interpreter
-sed                             # the GNU sed stream editor
+sed                             # the GNU stream editor
 tar                             # A GNU file archiving program
 tcsh                            # An enhanced version of csh, the C shell
 texinfo                         # GNU documentation formatter
 util-linux                      # Collection of basic system utilities
 unzip                           # Info-ZIP decompression utility
 zip                             # Info-ZIP compression utility
 
 #
 # Development packages:
 #
-autoconf                        # Wrapper scripts for autoconf commands
+autoconf                        # Wrapper script for autoconf commands
 automake                        # Wrapper for multiple versions of Automake
 gcc-core                        # GNU Compiler Collection (C, OpenMP)
 gcc-g++                         # GNU Compiler Collection (C++)
 gdb                             # The GNU Debugger
 git                             # Distributed version control system
 make                            # The GNU version of the 'make' utility
 
 #
 # Maths/Scientific packages:
 #
-gnuplot     [arch=x86,x86_64]   # A command-line driven interactive function plotting utility
+gnuplot-X11 [arch=x86,x86_64]   # A command-line driven interactive function plotting utility
 octave          [arch=x86]      # GNU Octave language for numerical computations
 python3-numpy   [arch=x86_64]
 
 #
 # X11 packages:
 #
 cygwin-x-doc                    # Cygwin/X-specific documentation
```

### Comparing `pmcyg-3.0/pmcyg/__init__.py` & `pmcyg-3.2.0/pmcyg/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,24 +15,9 @@
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __all__ = [ 'core', 'version' ]
 
 from .core import DEFAULT_INSTALLER_URL, GarbageConfirmer, \
                   HOST_IS_CYGWIN, PackageSet, PMbuilder
+from .apptools import ProcessPackageFiles
 from .version import PMCYG_VERSION
-
-
-def ProcessPackageFiles(builder, pkgfiles):
-    """Execute downloading and cleaning actions for a set of package-list files"""
-
-    pkgset = PackageSet(pkgfiles)
-
-    builder.BuildMirror(pkgset)
-    garbage = builder.GetGarbage()
-    confirmer = \
-        GarbageConfirmer(garbage, default=builder.GetOption('RemoveOutdated'))
-    confirmer.ActionResponse()
-
-    isofile = builder.GetOption('ISOfilename')
-    if isofile:
-        builder.BuildISO(isofile)
```

### Comparing `pmcyg-3.0/pmcyg/core.py` & `pmcyg-3.2.0/pmcyg/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Core downloading and package-list management tools for pmcyg
 """
 
-# (C)Copyright 2009-2020, RW Penney <rwpenney@users.sourceforge.net>
+# (C)Copyright 2009-2023, RW Penney <rwpenney@users.sourceforge.net>
 
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -14,48 +14,48 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
-import  bz2, codecs, hashlib, io, os, os.path, re, \
+import  bz2, codecs, hashlib, io, lzma, os, os.path, re, \
         string, subprocess, sys, threading, time, \
         urllib.request, urllib.parse, urllib.error, urllib.parse
 from .version import PMCYG_VERSION
 
 
 DEFAULT_CYGWIN_ARCH = 'x86_64'
-DEFAULT_INSTALLER_URL = 'http://cygwin.com/setup${_arch}.exe'
+DEFAULT_INSTALLER_URL = 'https://www.cygwin.com/setup${_arch}.exe'
 #DEFAULT_CYGWIN_MIRROR = 'ftp://cygwin.com/pub/cygwin/'
-DEFAULT_CYGWIN_MIRROR = 'http://www.mirrorservice.org/sites/sourceware.org/pub/cygwin'
-CYGWIN_MIRROR_LIST_URL = 'http://cygwin.com/mirrors.lst'
+DEFAULT_CYGWIN_MIRROR = 'https://www.mirrorservice.org/sites/sourceware.org/pub/cygwin'
+CYGWIN_MIRROR_LIST_URL = 'https://www.cygwin.com/mirrors.lst'
 
 # Character encoding used by the setup.ini file.
 # This should probably by 'ascii', but occasional unicode characters
 # have been observed within official set.ini files.
 SI_TEXT_ENCODING = 'utf-8'
 
 HOST_IS_CYGWIN = (sys.platform == 'cygwin')
 
 
-def ConcatShortDescription(desc):
+def ConcatShortDescription(desc: str) -> str:
     """Concatenate multi-line short package description into single line"""
     if desc:
         return desc.replace('\n', ' ').replace('\r', '').rstrip()
         # s.replace is more portable between python-2.x & 3.x than s.translate
     else:
         return '???'
         # A null or empty short-description shouldn't go unnoticed
 
 
 class PMCygException(Exception):
     """Wrapper for internally generated exceptions"""
 
-    def __init__(self, *args):
+    def __init__(self, *args) -> None:
         Exception.__init__(self, *args)
 
 
 class BuildViewer:
     """Conduit for status messages from PMbuilder and related classes,
     roughly corresponding to the Observer pattern."""
     SEV_mask =      0x0f        # Severity levels
@@ -65,53 +65,53 @@
     SEV_ERROR =     0x03          # Disastrous news
 
     VRB_mask =      0xf0        # Verbosity levels
     VRB_LOW =       0x00          # Essential messages
     VRB_MEDIUM =    0x10          # Informative messages
     VRB_HIGH =      0x20          # Debugging messages
 
-    def __init__(self, verbosity=VRB_MEDIUM):
+    def __init__(self, verbosity: int=VRB_MEDIUM) -> None:
         self._operation = None
         self._verbThresh = verbosity
 
-    def __call__(self, text, ctrl=SEV_NORMAL | VRB_MEDIUM):
+    def __call__(self, text: str, ctrl: int=SEV_NORMAL | VRB_MEDIUM) -> None:
         self.message(text, ctrl)
 
-    def message(self, text, ctrl=SEV_NORMAL | VRB_MEDIUM):
+    def message(self, text: str, ctrl: int=SEV_NORMAL | VRB_MEDIUM) -> None:
         if self._operation:
             self._emit('  >>>\n', self._operation[1])
         self._emit('{0}\n'.format(text), ctrl)
         if self._operation:
             self._emit('  >>> {0}...'.format(self._operation[0]),
                        self._operation[1])
 
-    def startOperation(self, text, ctrl=VRB_MEDIUM):
+    def startOperation(self, text: str, ctrl: int=VRB_MEDIUM) -> None:
         self._operation = (text, ((ctrl & self.VRB_mask) | self.SEV_NORMAL))
         self._emit('{0}...'.format(text), self.SEV_NORMAL)
 
-    def endOperation(self, text, ctrl=SEV_NORMAL):
+    def endOperation(self, text: str, ctrl: int=SEV_NORMAL) -> None:
         if not self._operation:
             return
         opVerbosity = (self._operation[1] & self.VRB_mask)
         self._emit(' {0}\n'.format(text),
                    ((ctrl & self.SEV_mask) | opVerbosity))
         self._operation = None
 
-    def flushOperation(self):
+    def flushOperation(self) -> None:
         if not self._operation:
             return
         self._emit('\n', (self._operation[1] & self.VRB_mask))
         self._operation = None
 
-    def _emit(self, text, ctrl):
+    def _emit(self, text: str, ctrl: int) -> None:
         if (ctrl & self.VRB_mask) > self._verbThresh:
             return
         self._output(text, (ctrl & self.SEV_mask))
 
-    def _output(self, text, severity): pass
+    def _output(self, text: str, severity: int): pass
 
 
 class SilentBuildViewer(BuildViewer):
     def __init__(self):
         BuildViewer.__init__(self)
 
     def _output(self, text, severity): pass
@@ -130,42 +130,42 @@
         stream.write(text)
         stream.flush()
 
 
 
 class BuildReporter:
     """Mixin class for hosting a BuildViewer object."""
-    def __init__(self, Viewer=None, Peer=None):
+    def __init__(self, Viewer: BuildViewer=None, Peer=None) -> None:
         self._statview = None
         if isinstance(Peer, BuildReporter) and not Viewer:
             Viewer = Peer._statview
         BuildReporter.SetViewer(self, Viewer)
 
     def SetViewer(self, Viewer):
         if not Viewer:
             Viewer = ConsoleBuildViewer()
         self._statview = Viewer
 
 
 
 class SetupIniFetcher:
-    """Facade for fetching setup.ini from URL,
-    with optional bz2-decompression"""
-    MaxIniFileLength = 1 << 24
+    """Facade for fetching setup.ini from URL, with optional decompression"""
+    MaxIniFileLength = 1 << 26
+
+    Decompressors = { 'bz2':    bz2.decompress,
+                      'xz':     lzma.decompress }
 
     def __init__(self, URL):
         self._buffer = None
+        suffix = URL.rsplit('.', 1)[-1]
+        expander = self.Decompressors.get(suffix, (lambda x: x))
         with urllib.request.urlopen(URL) as stream:
-            expander = lambda x: x
-            if URL.endswith('.bz2'):
-                expander = bz2.decompress
             rawfile = expander(stream.read(self.MaxIniFileLength))
 
-        self._buffer = io.StringIO(rawfile.decode(SI_TEXT_ENCODING,
-                                                        'ignore'))
+        self._buffer = io.StringIO(rawfile.decode(SI_TEXT_ENCODING, 'ignore'))
 
     def __del__(self):
         if self._buffer:
             self._buffer.close()
 
     def __iter__(self):
         return self
@@ -181,15 +181,15 @@
 class HashChecker:
     """Mechanism for checking md5/sha512 hash-code of downloaded packages.
 
     This includes heuristics for guessing a suitable hashing algorithm
     based on the length of a supplied hexadecimal hash code.
     """
 
-    len2alg = {}
+    len2alg: dict = {}
 
     def __call__(self, path, tgthash, blksize=1<<14):
         hasher = self._guessHashAlg(tgthash)
 
         try:
             with open(path, 'rb') as fp:
                 while True:
@@ -232,18 +232,18 @@
     of Cygwin(TM) distribution"""
     DL_Success =        1
     DL_AlreadyPresent = 2
     DL_SizeError =      3
     DL_HashError =      4
     DL_Failure =        5
 
-    def __init__(self, BuildDirectory='.',
-                MirrorSite=DEFAULT_CYGWIN_MIRROR,
-                CygwinInstaller=DEFAULT_INSTALLER_URL,
-                Viewer=None, **kwargs):
+    def __init__(self, BuildDirectory: str='.',
+                MirrorSite: str=DEFAULT_CYGWIN_MIRROR,
+                CygwinInstaller: str=DEFAULT_INSTALLER_URL,
+                Viewer: BuildViewer=None, **kwargs) -> None:
 
         BuildReporter.__init__(self, Viewer)
         self._hashCheck = HashChecker()
 
         # Directory into which to assemble local mirror:
         self._tgtdir = BuildDirectory
 
@@ -274,102 +274,101 @@
             'MakeAutorun':      False,
             'IncludeSources':   False,
             'RemoveOutdated':   'no',
             'ISOfilename':      None
         }
 
         self._fetchStats = FetchStats()
-        self._cygcheck_list = []
+        self._cygcheck_list: list = []
         for (opt, val) in kwargs.items():
             self.SetOption(opt, val)
 
-    def SetViewer(self, Viewer):
+    def SetViewer(self, Viewer: BuildViewer):
         BuildReporter.SetViewer(self, Viewer)
         self._masterList.SetViewer(self._statview)
         self._pkgProc.SetViewer(self._statview)
         self._garbage.SetViewer(self._statview)
 
-    def GetTargetDir(self):
+    def GetTargetDir(self) -> str:
         return self._tgtdir
 
-    def SetTargetDir(self, tgtdir):
+    def SetTargetDir(self, tgtdir: str) -> None:
         """Set the root directory beneath which packages will be downloaded"""
         self._tgtdir = tgtdir
 
     @property
-    def setup_exe_url(self):
+    def setup_exe_url(self) -> str:
         """The URL of the setup.exe Cygwin installer"""
         keywords = { 'arch': self._cygarch,
                      '_arch': '-' + self._cygarch }
         exe_expr = self._exeurl
         if not exe_expr:
             exe_expr = DEFAULT_INSTALLER_URL
         exe_template = string.Template(exe_expr)
         return exe_template.substitute(keywords)
 
     @setup_exe_url.setter
-    def setup_exe_url(self, URL):
+    def setup_exe_url(self, URL: str) -> None:
         self._exeurl = URL
 
     @property
-    def mirror_url(self):
+    def mirror_url(self) -> str:
         """The URL of the mirror site from which to download Cygwin packages"""
         return self._mirror
 
     @mirror_url.setter
-    def mirror_url(self, URL):
+    def mirror_url(self, URL: str) -> None:
         if not URL.endswith('/'):
             URL += '/'
         self._mirror = URL
 
     @property
-    def setup_ini_url(self):
+    def setup_ini_url(self) -> str:
         """The (architecture-dependent) URL for the setup.ini package-list."""
         if self._iniurl:
             # Use prescribed URL directly:
             return self._iniurl
         else:
             # Base URL on chosen mirror site, and selected architecture:
             if self._cygarch:
-                basename = '{0}/setup.bz2'.format(self._cygarch)
+                basename = '{0}/setup.xz'.format(self._cygarch)
             else:
-                basename = 'setup.bz2'
+                basename = 'setup.xz'
             return urllib.parse.urljoin(self._mirror, basename)
 
     @setup_ini_url.setter
-    def setup_ini_url(self, URL):
+    def setup_ini_url(self, URL: str) -> None:
         self._iniurl = URL
         self._masterList.SetSourceURL(self.setup_ini_url)
 
-    def GetArch(self):
+    def GetArch(self) -> str:
         return self._cygarch
 
-    def SetArch(self, arch):
+    def SetArch(self, arch: str) -> None:
         self._cygarch = arch
 
-    def GetEpochs(self):
+    def GetEpochs(self) -> list:
         return self._epochs
 
-    def SetEpochs(self, epochs):
+    def SetEpochs(self, epochs: list) -> None:
         self._epochs = epochs
 
-    def GetOption(self, optname):
+    def GetOption(self, optname: str):
         return self._optiondict.get(optname)
 
-    def SetOption(self, optname, value):
+    def SetOption(self, optname: str, value):
         oldval = None
         try:
             oldval = self._optiondict[optname]
             self._optiondict[optname] = value
         except:
             raise PMCygException('Invalid configuration option "{0}"' \
                                     ' for PMbuilder'.format(optname))
         return oldval
 
-
     def ReadMirrorList(self, reload=False):
         """Construct list of Cygwin mirror sites"""
 
         if self._mirrordict and not reload:
             return self._mirrordict
 
         self._mirrordict = {}
@@ -381,15 +380,22 @@
                            ' from {0}'.format(CYGWIN_MIRROR_LIST_URL),
                            BuildViewer.SEV_WARNING)
             fp = self._makeFallbackMirrorList()
 
         for line in fp:
             line = line.decode('ascii', 'ignore').strip()
             if not line: continue
-            (url, ident, region, country) = line.split(';')
+
+            fields = line.split(';')
+            n_fields = len(fields)
+            if n_fields < 4 or (n_fields > 4 and fields[4] == 'noshow'):
+                continue
+            else:
+                (url, ident, region, country) = fields[:4]
+
             regdict = self._mirrordict.setdefault(region, {})
             regdict.setdefault(country, []).append((ident, url))
 
         fp.close()
         return self._mirrordict
 
 
@@ -427,15 +433,15 @@
 
 
     def UpdatePackageLists(self, filenames, bckp=".orig"):
         self._masterList.SetSourceURL(self.setup_ini_url)
         self._pkgProc.UpdatePackageLists(filenames, bckp)
 
 
-    def BuildMirror(self, pkgset):
+    def BuildMirror(self, pkgset) -> None:
         """Download and configure packages into local directory
 
         Resolved the dependencies of the supplied PackageSet,
         and trigger downloading of all Cygwin packages
         together with installer artefacts."""
 
         self._cancelling = False
@@ -486,15 +492,16 @@
         else:
             return self._garbage
 
     def Cancel(self, flag=True):
         """Signal that downloading should be terminated"""
         self._cancelling = flag
 
-    def TemplateFromLists(self, outfile, pkgfiles, cygwinReplica=False):
+    def TemplateFromLists(self, outfile: str, pkgfiles: list,
+                          cygwinReplica: bool=False) -> None:
         """Wrapper for PkgSetProcessor.MakeTemplate(),
         taking collection of package files"""
         self._masterList.SetSourceURL(self.setup_ini_url)
 
         pkgset = PackageSet(pkgfiles)
         if cygwinReplica:
             pkgset.extend(self.ListInstalled())
@@ -504,25 +511,21 @@
 
     @staticmethod
     def _makeFallbackMirrorList():
         """Supply a static list of official Cygwin mirror sites,
         as a fall-back in case the live listing of mirrors cannot
         be downloaded."""
         return io.BytesIO(b'''
-ftp://ucmirror.canterbury.ac.nz/pub/cygwin/;ucmirror.canterbury.ac.nz;Australasia;New Zealand
 http://ucmirror.canterbury.ac.nz/cygwin/;ucmirror.canterbury.ac.nz;Australasia;New Zealand
-ftp://mirror.csclub.uwaterloo.ca/cygwin/;mirror.csclub.uwaterloo.ca;Canada;Ontario
-http://mirror.csclub.uwaterloo.ca/cygwin/;mirror.csclub.uwaterloo.ca;Canada;Ontario
-ftp://ftp.fsn.hu/pub/cygwin/;ftp.fsn.hu;Europe;Hungary
-ftp://ftp.iij.ad.jp/pub/cygwin/;ftp.iij.ad.jp;Asia;Japan
-http://ftp.iij.ad.jp/pub/cygwin/;ftp.iij.ad.jp;Asia;Japan
-ftp://cygwin.osuosl.org/pub/cygwin/;cygwin.osuosl.org;United States;Oregon
-http://cygwin.osuosl.org/;cygwin.osuosl.org;United States;Oregon
-http://mirrors.dotsrc.org/cygwin/;mirrors.dotsrc.org;Europe;Denmark
-http://www.mirrorservice.org/sites/sourceware.org/pub/cygwin/;www.mirrorservice.org;Europe;UK
+https://mirror.csclub.uwaterloo.ca/cygwin/;mirror.csclub.uwaterloo.ca;North America;Canada
+https://ftp.fsn.hu/pub/cygwin/;ftp.fsn.hu;Europe;Hungary
+https://ftp.iij.ad.jp/pub/cygwin/;ftp.iij.ad.jp;Asia;Japan
+https://cygwin.osuosl.org/;cygwin.osuosl.org;North America;United States
+https://mirrors.dotsrc.org/cygwin/;mirrors.dotsrc.org;Europe;Denmark
+https://www.mirrorservice.org/sites/sourceware.org/pub/cygwin/;www.mirrorservice.org;Europe;UK
                 ''')
 
     def _resolveDependencies(self, usrpkgs=None):
         """Constuct list of packages, including all their dependencies"""
 
         selected = self._extendPkgSelection(usrpkgs)
         return self._pkgProc.ExpandDependencies(selected, self._epochs)
@@ -617,15 +620,15 @@
         packages.sort()
         spkgs.sort()
         packages.extend(spkgs)
 
         # Reconstruct setup.ini file:
         spath = os.path.join(archdir, inibase)
         hashfiles.append(inibase)
-        with codecs.open(spath, 'w', SI_TEXT_ENCODING) as fp:
+        with codecs.open(spath, 'w', encoding=SI_TEXT_ENCODING) as fp:
             now = time.localtime()
             msgs = [
                     '# This file was automatically generated by' \
                         ' "pmcyg" (version {0}),'.format(PMCYG_VERSION),
                     '# {0},'.format(time.asctime(now)),
                     '# based on {0}'.format(self.setup_ini_url),
                     '# Manual edits may be overwritten',
@@ -635,14 +638,15 @@
                     'setup-version: {0}'.format(header['setup-version']),
                     ''
             ]
             fp.write('\n'.join(msgs))
             for pkg in packages:
                 fp.write('\n')
                 fp.write(pkgdict[pkg].GetAny('TEXT'))
+            fp.write('\n')
         with open(spath, 'rb') as fp:
             hashfiles.append(inibz2)
             cpsr = bz2.BZ2File(os.path.join(archdir, inibz2), mode='w')
             cpsr.write(fp.read())
             cpsr.close()
 
         # Create copy of Cygwin installer program:
@@ -663,15 +667,15 @@
             with open(apath, 'w+b') as fp:
                 fp.write(bytes('[autorun]\r\nopen=' + exebase
                                 +' --local-install\r\n', 'ascii'))
 
         # Generate message-digest of top-level files:
         for algo in ["md5", "sha256", "sha512"]:
             sumfile = os.path.join(archdir, '{0}.sum'.format(algo))
-            with open(sumfile, 'wt') as hp:
+            with open(sumfile, 'wt', encoding='utf-8') as hp:
                 for fl in hashfiles:
                     hshr = hashlib.new(algo)
                     with open(os.path.join(archdir, fl), 'rb') as fp:
                         hshr.update(fp.read())
                     hp.write('{0}  {1}\n'.format(hshr.hexdigest(), fl))
 
     def _doDummyDownloading(self, downloads):
@@ -986,15 +990,15 @@
                             BuildViewer.SEV_ERROR)
             raise PMCygException('Invalid package names {{ {p} }}[{n}]'
                                  ' in ExpandDependencies()'
                                  .format(n=nBad, p=', '.join(truncbad)))
         if badrequires:
             links = [ '{0}->{1}'.format(pkg, dep)
                         for (pkg, dep) in badrequires ]
-            self._statview('Master package list contains spurious'
+            self._statview('Master package list contains unresolvable'
                            ' dependencies: {0}'.format(', '.join(links)),
                            BuildViewer.SEV_WARNING)
 
         packages = list(packages)
         packages.sort()
 
         return packages
@@ -1066,20 +1070,20 @@
         for cat in catlist:
             if terse and not set(catgroups[cat]).intersection(userpkgs):
                 continue
 
             print('\n\n##\n## {0:s}\n##'.format(cat), file=stream)
 
             for pkg in catgroups[cat]:
-                desc = ConcatShortDescription(pkgdict[pkg].GetAny('sdesc'))
                 if pkgset and pkg in pkgset:
                     prefix = ('', ' ')
                 else:
                     if terse: continue
                     prefix = ('#', '')
+                desc = ConcatShortDescription(pkgdict[pkg].GetAny('sdesc'))
                 stream.write('{0:s}{1:<28s}   {2:s}# {3:s}\n' \
                                 .format(prefix[0], pkg, prefix[1], desc))
 
     def UpdatePackageLists(self, filenames, bckp=".orig"):
         """Rewrite a set of package lists, updating package-descriptions.
         The layout of the supplied files is assumed to be the same
         as that generated by MakeTemplate()."""
@@ -1141,20 +1145,22 @@
 class MasterPackageList(BuildReporter):
     """Database of available Cygwin packages built from 'setup.ini' file"""
 
     RE_DBline = re.compile(r'''
           ((?P<relinfo>^(release|arch|setup-\S+)) :
                                 \s+ (?P<relParam>\S+) $)
         | (?P<comment>\# .* $)
-        | (?P<package>^@ \s+ (?P<pkgName>\S+) $)
+        | (?P<package>^@ \s+ (?P<pkgName> \S+) $)
         | (?P<epoch>^\[ (?P<epochName>[a-z]+) \] $)
-        | ((?P<field>^[a-zA-Z][-a-zA-Z0-9]+) : \s+ (?P<fieldVal>.*) $)
+        | ((?P<field>^[a-zA-Z][-a-zA-Z0-9]+) : \s+ (?P<fieldVal> .*) $)
         | (?P<blank>^\s* $)
         ''', re.VERBOSE)
 
+    RE_RSTRIP = re.compile(r'\s+$')
+
     def __init__(self, iniURL=None, Viewer=None):
         BuildReporter.__init__(self, Viewer)
 
         self._pkgLock = threading.Lock()
         self._iniURL = None
         self.ClearCache()
         self.SetSourceURL(iniURL)
@@ -1327,18 +1333,15 @@
 
     def _finalizePackage(self):
         """Final assembly of text & field records describing single package"""
 
         if not self._pkgname:
             return
 
-        pkgtxt = self._pkgtxt
-        while pkgtxt and pkgtxt[-1].isspace():
-            pkgtxt.pop()
-        self._pkgdict.Set('TEXT', "".join(pkgtxt))
+        self._pkgdict.Set('TEXT', self.RE_RSTRIP.sub('', ''.join(self._pkgtxt)))
         self._ini_packages[self._pkgname] = self._pkgdict
 
         self._pkgname = None
         self._pkgtxt = []
         self._pkgdict = PackageSummary()
 
 
@@ -1398,17 +1401,21 @@
         """Determine whether the package depends on any other packages."""
         if self.GetAny('depends2') or self.GetAny('requires'):
             return True
         return False
 
     def GetDependencies(self, epochset=[]):
         """Return a list of other packages on which this package depends."""
-        return sorted(
-            { x.strip() for x in self.GetAny('depends2', epochset).split(',') }
-            | set(self.GetAny('requires', epochset).split()) )
+        all_deps = []
+        deps, reqs = ( self.GetAny(f) for f in ('depends2', 'requires') )
+        if deps:
+            all_deps.extend(x.strip() for x in deps.split(','))
+        if reqs:
+            all_deps.extend(x.split())
+        return sorted(set(all_deps))
 
     def Set(self, field, value, epoch=None):
         """Record field=value for a particular epoch (e.g. curr/prev/None)"""
         self._pkginfo[(field, epoch)] = value
         self._epochs.add(epoch)
```

### Comparing `pmcyg-3.0/pmcyg/gui.py` & `pmcyg-3.2.0/pmcyg/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         self._renewMirrorMenu = False
         self.mirrorthread = GUImirrorThread(self)
         self.mirrorthread.setDaemon(True)
         self.mirrorthread.start()
 
         def tick():
             # Check if list of mirror sites is available yet:
-            if self._renewMirrorMenu and not self.mirrorthread.isAlive():
+            if self._renewMirrorMenu and not self.mirrorthread.is_alive():
                 self.mirror_menu = self.mkMirrorMenu()
                 self.mirror_btn.config(menu=self.mirror_menu)
                 self.mirror_btn.config(state=Tk.NORMAL)
                 self._renewMirrorMenu = False
 
             try:
                 newstate = self._state.tick()
@@ -301,15 +301,15 @@
             win.title('About pmcyg')
             msg = Tk.Message(win, name='pmcyg_about', justify=Tk.CENTER,
                         aspect=300, border=2, relief=Tk.GROOVE, text= \
 """pmcyg
 - a tool for creating Cygwin\N{REGISTERED SIGN} partial mirrors
 Version {0:s}
 
-\N{COPYRIGHT SIGN}Copyright 2009-2020 RW Penney
+\N{COPYRIGHT SIGN}Copyright 2009-2023 RW Penney
 
 This program comes with ABSOLUTELY NO WARRANTY.
 This is free software, and you are welcome to redistribute it under
 the terms of the GNU General Public License (v3).""".format(PMCYG_VERSION))
             msg.pack(side=Tk.TOP, fill=Tk.X, padx=2, pady=2)
             self._aboutwin = win
         else:
@@ -470,15 +470,15 @@
     """Representation of the package-download state of the GUI."""
     def __init__(self, parent):
         GUIstate.__init__(self, parent)
         self._buildthread = None
 
     def tick(self):
         self._parent.updateProgress()
-        if self._buildthread and not self._buildthread.isAlive():
+        if self._buildthread and not self._buildthread.is_alive():
             return GUItidyState(self._parent)
         return self
 
     def enter(self):
         buildthread = GUIfetchThread(self._parent)
         buildthread.setDaemon(True)
         buildthread.start()
```

### Comparing `pmcyg-3.0/pmcyg/gui_imgs.py` & `pmcyg-3.2.0/pmcyg/gui_imgs.py`

 * *Files identical despite different names*

### Comparing `pmcyg-3.0/setup.py` & `pmcyg-3.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 #!/usr/bin/python3
 # Installation/setup script for Simple Python Fixed-Point Module
 # RW Penney, July 2010
 
-from distutils.core import setup
-import distutils.command.build_scripts as DIB
+from setuptools import setup
 import os, re, shutil
 from pmcyg.version import PMCYG_VERSION
 
 
-if os.name == 'posix':
-    if not os.path.exists('build/scripts'):
-        os.makedirs('build/scripts')
-    shutil.copyfile('pmcyg.py', 'build/scripts/pmcyg')
-    pmcyg_scripts = [ 'build/scripts/pmcyg' ]
-else:
-    pmcyg_scripts = [ 'pmcyg.py' ]
-
-
 setup(
     author = 'RW Penney',
     author_email = 'rwpenney@users.sourceforge.net',
     description = 'Utility for creating offline Cygwin installers',
     fullname = 'pmcyg - Cygwin partial mirror',
     keywords = 'Cygwin',
     license = 'GPL v3',
@@ -35,11 +25,12 @@
         'without internet access.',
     name = 'pmcyg',
     url = 'https://github.com/rwpenney/pmcyg',
     download_url = 'https://github.com/rwpenney/pmcyg/archive/pmcyg-' \
                 + PMCYG_VERSION + '.tar.gz',
     version = PMCYG_VERSION,
     packages = [ 'pmcyg' ],
-    scripts = pmcyg_scripts,
+    entry_points = {
+        'console_scripts': [ 'pmcyg=pmcyg.command_line:main' ] },
     classifiers = [ 'Programming Language :: Python :: 3',
                     'Topic :: Utilities' ]
 )
```

### Comparing `pmcyg-3.0/test/testPMCyg.py` & `pmcyg-3.2.0/test/testPMCyg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/python3
 # Unit-tests for Cygwin Partial Mirror (pmcyg)
 # RW Penney, August 2009
 
 import codecs, os, random, re, string, io, sys, \
-        tempfile, unittest, urllib.parse
+       tempfile, unittest, urllib.parse
 sys.path.insert(0, '..')
 from pmcyg.core import *
 
 
-def getSetupURL():
-    if os.path.isfile('setup.ini'):
-        cwd = os.getcwd()
-        urlprefix = 'file://' + cwd.replace('\\', '/') + '/'
-        return urllib.parse.urljoin(urlprefix, 'setup.ini')
-    else:
-        return 'http://www.mirrorservice.org/sites/sourceware.org/pub/cygwin/x86/setup.ini'
+TESTDIR = os.path.dirname(os.path.abspath(__file__))
+
 
+def getSetupURL():
+    urlprefix = 'file://' + TESTDIR.replace('\\', '/') + '/'
+    for suffix in ('xz', 'bz2', 'ini'):
+        fname = 'setup.' + suffix
+        if os.path.isfile(fname):
+            return urllib.parse.urljoin(urlprefix, fname)
+    return 'http://www.mirrorservice.org/sites/sourceware.org/pub/cygwin/x86_64/setup.xz'
 
 
 class testSetupIniFetcher(unittest.TestCase):
     """Test for opening of optionally compressed setup.ini via URL"""
     def setUp(self):
         self._tmpdir = tempfile.TemporaryDirectory()
 
@@ -109,21 +111,21 @@
 
     def testIngestion(self):
         (header, packages) = self.pkglist.GetHeaderAndPackages()
 
         self.assertFalse(header.get('setup-version') == None)
         try:
             ts = int(header['setup-timestamp'])
-            self.assertTrue(ts > (1 << 30))
-            self.assertTrue(ts < (1 << 31))
+            self.assertGreater(ts, (1 << 30))
+            self.assertLess(ts, (1 << 31))
         except:
             self.fail()
 
         self.assertFalse(packages == None)
-        self.assertTrue(len(packages) >= 1000)
+        self.assertGreaterEqual(len(packages), 1000)
 
     def testFieldPresence(self):
         fields = [ ('sdesc', 'curr'), ('category', None),
                     ('version', 'curr'), ('install', 'curr'),
                     ('source', 'curr'), ('install', 'prev') ]
         scores = {}
         for field in fields:
@@ -137,20 +139,20 @@
             for (field, epoch) in fields:
                 try:
                     fieldval = pkgdict.GetAny(field, [epoch])
                     scores[(field, epoch)] += 1
                 except:
                     pass
 
-        self.assertTrue(scores[('sdesc', 'curr')] == numpkgs)
-        self.assertTrue(scores[('category', None)] == numpkgs)
-        self.assertTrue(scores[('version', 'curr')] >= 0.8 * numpkgs)
-        self.assertTrue(scores[('install', 'curr')] >= 0.8 * numpkgs)
-        self.assertTrue(scores[('source', 'curr')] >= 0.75 * numpkgs)
-        self.assertTrue(scores[('install', 'prev')] >= 0.3 * numpkgs)
+        self.assertEqual(scores[('sdesc', 'curr')], numpkgs)
+        self.assertEqual(scores[('category', None)], numpkgs)
+        self.assertGreaterEqual(scores[('version', 'curr')], 0.8 * numpkgs)
+        self.assertGreaterEqual(scores[('install', 'curr')], 0.8 * numpkgs)
+        self.assertGreaterEqual(scores[('source', 'curr')], 0.75 * numpkgs)
+        self.assertGreaterEqual(scores[('install', 'prev')], 0.3 * numpkgs)
 
     def testLongDescriptions(self):
         (header, packages) = self.pkglist.GetHeaderAndPackages()
 
         numpkgs = 0
         numldesc = 0
         totlines = 0
@@ -166,18 +168,18 @@
             desclen = len(lines)
             totlines += desclen
             blanks = 0
             for line in lines:
                 if not line.strip():
                     blanks += 1
 
-            self.assertFalse(blanks > (desclen + 2) / 3)
+            self.assertLessEqual(blanks, (desclen + 2) / 3)
 
-        self.assertTrue(numldesc >= 0.7 * numpkgs)
-        self.assertTrue(totlines > 2 * numldesc)
+        self.assertGreaterEqual(numldesc, 0.7 * numpkgs)
+        self.assertGreater(totlines, 2 * numldesc)
 
     def testCategories(self):
         packages = self.pkglist.GetPackageDict()
         categories = self.pkglist.GetCategories()
 
         if not categories.get('All'):
             self.fail()
@@ -193,36 +195,45 @@
                     self.assertTrue(cat in cats)
             else:
                 self.assertEqual(len(members), len(packages))
 
                 for pkgname in members:
                     self.assertTrue(pkgname in iter(packages.keys()))
 
+    def testCoverage(self):
+        categories = set(self.pkglist.GetCategories().keys())
+        packages = set(self.pkglist.GetPackageDict().keys())
+
+        self.assertSetEqual({ 'Admin', 'Base', 'Devel', 'Math',
+                              'Python', 'X11' } - categories, set())
+        self.assertSetEqual({ 'aspell', 'bison', 'ed', 'lua', 'swig',
+                              'which', 'xlsfonts', 'zlib',
+                              'zsh' } - packages, set())
 
 
 class testPkgSetProcessor(unittest.TestCase):
     def setUp(self):
         self.masterList = MasterPackageList(Viewer=SilentBuildViewer())
         self.masterList.SetSourceURL(getSetupURL())
 
     def testExpand(self):
         pkgProc = PkgSetProcessor(self.masterList)
 
         explist = pkgProc.ExpandDependencies([])
         self.assertEqual(len(explist), 0)
 
         explist = pkgProc.ExpandDependencies(['make'])
-        self.assertTrue(len(explist) > 6)
-        self.checkSubset(explist, ['make', 'bash', 'coreutils', 'cygwin',
-                                    'libgcc1', 'terminfo'])
+        self.assertGreater(len(explist), 6)
+        self.checkSubset(explist, ['make', 'cygwin', 'libgcc1',
+                                   'libiconv2', 'terminfo'])
 
         explist = pkgProc.ExpandDependencies(['bash', 'libboost-devel', 'bvi'])
-        self.assertTrue(len(explist) > 20)
+        self.assertGreater(len(explist), 20)
         self.checkSubset(explist, ['bash', 'bvi', 'libboost-devel', 'cygwin',
-                                    'libattr1', 'libgcc1',
+                                    'libgcc1', 'libicu-devel',
                                     'libreadline7', 'pkg-config', 'terminfo'])
 
     def testInverse(self):
         """Check that contraction can be inverted by expansion"""
         pkgdict = self.masterList.GetPackageDict()
         pkglist = [p for p in pkgdict.keys()]
 
@@ -268,32 +279,32 @@
         f_bz2 = os.path.join(tgtdir, arch, 'setup.bz2')
         f_exe = os.path.join(tgtdir, 'setup-%s.exe' % arch)
 
         self.assertTrue(os.path.isfile(f_ini))
         self.assertTrue(os.path.isfile(f_bz2))
         self.assertTrue(os.path.isfile(f_exe))
 
-        self.assertTrue(os.path.getsize(f_ini) > (1 << 10))
-        self.assertTrue(os.path.getsize(f_bz2) > (1 << 9))
-        self.assertTrue(os.path.getsize(f_exe) > (1 << 18))
+        self.assertGreater(os.path.getsize(f_ini), (1 << 10))
+        self.assertGreater(os.path.getsize(f_bz2), (1 << 9))
+        self.assertGreater(os.path.getsize(f_exe), (1 << 18))
 
         pkgs = []
         re_pkg = re.compile(r'^@\s+(\S*)$')
-        fp = open(f_ini, 'rt')
+        fp = open(f_ini, 'rt', encoding='utf-8')
         for line in fp:
             match = re_pkg.match(line)
             if not match: continue
             pkgs.append(match.group(1))
         fp.close()
         self.assertEqual(len(pkgs), len(selected))
         for pkg in selected:
             self.assertTrue(pkg in pkgs)
 
     def testDummyDownloads(self):
-        for arch in [ 'x86', 'x86_64' ]:
+        for arch in [ 'x86_64' ]:
             builder = PMbuilder(Viewer=SilentBuildViewer())
             builder.SetOption('DummyDownload', True)
             builder.SetArch(arch)
 
             pkgset = PackageSet([ os.path.join('..', 'example.pkgs') ])
             for ident, pset, cfg in [ ( 'basic', None, None ),
                                       ( 'custom', pkgset, None ),
@@ -312,17 +323,17 @@
     def testTemplate(self):
         with tempfile.TemporaryDirectory() as topdir:
             tplt = os.path.join(topdir, 'templates.txt')
             with codecs.open(tplt, 'w', 'utf-8') as fp:
                 self.makeTemplate(fp)
 
             counts = self.templateCounts(tplt)
-            self.assertTrue(counts['categories'] >= 20)
-            self.assertTrue(counts['categories'] <= 100)
-            self.assertTrue(counts['packages'] >= 1000)
+            self.assertGreaterEqual(counts['categories'], 20)
+            self.assertLessEqual(counts['categories'], 100)
+            self.assertGreaterEqual(counts['packages'], 1000)
 
     def testTerseTemplate(self):
         with tempfile.TemporaryDirectory() as topdir:
             tplt = os.path.join(topdir, 'terse.txt')
             pkgset = PackageSet()
             pkgset.extend(['bash', 'flex', 'tcsh', 'vim', 'zsh'])
             with codecs.open(tplt, 'w', 'utf-8') as fp:
@@ -334,15 +345,15 @@
 
     def templateCounts(self, tplt):
         """Basic sanity checking on template package listing"""
         re_category = re.compile(r'^## [^#]+$')
         re_package = re.compile(r'^#?[a-zA-Z][^ ]*\s+#[^#]*$')
         counts = { 'categories':0, 'packages':0 }
 
-        fp = open(tplt, 'rt')
+        fp = open(tplt, 'rt', encoding='utf-8')
         for line in fp:
             if re_category.match(line):
                 counts['categories'] += 1
             if re_package.match(line):
                 counts['packages'] += 1
         fp.close()
 
@@ -459,76 +470,82 @@
         pkgs = pkgset.extract()
         self.assertEqual(pkgs, ['bash', 'sh'])
 
 
 
 class testPackageLists(unittest.TestCase):
     def setUp(self):
-        re_cfg = re.compile(r'^setup.*\.ini$')
-        cwd = os.getcwd()
+        re_cfg = re.compile(r'^setup.*\.(?:ini|bz2|xz)$')
         scheme = 'file:'
-        if sys.platform == 'win32' and not cwd.startswith('\\'):
+        if sys.platform == 'win32' and not TESTDIR.startswith('\\'):
             scheme += '/'
-        dirlist = os.listdir(cwd)
-        self._configs = [ f for f in dirlist if re_cfg.match(f)
-                                                and os.path.isfile(f) ]
-        self._urlprefix = '{s}{d}/'.format(s=scheme, d=cwd.replace('\\', '/'))
+        self._configs = []
+        for d in [ TESTDIR, os.path.join(TESTDIR, 'legacy') ]:
+            fls = [ os.path.join(d, f)
+                        for f in os.listdir(d)
+                        if re_cfg.match(f) ]
+            self._configs.extend(f for f in fls if os.path.isfile(f))
+        self._urlprefix = '{s}{d}/'.format(s=scheme, d=TESTDIR.replace('\\', '/'))
 
     def testIO(self):
         """Test that setup.ini files of various generations,
         and containing various mixes of ascii/latin-1/utf-8 characters
         can be parsed and rewritten without exceptions or glaring errors"""
         for cfg in self._configs:
             url = urllib.parse.urljoin(self._urlprefix, cfg)
 
             with tempfile.TemporaryDirectory() as tmpdir:
                 builder = PMbuilder(Viewer=SilentBuildViewer())
                 builder.setup_ini_url = url
                 builder.SetTargetDir(tmpdir)
 
+                if 'make' in builder._masterList.GetPackageDict():
+                    deps = builder._resolveDependencies(['make'])
+                    self.assertGreater(len(deps), 20, msg='src={}'.format(cfg))
+
                 builder._optiondict['AllPackages'] = True
                 pkglist = builder._extendPkgSelection()
-                self.assertTrue(len(pkglist) > 4)
+                self.assertGreater(len(pkglist), 4)
 
                 arch = builder.GetArch()
                 f_ini = os.path.join(tmpdir, arch, os.path.basename(cfg))
                 f_ini = os.path.join(tmpdir, arch, 'setup.ini')
                 f_tplt = os.path.join(tmpdir, 'tplt.txt')
 
                 self.assertFalse(os.path.isfile(f_ini))
                 builder._buildSetupFiles(pkglist)
                 self.assertTrue(os.path.isfile(f_ini))
 
                 self.assertFalse(os.path.isfile(f_tplt))
                 with codecs.open(f_tplt, 'w', 'utf-8') as fp:
                     builder._pkgProc.MakeTemplate(fp)
-                    self.assertTrue(fp.tell() > 100)
+                    self.assertGreater(fp.tell(), 100)
 
 
 
 class testMirrorLists(unittest.TestCase):
     def testHasFallback(self):
         fp = PMbuilder._makeFallbackMirrorList()
         (regionDict, urlDict) = self.mkSets(fp)
         fp.close()
-        self.assertTrue(len(regionDict) > 3)
-        self.assertTrue(len(urlDict) > 4)
+        self.assertGreater(len(regionDict), 3)
+        self.assertGreater(len(urlDict), 4)
         self.assertTrue(('Asia', 'Japan') in regionDict)
         self.assertTrue(('Europe', 'UK') in regionDict)
 
     def testValidFallback(self):
         fp0 = PMbuilder._makeFallbackMirrorList()
         (fb_regions, fb_urls) = self.mkSets(fp0)
         fp0.close()
         fp1 = urllib.request.urlopen(CYGWIN_MIRROR_LIST_URL)
         (cyg_regions, cyg_urls) = self.mkSets(fp1)
         fp1.close()
 
-        self.assertTrue(len(cyg_regions) > 8)
-        self.assertTrue(len(cyg_urls) > 12)
+        self.assertGreater(len(cyg_regions), 8)
+        self.assertGreater(len(cyg_urls), 12)
 
         for reg in fb_regions:
             if not reg in cyg_regions:
                 self.fail('Mirror region %s/%s does not appear'
                           ' in official list' % reg)
         for url in fb_urls:
             if not url in cyg_urls:
@@ -616,15 +633,15 @@
 
 
 def makeGarbageTree(treefile, topdir='.'):
     """Create outline directory tree for testing GarbageCollector"""
 
     treedict = { 'directories':[], 'files':[] }
 
-    fp = open(treefile, 'rt')
+    fp = open(treefile, 'rt', encoding='utf-8')
     for line in fp:
         idx = line.find('#')
         if idx >= 0:
             line = line[0:idx]
         line = line.strip()
         if not line:
             continue
@@ -637,15 +654,15 @@
         if ftype == 'D':
             try:
                 os.mkdir(fname)
                 treedict['directories'].append(fname)
             except OSError:
                 pass
         elif ftype == 'F':
-            fp2 = open(fname, 'wt')
+            fp2 = open(fname, 'wt', encoding='utf-8')
             flen = random.randint(0, 512)
             print((chr(0x5a) * flen), file=fp2)
             fp2.close()
             treedict['files'].append(fname)
         else:
             pass
     fp.close()
```

