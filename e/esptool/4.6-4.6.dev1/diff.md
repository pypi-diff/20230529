# Comparing `tmp/esptool-4.6.tar.gz` & `tmp/esptool-4.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esptool-4.6.tar", last modified: Mon May 29 14:06:14 2023, max compression
+gzip compressed data, was "dist/esptool-4.6.dev1.tar", last modified: Mon Mar 27 16:51:19 2023, max compression
```

## Comparing `esptool-4.6.tar` & `esptool-4.6.dev1.tar`

### file list

```diff
@@ -1,131 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-29 14:06:00.000000 esptool-4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-29 14:06:00.000000 esptool-4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-29 14:06:14.000000 esptool-4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-29 14:06:00.000000 esptool-4.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     9762 2023-05-29 14:06:00.000000 esptool-4.6/esp_rfc2217_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9718 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30650 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/base_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    27177 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/base_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/emulate_efuse_controller_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse/esp32/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse/esp32c2/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c2/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c2/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse/esp32c3/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c3/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c3/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c3/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse/esp32c6/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c6/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c6/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c6/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32c6/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse/esp32h2/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32h2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32h2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32h2/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32h2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32h2/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse/esp32h2beta1/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32h2beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17995 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32h2beta1/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32h2beta1/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14988 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32h2beta1/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse/esp32s2/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s2/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s2/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse/esp32s3/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s3/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s3/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s3/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse/esp32s3beta2/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s3beta2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s3beta2/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s3beta2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/esp32s3beta2/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/mem_definition_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espefuse/efuse_defs/
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse_defs/esp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15595 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse_defs/esp32c2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    33961 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse_defs/esp32c3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    33534 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse_defs/esp32c6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29352 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse_defs/esp32h2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35820 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse_defs/esp32s2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    40280 2023-05-29 14:06:00.000000 esptool-4.6/espefuse/efuse_defs/esp32s3.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1180 2023-05-29 14:06:00.000000 esptool-4.6/espefuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espsecure/
--rwxr-xr-x   0 runner    (1001) docker     (123)    63263 2023-05-29 14:06:00.000000 esptool-4.6/espsecure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-29 14:06:00.000000 esptool-4.6/espsecure/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/espsecure/esp_hsm_sign/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-29 14:06:00.000000 esptool-4.6/espsecure/esp_hsm_sign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-29 14:06:00.000000 esptool-4.6/espsecure/esp_hsm_sign/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1185 2023-05-29 14:06:00.000000 esptool-4.6/espsecure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/esptool/
--rw-r--r--   0 runner    (1001) docker     (123)    36382 2023-05-29 14:06:00.000000 esptool-4.6/esptool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-29 14:06:00.000000 esptool-4.6/esptool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46660 2023-05-29 14:06:00.000000 esptool-4.6/esptool/bin_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    47013 2023-05-29 14:06:00.000000 esptool-4.6/esptool/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-29 14:06:00.000000 esptool-4.6/esptool/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    60786 2023-05-29 14:06:00.000000 esptool-4.6/esptool/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-29 14:06:00.000000 esptool-4.6/esptool/reset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/esptool/targets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32c2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32c3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32c6.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32c6beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32h2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32h2beta1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32h2beta2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32s2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp32s3beta2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/esp8266.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/esptool/targets/stub_flasher/
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32.json
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32c2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32c3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32c6.json
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32c6beta.json
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32h2.json
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32s2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32s3.json
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32s3beta2.json
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-05-29 14:06:00.000000 esptool-4.6/esptool/targets/stub_flasher/stub_flasher_8266.json
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-29 14:06:00.000000 esptool-4.6/esptool/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:06:14.000000 esptool-4.6/esptool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-29 14:06:14.000000 esptool-4.6/esptool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-29 14:06:14.000000 esptool-4.6/esptool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:06:14.000000 esptool-4.6/esptool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-29 14:06:14.000000 esptool-4.6/esptool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 14:06:14.000000 esptool-4.6/esptool.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-05-29 14:06:00.000000 esptool-4.6/esptool.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-29 14:06:14.000000 esptool-4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-29 14:06:00.000000 esptool-4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/
+-rw-rw-rw-   0 root         (0) root         (0)    18092 2023-03-27 11:04:17.000000 esptool-4.6.dev1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-03-27 11:04:17.000000 esptool-4.6.dev1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-03-27 16:51:19.000000 esptool-4.6.dev1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-03-27 11:04:17.000000 esptool-4.6.dev1/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     9762 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esp_rfc2217_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/
+-rwxrwxrwx   0 root         (0) root         (0)     9431 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30121 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/base_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    25744 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/base_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)     8747 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/emulate_efuse_controller_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5250 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    18032 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    10833 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    12519 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    15486 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    11557 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    12287 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    18304 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    20780 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    14960 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3038 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    18299 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    22114 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    14955 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3015 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    18498 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    21925 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    15383 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3050 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    18149 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    20202 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    14979 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    20851 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    23423 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    18946 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    19340 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    22508 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    18946 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    19354 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    21654 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    18953 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/operations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/mem_definition_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     1089 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espsecure/
+-rwxrwxrwx   0 root         (0) root         (0)    62428 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espsecure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espsecure/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espsecure/esp_hsm_sign/
+-rw-rw-rw-   0 root         (0) root         (0)     5505 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espsecure/esp_hsm_sign/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espsecure/esp_hsm_sign/exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)     1094 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espsecure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool/
+-rw-rw-rw-   0 root         (0) root         (0)    35233 2023-03-27 16:51:18.000000 esptool-4.6.dev1/esptool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    46489 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/bin_image.py
+-rw-rw-rw-   0 root         (0) root         (0)    45474 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/cmds.py
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    60747 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5743 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/reset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool/targets/
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13506 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32.py
+-rw-rw-rw-   0 root         (0) root         (0)     5735 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32c2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32c3.py
+-rw-rw-rw-   0 root         (0) root         (0)     6219 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32c6.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32c6beta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1884 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32h2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32h2beta1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32h2beta2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10606 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32s2.py
+-rw-rw-rw-   0 root         (0) root         (0)    11158 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32s3beta2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5970 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp8266.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/
+-rw-rw-rw-   0 root         (0) root         (0)     4883 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32.json
+-rw-rw-rw-   0 root         (0) root         (0)     4779 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c2.json
+-rw-rw-rw-   0 root         (0) root         (0)     5291 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c3.json
+-rw-rw-rw-   0 root         (0) root         (0)     5231 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c6.json
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c6beta.json
+-rw-rw-rw-   0 root         (0) root         (0)     5231 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2.json
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json
+-rw-rw-rw-   0 root         (0) root         (0)     6119 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s2.json
+-rw-rw-rw-   0 root         (0) root         (0)     7155 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s3.json
+-rw-rw-rw-   0 root         (0) root         (0)     6219 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s3beta2.json
+-rw-rw-rw-   0 root         (0) root         (0)    12119 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_8266.json
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      243 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1084 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-03-27 16:51:19.000000 esptool-4.6.dev1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4254 2023-03-27 11:04:17.000000 esptool-4.6.dev1/setup.py
```

### Comparing `esptool-4.6/LICENSE` & `esptool-4.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `esptool-4.6/PKG-INFO` & `esptool-4.6.dev1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 Metadata-Version: 2.1
 Name: esptool
-Version: 4.6
+Version: 4.6.dev1
 Summary: A serial utility to communicate & flash code to Espressif chips.
 Home-page: https://github.com/espressif/esptool/
 Author: Fredrik Ahlberg (themadinventor) & Angus Gratton (projectgus) & Espressif Systems
 Author-email: 
 License: GPLv2+
 Project-URL: Documentation, https://docs.espressif.com/projects/esptool/
 Project-URL: Source, https://github.com/espressif/esptool/
 Project-URL: Tracker, https://github.com/espressif/esptool/issues/
-Description: 
-        ==========
-        esptool.py
-        ==========
-        A Python-based, open-source, platform-independent utility to communicate with the ROM bootloader in Espressif chips.
-        
-        The esptool.py project is `hosted on github <https://github.com/espressif/esptool>`_.
-        
-        Documentation
-        -------------
-        Visit online `esptool documentation <https://docs.espressif.com/projects/esptool/>`_ or run ``esptool.py -h``.
-        
-        Contributing
-        ------------
-        Please see the `contributions guide <https://docs.espressif.com/projects/esptool/en/latest/contributing.html>`_.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -38,7 +22,26 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Provides-Extra: dev
 Provides-Extra: hsm
+License-File: LICENSE
+
+
+==========
+esptool.py
+==========
+A Python-based, open-source, platform-independent utility to communicate with the ROM bootloader in Espressif chips.
+
+The esptool.py project is `hosted on github <https://github.com/espressif/esptool>`_.
+
+Documentation
+-------------
+Visit online `esptool documentation <https://docs.espressif.com/projects/esptool/>`_ or run ``esptool.py -h``.
+
+Contributing
+------------
+Please see the `contributions guide <https://docs.espressif.com/projects/esptool/en/latest/contributing.html>`_.
+
+
```

### Comparing `esptool-4.6/README.md` & `esptool-4.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esp_rfc2217_server.py` & `esptool-4.6.dev1/esp_rfc2217_server.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/espefuse/__init__.py` & `esptool-4.6.dev1/espefuse/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,29 +128,23 @@
             cmd = []
         cmd.append(item)
     if cmd:
         groups.append(cmd)
     return groups, used_cmds
 
 
-def main(custom_commandline=None, esp=None):
+def main(custom_commandline=None):
     """
     Main function for espefuse
 
     custom_commandline - Optional override for default arguments parsing
     (that uses sys.argv), can be a list of custom arguments as strings.
     Arguments and their values need to be added as individual items to the list
     e.g. "--port /dev/ttyUSB1" thus becomes ['--port', '/dev/ttyUSB1'].
-
-    esp - Optional override of the connected device previously
-    returned by esptool.get_default_connected_device()
     """
-
-    external_esp = esp is not None
-
     init_parser = argparse.ArgumentParser(
         description="espefuse.py v%s - [ESP32xx] efuse get/set tool"
         % esptool.__version__,
         prog="espefuse",
         add_help=False,
     )
 
@@ -213,32 +207,30 @@
     debug_mode = common_args.debug or ("dump" in remaining_args)
     just_print_help = [
         True for arg in remaining_args if arg in ["--help", "-h"]
     ] or remaining_args == []
 
     print("espefuse.py v{}".format(esptool.__version__))
 
-    if not external_esp:
-        try:
-            esp = get_esp(
-                common_args.port,
-                common_args.baud,
-                common_args.before,
-                common_args.chip,
-                just_print_help,
-                common_args.virt,
-                common_args.debug,
-                common_args.path_efuse_file,
-            )
-        except esptool.FatalError as e:
-            raise esptool.FatalError(
-                f"{e}\nPlease make sure that you have specified "
-                "the right port with the --port argument"
-            )
-            # TODO: Require the --port argument in the next major release, ESPTOOL-490
+    try:
+        esp = get_esp(
+            common_args.port,
+            common_args.baud,
+            common_args.before,
+            common_args.chip,
+            just_print_help,
+            common_args.virt,
+            common_args.debug,
+            common_args.path_efuse_file,
+        )
+    except esptool.FatalError as e:
+        raise esptool.FatalError(
+            f"{e}\nPlease make sure that you have specified "
+            "the right port with the --port argument"
+        )  # TODO: Require the --port argument in the next major release, ESPTOOL-490
 
     efuses, efuse_operations = get_efuses(
         esp, just_print_help, debug_mode, common_args.do_not_confirm
     )
 
     parser = argparse.ArgumentParser(parents=[init_parser])
     subparsers = parser.add_subparsers(
@@ -280,15 +272,15 @@
             operation_func(esp, efuses, args)
 
         if there_are_multiple_burn_commands_in_args:
             efuses.batch_mode_cnt -= 1
             if not efuses.burn_all(check_batch_mode=True):
                 raise esptool.FatalError("BURN was not done")
     finally:
-        if not external_esp and not common_args.virt and esp._port:
+        if not common_args.virt and esp._port:
             esp._port.close()
 
 
 def _main():
     try:
         main()
     except esptool.FatalError as e:
```

### Comparing `esptool-4.6/espefuse/efuse/base_fields.py` & `esptool-4.6.dev1/espefuse/efuse/base_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file describes the common eFuses structures for chips
 #
 # SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import binascii
+import re
 import sys
 
 from bitstring import BitArray, BitStream, CreationError
 
 import esptool
 
 from . import util
@@ -546,18 +547,14 @@
             if not self.force_write_always:
                 error_msg += "(use '--force-write-always' option to ignore it)"
         if self.force_write_always:
             print(error_msg, "Skipped because '--force-write-always' option.")
         else:
             raise esptool.FatalError(error_msg)
 
-    def get_block_errors(self, block_num):
-        """Returns (error count, failure boolean flag)"""
-        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
-
 
 class EfuseFieldBase(EfuseProtectBase):
     def __init__(self, parent, param):
         self.category = param.category
         self.parent = parent
         self.block = param.block
         self.word = param.word
@@ -565,19 +562,24 @@
         self.write_disable_bit = param.write_disable_bit
         self.read_disable_bit = param.read_disable_bit
         self.name = param.name
         self.efuse_class = param.class_type
         self.efuse_type = param.type
         self.description = param.description
         self.dict_value = param.dictionary
-        self.bit_len = param.bit_len
-        self.alt_names = param.alt_names
         self.fail = False
         self.num_errors = 0
-        self.bitarray = BitStream(self.bit_len)
+        if self.efuse_type.startswith("bool"):
+            field_len = 1
+        else:
+            field_len = int(re.search(r"\d+", self.efuse_type).group())
+            if self.efuse_type.startswith("bytes"):
+                field_len *= 8
+        self.bitarray = BitStream(field_len)
+        self.bit_len = field_len
         self.bitarray.set(0)
         self.update(self.parent.blocks[self.block].bitarray)
 
     def check_format(self, new_value_str):
         if new_value_str is None:
             return new_value_str
         else:
@@ -728,22 +730,7 @@
             )
             return block.wr_bitarray.read(self.bitarray.len)
 
     def burn(self, new_value):
         # Burn a efuse. Added for compatibility reason.
         self.save(new_value)
         self.parent.burn_all()
-
-    def get_info(self):
-        output = f"{self.name} (BLOCK{self.block})"
-        if self.block == 0:
-            if self.fail:
-                output += "[error]"
-        else:
-            errs, fail = self.parent.get_block_errors(self.block)
-            if errs != 0 or fail:
-                output += "[error]"
-        if self.efuse_class == "keyblock":
-            name = self.parent.blocks[self.block].key_purpose_name
-            if name is not None:
-                output += f"\n  Purpose: {self.parent[name].get()}\n "
-        return output
```

### Comparing `esptool-4.6/espefuse/efuse/base_operations.py` & `esptool-4.6.dev1/espefuse/efuse/base_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,53 +67,38 @@
         "name_value_pairs",
         help="Name of efuse register and New value pairs to burn",
         action=ActionEfuseValuePair,
         nargs="+",
         metavar="[EFUSE_NAME VALUE] [{} VALUE".format(
             " VALUE] [".join([e.name for e in efuses.efuses])
         ),
-        efuse_choices=[e.name for e in efuses.efuses]
-        + [name for e in efuses.efuses for name in e.alt_names if name != ""],
+        efuse_choices=[e.name for e in efuses.efuses],
         efuses=efuses,
     )
 
     read_protect_efuse = subparsers.add_parser(
         "read_protect_efuse",
         help="Disable readback for the efuse with the specified name",
     )
     read_protect_efuse.add_argument(
         "efuse_name",
         help="Name of efuse register to burn",
         nargs="+",
-        choices=[e.name for e in efuses.efuses if e.read_disable_bit is not None]
-        + [
-            name
-            for e in efuses.efuses
-            if e.read_disable_bit is not None
-            for name in e.alt_names
-            if name != ""
-        ],
+        choices=[e.name for e in efuses.efuses if e.read_disable_bit is not None],
     )
 
     write_protect_efuse = subparsers.add_parser(
         "write_protect_efuse",
         help="Disable writing to the efuse with the specified name",
     )
     write_protect_efuse.add_argument(
         "efuse_name",
         help="Name of efuse register to burn",
         nargs="+",
-        choices=[e.name for e in efuses.efuses if e.write_disable_bit is not None]
-        + [
-            name
-            for e in efuses.efuses
-            if e.write_disable_bit is not None
-            for name in e.alt_names
-            if name != ""
-        ],
+        choices=[e.name for e in efuses.efuses if e.write_disable_bit is not None],
     )
 
     burn_block_data = subparsers.add_parser(
         "burn_block_data",
         help="Burn non-key data to EFUSE blocks. "
         "(Don't use this command to burn key data for Flash Encryption or "
         "ESP32 Secure Boot V1, as the byte order of keys is swapped (use burn_key)).",
@@ -679,53 +664,30 @@
     block.save(data_block.bytes[::-1])
 
     if not efuses.burn_all(check_batch_mode=True):
         return
     print("Successful")
 
 
-def get_error_summary(efuses):
-    error_in_blocks = efuses.get_coding_scheme_warnings()
-    if not error_in_blocks:
-        return False
-    writable = True
-    for blk in efuses.blocks:
-        if blk.fail or blk.num_errors:
-            if blk.id == 0:
-                for field in efuses:
-                    if field.block == blk.id and (field.fail or field.num_errors):
-                        wr = "writable" if field.is_writeable() else "not writable"
-                        writable &= wr == "writable"
-                        name = field.name
-                        val = field.get()
-                        print(f"BLOCK{field.block:<2}: {name:<40} = {val:<8} ({wr})")
-            else:
-                wr = "writable" if blk.is_writeable() else "not writable"
-                writable &= wr == "writable"
-                name = f"{blk.name} [ERRORS:{blk.num_errors} FAIL:{int(blk.fail)}]"
-                val = str(blk.get_bitstring())
-                print(f"BLOCK{blk.id:<2}: {name:<40} = {val:<8} ({wr})")
-    if not writable and error_in_blocks:
-        print("Not all errors can be fixed because some fields are write-protected!")
-    return True
-
-
 def check_error(esp, efuses, args):
-    error_in_blocks = get_error_summary(efuses)
-    if args.recovery and error_in_blocks:
-        confirmed = False
-        for block in reversed(efuses.blocks):
-            if block.fail or block.num_errors > 0:
-                if not block.get_bitstring().all(False):
-                    block.save(block.get_bitstring().bytes[::-1])
-                    if not confirmed:
-                        confirmed = True
-                        efuses.confirm(
-                            "Recovery of block coding errors", args.do_not_confirm
-                        )
-                    block.burn()
-        if confirmed:
-            efuses.update_efuses()
-        error_in_blocks = get_error_summary(efuses)
-    if error_in_blocks:
-        raise esptool.FatalError("Error(s) were detected in eFuses")
+    error_in_blocks = efuses.get_coding_scheme_warnings()
+    if args.recovery:
+        if error_in_blocks:
+            confirmed = False
+            for block in reversed(efuses.blocks):
+                if block.fail or block.num_errors > 0:
+                    if not block.get_bitstring().all(False):
+                        block.save(block.get_bitstring().bytes[::-1])
+                        if not confirmed:
+                            confirmed = True
+                            efuses.confirm(
+                                "Recovery of block coding errors", args.do_not_confirm
+                            )
+                        block.burn()
+            # Reset the recovery flag to run check_error() without it,
+            # just to check the new state of eFuse blocks.
+            args.recovery = False
+            check_error(esp, efuses, args)
+    else:
+        if error_in_blocks:
+            raise esptool.FatalError("Error(s) were detected in eFuses")
     print("No errors detected")
```

### Comparing `esptool-4.6/espefuse/efuse/emulate_efuse_controller_base.py` & `esptool-4.6.dev1/espefuse/efuse/emulate_efuse_controller_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,15 +105,16 @@
         for b in self.Blocks.BLOCKS:
             blk = self.Blocks.get(b)
             for offset in range(0, blk.len * 4, 4):
                 wr_addr = blk.wr_addr + offset
                 self.write_reg(wr_addr, 0)
 
     def read_field(self, name, bitstring=True):
-        for field in self.Fields.EFUSES:
+        for e in self.Fields.EFUSES:
+            field = self.Fields.get(e)
             if field.name == name:
                 self.read_block(field.block)
                 block = self.read_block(field.block)
                 if field.type.startswith("bool"):
                     field_len = 1
                 else:
                     field_len = int(re.search(r"\d+", field.type).group())
@@ -161,15 +162,16 @@
         mask_wr_data.set(0)
         blk = self.Blocks.get(self.Blocks.BLOCKS[num_blk])
         if blk.write_disable_bit is not None and write_disable_bit & (
             1 << blk.write_disable_bit
         ):
             mask_wr_data.set(1)
         else:
-            for field in self.Fields.EFUSES:
+            for e in self.Fields.EFUSES:
+                field = self.Fields.get(e)
                 if blk.id == field.block and field.block == num_blk:
                     if field.write_disable_bit is not None and write_disable_bit & (
                         1 << field.write_disable_bit
                     ):
                         data = self.read_field(field.name)
                         data.set(1)
                         mask_wr_data.pos = mask_wr_data.length - (
@@ -187,15 +189,16 @@
             blk = self.Blocks.get(b)
             block = self.read_block(blk.id)
             if blk.read_disable_bit is not None and read_disable_bit & (
                 1 << blk.read_disable_bit
             ):
                 block.set(0)
             else:
-                for field in self.Fields.EFUSES:
+                for e in self.Fields.EFUSES:
+                    field = self.Fields.get(e)
                     if (
                         blk.id == field.block
                         and field.read_disable_bit is not None
                         and read_disable_bit & (1 << field.read_disable_bit)
                     ):
                         raw_data = self.read_field(field.name)
                         raw_data.set(0)
```

### Comparing `esptool-4.6/espefuse/efuse/esp32/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32/emulate_efuse_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operations. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
 
     """ esptool method start >> """
 
     def get_major_chip_version(self):
         return 3
```

### Comparing `esptool-4.6/espefuse/efuse/esp32/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32/fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,102 +61,132 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
         if esp.CHIP_NAME != "ESP32":
             raise esptool.FatalError(
                 "Expected the 'esp' param for ESP32 chip but got for '%s'."
                 % (esp.CHIP_NAME)
             )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS_256
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.KEYBLOCKS_256
             ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CUSTOM_MAC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CUSTOM_MAC
             ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.ADC_CALIBRATION
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.ADC_CALIBRATION
             ]
         else:
             if self.coding_scheme == self.REGS.CODING_SCHEME_NONE:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.KEYBLOCKS_256
                 ]
             elif self.coding_scheme == self.REGS.CODING_SCHEME_34:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.KEYBLOCKS_192
                 ]
             else:
                 raise esptool.FatalError(
                     "The coding scheme (%d) - is not supported" % self.coding_scheme
                 )
             if self["MAC_VERSION"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse) for efuse in self.Fields.CUSTOM_MAC
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
+                    for efuse in self.Fields.CUSTOM_MAC
                 ]
             if self["BLK3_PART_RESERVE"].get():
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.ADC_CALIBRATION
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.CUSTOM_MAC:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse) for efuse in self.Fields.CUSTOM_MAC
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
+                    for efuse in self.Fields.CUSTOM_MAC
                 ]
                 new_fields = True
         for efuse in self.Fields.ADC_CALIBRATION:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.ADC_CALIBRATION
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = (
             self.read_efuse(self.REGS.EFUSE_CODING_SCHEME_WORD)
             & self.REGS.EFUSE_CODING_SCHEME_MASK
@@ -229,35 +259,39 @@
                 )
         if (self.debug or err) and not silent:
             self.print_status_regs()
         return err != 0
 
     def summary(self):
         if self["XPD_SDIO_FORCE"].get() == 0:
-            output = "Flash voltage (VDD_SDIO) determined by GPIO12 on reset (High for 1.8V, Low/NC for 3.3V)"
+            output = "Flash voltage (VDD_SDIO) determined by GPIO12 on reset "
+            "(High for 1.8V, Low/NC for 3.3V)."
         elif self["XPD_SDIO_REG"].get() == 0:
             output = "Flash voltage (VDD_SDIO) internal regulator disabled by efuse."
         elif self["XPD_SDIO_TIEH"].get() == 0:
             output = "Flash voltage (VDD_SDIO) set to 1.8V by efuse."
         else:
             output = "Flash voltage (VDD_SDIO) set to 3.3V by efuse."
         return output
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "spipin": EfuseSpiPinField,
             "vref": EfuseVRefField,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
             "pkg": EfusePkg,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        return "%s (BLOCK%d):" % (self.name, self.block)
 
 
 class EfuseMacField(EfuseField):
     """
     Supports: MAC and CUSTOM_MAC fields.
     (if MAC_VERSION == 1 then the CUSTOM_MAC is used)
     """
@@ -364,17 +398,15 @@
             # as it's written in the factory.
             raise esptool.FatalError("Writing Factory MAC address is not supported")
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         rev_bit0 = self.parent["CHIP_VER_REV1"].get(from_read)
-        assert self.parent["CHIP_VER_REV1"].bit_len == 1
         rev_bit1 = self.parent["CHIP_VER_REV2"].get(from_read)
-        assert self.parent["CHIP_VER_REV2"].bit_len == 1
         apb_ctl_date = self.parent.read_reg(self.parent.REGS.APB_CTL_DATE_ADDR)
         rev_bit2 = (
             apb_ctl_date >> self.parent.REGS.APB_CTL_DATE_S
         ) & self.parent.REGS.APB_CTL_DATE_V
         combine_value = (rev_bit2 << 2) | (rev_bit1 << 1) | rev_bit0
 
         revision = {
```

### Comparing `esptool-4.6/espefuse/efuse/esp32/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/espefuse/efuse/esp32c2/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c2/emulate_efuse_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-C2"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 1
@@ -120,15 +120,16 @@
                             0, [i for i in range(blk.len * 32 // 2, blk.len * 32)]
                         )
                     if read_disable_bit & (1 << blk.read_disable_bit[1]):
                         block.set(0, [i for i in range(0, blk.len * 32 // 2)])
                 else:
                     block.set(0)
             else:
-                for field in self.Fields.EFUSES:
+                for e in self.Fields.EFUSES:
+                    field = self.Fields.get(e)
                     if (
                         blk.id == field.block
                         and field.read_disable_bit is not None
                         and read_disable_bit & get_read_disable_mask(field)
                     ):
                         raw_data = self.read_field(field.name)
                         raw_data.set(0)
```

### Comparing `esptool-4.6/espefuse/efuse/esp32c2/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c2/fields.py`

 * *Files 19% similar despite different names*

```diff
@@ -50,23 +50,24 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
         if esp.CHIP_NAME != "ESP32-C2":
             raise esptool.FatalError(
                 "Expected the 'esp' param for ESP32-C2 chip but got for '%s'."
                 % (esp.CHIP_NAME)
@@ -80,48 +81,61 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MINOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -129,14 +143,18 @@
         self.blocks[0].print_block(self.blocks[0].err_bitarray, "err__regs", debug=True)
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -216,21 +234,14 @@
         # Configure clock
         xtal_freq = self.get_crystal_freq()
         if xtal_freq not in [26, 40]:
             raise esptool.FatalError(
                 "The eFuse supports only xtal=26M and 40M (xtal was %d)" % xtal_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
         tpgm_inactive_val = 200 if xtal_freq == 40 else 130
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF0_REG,
@@ -245,17 +256,20 @@
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR_REG + offs * 4)
                     for offs in range(1)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
                     block.id
                 ]
                 if err_num_mask is None or err_num_offs is None or fail_bit is None:
@@ -278,21 +292,36 @@
     def summary(self):
         # TODO add support set_flash_voltage - "Flash voltage (VDD_SPI)"
         return ""
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseTempSensor(EfuseField):
     def get(self, from_read=True):
         value = self.get_bitstring(from_read)
         sig = -1 if value[0] else 1
         return sig * value[1:].uint * 0.1
@@ -360,18 +389,27 @@
             super(EfuseMacField, self).save(new_value)
         else:
             raise esptool.FatalError("Writing Factory MAC address is not supported")
 
 
 class EfuseKeyPurposeField(EfuseField):
     KEY_PURPOSES = [
-        # fmt: off
-        ("USER",                                        0, None),      # User purposes (software-only use)
-        ("XTS_AES_128_KEY",                             1, None),      # (whole 256bits) flash/PSRAM encryption
-        ("XTS_AES_128_KEY_DERIVED_FROM_128_EFUSE_BITS", 2, None),      # (lo 128bits) flash/PSRAM encryption
-        ("SECURE_BOOT_DIGEST",                          3, "DIGEST"),
-        # (hi 128bits) Secure Boot key digest
-        # fmt: on
+        ("USER", 0, None),  # User purposes (software-only use)
+        (
+            "XTS_AES_128_KEY",
+            1,
+            None,
+        ),  # (whole 256bits) XTS_AES_128_KEY (flash/PSRAM encryption)
+        (
+            "XTS_AES_128_KEY_DERIVED_FROM_128_EFUSE_BITS",
+            2,
+            None,
+        ),  # (lo 128bits) XTS_AES_128_KEY (flash/PSRAM encryption)
+        (
+            "SECURE_BOOT_DIGEST",
+            3,
+            "DIGEST",
+        ),  # (hi 128bits)SECURE_BOOT_DIGEST (Secure Boot key digest)
     ]
 
     KEY_PURPOSES_NAME = [name[0] for name in KEY_PURPOSES]
     DIGEST_KEY_PURPOSES = [name[0] for name in KEY_PURPOSES if name[2] == "DIGEST"]
```

### Comparing `esptool-4.6/espefuse/efuse/esp32c2/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c2/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/espefuse/efuse/esp32c3/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2/emulate_efuse_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# This file describes eFuses controller for ESP32-C3 chip
+# This file describes eFuses controller for ESP32-H2 chip
 #
-# SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import reedsolo
 
 from .mem_definition import EfuseDefineBlocks, EfuseDefineFields, EfuseDefineRegisters
 from ..emulate_efuse_controller_base import EmulateEfuseControllerBase, FatalError
 
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
-    CHIP_NAME = "ESP32-C3"
+    CHIP_NAME = "ESP32-H2"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
 
     def get_minor_chip_version(self):
-        return 4
+        return 0
 
     def get_crystal_freq(self):
-        return 40  # MHz (common for all chips)
+        return 32  # MHz
 
     def get_security_info(self):
         return {
             "flags": 0,
             "flash_crypt_cnt": 0,
             "key_purposes": 0,
             "chip_id": 0,
```

### Comparing `esptool-4.6/espefuse/efuse/esp32c3/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c6/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file describes eFuses for ESP32-C3 chip
+# This file describes eFuses for ESP32-C6 chip
 #
-# SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import binascii
 import struct
 import time
 
@@ -50,29 +50,30 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
-        if esp.CHIP_NAME != "ESP32-C3":
+        if esp.CHIP_NAME != "ESP32-C6":
             raise esptool.FatalError(
-                "Expected the 'esp' param for ESP32-C3 chip but got for '%s'."
+                "Expected the 'esp' param for ESP32-C6 chip but got for '%s'."
                 % (esp.CHIP_NAME)
             )
         if not skip_connect:
             flags = self._esp.get_security_info()["flags"]
             GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE = 1 << 2
             if flags & GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE:
                 raise esptool.FatalError(
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MAJOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -224,37 +245,33 @@
         # Configure clock
         apb_freq = self.get_crystal_freq()
         if apb_freq != 40:
             raise esptool.FatalError(
                 "The eFuse supports only xtal=40M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg_f, fail_bit = self.REGS.BLOCK_FAIL_BIT[block.id]
                 if fail_bit is None:
                     block.fail = False
                 else:
@@ -281,30 +298,43 @@
     def summary(self):
         # TODO add support set_flash_voltage - "Flash voltage (VDD_SPI)"
         return ""
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
@@ -425,18 +455,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value.startswith("XTS_AES"):
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6/espefuse/efuse/esp32c3/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c3/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/espefuse/efuse/esp32c6/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c6/emulate_efuse_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-C6"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
```

### Comparing `esptool-4.6/espefuse/efuse/esp32c6/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file describes eFuses for ESP32-C6 chip
+# This file describes eFuses for ESP32-H2 chip
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2021-2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import binascii
 import struct
 import time
 
@@ -50,29 +50,30 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
-        if esp.CHIP_NAME != "ESP32-C6":
+        if esp.CHIP_NAME != "ESP32-H2(beta1)":
             raise esptool.FatalError(
-                "Expected the 'esp' param for ESP32-C6 chip but got for '%s'."
+                "Expected the 'esp' param for ESP32-H2(beta1) chip but got for '%s'."
                 % (esp.CHIP_NAME)
             )
         if not skip_connect:
             flags = self._esp.get_security_info()["flags"]
             GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE = 1 << 2
             if flags & GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE:
                 raise esptool.FatalError(
@@ -80,51 +81,61 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
-            if self["BLK_VERSION_MINOR"].get() == 1:
+            if self["BLOCK2_VERSION"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
-            self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
-            ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +148,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -219,26 +234,19 @@
                     exit(0)  # finish without errors
             raise
 
     def set_efuse_timing(self):
         """Set timing registers for burning efuses"""
         # Configure clock
         apb_freq = self.get_crystal_freq()
-        if apb_freq != 40:
+        if apb_freq != 32:
             raise esptool.FatalError(
-                "The eFuse supports only xtal=40M (xtal was %d)" % apb_freq
+                "The eFuse supports only xtal=32M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
         old_addr_reg = 0
@@ -246,17 +254,20 @@
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
                     block.id
                 ]
                 if err_num_mask is None or err_num_offs is None or fail_bit is None:
@@ -279,34 +290,36 @@
     def summary(self):
         # TODO add support set_flash_voltage - "Flash voltage (VDD_SPI)"
         return ""
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
-            "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
-
-
-class EfuseWafer(EfuseField):
-    def get(self, from_read=True):
-        hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
-        lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
-        return (hi_bits << 3) + lo_bits
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
 
-    def save(self, new_value):
-        raise esptool.FatalError("Burning %s is not supported" % self.name)
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseTempSensor(EfuseField):
     def get(self, from_read=True):
         value = self.get_bitstring(from_read)
         sig = -1 if value[0] else 1
         return sig * value[1:].uint * 0.1
@@ -351,15 +364,19 @@
             output = "Block%d has ERRORS:%d FAIL:%d" % (self.block, errs, fail)
         else:
             output = "OK"
         return "(" + output + ")"
 
     def get(self, from_read=True):
         if self.name == "CUSTOM_MAC":
-            mac = self.get_raw(from_read)[::-1]
+            mac = self.get_raw(from_read)[::-1] + self.parent["MAC_EXT"].get_raw(
+                from_read
+            )
+        elif self.name == "MAC":
+            mac = self.get_raw(from_read) + self.parent["MAC_EXT"].get_raw(from_read)
         else:
             mac = self.get_raw(from_read)
         return "%s %s" % (util.hexify(mac, ":"), self.check())
 
     def save(self, new_value):
         def print_field(e, new_value):
             print(
@@ -379,24 +396,27 @@
 
 
 # fmt: off
 class EfuseKeyPurposeField(EfuseField):
     KEY_PURPOSES = [
         ("USER",                         0,  None,       None,      "no_need_rd_protect"),   # User purposes (software-only use)
         ("RESERVED",                     1,  None,       None,      "no_need_rd_protect"),   # Reserved
+        ("XTS_AES_256_KEY_1",            2,  None,       "Reverse", "need_rd_protect"),      # XTS_AES_256_KEY_1 (flash/PSRAM encryption)
+        ("XTS_AES_256_KEY_2",            3,  None,       "Reverse", "need_rd_protect"),      # XTS_AES_256_KEY_2 (flash/PSRAM encryption)
         ("XTS_AES_128_KEY",              4,  None,       "Reverse", "need_rd_protect"),      # XTS_AES_128_KEY (flash/PSRAM encryption)
         ("HMAC_DOWN_ALL",                5,  None,       None,      "need_rd_protect"),      # HMAC Downstream mode
         ("HMAC_DOWN_JTAG",               6,  None,       None,      "need_rd_protect"),      # JTAG soft enable key (uses HMAC Downstream mode)
         ("HMAC_DOWN_DIGITAL_SIGNATURE",  7,  None,       None,      "need_rd_protect"),      # Digital Signature peripheral key (uses HMAC Downstream mode)
         ("HMAC_UP",                      8,  None,       None,      "need_rd_protect"),      # HMAC Upstream mode
         ("SECURE_BOOT_DIGEST0",          9,  "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST0 (Secure Boot key digest)
         ("SECURE_BOOT_DIGEST1",          10, "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST1 (Secure Boot key digest)
         ("SECURE_BOOT_DIGEST2",          11, "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST2 (Secure Boot key digest)
     ]
 # fmt: on
+
     KEY_PURPOSES_NAME = [name[0] for name in KEY_PURPOSES]
     DIGEST_KEY_PURPOSES = [name[0] for name in KEY_PURPOSES if name[2] == "DIGEST"]
 
     def check_format(self, new_value_str):
         # str convert to int: "XTS_AES_128_KEY" - > str(4)
         # if int: 4 -> str(4)
         raw_val = new_value_str
@@ -423,18 +443,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value.startswith("XTS_AES"):
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6/espefuse/efuse/esp32c6/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c6/operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -163,16 +163,15 @@
 
     p = subparsers.add_parser(
         "burn_custom_mac", help="Burn a 48-bit Custom MAC Address to EFUSE BLOCK3."
     )
     p.add_argument(
         "mac",
         help="Custom MAC Address to burn given in hexadecimal format with bytes "
-        "separated by colons (e.g. AA:CD:EF:01:02:03). "
-        "Final CUSTOM_MAC = CUSTOM_MAC[48] + MAC_EXT[16]",
+        "separated by colons (e.g. AA:CD:EF:01:02:03).",
         type=fields.base_fields.CheckArgValue(efuses, "CUSTOM_MAC"),
     )
     add_force_write_always(p)
 
     p = subparsers.add_parser("get_custom_mac", help="Prints the Custom MAC Address.")
 
 
@@ -191,37 +190,46 @@
 def set_flash_voltage(esp, efuses, args):
     raise esptool.FatalError("set_flash_voltage is not supported!")
 
 
 def adc_info(esp, efuses, args):
     print("")
     # fmt: off
-    if efuses["BLK_VERSION_MINOR"].get() == 1:
-        print("Temperature Sensor Calibration = {}C".format(efuses["TEMP_CALIB"].get()))
+    if efuses["BLK_VERSION_MAJOR"].get() == 1:
+        print("Temperature Sensor Calibration = {}C".format(efuses["TEMP_SENSOR_CAL"].get()))
 
         print("")
-        print("ADC1 Calibration data stored in efuse BLOCK2:")
-        print(f"OCODE: {efuses['OCODE'].get()}")
-        print(f"INIT_CODE_ATTEN0: {efuses['ADC1_INIT_CODE_ATTEN0'].get()}")
-        print(f"INIT_CODE_ATTEN1: {efuses['ADC1_INIT_CODE_ATTEN1'].get()}")
-        print(f"INIT_CODE_ATTEN2: {efuses['ADC1_INIT_CODE_ATTEN2'].get()}")
-        print(f"INIT_CODE_ATTEN3: {efuses['ADC1_INIT_CODE_ATTEN3'].get()}")
-        print(f"CAL_VOL_ATTEN0: {efuses['ADC1_CAL_VOL_ATTEN0'].get()}")
-        print(f"CAL_VOL_ATTEN1: {efuses['ADC1_CAL_VOL_ATTEN1'].get()}")
-        print(f"CAL_VOL_ATTEN2: {efuses['ADC1_CAL_VOL_ATTEN2'].get()}")
-        print(f"CAL_VOL_ATTEN3: {efuses['ADC1_CAL_VOL_ATTEN3'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH0: {efuses['ADC1_INIT_CODE_ATTEN0_CH0'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH1: {efuses['ADC1_INIT_CODE_ATTEN0_CH1'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH2: {efuses['ADC1_INIT_CODE_ATTEN0_CH2'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH3: {efuses['ADC1_INIT_CODE_ATTEN0_CH3'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH4: {efuses['ADC1_INIT_CODE_ATTEN0_CH4'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH5: {efuses['ADC1_INIT_CODE_ATTEN0_CH5'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH6: {efuses['ADC1_INIT_CODE_ATTEN0_CH6'].get()}")
+        print("ADC1 readings stored in efuse BLOCK2:")
+        print("    MODE0 D1 reading  (250mV):  {}".format(efuses["ADC1_MODE0_D1"].get()))
+        print("    MODE0 D2 reading  (600mV):  {}".format(efuses["ADC1_MODE0_D2"].get()))
+
+        print("    MODE1 D1 reading  (250mV):  {}".format(efuses["ADC1_MODE1_D1"].get()))
+        print("    MODE1 D2 reading  (800mV):  {}".format(efuses["ADC1_MODE1_D2"].get()))
+
+        print("    MODE2 D1 reading  (250mV):  {}".format(efuses["ADC1_MODE2_D1"].get()))
+        print("    MODE2 D2 reading  (1000mV): {}".format(efuses["ADC1_MODE2_D2"].get()))
+
+        print("    MODE3 D1 reading  (250mV):  {}".format(efuses["ADC1_MODE3_D1"].get()))
+        print("    MODE3 D2 reading  (2000mV): {}".format(efuses["ADC1_MODE3_D2"].get()))
+
+        print("")
+        print("ADC2 readings stored in efuse BLOCK2:")
+        print("    MODE0 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE0_D1"].get()))
+        print("    MODE0 D2 reading  (600mV):  {}".format(efuses["ADC2_MODE0_D2"].get()))
+
+        print("    MODE1 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE1_D1"].get()))
+        print("    MODE1 D2 reading  (800mV):  {}".format(efuses["ADC2_MODE1_D2"].get()))
+
+        print("    MODE2 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE2_D1"].get()))
+        print("    MODE2 D2 reading  (1000mV): {}".format(efuses["ADC2_MODE2_D2"].get()))
+
+        print("    MODE3 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE3_D1"].get()))
+        print("    MODE3 D2 reading  (2000mV): {}".format(efuses["ADC2_MODE3_D2"].get()))
     else:
-        print("BLK_VERSION_MINOR = {}".format(efuses["BLK_VERSION_MINOR"].get_meaning()))
+        print("BLK_VERSION_MAJOR = {}".format(efuses["BLK_VERSION_MAJOR"].get_meaning()))
     # fmt: on
 
 
 def burn_key(esp, efuses, args, digest=None):
     if digest is None:
         datafile_list = args.keyfile[
             0 : len([name for name in args.keyfile if name is not None]) :
```

### Comparing `esptool-4.6/espefuse/efuse/esp32h2/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c3/emulate_efuse_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# This file describes eFuses controller for ESP32-H2 chip
+# This file describes eFuses controller for ESP32-C3 chip
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import reedsolo
 
 from .mem_definition import EfuseDefineBlocks, EfuseDefineFields, EfuseDefineRegisters
 from ..emulate_efuse_controller_base import EmulateEfuseControllerBase, FatalError
 
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
-    CHIP_NAME = "ESP32-H2"
+    CHIP_NAME = "ESP32-C3"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
 
     def get_minor_chip_version(self):
-        return 0
+        return 4
 
     def get_crystal_freq(self):
-        return 32  # MHz
+        return 40  # MHz (common for all chips)
 
     def get_security_info(self):
         return {
             "flags": 0,
             "flash_crypt_cnt": 0,
             "key_purposes": 0,
             "chip_id": 0,
```

### Comparing `esptool-4.6/espefuse/efuse/esp32h2/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c3/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file describes eFuses for ESP32-H2 chip
+# This file describes eFuses for ESP32-C3 chip
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import binascii
 import struct
 import time
 
@@ -50,29 +50,30 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
-        if esp.CHIP_NAME != "ESP32-H2":
+        if esp.CHIP_NAME != "ESP32-C3":
             raise esptool.FatalError(
-                "Expected the 'esp' param for ESP32-H2 chip but got for '%s'."
+                "Expected the 'esp' param for ESP32-C3 chip but got for '%s'."
                 % (esp.CHIP_NAME)
             )
         if not skip_connect:
             flags = self._esp.get_security_info()["flags"]
             GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE = 1 << 2
             if flags & GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE:
                 raise esptool.FatalError(
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MAJOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -219,58 +240,55 @@
                     exit(0)  # finish without errors
             raise
 
     def set_efuse_timing(self):
         """Set timing registers for burning efuses"""
         # Configure clock
         apb_freq = self.get_crystal_freq()
-        # Based on `CONFIG_SOC_XTAL_SUPPORT_32M=y` for this target from ESP-IDF configuration
-        if apb_freq != 32:
+        if apb_freq != 40:
             raise esptool.FatalError(
-                "The eFuse supports only xtal=32M (xtal was %d)" % apb_freq
+                "The eFuse supports only xtal=40M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
-        old_addr_reg = 0
-        reg_value = 0
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
-                addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
-                    block.id
-                ]
-                if err_num_mask is None or err_num_offs is None or fail_bit is None:
-                    continue
-                if addr_reg != old_addr_reg:
-                    old_addr_reg = addr_reg
-                    reg_value = self.read_reg(addr_reg)
-                block.fail = reg_value & (1 << fail_bit) != 0
-                block.num_errors = (reg_value >> err_num_offs) & err_num_mask
+                addr_reg_f, fail_bit = self.REGS.BLOCK_FAIL_BIT[block.id]
+                if fail_bit is None:
+                    block.fail = False
+                else:
+                    block.fail = self.read_reg(addr_reg_f) & (1 << fail_bit) != 0
+
+                addr_reg_n, num_mask, num_offs = self.REGS.BLOCK_NUM_ERRORS[block.id]
+                if num_mask is None or num_offs is None:
+                    block.num_errors = 0
+                else:
+                    block.num_errors = (
+                        self.read_reg(addr_reg_n) >> num_offs
+                    ) & num_mask
+
             ret_fail |= block.fail
             if not silent and (block.fail or block.num_errors):
                 print(
                     "Error(s) in BLOCK%d [ERRORS:%d FAIL:%d]"
                     % (block.id, block.num_errors, block.fail)
                 )
         if (self.debug or ret_fail) and not silent:
@@ -280,30 +298,43 @@
     def summary(self):
         # TODO add support set_flash_voltage - "Flash voltage (VDD_SPI)"
         return ""
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
@@ -352,19 +383,15 @@
             output = "Block%d has ERRORS:%d FAIL:%d" % (self.block, errs, fail)
         else:
             output = "OK"
         return "(" + output + ")"
 
     def get(self, from_read=True):
         if self.name == "CUSTOM_MAC":
-            mac = self.get_raw(from_read)[::-1] + self.parent["MAC_EXT"].get_raw(
-                from_read
-            )
-        elif self.name == "MAC":
-            mac = self.get_raw(from_read) + self.parent["MAC_EXT"].get_raw(from_read)
+            mac = self.get_raw(from_read)[::-1]
         else:
             mac = self.get_raw(from_read)
         return "%s %s" % (util.hexify(mac, ":"), self.check())
 
     def save(self, new_value):
         def print_field(e, new_value):
             print(
@@ -383,16 +410,15 @@
             raise esptool.FatalError("Writing Factory MAC address is not supported")
 
 
 # fmt: off
 class EfuseKeyPurposeField(EfuseField):
     KEY_PURPOSES = [
         ("USER",                         0,  None,       None,      "no_need_rd_protect"),   # User purposes (software-only use)
-        ("ECDSA_KEY",                    1,  None,       "Reverse", "need_rd_protect"),      # ECDSA key
-        ("RESERVED",                     2,  None,       None,      "no_need_rd_protect"),   # Reserved
+        ("RESERVED",                     1,  None,       None,      "no_need_rd_protect"),   # Reserved
         ("XTS_AES_128_KEY",              4,  None,       "Reverse", "need_rd_protect"),      # XTS_AES_128_KEY (flash/PSRAM encryption)
         ("HMAC_DOWN_ALL",                5,  None,       None,      "need_rd_protect"),      # HMAC Downstream mode
         ("HMAC_DOWN_JTAG",               6,  None,       None,      "need_rd_protect"),      # JTAG soft enable key (uses HMAC Downstream mode)
         ("HMAC_DOWN_DIGITAL_SIGNATURE",  7,  None,       None,      "need_rd_protect"),      # Digital Signature peripheral key (uses HMAC Downstream mode)
         ("HMAC_UP",                      8,  None,       None,      "need_rd_protect"),      # HMAC Upstream mode
         ("SECURE_BOOT_DIGEST0",          9,  "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST0 (Secure Boot key digest)
         ("SECURE_BOOT_DIGEST1",          10, "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST1 (Secure Boot key digest)
@@ -429,18 +455,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value in ["XTS_AES_128_KEY", "ECDSA_KEY"]:
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6/espefuse/efuse/esp32h2/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,27 +151,27 @@
             metavar="KEYPURPOSE",
             choices=fields.EfuseKeyPurposeField.DIGEST_KEY_PURPOSES,
         )
 
     p = subparsers.add_parser(
         "set_flash_voltage",
         help="Permanently set the internal flash voltage regulator "
-        "to either 1.8V, 3.3V or OFF. This means GPIO45 can be high or low "
-        "at reset without changing the flash voltage.",
+        "to either 1.8V, 3.3V or OFF. "
+        "This means GPIO45 can be high or low at reset without "
+        "changing the flash voltage.",
     )
     p.add_argument("voltage", help="Voltage selection", choices=["1.8V", "3.3V", "OFF"])
 
     p = subparsers.add_parser(
         "burn_custom_mac", help="Burn a 48-bit Custom MAC Address to EFUSE BLOCK3."
     )
     p.add_argument(
         "mac",
         help="Custom MAC Address to burn given in hexadecimal format with bytes "
-        "separated by colons (e.g. AA:CD:EF:01:02:03). "
-        "Final CUSTOM_MAC = CUSTOM_MAC[48] + MAC_EXT[16]",
+        "separated by colons (e.g. AA:CD:EF:01:02:03).",
         type=fields.base_fields.CheckArgValue(efuses, "CUSTOM_MAC"),
     )
     add_force_write_always(p)
 
     p = subparsers.add_parser("get_custom_mac", help="Prints the Custom MAC Address.")
```

### Comparing `esptool-4.6/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-H2(beta1)"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
```

### Comparing `esptool-4.6/espefuse/efuse/esp32h2beta1/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file describes eFuses for ESP32-H2 chip
 #
-# SPDX-FileCopyrightText: 2021-2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import binascii
 import struct
 import time
 
@@ -50,29 +50,30 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
-        if esp.CHIP_NAME != "ESP32-H2(beta1)":
+        if esp.CHIP_NAME != "ESP32-H2":
             raise esptool.FatalError(
-                "Expected the 'esp' param for ESP32-H2(beta1) chip but got for '%s'."
+                "Expected the 'esp' param for ESP32-H2 chip but got for '%s'."
                 % (esp.CHIP_NAME)
             )
         if not skip_connect:
             flags = self._esp.get_security_info()["flags"]
             GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE = 1 << 2
             if flags & GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE:
                 raise esptool.FatalError(
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MAJOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -219,57 +240,56 @@
                     exit(0)  # finish without errors
             raise
 
     def set_efuse_timing(self):
         """Set timing registers for burning efuses"""
         # Configure clock
         apb_freq = self.get_crystal_freq()
+        # Based on `CONFIG_SOC_XTAL_SUPPORT_32M=y` for this target from ESP-IDF configuration
         if apb_freq != 32:
             raise esptool.FatalError(
                 "The eFuse supports only xtal=32M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
-        old_addr_reg = 0
-        reg_value = 0
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
-                addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
-                    block.id
-                ]
-                if err_num_mask is None or err_num_offs is None or fail_bit is None:
-                    continue
-                if addr_reg != old_addr_reg:
-                    old_addr_reg = addr_reg
-                    reg_value = self.read_reg(addr_reg)
-                block.fail = reg_value & (1 << fail_bit) != 0
-                block.num_errors = (reg_value >> err_num_offs) & err_num_mask
+                addr_reg_f, fail_bit = self.REGS.BLOCK_FAIL_BIT[block.id]
+                if fail_bit is None:
+                    block.fail = False
+                else:
+                    block.fail = self.read_reg(addr_reg_f) & (1 << fail_bit) != 0
+
+                addr_reg_n, num_mask, num_offs = self.REGS.BLOCK_NUM_ERRORS[block.id]
+                if num_mask is None or num_offs is None:
+                    block.num_errors = 0
+                else:
+                    block.num_errors = (
+                        self.read_reg(addr_reg_n) >> num_offs
+                    ) & num_mask
+
             ret_fail |= block.fail
             if not silent and (block.fail or block.num_errors):
                 print(
                     "Error(s) in BLOCK%d [ERRORS:%d FAIL:%d]"
                     % (block.id, block.num_errors, block.fail)
                 )
         if (self.debug or ret_fail) and not silent:
@@ -279,30 +299,43 @@
     def summary(self):
         # TODO add support set_flash_voltage - "Flash voltage (VDD_SPI)"
         return ""
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
@@ -351,19 +384,15 @@
             output = "Block%d has ERRORS:%d FAIL:%d" % (self.block, errs, fail)
         else:
             output = "OK"
         return "(" + output + ")"
 
     def get(self, from_read=True):
         if self.name == "CUSTOM_MAC":
-            mac = self.get_raw(from_read)[::-1] + self.parent["MAC_EXT"].get_raw(
-                from_read
-            )
-        elif self.name == "MAC":
-            mac = self.get_raw(from_read) + self.parent["MAC_EXT"].get_raw(from_read)
+            mac = self.get_raw(from_read)[::-1]
         else:
             mac = self.get_raw(from_read)
         return "%s %s" % (util.hexify(mac, ":"), self.check())
 
     def save(self, new_value):
         def print_field(e, new_value):
             print(
@@ -382,26 +411,26 @@
             raise esptool.FatalError("Writing Factory MAC address is not supported")
 
 
 # fmt: off
 class EfuseKeyPurposeField(EfuseField):
     KEY_PURPOSES = [
         ("USER",                         0,  None,       None,      "no_need_rd_protect"),   # User purposes (software-only use)
-        ("RESERVED",                     1,  None,       None,      "no_need_rd_protect"),   # Reserved
+        ("ECDSA_KEY",                    1,  None,       "Reverse", "need_rd_protect"),      # ECDSA key
+        ("RESERVED",                     2,  None,       None,      "no_need_rd_protect"),   # Reserved
         ("XTS_AES_128_KEY",              4,  None,       "Reverse", "need_rd_protect"),      # XTS_AES_128_KEY (flash/PSRAM encryption)
         ("HMAC_DOWN_ALL",                5,  None,       None,      "need_rd_protect"),      # HMAC Downstream mode
         ("HMAC_DOWN_JTAG",               6,  None,       None,      "need_rd_protect"),      # JTAG soft enable key (uses HMAC Downstream mode)
         ("HMAC_DOWN_DIGITAL_SIGNATURE",  7,  None,       None,      "need_rd_protect"),      # Digital Signature peripheral key (uses HMAC Downstream mode)
         ("HMAC_UP",                      8,  None,       None,      "need_rd_protect"),      # HMAC Upstream mode
         ("SECURE_BOOT_DIGEST0",          9,  "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST0 (Secure Boot key digest)
         ("SECURE_BOOT_DIGEST1",          10, "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST1 (Secure Boot key digest)
         ("SECURE_BOOT_DIGEST2",          11, "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST2 (Secure Boot key digest)
     ]
 # fmt: on
-
     KEY_PURPOSES_NAME = [name[0] for name in KEY_PURPOSES]
     DIGEST_KEY_PURPOSES = [name[0] for name in KEY_PURPOSES if name[2] == "DIGEST"]
 
     def check_format(self, new_value_str):
         # str convert to int: "XTS_AES_128_KEY" - > str(4)
         # if int: 4 -> str(4)
         raw_val = new_value_str
@@ -428,18 +457,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value.startswith("XTS_AES"):
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6/espefuse/efuse/esp32h2beta1/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 def set_flash_voltage(esp, efuses, args):
     raise esptool.FatalError("set_flash_voltage is not supported!")
 
 
 def adc_info(esp, efuses, args):
     print("")
     # fmt: off
-    if efuses["BLK_VERSION_MAJOR"].get() == 1:
+    if efuses["BLOCK2_VERSION"].get() == 1:
         print("Temperature Sensor Calibration = {}C".format(efuses["TEMP_SENSOR_CAL"].get()))
 
         print("")
         print("ADC1 readings stored in efuse BLOCK2:")
         print("    MODE0 D1 reading  (250mV):  {}".format(efuses["ADC1_MODE0_D1"].get()))
         print("    MODE0 D2 reading  (600mV):  {}".format(efuses["ADC1_MODE0_D2"].get()))
 
@@ -221,15 +221,15 @@
 
         print("    MODE2 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE2_D1"].get()))
         print("    MODE2 D2 reading  (1000mV): {}".format(efuses["ADC2_MODE2_D2"].get()))
 
         print("    MODE3 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE3_D1"].get()))
         print("    MODE3 D2 reading  (2000mV): {}".format(efuses["ADC2_MODE3_D2"].get()))
     else:
-        print("BLK_VERSION_MAJOR = {}".format(efuses["BLK_VERSION_MAJOR"].get_meaning()))
+        print("BLOCK2_VERSION = {}".format(efuses["BLOCK2_VERSION"].get_meaning()))
     # fmt: on
 
 
 def burn_key(esp, efuses, args, digest=None):
     if digest is None:
         datafile_list = args.keyfile[
             0 : len([name for name in args.keyfile if name is not None]) :
```

### Comparing `esptool-4.6/espefuse/efuse/esp32s2/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s2/emulate_efuse_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-S2"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 1
```

### Comparing `esptool-4.6/espefuse/efuse/esp32s2/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s2/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,23 +50,24 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
         if esp.CHIP_NAME != "ESP32-S2":
             raise esptool.FatalError(
                 "Expected the 'esp' param for ESP32-S2 chip but got for '%s'."
                 % (esp.CHIP_NAME)
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MINOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -285,17 +306,20 @@
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
                     block.id
                 ]
                 if err_num_mask is None or err_num_offs is None or fail_bit is None:
@@ -314,45 +338,57 @@
         if (self.debug or ret_fail) and not silent:
             self.print_status_regs()
         return ret_fail
 
     def summary(self):
         if self["VDD_SPI_FORCE"].get() == 0:
             output = "Flash voltage (VDD_SPI) determined by GPIO45 on reset "
-            output += "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
+            "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
             output += "GPIO45=Low or NC: VDD_SPI pin is powered directly from "
-            output += "VDD3P3_RTC_IO via resistor Rspi. "
-            output += "Typically this voltage is 3.3 V)."
+            "VDD3P3_RTC_IO via resistor Rspi. Typically this voltage is 3.3 V)."
         elif self["VDD_SPI_XPD"].get() == 0:
             output = "Flash voltage (VDD_SPI) internal regulator disabled by efuse."
         elif self["VDD_SPI_TIEH"].get() == 0:
             output = "Flash voltage (VDD_SPI) set to 1.8V by efuse."
         else:
             output = "Flash voltage (VDD_SPI) set to 3.3V by efuse."
         return output
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
```

### Comparing `esptool-4.6/espefuse/efuse/esp32s2/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s2/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/espefuse/efuse/esp32s3/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3/emulate_efuse_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-S3"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
```

### Comparing `esptool-4.6/espefuse/efuse/esp32s3/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,23 +50,24 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
         if esp.CHIP_NAME != "ESP32-S3":
             raise esptool.FatalError(
                 "Expected the 'esp' param for ESP32-S3 chip but got for '%s'."
                 % (esp.CHIP_NAME)
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MAJOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -224,21 +245,14 @@
         # Configure clock
         apb_freq = self.get_crystal_freq()
         if apb_freq != 40:
             raise esptool.FatalError(
                 "The eFuse supports only xtal=40M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
         old_addr_reg = 0
@@ -246,17 +260,20 @@
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
                     block.id
                 ]
                 if err_num_mask is None or err_num_offs is None or fail_bit is None:
@@ -275,45 +292,57 @@
         if (self.debug or ret_fail) and not silent:
             self.print_status_regs()
         return ret_fail
 
     def summary(self):
         if self["VDD_SPI_FORCE"].get() == 0:
             output = "Flash voltage (VDD_SPI) determined by GPIO45 on reset "
-            output += "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
+            "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
             output += "GPIO45=Low or NC: VDD_SPI pin is powered directly from "
-            output += "VDD3P3_RTC_IO via resistor Rspi. "
-            output += "Typically this voltage is 3.3 V)."
+            "VDD3P3_RTC_IO via resistor Rspi. Typically this voltage is 3.3 V)."
         elif self["VDD_SPI_XPD"].get() == 0:
             output = "Flash voltage (VDD_SPI) internal regulator disabled by efuse."
         elif self["VDD_SPI_TIEH"].get() == 0:
             output = "Flash voltage (VDD_SPI) set to 1.8V by efuse."
         else:
             output = "Flash voltage (VDD_SPI) set to 3.3V by efuse."
         return output
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
@@ -438,18 +467,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value.startswith("XTS_AES"):
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6/espefuse/efuse/esp32s3/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-S3(beta2)"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
```

### Comparing `esptool-4.6/espefuse/efuse/esp32s3beta2/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,23 +50,24 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
         if esp.CHIP_NAME != "ESP32-S3(beta2)":
             raise esptool.FatalError(
                 "Expected the 'esp' param for ESP32-S3(beta2) chip but got for '%s'."
                 % (esp.CHIP_NAME)
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MAJOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -224,21 +245,14 @@
         # Configure clock
         apb_freq = self.get_crystal_freq()
         if apb_freq != 40:
             raise esptool.FatalError(
                 "The eFuse supports only xtal=40M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
         old_addr_reg = 0
@@ -246,17 +260,20 @@
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
                     block.id
                 ]
                 if err_num_mask is None or err_num_offs is None or fail_bit is None:
@@ -275,45 +292,57 @@
         if (self.debug or ret_fail) and not silent:
             self.print_status_regs()
         return ret_fail
 
     def summary(self):
         if self["VDD_SPI_FORCE"].get() == 0:
             output = "Flash voltage (VDD_SPI) determined by GPIO45 on reset "
-            output += "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
+            "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
             output += "GPIO45=Low or NC: VDD_SPI pin is powered directly from "
-            output += "VDD3P3_RTC_IO via resistor Rspi. "
-            output += "Typically this voltage is 3.3 V)."
+            "VDD3P3_RTC_IO via resistor Rspi. Typically this voltage is 3.3 V)."
         elif self["VDD_SPI_XPD"].get() == 0:
             output = "Flash voltage (VDD_SPI) internal regulator disabled by efuse."
         elif self["VDD_SPI_TIEH"].get() == 0:
             output = "Flash voltage (VDD_SPI) set to 1.8V by efuse."
         else:
             output = "Flash voltage (VDD_SPI) set to 3.3V by efuse."
         return output
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
@@ -438,18 +467,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value.startswith("XTS_AES"):
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6/espefuse/efuse/esp32s3beta2/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/espefuse/efuse/util.py` & `esptool-4.6.dev1/espefuse/efuse/util.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/espefuse.py` & `esptool-4.6.dev1/espefuse.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,20 +14,17 @@
 import os
 import sys
 
 if os.name != "nt":
     # Linux/macOS: remove current script directory to avoid importing this file
     # as a module; we want to import the installed espefuse module instead
     with contextlib.suppress(ValueError):
-        executable_dir = os.path.dirname(sys.executable)
-        sys.path = [
-            path
-            for path in sys.path
-            if not path.endswith(("/bin", "/sbin")) and path != executable_dir
-        ]
+        if sys.path[0].endswith("/bin"):
+            sys.path.pop(0)
+        sys.path.remove(os.path.dirname(sys.executable))
 
     # Linux/macOS: delete imported module entry to force Python to load
     # the module from scratch; this enables importing espefuse module in
     # other Python scripts
     with contextlib.suppress(KeyError):
         del sys.modules["espefuse"]
```

### Comparing `esptool-4.6/espsecure/__init__.py` & `esptool-4.6.dev1/espsecure/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,21 +198,15 @@
             raise esptool.FatalError(
                 "ERROR: Unsupported signing scheme (%s)" % args.scheme
             )
 
 
 def load_ecdsa_signing_key(keyfile):
     """Load ECDSA signing key"""
-    try:
-        sk = ecdsa.SigningKey.from_pem(keyfile.read())
-    except ValueError:
-        raise esptool.FatalError(
-            "Incorrect ECDSA private key specified. "
-            "Please check algorithm and/or format."
-        )
+    sk = ecdsa.SigningKey.from_pem(keyfile.read())
     if sk.curve not in [ecdsa.NIST192p, ecdsa.NIST256p]:
         raise esptool.FatalError("Supports NIST192p and NIST256p keys only")
     return sk
 
 
 def _load_ecdsa_signing_key(keyfile):
     """Load ECDSA signing key for Secure Boot V1 only"""
@@ -223,21 +217,15 @@
             "NIST256p (openssl calls this curve 'prime256v1')"
         )
     return sk
 
 
 def _load_ecdsa_verifying_key(keyfile):
     """Load ECDSA verifying key for Secure Boot V1 only"""
-    try:
-        vk = ecdsa.VerifyingKey.from_pem(keyfile.read())
-    except ValueError:
-        raise esptool.FatalError(
-            "Incorrect ECDSA public key specified. "
-            "Please check algorithm and/or format."
-        )
+    vk = ecdsa.VerifyingKey.from_pem(keyfile.read())
     if vk.curve != ecdsa.NIST256p:
         raise esptool.FatalError(
             "Signing key uses incorrect curve. ESP32 Secure Boot only supports "
             "NIST256p (openssl calls this curve 'prime256v1')"
         )
     return vk
 
@@ -1653,16 +1641,15 @@
         help="Secure boot v2 signed data file.",
         type=argparse.FileType("rb"),
     )
 
     p = subparsers.add_parser(
         "digest_private_key",
         help="Generate an SHA-256 digest of the private signing key. "
-        "This can be used as a reproducible secure bootloader (only secure boot v1) "
-        "or flash encryption key.",
+        "This can be used as a reproducible secure bootloader or flash encryption key.",
     )
     p.add_argument(
         "--keyfile",
         "-k",
         help="Private key file (PEM format) to generate a digest from.",
         type=argparse.FileType("rb"),
         required=True,
@@ -1808,21 +1795,11 @@
 
 def _main():
     try:
         main()
     except esptool.FatalError as e:
         print("\nA fatal error occurred: %s" % e)
         sys.exit(2)
-    except ValueError as e:
-        try:
-            if [arg for arg in e.args if "Could not deserialize key data." in arg]:
-                print(
-                    "Note: This error originates from the cryptography module. "
-                    "It is likely not a problem with espsecure, "
-                    "please make sure you are using a compatible OpenSSL backend."
-                )
-        finally:
-            raise
 
 
 if __name__ == "__main__":
     _main()
```

### Comparing `esptool-4.6/espsecure/esp_hsm_sign/__init__.py` & `esptool-4.6.dev1/espsecure/esp_hsm_sign/__init__.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/espsecure/esp_hsm_sign/exceptions.py` & `esptool-4.6.dev1/espsecure/esp_hsm_sign/exceptions.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/espsecure.py` & `esptool-4.6.dev1/espsecure.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,17 @@
 import os
 import sys
 
 if os.name != "nt":
     # Linux/macOS: remove current script directory to avoid importing this file
     # as a module; we want to import the installed espsecure module instead
     with contextlib.suppress(ValueError):
-        executable_dir = os.path.dirname(sys.executable)
-        sys.path = [
-            path
-            for path in sys.path
-            if not path.endswith(("/bin", "/sbin")) and path != executable_dir
-        ]
+        if sys.path[0].endswith("/bin"):
+            sys.path.pop(0)
+        sys.path.remove(os.path.dirname(sys.executable))
 
     # Linux/macOS: delete imported module entry to force Python to load
     # the module from scratch; this enables importing espsecure module in
     # other Python scripts
     with contextlib.suppress(KeyError):
         del sys.modules["espsecure"]
```

### Comparing `esptool-4.6/esptool/__init__.py` & `esptool-4.6.dev1/esptool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,26 +24,24 @@
     "verify_flash",
     "version",
     "write_flash",
     "write_flash_status",
     "write_mem",
 ]
 
-__version__ = "4.6"
-
+__version__ = "4.6.dev1"
 import argparse
 import inspect
 import os
 import shlex
 import sys
 import time
 import traceback
 
 from esptool.cmds import (
-    DETECTED_FLASH_SIZES,
     chip_id,
     detect_chip,
     detect_flash_size,
     dump_mem,
     elf2image,
     erase_flash,
     erase_region,
@@ -351,15 +349,15 @@
         "(default if --no-stub is specified)",
         action="store_true",
     )
 
     subparsers.add_parser("run", help="Run application code in flash")
 
     parser_image_info = subparsers.add_parser(
-        "image_info", help="Dump headers from a binary file (bootloader or application)"
+        "image_info", help="Dump headers from an application image"
     )
     parser_image_info.add_argument("filename", help="Image file to parse")
     parser_image_info.add_argument(
         "--version",
         "-v",
         help="Output format version (1 - legacy, 2 - extended)",
         choices=["1", "2"],
@@ -523,17 +521,15 @@
 
     parser_read_flash = subparsers.add_parser(
         "read_flash", help="Read SPI flash content"
     )
     add_spi_connection_arg(parser_read_flash)
     parser_read_flash.add_argument("address", help="Start address", type=arg_auto_int)
     parser_read_flash.add_argument(
-        "size",
-        help="Size of region to dump. Use `ALL` to read to the end of flash.",
-        type=arg_auto_size,
+        "size", help="Size of region to dump", type=arg_auto_int
     )
     parser_read_flash.add_argument("filename", help="Name of binary dump")
     parser_read_flash.add_argument(
         "--no-progress", "-p", help="Suppress progress output", action="store_true"
     )
 
     parser_verify_flash = subparsers.add_parser(
@@ -569,17 +565,16 @@
     )
     add_spi_connection_arg(parser_erase_region)
     parser_erase_region.add_argument(
         "address", help="Start address (must be multiple of 4096)", type=arg_auto_int
     )
     parser_erase_region.add_argument(
         "size",
-        help="Size of region to erase (must be multiple of 4096). "
-        "Use `ALL` to erase to the end of flash.",
-        type=arg_auto_size,
+        help="Size of region to erase (must be multiple of 4096)",
+        type=arg_auto_int,
     )
 
     parser_merge_bin = subparsers.add_parser(
         "merge_bin",
         help="Merge multiple raw binary files into a single file for later flashing",
     )
 
@@ -811,47 +806,24 @@
             try:
                 flash_xmc_startup()
             except FatalError as e:
                 esp.trace(f"Unable to perform XMC flash chip startup sequence ({e}).")
 
         if hasattr(args, "flash_size"):
             print("Configuring flash size...")
-            if args.flash_size == "detect":
-                flash_size = detect_flash_size(esp, args)
-            elif args.flash_size == "keep":
-                flash_size = detect_flash_size(esp, args=None)
-            else:
-                flash_size = args.flash_size
-
-            if flash_size is not None:  # Secure download mode
-                esp.flash_set_parameters(flash_size_bytes(flash_size))
+            detect_flash_size(esp, args)
+            if args.flash_size != "keep":  # TODO: should set this even with 'keep'
+                esp.flash_set_parameters(flash_size_bytes(args.flash_size))
                 # Check if stub supports chosen flash size
-                if esp.IS_STUB and flash_size in ("32MB", "64MB", "128MB"):
+                if esp.IS_STUB and args.flash_size in ("32MB", "64MB", "128MB"):
                     print(
                         "WARNING: Flasher stub doesn't fully support flash size larger "
                         "than 16MB, in case of failure use --no-stub."
                     )
 
-        if getattr(args, "size", "") == "all":
-            if esp.secure_download_mode:
-                raise FatalError(
-                    "Detecting flash size is not supported in secure download mode. "
-                    "Set an exact size value."
-                )
-            # detect flash size
-            flash_id = esp.flash_id()
-            size_id = flash_id >> 16
-            size_str = DETECTED_FLASH_SIZES.get(size_id)
-            if size_str is None:
-                raise FatalError(
-                    "Detecting flash size failed. Set an exact size value."
-                )
-            print(f"Detected flash size: {size_str}")
-            args.size = flash_size_bytes(size_str)
-
         if esp.IS_STUB and hasattr(args, "address") and hasattr(args, "size"):
             if args.address + args.size > 0x1000000:
                 print(
                     "WARNING: Flasher stub doesn't fully support flash size larger "
                     "than 16MB, in case of failure use --no-stub."
                 )
 
@@ -888,19 +860,14 @@
         operation_func(args)
 
 
 def arg_auto_int(x):
     return int(x, 0)
 
 
-def arg_auto_size(x):
-    x = x.lower()
-    return x if x == "all" else arg_auto_int(x)
-
-
 def get_port_list():
     if list_ports is None:
         raise FatalError(
             "Listing all serial ports is currently not available. "
             "Please try to specify the port when running esptool.py or update "
             "the pyserial package to the latest version"
         )
```

### Comparing `esptool-4.6/esptool/bin_image.py` & `esptool-4.6.dev1/esptool/bin_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,24 +636,14 @@
             # move ".flash.appdesc" segment to the top of the flash segment
             for segment in flash_segments:
                 if segment.name == ".flash.appdesc":
                     flash_segments.remove(segment)
                     flash_segments.insert(0, segment)
                     break
 
-            # For the bootloader image
-            # move ".dram0.bootdesc" segment to the top of the ram segment
-            # So bootdesc will be at the very top of the binary at 0x20 offset
-            # (in the first segment).
-            for segment in ram_segments:
-                if segment.name == ".dram0.bootdesc":
-                    ram_segments.remove(segment)
-                    ram_segments.insert(0, segment)
-                    break
-
             # check for multiple ELF sections that are mapped in the same
             # flash mapping region. This is usually a sign of a broken linker script,
             # but if you have a legitimate use case then let us know
             if len(flash_segments) > 0:
                 last_addr = flash_segments[0].addr
                 for segment in flash_segments[1:]:
                     if segment.addr // self.IROM_ALIGN == last_addr // self.IROM_ALIGN:
@@ -809,14 +799,21 @@
                 % (self.ROM_LOADER.IMAGE_CHIP_ID, self.chip_id)
             )
 
         self.min_rev = fields[5]
         self.min_rev_full = fields[6]
         self.max_rev_full = fields[7]
 
+        # reserved fields in the middle should all be zero
+        if any(f for f in fields[8:-1] if f != 0):
+            print(
+                "Warning: some reserved header fields have non-zero values. "
+                "This image may be from a newer esptool.py?"
+            )
+
         append_digest = fields[-1]  # last byte is append_digest
         if append_digest in [0, 1]:
             self.append_digest = append_digest == 1
         else:
             raise RuntimeError(
                 "Invalid value for append_digest field (0x%02x). Should be 0 or 1.",
                 append_digest,
```

### Comparing `esptool-4.6/esptool/cmds.py` & `esptool-4.6.dev1/esptool/cmds.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     NotImplementedInROMError,
     NotSupportedError,
     UnsupportedCommandError,
 )
 from .util import (
     div_roundup,
     flash_size_bytes,
-    get_file_size,
     hexify,
     pad_to,
     print_overwrite,
 )
 
 DETECTED_FLASH_SIZES = {
     0x12: "256KB",
@@ -205,38 +204,32 @@
                     "%d bytes read... (%d %%)" % (f.tell(), f.tell() * 100 // args.size)
                 )
             sys.stdout.flush()
         print_overwrite("Read %d bytes" % f.tell(), last_line=True)
     print("Done!")
 
 
-def detect_flash_size(esp, args=None):
-    # TODO: Remove the dependency on args in the next major release (v5.0)
-    if esp.secure_download_mode:
-        if args is not None and args.flash_size == "detect":
+def detect_flash_size(esp, args):
+    if args.flash_size == "detect":
+        if esp.secure_download_mode:
             raise FatalError(
                 "Detecting flash size is not supported in secure download mode. "
                 "Need to manually specify flash size."
             )
-        else:
-            return None
-    flash_id = esp.flash_id()
-    size_id = flash_id >> 16
-    flash_size = DETECTED_FLASH_SIZES.get(size_id)
-    if args is not None and args.flash_size == "detect":
-        if flash_size is None:
-            flash_size = "4MB"
+        flash_id = esp.flash_id()
+        size_id = flash_id >> 16
+        args.flash_size = DETECTED_FLASH_SIZES.get(size_id)
+        if args.flash_size is None:
             print(
-                "Warning: Could not auto-detect Flash size "
-                f"(FlashID={flash_id:#x}, SizeID={size_id:#x}), defaulting to 4MB"
+                "Warning: Could not auto-detect Flash size (FlashID=0x%x, SizeID=0x%x),"
+                " defaulting to 4MB" % (flash_id, size_id)
             )
+            args.flash_size = "4MB"
         else:
-            print("Auto-detected Flash size:", flash_size)
-        args.flash_size = flash_size
-    return flash_size
+            print("Auto-detected Flash size:", args.flash_size)
 
 
 def _update_image_flash_params(esp, address, args, image):
     """
     Modify the flash mode & size bytes if this looks like an executable bootloader image
     """
     if len(image) < 8:
@@ -459,18 +452,16 @@
                     "WARNING: Detected flash encryption enabled and "
                     "download manual encrypt disabled.\n"
                     "Flashing plaintext binary may brick your device! "
                     "Use --force to override the warning."
                 )
 
     # verify file sizes fit in flash
-    flash_end = flash_size_bytes(
-        detect_flash_size(esp) if args.flash_size == "keep" else args.flash_size
-    )
-    if flash_end is not None:  # Secure download mode
+    if args.flash_size != "keep":  # TODO: check this even with 'keep'
+        flash_end = flash_size_bytes(args.flash_size)
         for address, argfile in args.addr_filename:
             argfile.seek(0, os.SEEK_END)
             if address + argfile.tell() > flash_end:
                 raise FatalError(
                     "File %s (length %d) at offset %d "
                     "will not fit in %d bytes of flash. "
                     "Use --flash_size argument, or change flashing address."
@@ -734,39 +725,28 @@
 
         # Extended header (ESP32 and later only)
         if args.chip != "esp8266":
             print()
             title = "{} extended image header".format(args.chip.upper())
             print(title)
             print("=" * len(title))
-            print(
-                f"WP pin: {image.wp_pin:#02x}",
-                *["(disabled)"] if image.wp_pin == image.WP_PIN_DISABLED else [],
-            )
+            print("WP pin: {:#02x}".format(image.wp_pin))
             print(
                 "Flash pins drive settings: "
                 "clk_drv: {:#02x}, q_drv: {:#02x}, d_drv: {:#02x}, "
                 "cs0_drv: {:#02x}, hd_drv: {:#02x}, wp_drv: {:#02x}".format(
                     image.clk_drv,
                     image.q_drv,
                     image.d_drv,
                     image.cs_drv,
                     image.hd_drv,
                     image.wp_drv,
                 )
             )
-            try:
-                chip = next(
-                    chip
-                    for chip in CHIP_DEFS.values()
-                    if getattr(chip, "IMAGE_CHIP_ID", None) == image.chip_id
-                )
-                print(f"Chip ID: {image.chip_id} ({chip.CHIP_NAME})")
-            except StopIteration:
-                print(f"Chip ID: {image.chip_id} (Unknown ID)")
+            print("Chip ID: {}".format(image.chip_id))
             print(
                 "Minimal chip revision: "
                 f"v{image.min_rev_full // 100}.{image.min_rev_full % 100}, "
                 f"(legacy min_rev = {image.min_rev})"
             )
             print(
                 "Maximal chip revision: "
@@ -785,24 +765,19 @@
             )
         )
         print(
             "{}  {}  {}  {}  {}".format("-" * 7, "-" * 7, "-" * 10, "-" * 10, "-" * 12)
         )
         format_str = "{:7}  {:#07x}  {:#010x}  {:#010x}  {}"
         app_desc = None
-        bootloader_desc = None
         for idx, seg in enumerate(image.segments, start=1):
             segs = seg.get_memory_type(image)
             seg_name = ", ".join(segs)
             if "DROM" in segs:  # The DROM segment starts with the esp_app_desc_t struct
                 app_desc = seg.data[:256]
-            elif "DRAM" in segs:
-                # The DRAM segment starts with the esp_bootloader_desc_t struct
-                if len(seg.data) >= 80:
-                    bootloader_desc = seg.data[:80]
             print(
                 format_str.format(idx, len(seg.data), seg.addr, seg.file_offs, seg_name)
             )
         print()
 
         # Footer
         title = f"{args.chip.upper()} image footer"
@@ -852,35 +827,14 @@
                 print(f'Project name: {project_name.decode("utf-8")}')
                 print(f'App version: {version.decode("utf-8")}')
                 print(f'Compile time: {date.decode("utf-8")} {time.decode("utf-8")}')
                 print(f"ELF file SHA256: {hexify(app_elf_sha256, uppercase=False)}")
                 print(f'ESP-IDF: {idf_ver.decode("utf-8")}')
                 print(f"Secure version: {secure_version}")
 
-        elif bootloader_desc:
-            BOOTLOADER_DESC_STRUCT_FMT = "<B" + "3s" + "I32s24s" + "16s"
-            (
-                magic_byte,
-                reserved,
-                version,
-                idf_ver,
-                date_time,
-                reserved2,
-            ) = struct.unpack(BOOTLOADER_DESC_STRUCT_FMT, bootloader_desc)
-
-            if magic_byte == 80:
-                print()
-                title = "Bootloader information"
-                print(title)
-                print("=" * len(title))
-                print(f"Bootloader version: {version}")
-                print(f'ESP-IDF: {idf_ver.decode("utf-8")}')
-                print(f'Compile time: {date_time.decode("utf-8")}')
-
-    print(f"File size: {get_file_size(args.filename)} (bytes)")
     with open(args.filename, "rb") as f:
         # magic number
         try:
             common_header = f.read(8)
             magic = common_header[0]
         except IndexError:
             raise FatalError("File is empty")
@@ -892,14 +846,17 @@
                 "This is not a valid image "
                 "(invalid magic number: {:#x})".format(magic)
             )
 
         if args.chip == "auto":
             try:
                 extended_header = f.read(16)
+                # reserved fields, should all be zero
+                if int.from_bytes(extended_header[7:-1], "little") != 0:
+                    raise FatalError("Reserved fields not all zero")
 
                 # append_digest, either 0 or 1
                 if extended_header[-1] not in [0, 1]:
                     raise FatalError("Append digest field not 0 or 1")
 
                 chip_id = int.from_bytes(extended_header[4:5], "little")
                 for rom in [n for n in ROM_LIST if n.CHIP_NAME != "ESP8266"]:
```

### Comparing `esptool-4.6/esptool/config.py` & `esptool-4.6.dev1/esptool/config.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/loader.py` & `esptool-4.6.dev1/esptool/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,21 +93,21 @@
 # Timeout for serial port write
 DEFAULT_SERIAL_WRITE_TIMEOUT = cfg.getfloat("serial_write_timeout", 10)
 # Default number of times to try connection
 DEFAULT_CONNECT_ATTEMPTS = cfg.getint("connect_attempts", 7)
 # Number of times to try writing a data block
 WRITE_BLOCK_ATTEMPTS = cfg.getint("write_block_attempts", 3)
 
-STUBS_DIR = os.path.join(os.path.dirname(__file__), "targets", "stub_flasher")
+STUBS_DIR = os.path.join(os.path.dirname(__file__), "./targets/stub_flasher/")
 
 
 def get_stub_json_path(chip_name):
     chip_name = strip_chip_name(chip_name)
     chip_name = chip_name.replace("esp", "")
-    return os.path.join(STUBS_DIR, f"stub_flasher_{chip_name}.json")
+    return STUBS_DIR + "stub_flasher_" + chip_name + ".json"
 
 
 def timeout_per_mb(seconds_per_mb, size_bytes):
     """Scales timeouts which are size-specific"""
     result = seconds_per_mb * (size_bytes / 1e6)
     if result < DEFAULT_TIMEOUT:
         return DEFAULT_TIMEOUT
@@ -490,22 +490,20 @@
                 "COM and /dev/ serial ports."
             )
             return
         # Return the real path if the active port is a symlink
         if active_port.startswith("/dev/") and os.path.islink(active_port):
             active_port = os.path.realpath(active_port)
 
-        active_ports = [active_port]
-
         # The "cu" (call-up) device has to be used for outgoing communication on MacOS
         if sys.platform == "darwin" and "tty" in active_port:
-            active_ports.append(active_port.replace("tty", "cu"))
+            active_port = [active_port, active_port.replace("tty", "cu")]
         ports = list_ports.comports()
         for p in ports:
-            if p.device in active_ports:
+            if p.device in active_port:
                 return p.pid
         print(
             "\nFailed to get PID of a device on {}, "
             "using standard reset sequence.".format(active_port)
         )
 
     def _connect_attempt(self, reset_strategy, mode="default_reset"):
```

### Comparing `esptool-4.6/esptool/reset.py` & `esptool-4.6.dev1/esptool/reset.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/__init__.py` & `esptool-4.6.dev1/esptool/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/esp32.py` & `esptool-4.6.dev1/esptool/targets/esp32.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/esp32c2.py` & `esptool-4.6.dev1/esptool/targets/esp32c2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/esp32c3.py` & `esptool-4.6.dev1/esptool/targets/esp32c3.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,23 +71,18 @@
     SUPPORTS_ENCRYPTED_FLASH = True
 
     FLASH_ENCRYPTED_WRITE_ALIGN = 16
 
     UARTDEV_BUF_NO = 0x3FCDF07C  # Variable in ROM .bss which indicates the port in use
     UARTDEV_BUF_NO_USB_JTAG_SERIAL = 3  # The above var when USB-JTAG/Serial is used
 
+    RTC_CNTL_WDT_WKEY = 0x50D83AA1
     RTCCNTL_BASE_REG = 0x60008000
-    RTC_CNTL_SWD_CONF_REG = RTCCNTL_BASE_REG + 0x00AC
-    RTC_CNTL_SWD_AUTO_FEED_EN = 1 << 31
-    RTC_CNTL_SWD_WPROTECT_REG = RTCCNTL_BASE_REG + 0x00B0
-    RTC_CNTL_SWD_WKEY = 0x8F1D312A
-
     RTC_CNTL_WDTCONFIG0_REG = RTCCNTL_BASE_REG + 0x0090
     RTC_CNTL_WDTWPROTECT_REG = RTCCNTL_BASE_REG + 0x00A8
-    RTC_CNTL_WDT_WKEY = 0x50D83AA1
 
     MEMORY_MAP = [
         [0x00000000, 0x00010000, "PADDING"],
         [0x3C000000, 0x3C800000, "DROM"],
         [0x3FC80000, 0x3FCE0000, "DRAM"],
         [0x3FC88000, 0x3FD00000, "BYTE_ACCESSIBLE"],
         [0x3FF00000, 0x3FF20000, "DROM_MASK"],
@@ -176,35 +171,25 @@
         """
         Check the UARTDEV_BUF_NO register to see if USB-JTAG/Serial is being used
         """
         if self.secure_download_mode:
             return False  # Can't detect USB-JTAG/Serial in secure download mode
         return self.get_uart_no() == self.UARTDEV_BUF_NO_USB_JTAG_SERIAL
 
-    def disable_watchdogs(self):
-        # When USB-JTAG/Serial is used, the RTC WDT and SWD watchdog are not reset
-        # and can then reset the board during flashing. Disable or autofeed them.
+    def disable_rtc_watchdog(self):
+        # When USB-JTAG/Serial is used, the RTC watchdog is not reset
+        # and can then reset the board during flashing. Disable it.
         if self.uses_usb_jtag_serial():
-            # Disable RTC WDT
             self.write_reg(self.RTC_CNTL_WDTWPROTECT_REG, self.RTC_CNTL_WDT_WKEY)
             self.write_reg(self.RTC_CNTL_WDTCONFIG0_REG, 0)
             self.write_reg(self.RTC_CNTL_WDTWPROTECT_REG, 0)
 
-            # Automatically feed SWD
-            self.write_reg(self.RTC_CNTL_SWD_WPROTECT_REG, self.RTC_CNTL_SWD_WKEY)
-            self.write_reg(
-                self.RTC_CNTL_SWD_CONF_REG,
-                self.read_reg(self.RTC_CNTL_SWD_CONF_REG)
-                | self.RTC_CNTL_SWD_AUTO_FEED_EN,
-            )
-            self.write_reg(self.RTC_CNTL_SWD_WPROTECT_REG, 0)
-
     def _post_connect(self):
         if not self.sync_stub_detected:  # Don't run if stub is reused
-            self.disable_watchdogs()
+            self.disable_rtc_watchdog()
 
 
 class ESP32C3StubLoader(ESP32C3ROM):
     """Access class for ESP32C3 stub loader, runs on top of ROM.
 
     (Basically the same as ESP32StubLoader, but different base class.
     Can possibly be made into a mixin.)
```

### Comparing `esptool-4.6/esptool/targets/esp32c6.py` & `esptool-4.6.dev1/esptool/targets/esp32c6.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,14 @@
     UARTDEV_BUF_NO = 0x4087F580  # Variable in ROM .bss which indicates the port in use
     UARTDEV_BUF_NO_USB_JTAG_SERIAL = 3  # The above var when USB-JTAG/Serial is used
 
     DR_REG_LP_WDT_BASE = 0x600B1C00
     RTC_CNTL_WDTCONFIG0_REG = DR_REG_LP_WDT_BASE + 0x0  # LP_WDT_RWDT_CONFIG0_REG
     RTC_CNTL_WDTWPROTECT_REG = DR_REG_LP_WDT_BASE + 0x0018  # LP_WDT_RWDT_WPROTECT_REG
 
-    RTC_CNTL_SWD_CONF_REG = DR_REG_LP_WDT_BASE + 0x001C  # LP_WDT_SWD_CONFIG_REG
-    RTC_CNTL_SWD_AUTO_FEED_EN = 1 << 18
-    RTC_CNTL_SWD_WPROTECT_REG = DR_REG_LP_WDT_BASE + 0x0020  # LP_WDT_SWD_WPROTECT_REG
-    RTC_CNTL_SWD_WKEY = 0x50D83AA1  # LP_WDT_SWD_WKEY, same as WDT key in this case
-
     FLASH_FREQUENCY = {
         "80m": 0x0,  # workaround for wrong mspi HS div value in ROM
         "40m": 0x0,
         "20m": 0x2,
     }
 
     MEMORY_MAP = [
@@ -99,28 +94,27 @@
         [0x50000000, 0x50004000, "RTC_IRAM"],
         [0x50000000, 0x50004000, "RTC_DRAM"],
         [0x600FE000, 0x60100000, "MEM_INTERNAL2"],
     ]
 
     def get_pkg_version(self):
         num_word = 3
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 24) & 0x07
+        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 29) & 0x07
 
     def get_minor_chip_version(self):
         num_word = 3
         return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 18) & 0x0F
 
     def get_major_chip_version(self):
         num_word = 3
         return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 22) & 0x03
 
     def get_chip_description(self):
         chip_name = {
-            0: "ESP32-C6 (QFN40)",
-            1: "ESP32-C6FH4 (QFN32)",
+            0: "ESP32-C6",
         }.get(self.get_pkg_version(), "unknown ESP32-C6")
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
         return f"{chip_name} (revision v{major_rev}.{minor_rev})"
 
     def get_chip_features(self):
         return ["WiFi 6", "BT 5", "IEEE802.15.4"]
@@ -132,20 +126,16 @@
     def override_vddsdio(self, new_voltage):
         raise NotImplementedInROMError(
             "VDD_SDIO overrides are not supported for ESP32-C6"
         )
 
     def read_mac(self):
         mac0 = self.read_reg(self.MAC_EFUSE_REG)
-        mac_reg1 = self.read_reg(self.MAC_EFUSE_REG + 4)
-        mac1 = mac_reg1 & 0xFFFF
-        mac_ext = (mac_reg1 >> 16) & 0xFFFF
-        bitstring = struct.pack(">HIH", mac1, mac0, mac_ext)
-        # MAC: 60:55:f9:f7:2c:a2:ff:fe
-        #     | mac1|   mac0    | mac_ext|
+        mac1 = self.read_reg(self.MAC_EFUSE_REG + 4)  # only bottom 16 bits are MAC
+        bitstring = struct.pack(">II", mac1, mac0)[2:]
         return tuple(bitstring)
 
     def get_flash_crypt_config(self):
         return None  # doesn't exist on ESP32-C6
 
     def get_secure_boot_enabled(self):
         return (
```

### Comparing `esptool-4.6/esptool/targets/esp32c6beta.py` & `esptool-4.6.dev1/esptool/targets/esp32c6beta.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
     CHIP_DETECT_MAGIC_VALUE = [0x0DA1806F]
 
     UART_DATE_REG_ADDR = 0x00000500
 
     def get_chip_description(self):
         chip_name = {
-            0: "ESP32-C6 (QFN40)",
-            1: "ESP32-C6FH4 (QFN32)",
+            0: "ESP32-C6",
         }.get(self.get_pkg_version(), "unknown ESP32-C6")
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
         return f"{chip_name} (revision v{major_rev}.{minor_rev})"
 
     def _post_connect(self):
         pass
```

### Comparing `esptool-4.6/esptool/targets/esp32h2.py` & `esptool-4.6.dev1/esptool/targets/esp32h2.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,41 +9,27 @@
 class ESP32H2ROM(ESP32C6ROM):
     CHIP_NAME = "ESP32-H2"
     IMAGE_CHIP_ID = 16
 
     # Magic value for ESP32H2
     CHIP_DETECT_MAGIC_VALUE = [0xD7B73E80]
 
-    DR_REG_LP_WDT_BASE = 0x600B1C00
-    RTC_CNTL_WDTCONFIG0_REG = DR_REG_LP_WDT_BASE + 0x0  # LP_WDT_RWDT_CONFIG0_REG
-    RTC_CNTL_WDTWPROTECT_REG = DR_REG_LP_WDT_BASE + 0x001C  # LP_WDT_RWDT_WPROTECT_REG
-
-    RTC_CNTL_SWD_CONF_REG = DR_REG_LP_WDT_BASE + 0x0020  # LP_WDT_SWD_CONFIG_REG
-    RTC_CNTL_SWD_AUTO_FEED_EN = 1 << 18
-    RTC_CNTL_SWD_WPROTECT_REG = DR_REG_LP_WDT_BASE + 0x0024  # LP_WDT_SWD_WPROTECT_REG
-    RTC_CNTL_SWD_WKEY = 0x50D83AA1  # LP_WDT_SWD_WKEY, same as WDT key in this case
-
     FLASH_FREQUENCY = {
         "48m": 0xF,
         "24m": 0x0,
         "16m": 0x1,
         "12m": 0x2,
     }
 
     def get_pkg_version(self):
-        num_word = 4
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 0) & 0x07
-
-    def get_minor_chip_version(self):
-        num_word = 3
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 18) & 0x07
-
-    def get_major_chip_version(self):
         num_word = 3
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 21) & 0x03
+        block1_addr = self.EFUSE_BASE + 0x044
+        word3 = self.read_reg(block1_addr + (4 * num_word))
+        pkg_version = (word3 >> 21) & 0x0F
+        return pkg_version
 
     def get_chip_description(self):
         chip_name = {
             0: "ESP32-H2",
         }.get(self.get_pkg_version(), "unknown ESP32-H2")
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
```

### Comparing `esptool-4.6/esptool/targets/esp32h2beta1.py` & `esptool-4.6.dev1/esptool/targets/esp32h2beta1.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,24 +72,27 @@
         "48m": 0xF,
         "24m": 0x0,
         "16m": 0x1,
         "12m": 0x2,
     }
 
     def get_pkg_version(self):
-        num_word = 4
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 0) & 0x07
+        num_word = 3
+        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 21) & 0x0F
 
     def get_minor_chip_version(self):
-        num_word = 3
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 18) & 0x07
+        hi_num_word = 5
+        hi = (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * hi_num_word)) >> 23) & 0x01
+        low_num_word = 3
+        low = (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * low_num_word)) >> 18) & 0x07
+        return (hi << 3) + low
 
     def get_major_chip_version(self):
-        num_word = 3
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 21) & 0x03
+        num_word = 5
+        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 24) & 0x03
 
     def get_chip_description(self):
         chip_name = {
             0: "ESP32-H2",
         }.get(self.get_pkg_version(), "unknown ESP32-H2")
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
```

### Comparing `esptool-4.6/esptool/targets/esp32h2beta2.py` & `esptool-4.6.dev1/esptool/targets/esp32h2beta2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/esp32s2.py` & `esptool-4.6.dev1/esptool/targets/esp32s2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/esp32s3.py` & `esptool-4.6.dev1/esptool/targets/esp32s3.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,23 +79,18 @@
     PURPOSE_VAL_XTS_AES256_KEY_2 = 3
     PURPOSE_VAL_XTS_AES128_KEY = 4
 
     UARTDEV_BUF_NO = 0x3FCEF14C  # Variable in ROM .bss which indicates the port in use
     UARTDEV_BUF_NO_USB_OTG = 3  # The above var when USB-OTG is used
     UARTDEV_BUF_NO_USB_JTAG_SERIAL = 4  # The above var when USB-JTAG/Serial is used
 
+    RTC_CNTL_WDT_WKEY = 0x50D83AA1
     RTCCNTL_BASE_REG = 0x60008000
-    RTC_CNTL_SWD_CONF_REG = RTCCNTL_BASE_REG + 0x00B4
-    RTC_CNTL_SWD_AUTO_FEED_EN = 1 << 31
-    RTC_CNTL_SWD_WPROTECT_REG = RTCCNTL_BASE_REG + 0x00B8
-    RTC_CNTL_SWD_WKEY = 0x8F1D312A
-
     RTC_CNTL_WDTCONFIG0_REG = RTCCNTL_BASE_REG + 0x0090
     RTC_CNTL_WDTWPROTECT_REG = RTCCNTL_BASE_REG + 0x00B0
-    RTC_CNTL_WDT_WKEY = 0x50D83AA1
 
     USB_RAM_BLOCK = 0x800  # Max block size USB-OTG is used
 
     GPIO_STRAP_REG = 0x60004038
     GPIO_STRAP_SPI_BOOT_MASK = 0x8  # Not download mode
     RTC_CNTL_OPTION1_REG = 0x6000812C
     RTC_CNTL_FORCE_DOWNLOAD_BOOT_MASK = 0x1  # Is download mode forced over USB?
@@ -239,37 +234,27 @@
         """
         Check the UARTDEV_BUF_NO register to see if USB-JTAG/Serial is being used
         """
         if self.secure_download_mode:
             return False  # can't detect USB-JTAG/Serial in secure download mode
         return self.get_uart_no() == self.UARTDEV_BUF_NO_USB_JTAG_SERIAL
 
-    def disable_watchdogs(self):
-        # When USB-JTAG/Serial is used, the RTC WDT and SWD watchdog are not reset
-        # and can then reset the board during flashing. Disable them.
+    def disable_rtc_watchdog(self):
+        # When USB-JTAG/Serial is used, the RTC watchdog is not reset
+        # and can then reset the board during flashing. Disable it.
         if self.uses_usb_jtag_serial():
-            # Disable RTC WDT
             self.write_reg(self.RTC_CNTL_WDTWPROTECT_REG, self.RTC_CNTL_WDT_WKEY)
             self.write_reg(self.RTC_CNTL_WDTCONFIG0_REG, 0)
             self.write_reg(self.RTC_CNTL_WDTWPROTECT_REG, 0)
 
-            # Automatically feed SWD
-            self.write_reg(self.RTC_CNTL_SWD_WPROTECT_REG, self.RTC_CNTL_SWD_WKEY)
-            self.write_reg(
-                self.RTC_CNTL_SWD_CONF_REG,
-                self.read_reg(self.RTC_CNTL_SWD_CONF_REG)
-                | self.RTC_CNTL_SWD_AUTO_FEED_EN,
-            )
-            self.write_reg(self.RTC_CNTL_SWD_WPROTECT_REG, 0)
-
     def _post_connect(self):
         if self.uses_usb_otg():
             self.ESP_RAM_BLOCK = self.USB_RAM_BLOCK
         if not self.sync_stub_detected:  # Don't run if stub is reused
-            self.disable_watchdogs()
+            self.disable_rtc_watchdog()
 
     def _check_if_can_reset(self):
         """
         Check the strapping register to see if we can reset out of download mode.
         """
         if os.getenv("ESPTOOL_TESTING") is not None:
             print("ESPTOOL_TESTING is set, ignoring strapping mode check")
```

### Comparing `esptool-4.6/esptool/targets/esp32s3beta2.py` & `esptool-4.6.dev1/esptool/targets/esp32s3beta2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/esp8266.py` & `esptool-4.6.dev1/esptool/targets/esp8266.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32.json`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32c2.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c2.json`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32c3.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c3.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'IGvIP1YKOECmCjhA/go4QKILOEAODDhAvAs4QCIJOEBeCzhAngs4QBILOEDSCDhARgs4QNIIOEAwCjhAdgo4QKYKOED+CjhAQgo4QIYJOEC2CThAPgo4QGAOOECmCjhAJg04QBgOOEASCDhAQA44QBIIOEASCDhAEgg4QBIIOEASCDhAEgg4QBIIOEASCDhAwgw4QBIIOEBEDThAGA44QA=='",*

 * * "'text'": "'QREixCbCBsa3NwRgEUc3RMg/2Mu3NARgEwQEANxAkYuR57JAIkSSREEBgoCIQBxAE3X1D4KX3bcBEbcHAGBOxoOphwBKyDdJyD8mylLEBs4izLcEAGB9WhMJCQDATBN09D8N4PJAYkQjqDQBQknSRLJJIkoFYYKAiECDJwkAE3X1D4KXfRTjGUT/yb8TBwAMlEGqh2MY5QCFR4XGI6AFAHlVgoAFR2OH5gAJRmONxgB9VYKAQgUTB7ANQYVjlecCiUecwfW3kw […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "IGvIP3YKOEDGCjhAHgs4QMILOEAuDDhA3As4QEIJOEB+CzhAvgs4QDILOEDyCDhAZgs4QPIIOEBQCjhAlgo4QMYKOEAeCzhAYgo4QKYJOEDWCThAXgo4QIAOOEDGCjhARg04QDgOOEAyCDhAYA44QDIIOEAyCDhAMgg4QDIIOEAyCDhAMgg4QDIIOEAyCDhA4gw4QDIIOEBkDThAOA44QA==",
+    "data": "IGvIP1YKOECmCjhA/go4QKILOEAODDhAvAs4QCIJOEBeCzhAngs4QBILOEDSCDhARgs4QNIIOEAwCjhAdgo4QKYKOED+CjhAQgo4QIYJOEC2CThAPgo4QGAOOECmCjhAJg04QBgOOEASCDhAQA44QBIIOEASCDhAEgg4QBIIOEASCDhAEgg4QBIIOEASCDhAwgw4QBIIOEBEDThAGA44QA==",
     "data_start": 1070164912,
     "entry": 1077413532,
-    "text": "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",
+    "text": "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",
     "text_start": 1077411840
 }
```

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32c6.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c6.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'HCuEQCoKgEB6CoBA0gqAQHYLgEDiC4BAkAuAQPYIgEAyC4BAcguAQOYKgECmCIBAGguAQKYIgEAECoBASgqAQHoKgEDSCoBAFgqAQFoJgECKCYBAEgqAQDQOgEB6CoBA+gyAQOwNgEDmB4BAFA6AQOYHgEDmB4BA5geAQOYHgEDmB4BA5geAQOYHgEDmB4BAlgyAQOYHgEAYDYBA7A2AQA=='",*

 * * "'text'": "'QREixCbCBsa39wBgEUc3BIRA2Mu39ABgEwQEANxAkYuR57JAIkSSREEBgoCIQBxAE3X1D4KX3bcBEbcHAGBOxoOphwBKyDcJhEAmylLEBs4izLcEAGB9WhMJCQDATBN09A8N4PJAYkQjqDQBQknSRLJJIkoFYYKAiECDJwkAE3X1D4KXfRTjGUT/yb8TBwAMlEGqh2MY5QCFR4XGI6AFAHlVgoAFR2OH5gAJRmONxgB9VYKAQgUTB7ANQYVjlecCiUecwfW3kw […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "HCuEQEIKgECSCoBA6gqAQI4LgED6C4BAqAuAQA4JgEBKC4BAiguAQP4KgEC+CIBAMguAQL4IgEAcCoBAYgqAQJIKgEDqCoBALgqAQHIJgECiCYBAKgqAQEwOgECSCoBAEg2AQAQOgED+B4BALA6AQP4HgED+B4BA/geAQP4HgED+B4BA/geAQP4HgED+B4BArgyAQP4HgEAwDYBABA6AQA==",
+    "data": "HCuEQCoKgEB6CoBA0gqAQHYLgEDiC4BAkAuAQPYIgEAyC4BAcguAQOYKgECmCIBAGguAQKYIgEAECoBASgqAQHoKgEDSCoBAFgqAQFoJgECKCYBAEgqAQDQOgEB6CoBA+gyAQOwNgEDmB4BAFA6AQOYHgEDmB4BA5geAQOYHgEDmB4BA5geAQOYHgEDmB4BAlgyAQOYHgEAYDYBA7A2AQA==",
     "data_start": 1082469292,
     "entry": 1082132112,
-    "text": "QREixCbCBsa39wBgEUc3BIRA2Mu39ABgEwQEANxAkYuR57JAIkSSREEBgoCIQBxAE3X1D4KX3bcBEbcHAGBOxoOphwBKyDcJhEAmylLEBs4izLcEAGB9WhMJCQDATBN09A8N4PJAYkQjqDQBQknSRLJJIkoFYYKAiECDJwkAE3X1D4KXfRTjGUT/yb8TBwAMlEGqh2MY5QCFR4XGI6AFAHlVgoAFR2OH5gAJRmONxgB9VYKAQgUTB7ANQYVjlecCiUecwfW3kwbADWMW1QCYwRMFAAyCgJMG0A19VWOV1wCYwRMFsA2CgLc1hUBBEZOFRboGxmE/Y0UFBrc3hUCTh8exA6cHCAPWRwgTdfUPkwYWAMIGwYIjktcIMpcjAKcAA9dHCJFnk4cHBGMe9wI3t4RAEwfHsaFnupcDpgcIt/aEQLc3hUCTh8exk4bGtWMf5gAjpscII6DXCCOSBwghoPlX4wb1/LJAQQGCgCOm1wgjoOcI3bc3NwBgfEudi/X/NycAYHxLnYv1/4KAQREGxt03tzcAYCOmBwI3BwAImMOYQ33/yFeyQBNF9f8FiUEBgoBBEQbG2T993TcHAEC3NwBgmMM3NwBgHEP9/7JAQQGCgEERIsQ3BIRAkwcEAUrAA6kHAQbGJsJjCgkERTc5xb1HEwQEAYFEY9YnAQREvYiTtBQAfTeFPxxENwaAABOXxwCZ4DcGAAG39v8AdY+3NgBg2MKQwphCff9BR5HgBUczCelAupcjKCQBHMSyQCJEkkQCSUEBgoABEQbOIswlNzcEzj9sABMFRP+XAID/54Cg8qqHBUWV57JHk/cHID7GiTc3NwBgHEe3BkAAEwVE/9WPHMeyRZcAgP/ngCDwMzWgAPJAYkQFYYKAQRG3B4RABsaThwcBBUcjgOcAE9fFAJjHBWd9F8zDyMf5jTqVqpWxgYzLI6oHAEE3GcETBVAMskBBAYKAAREizDcEhECTBwQBJsrER07GBs5KyKqJEwQEAWPzlQCuhKnAAylEACaZE1nJABxIY1XwABxEY175ArU9fd1IQCaGzoWXAID/54Ag4xN19Q8BxZMHQAxcyFxAppdcwFxEhY9cxPJAYkTSREJJskkFYYKAaTVtv0ERBsaXAID/54BA1gNFhQGyQHUVEzUVAEEBgoBBEQbGxTcNxbcHhECThwcA1EOZzjdnCWATBwcRHEM3Bv3/fRbxjzcGAwDxjtWPHMOyQEEBgoBBEQbGbTcRwQ1FskBBARcDgP9nAIPMQREGxpcAgP/ngEDKcTcBxbJAQQHZv7JAQQGCgEERBsYTBwAMYxrlABMFsA3RPxMFwA2yQEEB6bcTB7AN4xvl/sE3EwXQDfW3QREixCbCBsYqhLMEtQBjF5QAskAiRJJEQQGCgANFBAAFBE0/7bc1cSbLTsf9coVp/XQizUrJUsVWwwbPk4SE+haRk4cJB6aXGAizhOcAKokmhS6ElwCA/+eAwC+ThwkHGAgFarqXs4pHQTHkBWd9dZMFhfqTBwcHEwWF+RQIqpczhdcAkwcHB66Xs4XXACrGlwCA/+eAgCwyRcFFlTcBRYViFpH6QGpE2kRKSbpJKkqaSg1hgoCiiWNzigCFaU6G1oVKhZcAgP/ngADJE3X1DwHtTobWhSaFlwCA/+eAwCdOmTMENEFRtxMFMAZVvxMFAAzZtTFx/XIFZ07XUtVW017PBt8i3SbbStla0WLNZstqyW7H/XcWkRMHBwc+lxwIupc+xiOqB/iqiS6Ksoq2iwU1kwcAAhnBtwcCAD6FlwCA/+eAYCCFZ2PlVxMFZH15EwmJ+pMHBAfKlxgIM4nnAEqFlwCA/+eA4B59exMMO/mTDIv5EwcEB5MHBAcUCGKX5peBRDMM1wCzjNcAUk1jfE0JY/GkA0GomT+ihQgBjTW5NyKGDAFKhZcAgP/ngMAaopmilGP1RAOzh6RBY/F3AzMEmkBj84oAVoQihgwBToWXAID/54BAuBN19Q9V3QLMAUR5XY1NowkBAGKFlwCA/+eAgKd9+QNFMQHmhVE8Y08FAOPijf6FZ5OHBweilxgIupfalyOKp/gFBPG34xWl/ZFH4wX09gVnfXWTBwcHkwWF+hMFhfkUCKqXM4XXAJMHBweul7OF1wAqxpcAgP/ngOAQcT0yRcFFZTNRPdU5twcCABnhkwcAAj6FlwCA/+eA4A2FYhaR+lBqVNpUSlm6WSpamloKW/pLakzaTEpNuk0pYYKAt1dBSRlxk4f3hAFFht6i3KbaytjO1tLU1tLa0N7O4szmyurI7sY+zpcAgP/ngMCgcTENwTdnCWATBwcRHEO3BoRAI6L2ALcG/f/9FvWPwWbVjxzDpTEFzbcnC2A3R9hQk4aHwRMHF6qYwhOGB8AjIAYAI6AGAJOGB8KYwpOHx8GYQzcGBABRj5jDI6AGALcHhEA3N4VAk4cHABMHx7ohoCOgBwCRB+Pt5/5FO5FFaAh1OWUzt7eEQJOHx7EhZz6XIyD3CLcHgEA3CYRAk4eHDiMg+QC3OYVA1TYTCQkAk4nJsWMHBRC3BwFgRUcjoOcMhUVFRZcAgP/ngED5twWAQAFGk4UFAEVFlwCA/+eAQPo39wBgHEs3BQIAk+dHABzLlwCA/+eAQPm3FwlgiF+BRbcEhEBxiWEVEzUVAJcAgP/ngAChwWf9FxMHABCFZkFmtwUAAQFFk4QEAQ1qtzqEQJcAgP/ngACXJpoTi8qxg6fJCPXfg6vJCIVHI6YJCCMC8QKDxxsACUcjE+ECowLxAgLUTUdjgecIUUdjj+cGKUdjn+cAg8c7AAPHKwCiB9mPEUdjlucAg6eLAJxDPtRxOaFFSBBlNoPHOwADxysAogfZjxFnQQdjdPcEEwWwDZk2EwXADYE2EwXgDi0+vTFBt7cFgEABRpOFhQMVRZcAgP/ngADrNwcAYFxHEwUAApPnFxBcxzG3yUcjE/ECTbcDxxsA0UZj5+YChUZj5uYAAUwTBPAPhah5FxN39w/JRuPo5v63NoVACgeThga7NpcYQwKHkwYHA5P29g8RRuNp1vwTB/cCE3f3D41GY+vmCLc2hUAKB5OGxr82lxhDAocTB0ACY5jnEALUHUQBRWE8AUVFPOE22TahRUgQfRTBPHX0AUwBRBN19A9hPBN1/A9JPG024x4E6oPHGwBJR2Nj9y4JR+N29+r1F5P39w89R+Ng9+o3N4VAigcTB8fAupecQ4KHBUSd63AQgUUBRZfwf//ngAB0HeHRRWgQjTwBRDGoBUSB75fwf//ngAB5MzSgACmgIUdjhecABUQBTGG3A6yLAAOkywCzZ4wA0gf19+/wv4h98cFsIpz9HH19MwWMQFXcs3eVAZXjwWwzBYxAY+aMAv18MwWMQFXQMYGX8H//54CAdVX5ZpT1tzGBl/B//+eAgHRV8WqU0bdBgZfwf//ngMBzUfkzBJRBwbchR+OJ5/ABTBMEAAwxt0FHzb9BRwVE45zn9oOlywADpYsA1TKxv0FHBUTjkuf2A6cLAZFnY+XnHIOlSwEDpYsA7/D/gzW/QUcFROOS5/SDpwsBEWdjZfcaA6fLAIOlSwEDpYsAM4TnAu/wf4EjrAQAIySKsDG3A8cEAGMOBxADp4sAwRcTBAAMYxP3AMBIAUeTBvAOY0b3AoPHWwADx0sAAUyiB9mPA8drAEIHXY+Dx3sA4gfZj+OB9uYTBBAMqb0zhusAA0aGAQUHsY7ht4PHBADxw9xEY5gHEsBII4AEAH21YUdjlucCg6fLAQOniwGDpksBA6YLAYOlywADpYsAl/B//+eAQGQqjDM0oAAptQFMBUQRtRFHBUTjmufmA6WLAIFFl/B//+eAwGmRtRP39wDjGgfsk9xHABOEiwABTH1d43mc3UhEl/B//+eAwE0YRFRAEED5jmMHpwEcQhNH9/99j9mOFMIFDEEE2b8RR0m9QUcFROOc5+CDp4sAA6dLASMm+QAjJOkA3bODJYkAwReR5YnPAUwTBGAMtbsDJ8kAY2b3BhP3NwDjHgfkAyjJAAFGAUczBehAs4blAGNp9wDjCQbUIyapACMk2QCZszOG6wAQThEHkMIFRum/IUcFROOW59oDJMkAGcATBIAMIyYJACMkCQAzNIAASbsBTBMEIAwRuwFMEwSADDGzAUwTBJAMEbMTByANY4PnDBMHQA3jkOe8A8Q7AIPHKwAiBF2Ml/B//+eA4EwDrMQAQRRjc4QBIozjDgy4wEBilDGAnEhjVfAAnERjW/QK7/BP0XXdyEBihpOFiwGX8H//54DgSAHFkwdADNzI3EDil9zA3ESzh4dB3MSX8H//54DAR4m+CWUTBQVxA6zLAAOkiwCX8H//54BAOLcHAGDYS7cGAAHBFpNXRwESB3WPvYvZj7OHhwMBRbPVhwKX8H//54BgORMFgD6X8H//54DgNBG2g6ZLAQOmCwGDpcsAA6WLAO/wT/79tIPFOwCDxysAE4WLAaIF3Y3BFe/wL9vZvO/wj8o9v4PHOwADxysAE4yLAaIH2Y8TjQf/BUS3O4VA3ERjBQ0AmcNjTIAAY1AEChMHcAzYyOOfB6iTB5AMYaiTh8u6mEO3t4RAk4fHsZmPPtaDJ4qwtzyEQGrQk4wMAZONy7oFSGNz/QANSELGOsTv8I/DIkcySDcFhEDihXwQk4bKsRAQEwWFApfwf//ngEA0glcDp4ywg6UNADMN/UAdjz6cslcjpOywKoS+lSOgvQCTh8qxnY0BxaFn45L19lqF7/CvziOgbQGZvy3044MHoJMHgAzcyPW6g6eLAOObB57v8C/ZCWUTBQVxl/B//+eAoCLv8K/Ul/B//+eA4CbRugOkywDjBwSc7/Cv1hMFgD6X8H//54BAIO/wT9IClFW67/DP0fZQZlTWVEZZtlkmWpZaBlv2S2ZM1kxGTbZNCWGCgAAA",
+    "text": "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",
     "text_start": 1082130432
 }
```

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32c6beta.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c6beta.json`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32h2.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'HCuDQCoKgEB6CoBA0gqAQHYLgEDiC4BAkAuAQPYIgEAyC4BAcguAQOYKgECmCIBAGguAQKYIgEAECoBASgqAQHoKgEDSCoBAFgqAQFoJgECKCYBAEgqAQDQOgEB6CoBA+gyAQOwNgEDmB4BAFA6AQOYHgEDmB4BA5geAQOYHgEDmB4BA5geAQOYHgEDmB4BAlgyAQOYHgEAYDYBA7A2AQA=='",*

 * * "'text'": "'QREixCbCBsa39wBgEUc3BINA2Mu39ABgEwQEANxAkYuR57JAIkSSREEBgoCIQBxAE3X1D4KX3bcBEbcHAGBOxoOphwBKyDcJg0AmylLEBs4izLcEAGB9WhMJCQDATBN09A8N4PJAYkQjqDQBQknSRLJJIkoFYYKAiECDJwkAE3X1D4KXfRTjGUT/yb8TBwAMlEGqh2MY5QCFR4XGI6AFAHlVgoAFR2OH5gAJRmONxgB9VYKAQgUTB7ANQYVjlecCiUecwfW3kw […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "HCuDQEIKgECSCoBA6gqAQI4LgED6C4BAqAuAQA4JgEBKC4BAiguAQP4KgEC+CIBAMguAQL4IgEAcCoBAYgqAQJIKgEDqCoBALgqAQHIJgECiCYBAKgqAQEwOgECSCoBAEg2AQAQOgED+B4BALA6AQP4HgED+B4BA/geAQP4HgED+B4BA/geAQP4HgED+B4BArgyAQP4HgEAwDYBABA6AQA==",
+    "data": "HCuDQCoKgEB6CoBA0gqAQHYLgEDiC4BAkAuAQPYIgEAyC4BAcguAQOYKgECmCIBAGguAQKYIgEAECoBASgqAQHoKgEDSCoBAFgqAQFoJgECKCYBAEgqAQDQOgEB6CoBA+gyAQOwNgEDmB4BAFA6AQOYHgEDmB4BA5geAQOYHgEDmB4BA5geAQOYHgEDmB4BAlgyAQOYHgEAYDYBA7A2AQA==",
     "data_start": 1082403756,
     "entry": 1082132112,
-    "text": "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",
+    "text": "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",
     "text_start": 1082130432
 }
```

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32s2.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s2.json`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32s3.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s3.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7%*

 * *Differences: {"'data'": "'ZCvKP5aNN0B7jjdAPJM3QAaPN0CbjjdABo83QGWPN0AykDdApZA3QE2QN0AhjTdAyI83QCSQN0CIjzdAx5A3QLKPN0DHkDdAaY43QMaON0AGjzdAZY83QIGON0BijTdAiJE3QAKTN0A+jDdAIpM3QD6MN0A+jDdAPow3QD6MN0A+jDdAPow3QD6MN0A+jDdAIpE3QD6MN0AdkjdAApM3QAQInwAAAAAAAAAYAQQIBQAAAAAAAAAIAQQIBgAAAAAAAAAAAQQIIQAAAAAAIAAAEQQI3AAAAAAAIAAAEQQIDAAAAAAAIAAAAQQIEgAAAAAAIAAAESAoDAAQAQAA'",*

 * * "'entry'": '1077381684',*

 * * "'text'": "'FIADYACAA2BIAMo/BIADYDZBAIH7/wxJwCAAmQjGBAAAgfj/wCAAqAiB9/+goHSICOAIACH2/8AgAIgCJ+jhHfAAAAAIAABgHAAAYBAAAGA2QQAh/P/AIAA4 […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "ZCvKP8qNN0CvjjdAcJM3QDqPN0DPjjdAOo83QJmPN0BmkDdA2ZA3QIGQN0BVjTdA/I83QFiQN0C8jzdA+5A3QOaPN0D7kDdAnY43QPqON0A6jzdAmY83QLWON0CWjTdAvJE3QDaTN0ByjDdAVpM3QHKMN0ByjDdAcow3QHKMN0ByjDdAcow3QHKMN0ByjDdAVpE3QHKMN0BRkjdANpM3QAQInwAAAAAAAAAYAQQIBQAAAAAAAAAIAQQIBgAAAAAAAAAAAQQIIQAAAAAAIAAAEQQI3AAAAAAAIAAAEQQIDAAAAAAAIAAAAQQIEgAAAAAAIAAAESAoDAAQAQAA",
+    "data": "ZCvKP5aNN0B7jjdAPJM3QAaPN0CbjjdABo83QGWPN0AykDdApZA3QE2QN0AhjTdAyI83QCSQN0CIjzdAx5A3QLKPN0DHkDdAaY43QMaON0AGjzdAZY83QIGON0BijTdAiJE3QAKTN0A+jDdAIpM3QD6MN0A+jDdAPow3QD6MN0A+jDdAPow3QD6MN0A+jDdAIpE3QD6MN0AdkjdAApM3QAQInwAAAAAAAAAYAQQIBQAAAAAAAAAIAQQIBgAAAAAAAAAAAQQIIQAAAAAAIAAAEQQI3AAAAAAAIAAAEQQIDAAAAAAAIAAAAQQIEgAAAAAAIAAAESAoDAAQAQAA",
     "data_start": 1070279668,
-    "entry": 1077381696,
-    "text": "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",
+    "entry": 1077381684,
+    "text": "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",
     "text_start": 1077379072
 }
```

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_32s3beta2.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s3beta2.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7%*

 * *Differences: {"'data'": "'ZCvKP4KLN0APjDdA15A3QJqMN0AvjDdAmow3QPmMN0DGjTdAOY43QOGNN0ANizdAXI03QLiNN0AcjTdAXI43QEaNN0BcjjdA/Ys3QFqMN0CajDdA+Yw3QBWMN0BOizdAHI83QJuQN0AsijdAvZA3QCyKN0AsijdALIo3QCyKN0AsijdALIo3QCyKN0AsijdAto43QCyKN0CyjzdAm5A3QA=='",*

 * * "'entry'": '1077381176',*

 * * "'text'": "'FIADYACAA2BIAMo/BIADYDZBAIH7/wxJwCAAmQjGBAAAgfj/wCAAqAiB9/+goHSICOAIACH2/8AgAIgCJ+jhHfAAAAAIAABgHAAAYBAAAGA2QQAh/P/AIAA4AkH7/8AgACgEICCUnOJB6P9GBAAMODCIAcAgAKgIiASgoHTgCAALImYC6Ib0/yHx/8AgADkCHfAAAOwryz9kq8o/hIAAAEBAAACk68o/8CvLPzZBALH5/yCg […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "ZCvKP7aLN0BDjDdAC5E3QM6MN0BjjDdAzow3QC2NN0D6jTdAbY43QBWON0BBizdAkI03QOyNN0BQjTdAkI43QHqNN0CQjjdAMYw3QI6MN0DOjDdALY03QEmMN0CCizdAUI83QM+QN0BgijdA8ZA3QGCKN0BgijdAYIo3QGCKN0BgijdAYIo3QGCKN0BgijdA6o43QGCKN0DmjzdAz5A3QA==",
+    "data": "ZCvKP4KLN0APjDdA15A3QJqMN0AvjDdAmow3QPmMN0DGjTdAOY43QOGNN0ANizdAXI03QLiNN0AcjTdAXI43QEaNN0BcjjdA/Ys3QFqMN0CajDdA+Yw3QBWMN0BOizdAHI83QJuQN0AsijdAvZA3QCyKN0AsijdALIo3QCyKN0AsijdALIo3QCyKN0AsijdAto43QCyKN0CyjzdAm5A3QA==",
     "data_start": 1070279668,
-    "entry": 1077381188,
-    "text": "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",
+    "entry": 1077381176,
+    "text": "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",
     "text_start": 1077379072
 }
```

### Comparing `esptool-4.6/esptool/targets/stub_flasher/stub_flasher_8266.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_8266.json`

 * *Files identical despite different names*

### Comparing `esptool-4.6/esptool/util.py` & `esptool-4.6.dev1/esptool/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-FileCopyrightText: 2014-2022 Fredrik Ahlberg, Angus Gratton,
 # Espressif Systems (Shanghai) CO LTD, other contributors as noted.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
-import os
 import re
 import struct
 import sys
 
 
 def byte(bitstr, index):
     return bitstr[index]
@@ -84,23 +83,14 @@
 
 
 def strip_chip_name(chip_name):
     """Strip chip name to normalized form, e.g. `ESP32-S3(beta2)` -> `esp32s3beta2`"""
     return re.sub(r"[-()]", "", chip_name.lower())
 
 
-def get_file_size(path_to_file):
-    """Returns the file size in bytes"""
-    file_size = 0
-    with open(path_to_file, "rb") as f:
-        f.seek(0, os.SEEK_END)
-        file_size = f.tell()
-    return file_size
-
-
 class FatalError(RuntimeError):
     """
     Wrapper class for runtime errors that aren't caused by internal bugs, but by
     ESP ROM responses or input content.
     """
 
     def __init__(self, message):
```

### Comparing `esptool-4.6/esptool.egg-info/PKG-INFO` & `esptool-4.6.dev1/esptool.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 Metadata-Version: 2.1
 Name: esptool
-Version: 4.6
+Version: 4.6.dev1
 Summary: A serial utility to communicate & flash code to Espressif chips.
 Home-page: https://github.com/espressif/esptool/
 Author: Fredrik Ahlberg (themadinventor) & Angus Gratton (projectgus) & Espressif Systems
 Author-email: 
 License: GPLv2+
 Project-URL: Documentation, https://docs.espressif.com/projects/esptool/
 Project-URL: Source, https://github.com/espressif/esptool/
 Project-URL: Tracker, https://github.com/espressif/esptool/issues/
-Description: 
-        ==========
-        esptool.py
-        ==========
-        A Python-based, open-source, platform-independent utility to communicate with the ROM bootloader in Espressif chips.
-        
-        The esptool.py project is `hosted on github <https://github.com/espressif/esptool>`_.
-        
-        Documentation
-        -------------
-        Visit online `esptool documentation <https://docs.espressif.com/projects/esptool/>`_ or run ``esptool.py -h``.
-        
-        Contributing
-        ------------
-        Please see the `contributions guide <https://docs.espressif.com/projects/esptool/en/latest/contributing.html>`_.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -38,7 +22,26 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Provides-Extra: dev
 Provides-Extra: hsm
+License-File: LICENSE
+
+
+==========
+esptool.py
+==========
+A Python-based, open-source, platform-independent utility to communicate with the ROM bootloader in Espressif chips.
+
+The esptool.py project is `hosted on github <https://github.com/espressif/esptool>`_.
+
+Documentation
+-------------
+Visit online `esptool documentation <https://docs.espressif.com/projects/esptool/>`_ or run ``esptool.py -h``.
+
+Contributing
+------------
+Please see the `contributions guide <https://docs.espressif.com/projects/esptool/en/latest/contributing.html>`_.
+
+
```

### Comparing `esptool-4.6/esptool.egg-info/SOURCES.txt` & `esptool-4.6.dev1/esptool.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -56,21 +56,14 @@
 espefuse/efuse/esp32s3/mem_definition.py
 espefuse/efuse/esp32s3/operations.py
 espefuse/efuse/esp32s3beta2/__init__.py
 espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py
 espefuse/efuse/esp32s3beta2/fields.py
 espefuse/efuse/esp32s3beta2/mem_definition.py
 espefuse/efuse/esp32s3beta2/operations.py
-espefuse/efuse_defs/esp32.yaml
-espefuse/efuse_defs/esp32c2.yaml
-espefuse/efuse_defs/esp32c3.yaml
-espefuse/efuse_defs/esp32c6.yaml
-espefuse/efuse_defs/esp32h2.yaml
-espefuse/efuse_defs/esp32s2.yaml
-espefuse/efuse_defs/esp32s3.yaml
 espsecure/__init__.py
 espsecure/__main__.py
 espsecure/esp_hsm_sign/__init__.py
 espsecure/esp_hsm_sign/exceptions.py
 esptool/__init__.py
 esptool/__main__.py
 esptool/bin_image.py
```

### Comparing `esptool-4.6/esptool.py` & `esptool-4.6.dev1/esptool.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,20 +14,17 @@
 import os
 import sys
 
 if os.name != "nt":
     # Linux/macOS: remove current script directory to avoid importing this file
     # as a module; we want to import the installed esptool module instead
     with contextlib.suppress(ValueError):
-        executable_dir = os.path.dirname(sys.executable)
-        sys.path = [
-            path
-            for path in sys.path
-            if not path.endswith(("/bin", "/sbin")) and path != executable_dir
-        ]
+        if sys.path[0].endswith("/bin"):
+            sys.path.pop(0)
+        sys.path.remove(os.path.dirname(sys.executable))
 
     # Linux/macOS: delete imported module entry to force Python to load
     # the module from scratch; this enables importing esptool module in
     # other Python scripts
     with contextlib.suppress(KeyError):
         del sys.modules["esptool"]
```

### Comparing `esptool-4.6/setup.py` & `esptool-4.6.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,15 @@
         ],
     },
     install_requires=[
         "bitstring>=3.1.6",
         "cryptography>=2.1.4",
         "ecdsa>=0.16.0",
         "pyserial>=3.0",
-        "reedsolo>=1.5.3,<1.8",
-        "PyYAML>=5.1",
+        "reedsolo>=1.5.3,<=1.6.0",
     ],
     packages=find_packages(),
     include_package_data=True,
     package_data={"": ["esptool/targets/stub_flasher/*.json"]},
     entry_points=entry_points,
     scripts=scripts,
 )
```

