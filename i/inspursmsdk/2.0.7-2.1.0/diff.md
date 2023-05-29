# Comparing `tmp/inspursmsdk-2.0.7.tar.gz` & `tmp/inspursmsdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inspursmsdk-2.0.7.tar", last modified: Thu Apr 27 09:29:54 2023, max compression
+gzip compressed data, was "dist/inspursmsdk-2.1.0.tar", last modified: Mon May 29 03:09:04 2023, max compression
```

## Comparing `inspursmsdk-2.0.7.tar` & `inspursmsdk-2.1.0.tar`

### file list

```diff
@@ -1,86 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/
--rw-r--r--   0 root         (0) root         (0)      991 2023-04-27 09:29:31.000000 inspursmsdk-2.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      888 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-04-27 09:29:31.000000 inspursmsdk-2.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-27 09:29:31.000000 inspursmsdk-2.0.7/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspur_sm_sdk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/
--rw-r--r--   0 root         (0) root         (0)    49352 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/IpmiFunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
--rw-r--r--   0 root         (0) root         (0)    16391 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/commonInfoStr.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/eventLogString.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/sensorEventStr.py
--rw-r--r--   0 root         (0) root         (0)    51098 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/showSensorDesc.py
--rw-r--r--   0 root         (0) root         (0)    20338 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/RedfishFunc.py
--rw-r--r--   0 root         (0) root         (0)   306678 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/RestFunc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11954 2023-04-27 09:29:31.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/backup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/
--rw-r--r--   0 root         (0) root         (0)    44672 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/A7.xml
--rw-r--r--   0 root         (0) root         (0)    18131 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/M4.xml
--rw-r--r--   0 root         (0) root         (0)    54444 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/M5.xml
--rw-r--r--   0 root         (0) root         (0)    84520 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/M6-N.xml
--rw-r--r--   0 root         (0) root         (0)    81800 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/M6.xml
--rw-r--r--   0 root         (0) root         (0)    46175 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/M7.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF3180A6.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF3280A6.xml
--rw-r--r--   0 root         (0) root         (0)   360127 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF5180M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF5280M5.xml
--rw-r--r--   0 root         (0) root         (0)    36922 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF5468A5.xml
--rw-r--r--   0 root         (0) root         (0)    29961 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF5488A5.xml
--rw-r--r--   0 root         (0) root         (0)   360290 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/SA5112M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/SA5212M5.xml
--rw-r--r--   0 root         (0) root         (0)    65986 2023-04-27 09:29:30.000000 inspursmsdk-2.0.7/inspur_sm_sdk/command/restore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspur_sm_sdk/conf/
--rw-r--r--   0 root         (0) root         (0)     1613 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/conf/NF5180M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/conf/NF5280M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/conf/SA5112M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/conf/SA5212M5.yml
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/conf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/
--rw-r--r--   0 root         (0) root         (0)    43783 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/Base.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonA5.py
--rw-r--r--   0 root         (0) root         (0)     2998 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonA6.py
--rw-r--r--   0 root         (0) root         (0)     6333 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonA7.py
--rw-r--r--   0 root         (0) root         (0)   743806 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonM5.py
--rw-r--r--   0 root         (0) root         (0)   631511 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonM6.py
--rw-r--r--   0 root         (0) root         (0)    17358 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonM6_41401.py
--rw-r--r--   0 root         (0) root         (0)    16476 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonM6_4140a.py
--rw-r--r--   0 root         (0) root         (0)   259774 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonM7.py
--rw-r--r--   0 root         (0) root         (0)    45791 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/I24M6.py
--rw-r--r--   0 root         (0) root         (0)     8475 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/IBase.py
--rw-r--r--   0 root         (0) root         (0)    14793 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/NF5180M5.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/NF5180M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    15217 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/NF5280M5.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/NF5280M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    59696 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/NF5280M5_435.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-04-27 09:29:29.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/NF5280M5_436.py
--rw-r--r--   0 root         (0) root         (0)    47127 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/NS5160M6.py
--rw-r--r--   0 root         (0) root         (0)   120002 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/ResEntity.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/SA5212M5Impl.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspur_sm_sdk/route/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/route/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/route/route.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspur_sm_sdk/util/
--rw-r--r--   0 root         (0) root         (0)     4652 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/util/HostTypeJudge.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/util/RedfishClient.py
--rw-r--r--   0 root         (0) root         (0)    10339 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/util/RegularCheckUtil.py
--rw-r--r--   0 root         (0) root         (0)     7686 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/util/RequestClient.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7550 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/util/configUtil.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/util/fileUtil.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-04-27 09:29:28.000000 inspursmsdk-2.0.7/inspur_sm_sdk/util/parameterConversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspursmsdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      888 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspursmsdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2598 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspursmsdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspursmsdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspursmsdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/inspursmsdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5216 2023-04-27 09:29:31.000000 inspursmsdk-2.0.7/ism.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 09:29:54.000000 inspursmsdk-2.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2023-04-27 09:29:31.000000 inspursmsdk-2.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)      991 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      888 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspur_sm_sdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/
+-rw-r--r--   0 root         (0) root         (0)    49818 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/IpmiFunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    16391 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/commonInfoStr.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/eventLogString.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/sensorEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    51098 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/showSensorDesc.py
+-rw-r--r--   0 root         (0) root         (0)    21216 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/RedfishFunc.py
+-rw-r--r--   0 root         (0) root         (0)   306808 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/RestFunc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12152 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/backup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/
+-rw-r--r--   0 root         (0) root         (0)    44672 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/A7.xml
+-rw-r--r--   0 root         (0) root         (0)    18131 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M4.xml
+-rw-r--r--   0 root         (0) root         (0)    54444 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M5.xml
+-rw-r--r--   0 root         (0) root         (0)    84520 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M6-N.xml
+-rw-r--r--   0 root         (0) root         (0)    81800 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M6.xml
+-rw-r--r--   0 root         (0) root         (0)    46175 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M7.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF3180A6.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF3280A6.xml
+-rw-r--r--   0 root         (0) root         (0)   360127 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5180M5.xml
+-rw-r--r--   0 root         (0) root         (0)   360210 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5280M5.xml
+-rw-r--r--   0 root         (0) root         (0)    36922 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5468A5.xml
+-rw-r--r--   0 root         (0) root         (0)    29961 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5488A5.xml
+-rw-r--r--   0 root         (0) root         (0)   360290 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/SA5112M5.xml
+-rw-r--r--   0 root         (0) root         (0)   360210 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/SA5212M5.xml
+-rw-r--r--   0 root         (0) root         (0)    66019 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/restore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/NF5180M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/NF5280M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/SA5112M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/SA5212M5.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/
+-rw-r--r--   0 root         (0) root         (0)    44074 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/Base.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA5.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA6.py
+-rw-r--r--   0 root         (0) root         (0)     6333 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA7.py
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA7_11308.py
+-rw-r--r--   0 root         (0) root         (0)   744015 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM5.py
+-rw-r--r--   0 root         (0) root         (0)   598814 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6.py
+-rw-r--r--   0 root         (0) root         (0)    17358 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6_41401.py
+-rw-r--r--   0 root         (0) root         (0)    16476 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6_4140a.py
+-rw-r--r--   0 root         (0) root         (0)   276843 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM7.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM7_13505.py
+-rw-r--r--   0 root         (0) root         (0)    45791 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/I24M6.py
+-rw-r--r--   0 root         (0) root         (0)     8475 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/IBase.py
+-rw-r--r--   0 root         (0) root         (0)    14826 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5180M5.py
+-rw-r--r--   0 root         (0) root         (0)      339 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5180M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    15217 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    59696 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5_435.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5_436.py
+-rw-r--r--   0 root         (0) root         (0)    47115 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NS5160M6.py
+-rw-r--r--   0 root         (0) root         (0)   120002 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/ResEntity.py
+-rw-r--r--   0 root         (0) root         (0)      512 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/SA5212M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/route/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/route/route.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/
+-rw-r--r--   0 root         (0) root         (0)     4718 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/HostTypeJudge.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/RedfishClient.py
+-rw-r--r--   0 root         (0) root         (0)    10339 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/RegularCheckUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/RequestClient.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7550 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/configUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/fileUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/parameterConversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      888 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/ism.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/setup.py
```

### Comparing `inspursmsdk-2.0.7/MANIFEST.in` & `inspursmsdk-2.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/PKG-INFO` & `inspursmsdk-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.0.7
+Version: 2.1.0
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/IpmiFunc.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/IpmiFunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
     res = {}
     import platform
     sysstr = platform.system()
     cmd_get = 'sensor list'
     if findname != None:
         if sysstr == 'Windows':
             cmd_get = cmd_get + ' | find "' + findname + '" '
-        elif sysstr == 'Linux':
+        elif sysstr == 'Linux' or sysstr == 'Darwin':
             cmd_get = cmd_get + ' | grep "' + findname + '" '
     result = getLinesRawByIpmi(client, cmd_get)
     if result['code'] != 0:
         return result
     line_list = result['data']
     Normal_list = ['ok', '0x8080', '0x4080', '0x0280', '0x0180']
     Absent_list = ['na', '0x0080']
@@ -918,27 +918,30 @@
     cmd_get = 'raw 0x3c 0x03 0x01 0x00'
     result = getLinesRawByIpmi(client, cmd_get)
     if result['code'] != 0:
         return result
     num_list = result['data']
     cmd_str = ' '.join(num_list).replace(' ', '').replace('\n', '')
     res['code'] = 0
+    res['data'] = {}
     res['data']['Version'] = __hex2ascii(cmd_str)
     return res
 
+
 def getPowerStatusByIpmi(client):
     res = {}
     cmd_get = 'power status'
     result = getLineRawByIpmi(client, cmd_get)
     if result['code'] != 0:
         return result
     cmd_str = result['data']
     cmd_str = cmd_str.replace('\n', '')
     cmd_str = str(cmd_str).split(' ')[-1]
     res['code'] = 0
+    res['data'] = {}
     res['data']['status'] = cmd_str
     return res
 
 
 # 设置电源开关状态
 # status : on off soft reset cycle
 def powerControlByIpmi(client, status):
@@ -1229,14 +1232,25 @@
             data['aux_firmware_rev_info'] = value[2:]
             break
     JSON['code'] = 0
     JSON['data'] = data
     return JSON
 
 
+def getFirmwareVersoinByMcinfo(client):
+    result = getMcInfoByIpmi(client)
+    if result['code'] != 0:
+        return ''
+    data = result['data']
+    bmcVersion_0 = data['firmware_revision']
+    bmcVersion_1 = eval(data['aux_firmware_rev_info'].split(";")[0])
+    bmcVersion = str(bmcVersion_0) + str(int(str(bmcVersion_1), 16)).zfill(2)
+    return bmcVersion
+
+
 # 获取M6机型web界面的登录加密方式，01加密，00不加密
 def judge_encrypt(client):
     cmd = "raw 0x3c 0x05 0x28"
     result = getLineRawByIpmi(client, cmd)
     if result['code'] == 0:
         data = result['data'].replace('\n', '').replace(' ', '')
         if data == "01":
@@ -1490,15 +1504,15 @@
 
 def __getCmd_type(client, cmd_get, rt):
     res = {}
     import platform
     sysstr = platform.system()
     if sysstr == 'Windows':
         cmdPrefix = "D:\\ipmitool\\ipmitool.exe -U " + client.username + " -P " + client.passcode + " -H " + client.host + " -I " + client.lantype + " " + cmd_get + " 2>nul"
-    elif sysstr == 'Linux':
+    elif sysstr == 'Linux' or sysstr == 'Darwin':
         cmdPrefix = "ipmitool -U " + client.username + " -P " + client.passcode + " -H " + client.host + " -I " + client.lantype + " " + cmd_get + " 2>/dev/null"
     cmd_str = ''
     str_list = []
     try:
         with os.popen(cmdPrefix, 'r') as p:
             if rt == 'readline':
                 cmd_str = p.readline()
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/biosPostEventStr.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/biosPostEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/commonInfoStr.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/commonInfoStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/eventLogString.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/eventLogString.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/sensorEventStr.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/sensorEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/M5Log/showSensorDesc.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/showSensorDesc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/RedfishFunc.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/RedfishFunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,7 +514,28 @@
             JSON['data'] = 'request failed, response content: ' + str(
                 res["error"]["message"]) + ' the status code is ' + str(response.status_code) + "."
         except:
             JSON['code'] = 1
             JSON['data'] = 'request failed, BMC interface ' + str(url) + ' response status code is ' + \
                            str(response.status_code) + ', text is ' + str(response.text)
     return JSON
+
+
+def remoteFWUpdate(client, data):
+    JSON = {}
+    response = client.request("POST", "redfish/v1/UpdateService/Actions/UpdateService.SimpleUpdate", json=data,
+                              auth=HTTPBasicAuth(client.username, client.passcode))
+    if response is None:
+        JSON['code'] = 1
+        JSON['data'] = 'response is none'
+    elif response.status_code == 204 or response.status_code == 200:
+        JSON['code'] = 0
+        JSON['data'] = ""
+    else:
+        try:
+            res = response.json()
+            JSON['code'] = 2
+            JSON['data'] = 'request failed, response content: ' + str(res["error"]["message"]) + ' the status code is ' + str(response.status_code) + "."
+        except:
+            JSON['code'] = 1
+            JSON['data'] = 'request failed, response status code is ' + str(response.status_code)
+    return JSON
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/RestFunc.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/RestFunc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1889,16 +1889,16 @@
     }
     action_dict = {
         "remove": 0,
         "global": 1,
         "dedicate": 2
     }
     data = {
-        "ctrlId": ctrlId, 
-        "deviceId": deviceId, 
+        "ctrlId": ctrlId,
+        "deviceId": deviceId,
         "configure_type": action_dict.get(action)
     }
     data['affinity'] = yes_no_dict.get(encl) if action != "remove" else 0
     data['revertible'] = yes_no_dict.get(revertible) if action != "remove" else 0
     if action == "dedicate":
         LID_list = logicalDrivers.split(',')
         LID_list.sort()
@@ -4734,15 +4734,15 @@
         JSON['code'] = 1
         JSON['data'] = 'cannot find file.'
         return JSON
     if not os.path.isfile(updatefile):
         JSON['code'] = 1
         JSON['data'] = 'input is not a file.'
         return JSON
-    if platform.system() == 'Linux':
+    if platform.system() == 'Linux' or platform.system() == 'Darwin':
         file_name = updatefile.split('/')[-1]
     else:
         file_name = updatefile.split('\\')[-1]
     try:
         with open(updatefile.decode('utf8'), 'rb') as f:
             content = f.read()
             data = '------{0}{1}Content-Disposition: form-data; name="fwimage"; filename="{3}" {1}Content-Type: application/octet-stream{1}{1}{2}{1}------{0}--{1}'.format(
@@ -5027,15 +5027,15 @@
         JSON['code'] = 1
         JSON['data'] = 'cannot find file.'
         return JSON
     if not os.path.isfile(updatefile):
         JSON['code'] = 1
         JSON['data'] = 'can not find file.'
         return JSON
-    if platform.system() == 'Linux':
+    if platform.system() == 'Linux' or platform.system() == 'Darwin':
         file_name = updatefile.split('/')[-1]
     else:
         file_name = updatefile.split('\\')[-1]
 
     try:
         if sys.version_info < (3, 0):
             with open(updatefile.decode('utf-8'), 'rb') as f:
@@ -5147,15 +5147,15 @@
 def uploadBMCfgByRest(client, filepath):
     JSON = {}
     header = client.getHearder()
     header["X-Requested-With"] = "XMLHttpRequest"
     header["Content-Type"] = "multipart/form-data;boundary=----WebKitFormBoundaryF4ZROI7nayCrLnwy"
     header["Cookie"] = "" + header["Cookie"] + ";refresh_disable=1"
 
-    if platform.system() == 'Linux':
+    if platform.system() == 'Linux' or platform.system() == 'Darwin':
         file_name = filepath.split('/')[-1]
     else:
         file_name = filepath.split('\\')[-1]
 
     if not os.path.exists(filepath):
         JSON["code"] = 1
         JSON["data"] = "File path is error."
@@ -6332,15 +6332,15 @@
         JSON["code"] = 1
         JSON["data"] = 'CPLD Image file ' + updatefile + ' not exists.'
         return JSON
     if not os.path.isfile(updatefile):
         JSON["code"] = 1
         JSON["data"] = 'CPLD Image file ' + updatefile + ' is not a file.'
         return JSON
-    if platform.system() == 'Linux':
+    if platform.system() == 'Linux' or platform.system() == 'Darwin':
         file_name = updatefile.split('/')[-1]
     else:
         file_name = updatefile.split('\\')[-1]
     try:
         if sys.version_info < (3, 0):
             with open(updatefile.decode('utf-8'), 'rb') as f:
                 content = f.read()
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/backup.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/backup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 from inspur_sm_sdk.interface.ResEntity import ResultBean
 
 
 def dns(client, args):
     responds = RestFunc.getDNSByRestM5(client)
     if responds['code'] == 0 and responds['data'] is not None:
         result = responds['data']
-        if platform.system() == 'Linux':
+        if platform.system() == 'Linux' or platform.system() == 'Darwin':
             f = open(args.backuppath + '/DNS.conf', 'wb')
         else:
             f = open(args.backuppath + '\\DNS.conf', 'wb')
         f.write(json.dumps(result, indent=4))
         f.close()
         return 1, "ok"
     else:
         return -1, "can not get dns info"
 
 
 def network(client, args):
     responds = RestFunc.getNetworkByRest(client)
     if responds['code'] == 0 and responds['data'] is not None:
         result = responds['data']
-        if platform.system() == 'Linux':
+        if platform.system() == 'Linux' or platform.system() == 'Darwin':
             f = open(args.backuppath + '/network.conf', 'w')
         else:
             f = open(args.backuppath + '\\network.conf', 'w')
         f.write(json.dumps(result, indent=4))
         f.close()
         return 1, "ok"
     else:
@@ -56,45 +56,45 @@
         return -1, "can not get service info"
 
 
 def ntp(client, args):
     responds = RestFunc.getDatetimeByRest(client)
     if responds['code'] == 0 and responds['data'] is not None:
         result = responds['data']
-        if platform.system() == 'Linux':
+        if platform.system() == 'Linux' or platform.system() == 'Darwin':
             f = open(args.backuppath + '/NTP.conf', 'w')
         else:
             f = open(args.backuppath + '\\NTP.conf', 'w')
         f.write(json.dumps(result, indent=4))
         f.close()
         return 1, "ok"
     else:
         return -1, "can not get ntp info"
 
 
 def smtp(client, args):
     responds = RestFunc.getSMTPM5ByRest(client)
     if responds['code'] == 0 and responds['data'] is not None:
         result = responds['data']
-        if platform.system() == 'Linux':
+        if platform.system() == 'Linux' or platform.system() == 'Darwin':
             f = open(args.backuppath + '/SMTP.conf', 'w')
         else:
             f = open(args.backuppath + '\\SMTP.conf', 'w')
         f.write(json.dumps(result, indent=4))
         f.close()
         return 1, "ok"
     else:
         return -1, "can not get smtp info"
 
 
 def snmptrap(client, args):
     responds = RestFunc.getSnmpInfoByRest(client)
     if responds['code'] == 0 and responds['data'] is not None:
         result = responds['data']
-        if platform.system() == 'Linux':
+        if platform.system() == 'Linux' or platform.system() == 'Darwin':
             f = open(args.backuppath + '/SNMPtrap.conf', 'w')
         else:
             f = open(args.backuppath + '\\SNMPtrap.conf', 'w')
         f.write(json.dumps(result, indent=4))
         f.close()
         return 1, "ok"
     else:
@@ -184,15 +184,15 @@
         return 1, "ok"
     else:
         return -1, "can not get bios info"
 
 
 def backup(client, args):
     backtime = time.strftime('%Y%m%d%H%M%S', time.localtime(time.time()))
-    if platform.system() == 'Linux':
+    if platform.system() == 'Linux' or platform.system() == 'Darwin':
         path = args.bak_file + "backup/" + args.host + "-" + backtime + "/"
     else:
         path = args.bak_file + "backup\\" + args.host + "-" + backtime + "\\"
     if not os.path.exists(path):
         os.makedirs(path)
     args.backuppath = path
     password_path = path + "password.txt"
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/A7.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/A7.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/M4.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M4.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/M5.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/M6-N.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M6-N.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/M6.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/M7.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M7.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF3180A6.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF3180A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF3280A6.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF3280A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF5180M5.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5180M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF5280M5.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5280M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF5468A5.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5468A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/NF5488A5.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5488A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/SA5112M5.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/SA5112M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/bios/SA5212M5.xml` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/SA5212M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/command/restore.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/command/restore.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         return status, info
 
     return 1, "ok"
 
 
 def restore(client, args):
     result = ResultBean
-    if platform.system() == 'Linux':
+    if platform.system() == 'Linux' or platform.system() == 'Darwin':
         file_separator = "/"
     else:
         file_separator = "\\"
     # Windows下 -F "D:\100.2.38.46\" 最后的'\"'会被解析为'"'
     # 判断并删除
     if args.bak_file[-1] == '"':
         args.bak_file = args.bak_file[:-1] + "\\"
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/conf/NF5180M5.yml` & `inspursmsdk-2.1.0/inspur_sm_sdk/conf/NF5180M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/conf/NF5280M5.yml` & `inspursmsdk-2.1.0/inspur_sm_sdk/conf/NF5280M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/conf/SA5112M5.yml` & `inspursmsdk-2.1.0/inspur_sm_sdk/conf/SA5112M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/conf/SA5212M5.yml` & `inspursmsdk-2.1.0/inspur_sm_sdk/conf/SA5212M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/Base.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/Base.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def getfru(self, client, args):
         fru = IpmiFunc.getAllFruByIpmi(client)
         res = ResultBean()
         if fru:
             FRUlist = []
             product = fru
             frubean = collections.OrderedDict()
-            if product['Product Name']:
+            if product.get('Product Name', None):
                 frubean["FRUName"] = product['Product Name']
             else:
                 frubean["FRUName"] = None
 
             if product['Chassis Type']:
                 frubean["ChassisType"] = product['Chassis Type']
             else:
@@ -116,15 +116,15 @@
                 frubean["ProductName"] = None
 
             if product['Product Part Number']:
                 frubean["ProductPartNumber"] = product['Product Part Number']
             else:
                 frubean["ProductPartNumber"] = None
 
-            if product['Product Version']:
+            if product.get('Product Version', None):
                 frubean["ProductVersion"] = product['Product Version']
             else:
                 frubean["ProductVersion"] = None
 
             if product['Product Serial']:
                 frubean["ProductSerial"] = product['Product Serial']
             else:
@@ -1428,14 +1428,24 @@
     def methods(self, client, args):
         return(list(filter(lambda m: not m.startswith("__") and not m.endswith("__") and callable(getattr(self, client, args, m)), dir(self, client, args))))
 
     def setbmclogcfg(self, client, args):
         result = ResultBean()
         result.State("Not Support")
         return result
+
+    def remoteFWUpdate(self, client, args):
+        result = ResultBean()
+        result.State("Not Support")
+        return result
+
+    def updatepsu(self, client, args):
+        result = ResultBean()
+        result.State("Not Support")
+        return result
 # Ascii转十六进制
 
 
 def ascii2hex(data, length):
     count = length - len(data)
     list_h = []
     for c in data:
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonA5.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonA6.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonA7.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA7.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonM5.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM5.py`

 * *Files 0% similar despite different names*

```diff
@@ -8942,21 +8942,26 @@
 
     def setsmtpcom(self, client, args):
         result = ResultBean()
         result.State("Not Support")
         result.Message(['The M5 model does not support this feature.'])
         return result
 
-
     def setsmtpdest(self, client, args):
         result = ResultBean()
         result.State("Not Support")
         result.Message(['The M5 model does not support this feature.'])
         return result
 
+    def remoteFWUpdate(self, client, args):
+        result = ResultBean()
+        result.State("Not Support")
+        result.Message(['The M5 model does not support this feature.'])
+        return result
+
 
 def getWeek(binr):
     bin_dict = {1: 'Mon', 2: 'Tue', 3: 'Wed', 4: 'Thur', 5: 'Fri', 6: 'Sat', 7: 'Sun'}
     list = []
     for i in range(1, 7):
         weeki = binr[8 - i:9 - i]
         if weeki == '1':
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonM6.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6.py`

 * *Files 2% similar despite different names*

```diff
@@ -946,15 +946,15 @@
                                 for item_2 in item_value:
                                     setter_list.append(
                                         {"cmd": item_2.get("ValueName"), "value": item_2.get("ValueName")})
                                 item_1['setter'] = setter_list
             return flag, infoList
 
         Bios_result = ResultBean()
-        args.list = False
+        # args.list = False
         if 'list' not in args or ('list' in args and args.list is False):
             if args.attribute is None and args.value is None and args.fileurl is None:
                 Bios_result.Message(['please input a command at least.'])
                 Bios_result.State('Failure')
                 return Bios_result
             elif args.attribute is None and args.value is None and args.fileurl is not None:
                 if not os.path.exists(args.fileurl) or not os.path.isfile(args.fileurl):
@@ -1793,14 +1793,19 @@
         return import_Info
 
     def updatecpld(self, client, args):
         args.type = None
         result = self.fwupdate(client, args)
         return result
 
+    def updatepsu(self, client, args):
+        args.type = None
+        result = self.fwupdate(client, args)
+        return result
+
     def fwupdate(self, client, args):
         if args.type == "FPGA":
             res = ResultBean()
             res.State("Failure")
             res.Message(["Not Support, Update FPGA is not support"])
             return res
 
@@ -2150,16 +2155,18 @@
                 wirte_log(
                     log_path,
                     "Upload File",
                     "Connect Failed",
                     version_info)
 
             # BIOS PSU 升级自动重启
+            flag = False
             if args.mode == "Auto" and getServerStatus(client) != "off" and (
                     args.type == "BIOS" or args.type == "PSUFW"):
+                flag = True
                 choices = {'on': 1, 'off': 0, 'cycle': 2, 'reset': 3, 'shutdown': 5}
                 Power = RestFunc.setM6PowerByRest(client, choices["off"])
                 if Power.get('code') == 0 and Power.get('data') is not None:
                     off_count = 0
                     import time
                     while True:
                         if getServerStatus(client) == "off" or off_count > 5:
@@ -2508,14 +2515,30 @@
                             result.Message(
                                 ["get new fw information error, " + str(fw_res.get('data'))])
                             wirte_log(
                                 log_path,
                                 "Activate",
                                 "Data Verify Failed",
                                 result.Message)
+                    if flag and args.type == "PSUFW" and getServerStatus(client) == "off":
+                        result = ResultBean()
+                        ctr_info = IpmiFunc.powerControlByIpmi(client, "on")
+                        if ctr_info:
+                            if ctr_info.get('code') == 0 and ctr_info.get('data') is not None and ctr_info.get('data').get('result') is not None:
+                                result.State("Success")
+                                result.Message(['Update PSU complete, system auto power on success'])
+                                self.wirte_log(log_path, "Restart", "Set power on success", result.Message)
+                            else:
+                                result.State("Failure")
+                                result.Message(['Update PSU complete. But system auto reset failed, please power on manually ...'])
+                                self.wirte_log(log_path, "Restart", "Set power on failed", result.Message)
+                        else:
+                            result.State("Failure")
+                            result.Message(['set power failed.please check server manually'])
+                            self.wirte_log(log_path, "Restart", "Set power on failed", result.Message)
                 else:
                     if args.mode == "Manual":
                         # manual 需要手动重启bmc
                         result.State('Success')
                         result.Message(
                             [
                                 "Activate pending, host is power " +
@@ -2821,680 +2844,14 @@
                 image1_update_info +
                 image2_update_info)
 
             result.State("Success")
             result.Message([image1_update_info, image2_update_info])
             continue
 
-    # def fwupdate(self, client, args):
-    #     if args.type == "FPGA":
-    #         res = ResultBean()
-    #         res.State("Not Support")
-    #         res.Message(["Update FPGA is not support"])
-    #         return res
-    #     def ftime(ff="%Y-%m-%d %H:%M:%S "):
-    #         try:
-    #             import time
-    #             localtime = time.localtime()
-    #             f_localtime = time.strftime(ff, localtime)
-    #             return f_localtime
-    #         except:
-    #             return ""
-    #
-    #     def getServerStatus(client):
-    #         try:
-    #             res_1 = RestFunc.getChassisStatusByRest(client)
-    #             if res_1.get('code') == 0 and res_1.get('data') is not None:
-    #                 status = res_1.get('data').get('power_status', "unknown")
-    #                 if status == "On":
-    #                     return "on"
-    #                 elif status == "Off":
-    #                     return "off"
-    #                 else:
-    #                     return "unknown"
-    #             else:
-    #                 return "unknown"
-    #         except:
-    #             return "unknown"
-    #
-    #     result = ResultBean()
-    #     # getpsn
-    #     psn = "UNKNOWN"
-    #     res_syn = self.getfru(client, args)
-    #     if res_syn.State == "Success":
-    #         frulist = res_syn.Message[0].get("FRU", [])
-    #         if frulist != []:
-    #             psn = frulist[0].get('ProductSerial','UNKNOWN')
-    #     else:
-    #         return res_syn
-    #     logtime = ftime("%Y%m%d%H%M%S")
-    #     dir_name = logtime + "_" + psn
-    #     # 创建目录
-    #     T6_path = os.path.abspath(__file__)
-    #     interface_path = os.path.split(T6_path)[0]
-    #     root_path = os.path.dirname(interface_path)
-    #     update_path = os.path.join(root_path, "update")
-    #     if not os.path.exists(update_path):
-    #         os.makedirs(update_path)
-    #     update_plog_path = os.path.join(update_path, dir_name)
-    #     if not os.path.exists(update_plog_path):
-    #         os.makedirs(update_plog_path)
-    #
-    #     log_path = os.path.join(update_plog_path, "updatelog")
-    #     if not os.path.exists(log_path):
-    #         with open(log_path, 'w') as newlog:
-    #             log_dict = {"log": []}
-    #             newlog.write(str(log_dict))
-    #     # session文件
-    #     session_path = os.path.join(update_plog_path, "session")
-    #
-    #     # checkname
-    #     p = '\.hpm$'
-    #     file_name = os.path.basename(args.url)
-    #     if not re.search(p, file_name, re.I):
-    #         result.State("Failure")
-    #         result.Message(["Please select valid hpm image file."])
-    #         return result
-    #
-    #     # 文件校验
-    #     if not os.path.exists(args.url):
-    #         result.State("Failure")
-    #         result.Message(["Please select valid hpm image file."])
-    #         return result
-    #     if not os.path.isfile(args.url):
-    #         result.State("Failure")
-    #         result.Message(["Please select valid hpm image file."])
-    #         return result
-    #
-    #     if args.type == "BMC":
-    #         if args.override == 1 and args.mode == "Manual":
-    #             result.State("Failure")
-    #             result.Message(["BMC upgrade cannot set mode to manual if override configuration."])
-    #             return result
-    #
-    #     upgrade_count = 0
-    #     while True:
-    #         # 判断session是否存在，存在则logout&del
-    #         if os.path.exists(session_path):
-    #             with open(session_path, 'r') as oldsession:
-    #                 headers = oldsession.read()
-    #                 #client.setHearder(headers)
-    #                 #读取的是str 需要转化为dict
-    #                 #读取的是"{'Cookie': 'QSESSIONID=493e0d444e127be0edkjBnS3AhsKpM; path=/; secure;HttpOnly', 'X-CSRFToken': 'z4flbXNp'}"
-    #                 #直接loads报错 json.decoder.JSONDecodeError: Expecting property name enclosed in double quotes: line 1 column 2 (char 1)
-    #                 #解决方法 1 单引号替换为双引号
-    #                 #解决方法 2 json.dumps(eval(headers))
-    #                 headers_json = json.loads(json.dumps(eval(headers)))
-    #                 client.setHearder(headers_json)
-    #                 # logout
-    #                 RestFunc.logout(client)  # 删除session
-    #             if os.path.exists(session_path):
-    #                 os.remove(session_path)
-    #         # 删除
-    #         if result.State == "Success":
-    #             return result
-    #         elif result.State == "Abort":
-    #             result.State = "Failure"
-    #             return result
-    #         else:
-    #             if upgrade_count > retry_count:
-    #                 return result
-    #             else:
-    #                 if upgrade_count >= 1:
-    #                     # 重新升级 初始化result
-    #                     result = ResultBean()
-    #                 upgrade_count = upgrade_count + 1
-    #         # login
-    #         headers = {}
-    #         logcount = 0
-    #         while True:
-    #             # 等6分钟
-    #             if logcount > 18:
-    #                 break
-    #             else:
-    #                 logcount = logcount + 1
-    #                 import time
-    #                 time.sleep(20)
-    #             # login
-    #             headers = RestFunc.login_M6(client)
-    #             if headers != {}:
-    #                 # 记录session
-    #                 with open(session_path, 'w') as new_session:
-    #                     new_session.write(str(headers))
-    #                 client.setHearder(headers)
-    #                 break
-    #         # 10次无法登陆 不再重试
-    #         if headers == {}:
-    #             result.State("Failure")
-    #             result.Message(["Cannot log in to BMC."])
-    #             return result
-    #
-    #         # 获取BMC版本
-    #         # get old version
-    #         fw_res = RestFunc.getFwVersion(client)
-    #         fw_old = {}
-    #         if fw_res != {} and fw_res.get('code') == 0 and fw_res.get('data') is not None:
-    #             fwdata = fw_res.get('data')
-    #             for fw in fwdata:
-    #                 if fw.get('dev_version') == '':
-    #                     version = "-"
-    #                 else:
-    #                     index_version = fw.get('dev_version', "").find('(')
-    #                     if index_version == -1:
-    #                         version = fw.get('dev_version')
-    #                     else:
-    #                         version = fw.get('dev_version')[:index_version].strip()
-    #                 if "BMC0" in fw.get("dev_name", ""):
-    #                     fw_old["BMC0"] = version
-    #                     if "Inactivate" in fw.get("dev_name", ""):
-    #                         fw_old["InactivateBMC"] = "BMC0"
-    #                     else:
-    #                         fw_old["ActivateBMC"] = "BMC0"
-    #                 elif "BMC1" in fw.get("dev_name", ""):
-    #                     fw_old["BMC1"] = version
-    #                     if "Inactivate" in fw.get("dev_name", ""):
-    #                         fw_old["InactivateBMC"] = "BMC1"
-    #                     else:
-    #                         fw_old["ActivateBMC"] = "BMC1"
-    #                 elif "BIOS" in  fw.get("dev_name", ""):
-    #                     fw_old["BIOS"] = version
-    #                 elif "PSU" in  fw.get("dev_name", ""):
-    #                     fw_old["PSUFW"] = version
-    #                 elif "BIOS" == fw.get("dev_name", ""):
-    #                     fw_old["BIOS"] = version
-    #                 elif "CPLD" == fw.get("dev_name", ""):
-    #                     fw_old["CPLD"] = version
-    #                 elif "Front" in fw.get("dev_name", ""):
-    #                     fw_old["FRONTDISKBPCPLD"] = version
-    #                 elif "Rear" in fw.get("dev_name", ""):
-    #                     fw_old["REARDISKBPCPLD"] = version
-    #
-    #         # set syn mode
-    #         res_syn == {}
-    #         if args.type == "BMC":
-    #             preserveConfig = RestFunc.preserveBMCConfig(client, args.override)
-    #             if preserveConfig == {}:
-    #                 result.State("Failure")
-    #                 result.Message(["Cannot override config"])
-    #                 continue
-    #             elif preserveConfig.get('code') == 0:
-    #                 res_syn = RestFunc.syncmodeByRest(client, args.override, args.mode)
-    #             else:
-    #                 result.State("Failure")
-    #                 result.Message(["set override config error, " + str(preserveConfig.get('data'))])
-    #                 continue
-    #         elif args.type == "BIOS":
-    #             res_syn = RestFunc.syncmodeByRest(client, args.override, None)
-    #         else:
-    #             # 其他不需要本步骤
-    #             res_syn = {"code": 0}
-    #         if res_syn == {}:
-    #             result.State("Failure")
-    #             result.Message(["cannot set syncmode"])
-    #             continue
-    #         elif res_syn.get('code') != 0:
-    #             result.State("Failure")
-    #             result.Message(["set sync mode error, " + str(res_syn.get('data'))])
-    #             continue
-    #
-    #         # upload
-    #         res_upload = RestFunc.uploadfirmwareByRest(client, args.url)
-    #         if res_upload == {}:
-    #             result.State("Failure")
-    #             result.Message(["cannot upload firmware update file"])
-    #             continue
-    #         elif res_upload.get('code') != 0:
-    #             result.State("Failure")
-    #             result.Message(["upload firmware error, " + str(res_upload.get('data'))])
-    #             continue
-    #
-    #         # verify
-    #         time.sleep(20)
-    #         res_verify = RestFunc.getverifyresultByRest(client)
-    #         if res_verify == {}:
-    #             result.State("Failure")
-    #             result.Message(["cannot verify firmware update file"])
-    #             continue
-    #         elif res_verify.get('code') != 0:
-    #             result.State("Failure")
-    #             result.Message(["cannot verify firmware update file " + str(res_verify.get('data'))])
-    #             continue
-    #
-    #         # apply
-    #         task_dict = {"BMC": 0, "BIOS": 1, "PSUFW": 5, "CPLD": 2, "FRONTDISKBPCPLD": 3, "REARDISKBPCPLD": 4}
-    #         #
-    #         if getServerStatus(client) != "off" and args.type != "BMC":
-    #             time.sleep(10)
-    #             res_progress = RestFunc.getTaskInfoByRest(client)
-    #             if res_progress == {}:
-    #                 result.State("Failure")
-    #                 result.Message(["No apply task found in task list. Call interface api/maintenance/background/task_info returns: " + str(res_progress)])
-    #                 continue
-    #             elif res_progress.get('code') == 0 and res_progress.get('data') is not None:
-    #                 tasks = res_progress.get('data')
-    #                 task = None
-    #                 for t in tasks:
-    #                     if t["id"] == task_dict.get(args.type, -1):
-    #                         task = t
-    #                         break
-    #                 # 无任务则退出
-    #                 if task == None:
-    #                     result.State("Failure")
-    #                     result.Message(["No apply task found in task list." + str(res_progress)])
-    #                     continue
-    #                 if task["status"] == "FAILED":
-    #                     result.State("Failure")
-    #                     result.Message(["Apply task failed." + str(res_progress)])
-    #                     continue
-    #
-    #                 result.State('Success')
-    #                 result.Message([
-    #                     "Apply(FLASH) pending, host is power on now, image save in BMC FLASH and will apply later, trigger: poweroff, dcpowercycle, systemreboot. (TaskId=" + str(
-    #                         task_dict.get(args.type, 0)) + ")"])
-    #                 continue
-    #             else:
-    #                 result.State("Failure")
-    #                 result.Message(["No apply task found in task list." + res_progress])
-    #                 continue
-    #
-    #         else:
-    #             # max error number
-    #             error_count = 0
-    #             # max progress number
-    #             count = 0
-    #             # 100num  若进度10次都是100 则主动reset
-    #             count_100 = 0
-    #             # 循环查看apply进度
-    #             while True:
-    #                 #CPLD PUSU BIOS 的启动过程可能会1h, 因此从60改为180
-    #                 if args.type == "BMC" or args.type == "BIOS":
-    #                     if count > 60:
-    #                         break
-    #                 else:
-    #                     if count > 180:
-    #                         break
-    #                 if error_count > 10:
-    #                     break
-    #                 if count_100 > 5:
-    #                     break
-    #                 count = count + 1
-    #                 import time
-    #                 time.sleep(10)
-    #                 res_progress = RestFunc.getTaskInfoByRest(client)
-    #                 if res_progress == {}:
-    #                     error_count = error_count + 1
-    #                 elif res_progress.get('code') == 0 and res_progress.get('data') is not None:
-    #                     tasks = res_progress.get('data')
-    #                     task = None
-    #                     for t in tasks:
-    #                         if t["id"] == task_dict.get(args.type, -1):
-    #                             task = t
-    #                             break
-    #                     # 无任务则退出
-    #                     if task == None:
-    #                         result.State("Failure")
-    #                         result.Message(["No apply task found in task list."])
-    #                         break
-    #                     if task["status"] == "COMPLETE":
-    #                         break
-    #                     elif task["status"] == "FAILED":
-    #                         result.State("Failure")
-    #                         result.Message(["Apply(FLASH) failed."])
-    #                         break
-    #                     elif task["status"] == "CANCELED":
-    #                         result.State("Failure")
-    #                         result.Message(["Apply(FLASH) canceled."])
-    #                         break
-    #                     else:
-    #                         if str(task["progress"]) == 100:
-    #                             count_100 = count_100 + 1
-    #                 else:
-    #                     error_count = error_count + 1
-    #
-    #             # 判断apply是否结束
-    #             if result.State == "Failure":
-    #                 continue
-    #
-    #             #获取apply进度结束
-    #             if args.type != "BMC":
-    #                 if args.type == "BIOS":
-    #                     result.State('Success')
-    #                     #systemreboot 改为 poweron 2020年3月10日 小榕树 王小龙
-    #                     #2020年3月18日 set BIOS setup options will activate later 改为 BIOS will activate later
-    #                     result.Message([
-    #                         "Activate pending, host is power off now, BIOS will activate later, trigger: power on."])
-    #                 else:
-    #                     fw_res_new = RestFunc.getFwVersion(client)
-    #                     fw_new = {}
-    #                     if fw_res_new == {}:
-    #                         result.State("Failure")
-    #                         result.Message(["Failed to call BMC interface api/version_summary, response is none"])
-    #                     elif fw_res_new.get('code') == 0 and fw_res_new.get('data') is not None:
-    #                         fwdata = fw_res_new.get('data')
-    #                         for fw in fwdata:
-    #                             if fw.get('dev_version') == '':
-    #                                 version = "-"
-    #                             else:
-    #                                 index_version = fw.get('dev_version', "").find('(')
-    #                                 if index_version == -1:
-    #                                     version = fw.get('dev_version')
-    #                                 else:
-    #                                     version = fw.get('dev_version')[:index_version].strip()
-    #
-    #                             if "PSU" in fw.get("dev_name", ""):
-    #                                 fw_new["PSUFW"] = version
-    #                             elif "BIOS" == fw.get("dev_name", ""):
-    #                                 fw_new["BIOS"] = version
-    #                             elif "CPLD" == fw.get("dev_name", ""):
-    #                                 fw_new["CPLD"] = version
-    #                             elif "Front" in fw.get("dev_name", ""):
-    #                                 fw_new["FRONTDISKBPCPLD"] = version
-    #                             elif "Rear" in fw.get("dev_name", ""):
-    #                                 fw_new["REARDISKBPCPLD"] = version
-    #
-    #                         if args.type in fw_new:
-    #                             if args.type in fw_old:
-    #                                 versioncheck = str(args.type) + " update successfully, Version: image change from " + fw_old[args.type] + " to " + fw_new[args.type]
-    #                             else:
-    #                                 versioncheck = str(args.type) + " update successfully, new version: " + fw_new[args.type]
-    #                             result.State("Success")
-    #                             result.Message([versioncheck])
-    #                         else:
-    #                             versioncheck = " Cannot get " + str(args.type) + " version: " + str(fwdata)
-    #                             result.State("Failure")
-    #                             result.Message([versioncheck])
-    #                     else:
-    #                         result.State("Failure")
-    #                         result.Message(["get new fw information error, " + str(fw_res.get('data'))])
-    #             else:
-    #                 if args.mode == "Manual":
-    #                     # manual 需要手动重启bmc
-    #                     result.State('Success')
-    #                     result.Message(["Activate pending, host is power " + getServerStatus(
-    #                         client) + " now, image save in BMC FLASH and will apply later, trigger: bmcreboot."])
-    #
-    #             # 判断apply是否结束
-    #             if result.State == "Failure" or result.State == "Success":
-    #                 continue
-    #
-    #         # 未结束需要等待重启
-    #         # 查看bmc activate状态
-    #         # 并且刷新另一块
-    #         # 一般4 5分钟即可从备镜像启动成功
-    #         # 15分钟未启动则升级失败 从备份镜像启动，启动成功需要rollback
-    #         # 10分钟内启动成功则说明刷新成功
-    #         time.sleep(180)
-    #         uname = client.username
-    #         pword = client.passcode
-    #         # web service 是否启动
-    #         reset_try_count = 0
-    #         headers = {}
-    #         while True:
-    #             time.sleep(20)
-    #             reset_try_count = reset_try_count + 1
-    #             # 10分钟未启动 尝试使用 admin 登陆
-    #             if reset_try_count == 30:
-    #                 client.username = "admin"
-    #                 client.passcode = "admin"
-    #             # 使用默认用户admin尝试登陆
-    #             if reset_try_count > 32:
-    #                 result.State('Failure')
-    #                 result.Message(["Cannot login BMC."])
-    #                 break
-    #             try:
-    #                 headers = RestFunc.login_M6(client)
-    #                 if headers != {}:
-    #                     with open(session_path, 'w') as new_session:
-    #                         new_session.write(str(headers))
-    #                     break
-    #             except Exception as e:
-    #                 continue
-    #
-    #         if result.State == 'Failure':
-    #             client.username = uname
-    #             client.passcode = pword
-    #             continue
-    #
-    #         client.setHearder(headers)
-    #
-    #         # BMC有bug 回滚的时候CPU利用率超高不准 可能出现都不是active的bug
-    #         # 查看BMC启动的主备
-    #         fw_now = {}
-    #         bmcfw_try_count = 0
-    #         bmcfw_error_count = 0
-    #         # 放弃了
-    #         while False:
-    #             fw_now = {}
-    #             if bmcfw_try_count > 9:
-    #                 result.State('Failure')
-    #                 result.Message(["Get BMC active image fw version failed"])
-    #                 break
-    #             else:
-    #                 bmcfw_try_count = bmcfw_try_count + 1
-    #             if bmcfw_error_count > 3:
-    #                 result.State('Failure')
-    #                 result.Message(["Get BMC fw version failed"])
-    #                 break
-    #
-    #             res_fw = RestFunc.getFwVersion(client)
-    #             if res_fw == {}:
-    #                 bmcfw_error_count = bmcfw_error_count + 1
-    #             elif res_fw.get('code') == 0 and res_fw.get('data') is not None:
-    #                 fwlist = res_fw.get('data')
-    #                 for fw in fwlist:
-    #                     if fw.get('dev_version') == '':
-    #                         version = "0.00.00"
-    #                     else:
-    #                         index_version = fw.get('dev_version', "").find('(')
-    #                         if index_version == -1:
-    #                             version = fw.get('dev_version')
-    #                         else:
-    #                             version = fw.get('dev_version')[
-    #                                       :index_version].strip()
-    #                     if "BMC0" in fw.get("dev_name", ""):
-    #                         fw_now["BMC0"] = version
-    #                         if "Inactivate" in fw.get("dev_name", ""):
-    #                             fw_now["InactivateBMC"] = "BMC0"
-    #                         else:
-    #                             fw_now["ActivateBMC"] = "BMC0"
-    #                     elif "BMC1" in fw.get("dev_name", ""):
-    #                         fw_now["BMC1"] = version
-    #                         if "Inactivate" in fw.get("dev_name", ""):
-    #                             fw_now["InactivateBMC"] = "BMC1"
-    #                         else:
-    #                             fw_now["ActivateBMC"] = "BMC1"
-    #                     if "ActivateBMC" in fw_now:
-    #                         break
-    #                 if "BMC0" not in fw_now and "BMC1" not in fw_now:
-    #                     continue
-    #                 if "ActivateBMC" not in fw_now:
-    #                     continue
-    #                 if "ActivateBMC" in fw_now and fw_now[fw_now["ActivateBMC"]] != "0.00.00":
-    #                     break
-    #             else:
-    #                 bmcfw_error_count = bmcfw_error_count + 1
-    #             time.sleep(20)
-    #
-    #         res_ver = IpmiFunc.getMcInfoByIpmi(client)
-    #         # {'code': 0, 'data': {'device_id': 32, 'device_revision': 1, 'manufacturer_id': 37945, 'firmware_revision': '15.11', 'ipmi_version': '2.0', 'manufacturer_name': 'Unknown (0x9439)', 'product_id': '514 (0x0202)', 'product_name': 'Unknown (0x202)', 'device_available': 'yes', 'provides_device_sdrs': 'no', 'additional_device_support': 'Sensor Device;SDR Repository Device;SEL Device;FRU Inventory Device;IPMB Event Receiver;IPMB Event Generator;Chassis Device', 'aux_firmware_rev_info': '0x00;0x00;0x00;0x00'}}
-    #         image1_update_info = ""
-    #         image2_update_info = ""
-    #         if 'code' in res_ver and res_ver.get("code", 1) == 0:
-    #             #version_new = res_ver.get("data").get("firmware_revision")
-    #             version_12 = res_ver.get("data").get("firmware_revision")
-    #             version_3 = int(res_ver.get("data").get("aux_firmware_rev_info").split(";")[0],16)
-    #             version_new = version_12 + "." + str(version_3)
-    #             if fw_old.get("ActivateBMC","") == "BMC1":
-    #                 image1_update_info = "BMC update successfully, Version: image1 change from " + fw_old.get(
-    #                     "BMC0","-") + " to " + version_new
-    #             elif fw_old.get("ActivateBMC","") == "BMC0":
-    #                 image2_update_info = "BMC update successfully, Version: image2 change from " + fw_old.get(
-    #                     "BMC1","-") + " to " + version_new
-    #             else:
-    #                 image1_update_info = "BMC update successfully, new version: " + version_new
-    #         else:
-    #             result.State("Failure")
-    #             result.Message(["Flash image " + fw_old.get("InactivateBMC","") + " error." + res_ver.get("data", "")])
-    #             continue
-    #
-    #         # 校验第二个镜像
-    #         image_to_set2 = ""
-    #         if "ActivateBMC" in fw_old:
-    #             if fw_old["ActivateBMC"] == "BMC1":
-    #                 image_to_set2 = "Image2"
-    #             elif fw_old["ActivateBMC"] == "BMC0":
-    #                 image_to_set2 = "Image1"
-    #
-    #         # max error number
-    #         error_count2 = 0
-    #         # max progress number
-    #         count2 = 0
-    #         # 100num  若进度10次都是100 则主动reset
-    #         count_1002 = 0
-    #         # 循环查看apply进度
-    #         error_info2 = ""
-    #         while True:
-    #             if count2 > 120:
-    #                 result.State("Abort")
-    #                 result.Message(["Apply cost too much time, please check if upgrade is ok or not. Last response is " + error_info2])
-    #                 break
-    #             if error_count2 > 10:
-    #                 result.State("Abort")
-    #                 result.Message(["Get apply progress error, please check is upgraded or not. Last response is " + error_info2])
-    #                 # check是否升级成功
-    #                 break
-    #             if count_1002 > 5:
-    #                 result.State("Abort")
-    #                 result.Message(["Apply progress is 100% but it does not complete, check if upgrade is ok or not. Last response is " + error_info2])
-    #                 break
-    #             count2 = count2 + 1
-    #             import time
-    #             time.sleep(10)
-    #             res_progress = RestFunc.getTaskInfoByRest(client)
-    #             if res_progress == {}:
-    #                 error_count2 = error_count2 + 1
-    #                 error_info2 = "Failed to call BMC interface api/maintenance/background/task_info ,response is none"
-    #             elif res_progress.get('code') == 0 and res_progress.get('data') is not None:
-    #                 tasks = res_progress.get('data')
-    #                 task = None
-    #                 for t in tasks:
-    #                     if t["id"] == task_dict.get(args.type, -1):
-    #                         task = t
-    #                         break
-    #                 # 无任务则退出
-    #                 if task == None:
-    #                     break
-    #                 error_info2 = str(task)
-    #                 if task["status"] == "COMPLETE":
-    #                     break
-    #                 elif task["status"] == "FAILED":
-    #                     result.State("Failure")
-    #                     result.Message(["Apply(FLASH) failed."])
-    #                     break
-    #                 elif task["status"] == "CANCELED":
-    #                     result.State("Failure")
-    #                     result.Message(["Apply(FLASH) canceled."])
-    #                     break
-    #                 else:
-    #                     if str(task["progress"]) == 100:
-    #                         count_1002 = count_1002 + 1
-    #
-    #             else:
-    #                 error_count2 = error_count2 + 1
-    #                 error_info2 = str(res_progress.get('data'))
-    #
-    #         # 判断第二个bmc apply是否结束
-    #         if result.State == "Failure" or result.State == "Abort" :
-    #             if image1_update_info == "":
-    #                 image1_update_info = "BMC image1 update failed: " + result.Message[0]
-    #             if image2_update_info == "":
-    #                 image2_update_info = "BMC image2 update failed: " + result.Message[0]
-    #             result = ResultBean()
-    #             result.State("Success")
-    #             result.Message([image1_update_info, image2_update_info])
-    #             continue
-    #         # 获取第二个bmc的版本
-    #         fw_now2 = {}
-    #         bmcfw_try_count2 = 0
-    #         bmcfw_error_count2 = 0
-    #         while True:
-    #             fw_now2 = {}
-    #             if bmcfw_try_count2 > 3:
-    #                 result.State('Failure')
-    #                 result.Message(["Flash BMC inactive image failed: " + str(res_fw2.get('data'))])
-    #                 break
-    #             else:
-    #                 bmcfw_try_count2 = bmcfw_try_count2 + 1
-    #                 time.sleep(20)
-    #             if bmcfw_error_count2 > 3:
-    #                 result.State('Failure')
-    #                 result.Message(["Get BMC fw version failed(inactiveBMC): " + str(res_fw2.get('data'))])
-    #                 break
-    #
-    #             res_fw2 = RestFunc.getFwVersion(client)
-    #             if res_fw2 == {}:
-    #                 bmcfw_error_count2 = bmcfw_error_count2 + 1
-    #             elif res_fw2.get('code') == 0 and res_fw2.get('data') is not None:
-    #                 fwlist2 = res_fw2.get('data')
-    #                 for fw in fwlist2:
-    #                     if fw.get('dev_version') == '':
-    #                         version = "0.00.00"
-    #                     else:
-    #                         index_version = fw.get('dev_version', "").find('(')
-    #                         if index_version == -1:
-    #                             version = fw.get('dev_version')
-    #                         else:
-    #                             version = fw.get('dev_version')[
-    #                                       :index_version].strip()
-    #                     if "BMC0" in fw.get("dev_name", ""):
-    #                         fw_now2["BMC0"] = version
-    #                         if "Inactivate" in fw.get("dev_name", ""):
-    #                             fw_now2["InactivateBMC"] = "BMC0"
-    #                         else:
-    #                             fw_now2["ActivateBMC"] = "BMC0"
-    #                     elif "BMC1" in fw.get("dev_name", ""):
-    #                         fw_now2["BMC1"] = version
-    #                         if "Inactivate" in fw.get("dev_name", ""):
-    #                             fw_now2["InactivateBMC"] = "BMC1"
-    #                         else:
-    #                             fw_now2["ActivateBMC"] = "BMC1"
-    #                     if "ActivateBMC" in fw_now2 and "InactivateBMC" in fw_now2:
-    #                         break
-    #                 if "BMC0" not in fw_now2 and "BMC1" not in fw_now2:
-    #                     bmcfw_error_count2 = bmcfw_error_count2 + 1
-    #                     continue
-    #                 if "ActivateBMC" not in fw_now2 or "InactivateBMC" not in fw_now2:
-    #                     bmcfw_error_count2 = bmcfw_error_count2 + 1
-    #                     continue
-    #                 if fw_now2["BMC0"] == fw_now2["BMC1"]:
-    #                     break
-    #             else:
-    #                 bmcfw_error_count2 = bmcfw_error_count2 + 1
-    #
-    #         if result.State == 'Failure':
-    #             if image1_update_info == "":
-    #                 image1_update_info = "BMC image1 update failed: " + result.Message[0]
-    #             if image2_update_info == "":
-    #                 image2_update_info = "BMC image2 update failed: " + result.Message[0]
-    #             result = ResultBean()
-    #             result.State("Success")
-    #             result.Message([image1_update_info, image2_update_info])
-    #             continue
-    #
-    #         if "ActivateBMC" in fw_old:
-    #             if fw_old["ActivateBMC"] == "BMC1":
-    #                 image2_update_info = "BMC update successfully, Version: image2 change from " + fw_old.get("BMC1","-") + " to " + fw_now2.get("BMC1","-")
-    #                 image1_update_info = "BMC update successfully, Version: image1 change from " + fw_old.get("BMC0","-") + " to " + fw_now2.get("BMC0","-")
-    #             elif fw_old["ActivateBMC"] == "BMC0":
-    #                 image1_update_info = "BMC update successfully, Version: image1 change from " + fw_old.get("BMC0","-") + " to " + fw_now2.get("BMC0","-")
-    #                 image2_update_info = "BMC update successfully, Version: image2 change from " + fw_old.get("BMC1","-") + " to " + fw_now2.get("BMC1","-")
-    #
-    #         result.State("Success")
-    #         result.Message([image1_update_info, image2_update_info])
-    #         continue
 
     def getusergroup(self, client, args):
         headers = RestFunc.login_M6(client)
         if headers == {}:
             login_res = ResultBean()
             login_res.State("Failure")
             login_res.Message(
@@ -12065,15 +11422,14 @@
                 res.State("Failure")
                 res.Message(["get psu count failed."])
         except Exception as e:
             res.State("Failure")
             res.Message([str(e)])
         return res
 
-
     def getbootimage(self, client, args):
         result = ResultBean()
         result.State("Not Support")
         result.Message(['The M6 model does not support this feature.'])
         return result
 
     def setbootimage(self, client, args):
@@ -12405,14 +11761,21 @@
 
     def setsmtp(self, client, args):
         result = ResultBean()
         result.State("Not Support")
         result.Message(['The M6 model does not support this feature.'])
         return result
 
+    def remoteFWUpdate(self, client, args):
+        result = ResultBean()
+        result.State("Not Support")
+        result.Message(['The M6 model does not support this feature.'])
+        return result
+
+
 
 # 检查日志进度，进度到100 后下载文件
 def getProgressAndDown(client, args):
     bmcres = ResultBean()
     state = 0
     count = 0
     error_count = 0
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonM6_41401.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6_41401.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonM6_4140a.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6_4140a.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/CommonM7.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM7.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,15 +435,15 @@
             return value_map.get(str(origin_value), None)
 
     def setbios(self, client, args):
         res = ResultBean()
         attr_dict = {}
         # 读取映射文件
         mapper_result = self._get_xml_mapper(args, 'value', 'cmd')
-        args.list = False
+        # args.list = False
         if mapper_result[0]:
             if 'list' in args and args.list:  # 打印信息
                 help_list = []
                 for key, value in mapper_result[1].items():
                     help_list.append('{:<35}: {}'.format(value['description'], list(value['setter'].keys())))
                 res.Message(help_list)
                 res.State('Success')
@@ -593,24 +593,28 @@
         if not conditionflag:
             res.State('Failure')
             res.Message([conditionmessage])
             # logout
             RedfishFunc.logout(client, login_id, login_header)
             return res
 
-        set_result = RedfishFunc.setBiosV1SDByRedfish(client, user_bios, get_result.get('headers'), login_header)
+        user_bios_f = self.formatBiosPatchBody(user_bios)
+        set_result = RedfishFunc.setBiosV1SDByRedfish(client, user_bios_f, get_result.get('headers'), login_header)
         if set_result.get('code') == 0:
             res.Message([''])
             res.State("Success")
         else:
             res.Message([set_result.get('data')])
             res.State('Failure')
         RedfishFunc.logout(client, login_id, login_header)
         return res
 
+    def formatBiosPatchBody(self, user_bios):
+        return user_bios
+
     def _get_xml_file(self):
         xml_path = os.path.join(IpmiFunc.command_path, "bios") + os.path.sep
         return xml_path + 'M7.xml'
 
     def _get_xml_mapper(self, args, key, value):
         """
             {
@@ -772,15 +776,15 @@
                     if conditionvalue == conditonvalue_current:
                         continue
                     else:
                         errorlist.append(self.formatCondition(conditionkeyshow, conditionvalueshow, conditionvaluedict.get(conditonvalue_current), 3))
                         continue
             if errorlist != []:
                 errorinfo = ",".join(errorlist)
-                errordict[bios_all_info.get(bioskey).get("description")]=errorinfo
+                errordict[bios_all_info.get(bioskey).get("description")] = errorinfo
         if errordict == {}:
             return True, None
         else:
             return False, errordict
 
     def getbiosraw(self, client, args):
         bios_result = ResultBean()
@@ -991,15 +995,16 @@
                             break
                 else:
                     bios_result.Message(['not support setting value for [{}]'.format(key)])
                     bios_result.State('Failure')
                     break
             else:
                 # 调用接口设置
-                set_server_result = RedfishFunc.setBiosV1SDByRedfish(client, set_bios, server_result.get('headers'),
+                user_bios_f = self.formatBiosPatchBody(set_bios)
+                set_server_result = RedfishFunc.setBiosV1SDByRedfish(client, user_bios_f, server_result.get('headers'),
                                                                      login_header)
                 if set_server_result.get('code') == 0:
                     bios_result.State("Success")
                     bios_result.Message([])
                 else:
                     bios_result.State('Failure')
                     bios_result.Message([set_server_result.get('data')])
@@ -2214,14 +2219,16 @@
         args.session_path = session_path
         if args.type == "BMC" or args.type == "BMC_PFR":
             result = self.updatebmc(client, args)
         elif args.type == "BIOS" or args.type == "BIOS_PFR":
             result = self.updatebios(client, args)
         elif args.type == "CPLD" or args.type == "DISKBPCPLD" or args.type == "CPLD_PFR":
             result = self.updatecpld1(client, args)
+        elif args.type == "PSUFW":
+            result = self.updatepsu1(client, args)
         else:
             result.State("Not Support")
             result.Message(["Update firmware only support bmc, bios and cpld"])
         return result
 
     def updatebmc(self, client, args):
         result = ResultBean()
@@ -3081,15 +3088,15 @@
                     continue
 
                 client.setHearder(headers)
 
                 ctr_info = IpmiFunc.powerControlByIpmi(client, "on")
                 if ctr_info:
                     if ctr_info.get('code') == 0 and ctr_info.get('data') is not None and ctr_info.get('data').get(
-                            'result') is not None:
+                            'status') is not None:
                         result.State("Success")
                         result.Message(["Set power on success"])
                         self.wirte_log(log_path, "Restart", "Set power on success", result.Message)
                     else:
                         result.State("Failure")
                         result.Message(['set power failed: ' + ctr_info.get('data', ' ')])
                         self.wirte_log(log_path, "Restart", "Set power on failed", result.Message)
@@ -3473,14 +3480,340 @@
                         result.Message(["get new fw information error, " + str(fw_res.get('data'))])
                         self.wirte_log(log_path, "Activate", "Data Verify Failed", result.Message)
 
                 # 判断apply是否结束
                 if result.State == "Failure" or result.State == "Success":
                     continue
 
+    def updatepsu(self, client, args):
+        args.type = None
+        args.auto_flag = None
+        result = self.fwupdate(client, args)
+        return result
+
+    def updatepsu1(self, client, args):
+        result = ResultBean()
+        log_path = args.log_path
+        session_path = args.session_path
+        upgrade_count = 0
+        while True:
+            # 判断session是否存在，存在则logout&del
+            if os.path.exists(session_path):
+                with open(session_path, 'r') as oldsession:
+                    headers = oldsession.read()
+                    headers_json = json.loads(str(headers).replace("'", '"'))
+                    client.setHearder(headers_json)
+                    # logout
+                    RestFunc.logout(client)  # 删除session
+                if os.path.exists(session_path):
+                    os.remove(session_path)
+            # 删除
+            if result.State == "Success":
+                return result
+            elif result.State == "Abort":
+                result.State = "Failure"
+                return result
+            else:
+                if upgrade_count > retry_count:
+                    return result
+                else:
+                    if upgrade_count >= 1:
+                        # 重新升级 初始化result
+                        self.wirte_log(log_path, "Upload File", "Upgrade Retry " + str(upgrade_count) + " Times", "")
+                        result = ResultBean()
+                    upgrade_count = upgrade_count + 1
+            # login
+            headers = {}
+            logcount = 0
+            while True:
+                # 等6分钟
+                if logcount > 18:
+                    break
+                else:
+                    logcount = logcount + 1
+                    time.sleep(20)
+                # login
+                headers = RestFunc.login_M6(client)
+                if headers != {}:
+                    # 记录session
+                    with open(session_path, 'w') as new_session:
+                        new_session.write(str(headers))
+                    client.setHearder(headers)
+                    break
+                else:
+                    # print(ftime() + "Create session failed")
+                    self.wirte_log(log_path, "Upload File", "Connect Failed", "Connect number:" + str(logcount))
+            # 10次无法登陆 不再重试
+            if headers == {}:
+                result.State("Failure")
+                result.Message(["Cannot log in to BMC."])
+                return result
+            # get old version
+            fw_res = RestFunc.getFwVersion(client)
+            fw_old = {}
+            if fw_res == {}:
+                self.wirte_log(log_path, "Upload File", "Connect Failed", "Cannot get current firmware version.")
+            elif fw_res.get('code') == 0 and fw_res.get('data') is not None:
+                fwdata = fw_res.get('data')
+                for fw in fwdata:
+                    if fw.get('dev_version') == '':
+                        version = "-"
+                    else:
+                        index_version = fw.get('dev_version', "").find('(')
+                        if index_version == -1:
+                            version = fw.get('dev_version')
+                        else:
+                            version = fw.get('dev_version')[:index_version].strip()
+                    if "PSU" in fw.get("dev_name", ""):
+                        fw_old["PSUFW"] = version
+                        break
+                if args.type not in fw_old:
+                    version_info = "Cannot get current firmware version, " + str(fwdata)
+                    self.wirte_log(log_path, "Upload File", "Connect Failed", version_info)
+            else:
+                version_info = "Cannot get current firmware version, " + str(fw_res.get('data'))
+                self.wirte_log(log_path, "Upload File", "Connect Failed", version_info)
+
+            # PSU 升级自动重启，先关机
+            #
+            flag = False
+            if args.mode == "Auto" and self.getServerStatus(client) != "off":
+                flag = True
+                choices = {'on': 1, 'off': 0, 'cycle': 2, 'reset': 3, 'shutdown': 5}
+                Power = RestFunc.setM6PowerByRest(client, choices["off"])
+                if Power.get('code') == 0 and Power.get('data') is not None:
+                    off_count = 0
+                    while True:
+                        if self.getServerStatus(client) == "off" or off_count > 5:
+                            break
+                        time.sleep(10)
+                        off_count += 1
+                    if self.getServerStatus(client) != "off":
+                        result.State('Failure')
+                        result.Message(['set power off complete, but get power status error.'])
+                        self.wirte_log(log_path, "Auto Reset Server", "Get Power Status Error", result.Message)
+                        continue
+                    else:
+                        self.wirte_log(log_path, "Set Power Off", "Successfully", "")
+                else:
+                    result.State('Failure')
+                    result.Message(['set power off failed.'])
+                    self.wirte_log(log_path, "Auto Reset Server", "Set Power Off Failed", result.Message)
+                    continue
+
+            # set syn mode
+            RestFunc.securityCheckByRest(client)
+            self.wirte_log(log_path, "Upload File", "Start", "")
+
+            # upload
+            res_upload = RestFunc.uploadfirmwareByRest1(client, args.url)
+            if res_upload == {}:
+                result.State("Failure")
+                result.Message(["cannot upload firmware update file"])
+                self.wirte_log(log_path, "Upload File", "Connect Failed", "Exceptions occurred while calling interface")
+                continue
+            elif res_upload.get('code') == 0:
+                self.wirte_log(log_path, "Upload File", "Success", "")
+            else:
+                result.State("Failure")
+                result.Message(["upload firmware error, " + str(res_upload.get('data'))])
+                if res_upload.get('data', 0) == 1 or res_upload.get('data', 0) == 2:
+                    self.wirte_log(log_path, "Upload File", "File Not Exist", str(res_upload.get('data')))
+                elif res_upload.get('data', 0) == 404:
+                    self.wirte_log(log_path, "Upload File", "Invalid URI", str(res_upload.get('data')))
+                else:
+                    self.wirte_log(log_path, "Upload File", "Connect Failed", str(res_upload.get('data')))
+                continue
+
+            # verify
+            time.sleep(20)
+            self.wirte_log(log_path, "File Verify", "Start", "")
+            res_verify = RestFunc.getverifyresultByRest(client)
+            if res_verify == {}:
+                result.State("Failure")
+                result.Message(["cannot verify firmware update file"])
+                self.wirte_log(log_path, "File Verify", "Connect Failed",
+                               "Exceptions occurred while calling interface")
+                continue
+            elif res_verify.get('code') == 0:
+                self.wirte_log(log_path, "File Verify", "Success", "")
+            else:
+                result.State("Failure")
+                result.Message(["cannot verify firmware update file, " + str(res_verify.get('data'))])
+                self.wirte_log(log_path, "File Verify", "Data Verify Failed", str(res_verify.get('data')))
+                continue
+
+            # apply
+            task_dict = {"BMC": 0, "BIOS": 1, "PSUFW": 5, "CPLD": 2, "FRONTDISKBPCPLD": 3, "REARDISKBPCPLD": 4,
+                         "CPLD_PFR": 10}
+            if self.getServerStatus(client) != "off":
+                time.sleep(10)
+                res_progress = RestFunc.getTaskInfoByRest(client)
+                if res_progress == {}:
+                    result.State("Failure")
+                    result.Message(["No apply task found in task list. Call interface "
+                                    "api/maintenance/background/task_info returns: " + str(res_progress)])
+                    self.wirte_log(log_path, "Apply", "Image and Target Component Mismatch", result.Message)
+                    continue
+                elif res_progress.get('code') == 0 and res_progress.get('data') is not None:
+                    tasks = res_progress.get('data')
+                    task = None
+                    for t in tasks:
+                        if t["id"] == task_dict.get(args.type, -1):
+                            task = t
+                            break
+                    # 无任务则退出
+                    if task is None:
+                        result.State("Failure")
+                        result.Message(["No apply task found in task list." + str(res_progress)])
+                        self.wirte_log(log_path, "Apply", "Image and Target Component Mismatch", result.Message)
+                        continue
+                    if task["status"] == "FAILED":
+                        result.State("Failure")
+                        result.Message(["Apply task failed." + str(res_progress)])
+                        self.wirte_log(log_path, "Apply", "Data Verify Failed", result.Message)
+                        continue
+
+                    result.State('Success')
+                    result.Message(["Apply(FLASH) pending, host is power on now, image save in BMC FLASH and will "
+                                    "apply later, trigger: poweroff, dcpowercycle, systemreboot. (TaskId=" +
+                                    str(task_dict.get(args.type, 0)) + ")"])
+                    self.wirte_log(log_path, "Apply", "Finish", result.Message)
+                    continue
+                else:
+                    result.State("Failure")
+                    result.Message(["No apply task found in task list." + str(res_progress)])
+                    self.wirte_log(log_path, "Apply", "Image and Target Component Mismatch", result.Message)
+                    continue
+            else:
+                self.wirte_log(log_path, "Apply", "Start", "")
+                # max error number
+                error_count = 0
+                # max progress number
+                count = 0
+                # 100num  若进度10次都是100 则主动reset
+                count_100 = 0
+                # 循环查看apply进度
+                error_info = ""
+                while True:
+                    if count > 60:
+                        break
+                    if error_count > 10:
+                        break
+                    if count_100 > 5:
+                        break
+                    count = count + 1
+                    time.sleep(20)
+                    res_progress = RestFunc.getTaskInfoByRest(client)
+                    if res_progress == {}:
+                        error_count = error_count + 1
+                        error_info = 'Failed to call BMC interface api/maintenance/background/task_info ,response is none'
+                    elif res_progress.get('code') == 0 and res_progress.get('data') is not None:
+                        tasks = res_progress.get('data')
+                        task = None
+                        for t in tasks:
+                            if t["id"] == task_dict.get(args.type, -1):
+                                task = t
+                                break
+                        # 无任务则退出
+                        if task is None:
+                            result.State("Failure")
+                            result.Message(["No apply task found in task list."])
+                            self.wirte_log(log_path, "Apply", "Image and Target Component Mismatch", result.Message)
+                            break
+                        error_info = str(task)
+                        if task["status"] == "COMPLETE":
+                            break
+                        elif task["status"] == "FAILED":
+                            self.wirte_log(log_path, "Apply", "Finish", "Apply(FLASH) failed.")
+                            result.State("Failure")
+                            result.Message(["Apply(FLASH) failed."])
+                            break
+                        elif task["status"] == "CANCELED":
+                            self.wirte_log(log_path, "Apply", "Finish", "Apply(FLASH) canceled.")
+                            result.State("Failure")
+                            result.Message(["Apply(FLASH) canceled."])
+                            break
+                        else:
+                            self.wirte_log(log_path, "Apply", "In Progress",
+                                           "progress:" + str(task["progress"]) + "%")
+                            if str(task["progress"]) == 100:
+                                count_100 = count_100 + 1
+                    else:
+                        error_count = error_count + 1
+                        error_info = str(res_progress.get('data'))
+
+                # 判断apply是否结束
+                if result.State == "Failure":
+                    continue
+
+                # 获取apply进度结束
+                self.wirte_log(log_path, "Apply", "Success", "")
+
+                fw_res_new = RestFunc.getFwVersion(client)
+                fw_new = {}
+                if fw_res_new == {}:
+                    result.State("Failure")
+                    result.Message(
+                        ["Failed to call BMC interface api/version_summary, response is none"])
+                    self.wirte_log(log_path, "Activate", "Data Verify Failed", result.Message)
+                elif fw_res_new.get('code') == 0 and fw_res_new.get('data') is not None:
+                    fwdata = fw_res_new.get('data')
+                    for fw in fwdata:
+                        if fw.get('dev_version') == '':
+                            version = "-"
+                        else:
+                            index_version = fw.get('dev_version', "").find('(')
+                            if index_version == -1:
+                                version = fw.get('dev_version')
+                            else:
+                                version = fw.get('dev_version')[:index_version].strip()
+                        if "PSU" in fw.get("dev_name", ""):
+                            fw_new["PSUFW"] = version
+                            break
+
+                    if args.type in fw_new:
+                        if args.type in fw_old:
+                            versioncheck = str(args.type) + " update successfully, Version: image change from " + fw_old[args.type] + " to " + fw_new[args.type]
+                        else:
+                            versioncheck = str(args.type) + " update successfully, new version: " + fw_new[args.type]
+                        result.State("Success")
+                        result.Message([versioncheck])
+                        self.wirte_log(log_path, "Activate", "Success", versioncheck)
+                    else:
+                        versioncheck = " Cannot get " + str(args.type) + " version: " + str(fwdata)
+                        result.State("Failure")
+                        result.Message([versioncheck])
+                        self.wirte_log(log_path, "Upload File", "Connect Failed", versioncheck)
+                else:
+                    result.State("Failure")
+                    result.Message(["get new fw information error, " + str(fw_res.get('data'))])
+                    self.wirte_log(log_path, "Activate", "Data Verify Failed", result.Message)
+
+                if flag:
+                    result = ResultBean()
+                    ctr_info = IpmiFunc.powerControlByIpmi(client, "on")
+                    if ctr_info:
+                        if ctr_info.get('code') == 0 and ctr_info.get('data') is not None and ctr_info.get('data').get('result') is not None:
+                            result.State("Success")
+                            result.Message(['Update PSU complete, system auto power on success'])
+                            self.wirte_log(log_path, "Restart", "Set power on success", result.Message)
+                        else:
+                            result.State("Failure")
+                            result.Message(['Update PSU complete. But system auto reset failed, please power on manually ...'])
+                            self.wirte_log(log_path, "Restart", "Set power on failed", result.Message)
+                    else:
+                        result.State("Failure")
+                        result.Message(['set power failed.please check server manually'])
+                        self.wirte_log(log_path, "Restart", "Set power on failed", result.Message)
+
+                # 判断reboot是否结束
+                if result.State == "Failure" or result.State == "Success":
+                    continue
+
     def ftime(self, ff="%Y-%m-%d %H:%M:%S "):
         try:
             localtime = time.localtime()
             f_localtime = time.strftime(ff, localtime)
             return f_localtime
         except:
             return ""
@@ -5200,26 +5533,14 @@
 
     def setnetworklink(self, client, args):
         result = ResultBean()
         result.State("Not Support")
         result.Message(['The M7 model does not support this feature.'])
         return result
 
-    # def getpowerrestore(self, client, args):
-    #     result = ResultBean()
-    #     result.State("Not Support")
-    #     result.Message(['The M7 model does not support this feature.'])
-    #     return result
-    #
-    # def setpowerrestore(self, client, args):
-    #     result = ResultBean()
-    #     result.State("Not Support")
-    #     result.Message(['The M7 model does not support this feature.'])
-    #     return result
-
     def setpsupeak(self, client, args):
         result = ResultBean()
         result.State("Not Support")
         result.Message(['The M7 model does not support this feature.'])
         return result
 
     def getpreserveconfig(self, client, args):
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/I24M6.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/I24M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/IBase.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/IBase.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/NF5180M5.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5180M5.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
                     with open(download_res.get("data"), 'rb') as f:
                         a = f.read()
                     try:
                         b = a.decode("utf-8")
                     except BaseException:
                         # 需要解码
                         import platform
-                        if platform.system() == 'Linux':
+                        if platform.system() == 'Linux' or platform.system() == 'Darwin':
                             cmd = '/tools//blackbox_decrypt/blackbox_decrypt '
                         else:
                             cmd = "\\tools\\blackbox_decrypt\\blackbox_decrypt.exe "
                         cmd = os.path.dirname(os.path.dirname(
                             __file__)) + cmd + download_res.get("data") + " > " + os.path.join(bbl_path, "res")
                         try:
                             pathnow = os.getcwd()
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/NF5280M5.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/NF5280M5_435.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5_435.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/NF5280M5_436.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5_436.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/NS5160M6.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/NS5160M6.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
                 if logcount > 18:
                     break
                 else:
                     logcount = logcount + 1
                     import time
                     time.sleep(20)
                 # login
-                headers = RestFunc.loginNoEncrypt(client)
+                headers = RestFunc.login_M6(client)
                 if headers != {}:
                     # 记录session
                     with open(session_path, 'w') as new_session:
                         new_session.write(str(headers))
                     client.setHearder(headers)
                     client.setHearder(headers)
                     break
@@ -677,15 +677,15 @@
                 # 使用默认用户admin尝试登陆
                 if reset_try_count > 32:
                     result.State('Failure')
                     result.Message(["Cannot login BMC."])
                     wirte_log(log_path, "Activate", "BMC Reboot Failed", result.Message)
                     break
                 try:
-                    headers = RestFunc.loginNoEncrypt(client)
+                    headers = RestFunc.login_M6(client)
                     if headers != {}:
                         with open(session_path, 'w') as new_session:
                             new_session.write(str(headers))
                         break
                 except Exception as e:
                     continue
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/ResEntity.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/ResEntity.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/interface/SA5212M5Impl.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/interface/SA5212M5Impl.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/route/route.yml` & `inspursmsdk-2.1.0/inspur_sm_sdk/route/route.yml`

 * *Files 15% similar despite different names*

```diff
@@ -106,29 +106,41 @@
     common: I24M6
 I24A5:
     common: I24M6
 NS5160M6:
     common: NS5160M6
 NF5468M7:
     common: CommonM7
+    1.3505: CommonM7_13505
 NF5688M7:
     common: CommonM7
+    1.3505: CommonM7_13505
 NS5170-M7-A0-R0-00:
     common: CommonM7
+    1.3505: CommonM7_13505
 NF5180M7:
     common: CommonM7
+    1.3505: CommonM7_13505
 NF5280M7:
     common: CommonM7
+    1.3505: CommonM7_13505
 NF8260M7:
     common: CommonM7
+    1.3505: CommonM7_13505
 I24M7:
     common: CommonM7
+    1.3505: CommonM7_13505
 NF5180A7:
     common: CommonA7
+    1.1308: CommonA7_11308
 NF5280A7:
     common: CommonA7
+    1.1308: CommonA7_11308
 I24A7:
     common: CommonA7
+    1.1308: CommonA7_11308
 NF5468A7:
     common: CommonA7
+    1.1308: CommonA7_11308
 NF5688A7:
-    common: CommonA7
+    common: CommonA7
+    1.1308: CommonA7_11308
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/util/HostTypeJudge.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/util/HostTypeJudge.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     # raw 0x3c 0x42 获取型号不通用，仅在Korea定制化使用。5288返回5280
 
     def getHostInfoByRaw(self, args):
         sysstr = platform.system()
         if sysstr == 'Windows':
             cmd = "..\\tools\\ipmitool\\ipmitool.exe -I lanplus -H " + args.host + \
                 " -U " + args.username + " -P " + args.password + " raw 0x3c 0x42 2>nul"
-        elif sysstr == 'Linux':
+        elif sysstr == 'Linux' or sysstr == 'Darwin':
             cmd = "ipmitool -I lanplus -H " + args.host + " -U " + args.username + \
                 " -P " + args.password + " raw 0x3c 0x42" + " 2>/dev/null"
         result = self.execCmd(cmd).strip()
         if len(result) == 0:
             userInfo = self.getUserInfo(args)
             if userInfo == "":
                 return userInfo(args)
@@ -65,15 +65,15 @@
         for i in range(8):
             PN = PN + chr(int(arr[i], 16))
         #print PN
         if PN == "NF5280M5":
             if sysstr == 'Windows':
                 cmdb = "..\\tools\\ipmitool\\ipmitool.exe -I lanplus -H " + args.host + " -U " + \
                     args.username + " -P " + args.password + " mc info|findstr /c:\"Firmware Revision\" 2>nul"
-            elif sysstr == 'Linux':
+            elif sysstr == 'Linux' or sysstr == 'Darwin':
                 cmdb = "ipmitool -I lanplus -H " + args.host + " -U " + args.username + \
                     " -P " + args.password + " mc info |grep 'Firmware Revision'" + " 2>/dev/null"
             resultb = self.execCmd(cmdb).strip()
             if "1." in resultb:
                 PN = "NF5288M5"
         PNL = [PN]
         return PNL
@@ -83,15 +83,15 @@
     # 1-M4不支持
     # 2-密码错误
     def getUserInfo(self, args):
         sysstr = platform.system()
         if sysstr == 'Windows':
             cmd = "..\\tools\\ipmitool\\ipmitool.exe -I lanplus -H " + args.host + \
                 " -U " + args.username + " -P " + args.password + " user list" + " 2>nul"
-        elif sysstr == 'Linux':
+        elif sysstr == 'Linux' or sysstr == 'Darwin':
             cmd = "ipmitool -I lanplus -H " + args.host + " -U " + args.username + \
                 " -P " + args.password + " user list" + " 2>/dev/null"
         result = self.execCmd(cmd).strip()
         if len(result) == 0:
             return "PWError"
         return "M4"
```

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/util/RedfishClient.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/util/RedfishClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/util/RegularCheckUtil.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/util/RegularCheckUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/util/RequestClient.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/util/RequestClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/util/configUtil.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/util/configUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/util/fileUtil.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/util/fileUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspur_sm_sdk/util/parameterConversion.py` & `inspursmsdk-2.1.0/inspur_sm_sdk/util/parameterConversion.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.7/inspursmsdk.egg-info/PKG-INFO` & `inspursmsdk-2.1.0/inspursmsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.0.7
+Version: 2.1.0
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
```

### Comparing `inspursmsdk-2.0.7/inspursmsdk.egg-info/SOURCES.txt` & `inspursmsdk-2.1.0/inspursmsdk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -37,19 +37,21 @@
 inspur_sm_sdk/conf/SA5112M5.yml
 inspur_sm_sdk/conf/SA5212M5.yml
 inspur_sm_sdk/conf/__init__.py
 inspur_sm_sdk/interface/Base.py
 inspur_sm_sdk/interface/CommonA5.py
 inspur_sm_sdk/interface/CommonA6.py
 inspur_sm_sdk/interface/CommonA7.py
+inspur_sm_sdk/interface/CommonA7_11308.py
 inspur_sm_sdk/interface/CommonM5.py
 inspur_sm_sdk/interface/CommonM6.py
 inspur_sm_sdk/interface/CommonM6_41401.py
 inspur_sm_sdk/interface/CommonM6_4140a.py
 inspur_sm_sdk/interface/CommonM7.py
+inspur_sm_sdk/interface/CommonM7_13505.py
 inspur_sm_sdk/interface/I24M6.py
 inspur_sm_sdk/interface/IBase.py
 inspur_sm_sdk/interface/NF5180M5.py
 inspur_sm_sdk/interface/NF5180M5Impl.py
 inspur_sm_sdk/interface/NF5280M5.py
 inspur_sm_sdk/interface/NF5280M5Impl.py
 inspur_sm_sdk/interface/NF5280M5_435.py
```

### Comparing `inspursmsdk-2.0.7/ism.py` & `inspursmsdk-2.1.0/ism.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError:
     ISM_EXIST = False
 sys.path.append(os.path.join(sys.path[0], "interface"))
 current_time = time.strftime(
     '%Y-%m-%d   %H:%M:%S',
     time.localtime(
         time.time()))
-__version__ = '2.0.7'
+__version__ = '2.1.0'
 
 
 ERR_dict = {
     'ERR_CODE_CMN_FAIL': 'data acquisition exception',
     'ERR_CODE_PARAM_NULL': 'parameter is null',
     'ERR_CODE_INPUT_ERROR': 'parameter error',
     'ERR_CODE_INTF_FAIL': 'create link exception',
```

### Comparing `inspursmsdk-2.0.7/setup.py` & `inspursmsdk-2.1.0/setup.py`

 * *Files identical despite different names*

