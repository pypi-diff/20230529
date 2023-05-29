# Comparing `tmp/boardgen-0.6.1.tar.gz` & `tmp/boardgen-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boardgen-0.6.1.tar", max compression
+gzip compressed data, was "boardgen-0.6.2.tar", max compression
```

## Comparing `boardgen-0.6.1.tar` & `boardgen-0.6.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1076 2023-03-20 20:18:28.486823 boardgen-0.6.1/LICENSE
--rw-r--r--   0        0        0     4785 2023-03-20 20:18:28.486823 boardgen-0.6.1/README.md
--rw-r--r--   0        0        0      353 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/__init__.py
--rw-r--r--   0        0        0    11411 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/cli.py
--rw-r--r--   0        0        0       92 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/core/__init__.py
--rw-r--r--   0        0        0     2146 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/core/cache.py
--rw-r--r--   0        0        0     9853 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/core/core.py
--rw-r--r--   0        0        0      925 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/core/getters.py
--rw-r--r--   0        0        0      773 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/mixins.py
--rw-r--r--   0        0        0      439 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/models/__init__.py
--rw-r--r--   0        0        0     1705 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/models/board.py
--rw-r--r--   0        0        0     1015 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/models/enums.py
--rw-r--r--   0        0        0     1156 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/models/flash_region.py
--rw-r--r--   0        0        0     1257 2023-03-20 20:18:28.486823 boardgen-0.6.1/boardgen/models/pcb.py
--rw-r--r--   0        0        0     2348 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/models/role.py
--rw-r--r--   0        0        0      358 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/models/template.py
--rw-r--r--   0        0        0      117 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/readme/__init__.py
--rw-r--r--   0        0        0     2229 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/readme/parts.py
--rw-r--r--   0        0        0     8123 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/readme/writer.py
--rw-r--r--   0        0        0      109 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/boards/README.md
--rw-r--r--   0        0        0      564 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/flash.json
--rw-r--r--   0        0        0      831 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/presets.json
--rw-r--r--   0        0        0     1497 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/roles.json
--rw-r--r--   0        0        0      398 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/label_line_2mm_down.json
--rw-r--r--   0        0        0      412 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/label_line_2mm_up.json
--rw-r--r--   0        0        0      690 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/labels_horz5_2mm.json
--rw-r--r--   0        0        0      829 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/labels_horz6_2mm.json
--rw-r--r--   0        0        0      967 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/labels_horz7_2mm.json
--rw-r--r--   0        0        0     1106 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/labels_horz8_2mm.json
--rw-r--r--   0        0        0      133 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pad_10x25.json
--rw-r--r--   0        0        0      525 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pads_horz5_2mm.json
--rw-r--r--   0        0        0      631 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pads_horz6_2mm.json
--rw-r--r--   0        0        0      386 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pin_horz_2mm_cast_hole.json
--rw-r--r--   0        0        0      244 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pin_horz_2mm_cast_nohole.json
--rw-r--r--   0        0        0      388 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pin_vert_2mm_cast_hole.json
--rw-r--r--   0        0        0      245 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pin_vert_2mm_cast_nohole.json
--rw-r--r--   0        0        0      540 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json
--rw-r--r--   0        0        0      649 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json
--rw-r--r--   0        0        0      757 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json
--rw-r--r--   0        0        0      866 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json
--rw-r--r--   0        0        0      789 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json
--rw-r--r--   0        0        0      902 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json
--rw-r--r--   0        0        0       80 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/test_pad_1mm.json
--rw-r--r--   0        0        0      980 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/shapes/tuya2-pcb.json
--rw-r--r--   0        0        0     2931 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/custom-20x24-22.json
--rw-r--r--   0        0        0     2594 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/esp12e-21.json
--rw-r--r--   0        0        0     2640 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/esp12e-22.json
--rw-r--r--   0        0        0      256 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/esp12e-shield-nohole.json
--rw-r--r--   0        0        0      233 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/esp12e-shield.json
--rw-r--r--   0        0        0      233 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/esp12s-shield.json
--rw-r--r--   0        0        0     1666 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/esp12s.json
--rw-r--r--   0        0        0     1222 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/rf-15mm-type1.json
--rw-r--r--   0        0        0     1224 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/rf-16mm-type1.json
--rw-r--r--   0        0        0     1226 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/rf-20mm-type1.json
--rw-r--r--   0        0        0      450 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/tuya-16x24.json
--rw-r--r--   0        0        0      227 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/tuya2-shield.json
--rw-r--r--   0        0        0     1308 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/tuya2.json
--rw-r--r--   0        0        0      229 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/tuya2l-shield.json
--rw-r--r--   0        0        0      909 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/res/templates/tuya2l.json
--rw-r--r--   0        0        0      341 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/__init__.py
--rw-r--r--   0        0        0     4324 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/base.py
--rw-r--r--   0        0        0     1120 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/circle.py
--rw-r--r--   0        0        0     1268 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/fill_style.py
--rw-r--r--   0        0        0     2268 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/group.py
--rw-r--r--   0        0        0      182 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/label/__init__.py
--rw-r--r--   0        0        0     1706 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/label/block.py
--rw-r--r--   0        0        0      543 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/label/io_line.py
--rw-r--r--   0        0        0     3306 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/label/label.py
--rw-r--r--   0        0        0     1082 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/rect.py
--rw-r--r--   0        0        0      833 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/shapes/text.py
--rw-r--r--   0        0        0     2003 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/utils.py
--rw-r--r--   0        0        0      119 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/variant/__init__.py
--rw-r--r--   0        0        0      362 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/variant/features.py
--rw-r--r--   0        0        0     6271 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/variant/parts.py
--rw-r--r--   0        0        0      319 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/variant/section.py
--rw-r--r--   0        0        0     8502 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/variant/writer.py
--rw-r--r--   0        0        0     8765 2023-03-20 20:18:28.490824 boardgen-0.6.1/boardgen/vector.py
--rw-r--r--   0        0        0      546 2023-03-20 20:18:28.490824 boardgen-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5427 1970-01-01 00:00:00.000000 boardgen-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-29 14:14:22.593899 boardgen-0.6.2/LICENSE
+-rw-r--r--   0        0        0     4785 2023-05-29 14:14:22.593899 boardgen-0.6.2/README.md
+-rw-r--r--   0        0        0      353 2023-05-29 14:14:22.593899 boardgen-0.6.2/boardgen/__init__.py
+-rw-r--r--   0        0        0    11411 2023-05-29 14:14:22.593899 boardgen-0.6.2/boardgen/cli.py
+-rw-r--r--   0        0        0       92 2023-05-29 14:14:22.593899 boardgen-0.6.2/boardgen/core/__init__.py
+-rw-r--r--   0        0        0     2146 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/core/cache.py
+-rw-r--r--   0        0        0     9853 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/core/core.py
+-rw-r--r--   0        0        0      925 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/core/getters.py
+-rw-r--r--   0        0        0      773 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/mixins.py
+-rw-r--r--   0        0        0      439 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/__init__.py
+-rw-r--r--   0        0        0     1705 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/board.py
+-rw-r--r--   0        0        0     1015 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/enums.py
+-rw-r--r--   0        0        0     1156 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/flash_region.py
+-rw-r--r--   0        0        0     1257 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/pcb.py
+-rw-r--r--   0        0        0     2348 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/role.py
+-rw-r--r--   0        0        0      358 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/template.py
+-rw-r--r--   0        0        0      117 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/readme/__init__.py
+-rw-r--r--   0        0        0     2229 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/readme/parts.py
+-rw-r--r--   0        0        0     8123 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/readme/writer.py
+-rw-r--r--   0        0        0      109 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/boards/README.md
+-rw-r--r--   0        0        0      589 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/flash.json
+-rw-r--r--   0        0        0      831 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/presets.json
+-rw-r--r--   0        0        0     1497 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/roles.json
+-rw-r--r--   0        0        0      398 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/label_line_2mm_down.json
+-rw-r--r--   0        0        0      412 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/label_line_2mm_up.json
+-rw-r--r--   0        0        0      690 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/labels_horz5_2mm.json
+-rw-r--r--   0        0        0      829 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/labels_horz6_2mm.json
+-rw-r--r--   0        0        0      967 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/labels_horz7_2mm.json
+-rw-r--r--   0        0        0     1106 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/labels_horz8_2mm.json
+-rw-r--r--   0        0        0      133 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pad_10x25.json
+-rw-r--r--   0        0        0      525 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pads_horz5_2mm.json
+-rw-r--r--   0        0        0      631 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pads_horz6_2mm.json
+-rw-r--r--   0        0        0      386 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pin_horz_2mm_cast_hole.json
+-rw-r--r--   0        0        0      244 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pin_horz_2mm_cast_nohole.json
+-rw-r--r--   0        0        0      388 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pin_vert_2mm_cast_hole.json
+-rw-r--r--   0        0        0      245 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pin_vert_2mm_cast_nohole.json
+-rw-r--r--   0        0        0      540 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json
+-rw-r--r--   0        0        0      649 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json
+-rw-r--r--   0        0        0      757 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json
+-rw-r--r--   0        0        0      866 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json
+-rw-r--r--   0        0        0      789 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json
+-rw-r--r--   0        0        0      902 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json
+-rw-r--r--   0        0        0       80 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/test_pad_1mm.json
+-rw-r--r--   0        0        0      980 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/tuya2-pcb.json
+-rw-r--r--   0        0        0     2931 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/custom-20x24-22.json
+-rw-r--r--   0        0        0     2594 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12e-21.json
+-rw-r--r--   0        0        0     2640 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12e-22.json
+-rw-r--r--   0        0        0      256 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12e-shield-nohole.json
+-rw-r--r--   0        0        0      233 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12e-shield.json
+-rw-r--r--   0        0        0      233 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12s-shield.json
+-rw-r--r--   0        0        0     1666 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12s.json
+-rw-r--r--   0        0        0     1222 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/rf-15mm-type1.json
+-rw-r--r--   0        0        0     1224 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/rf-16mm-type1.json
+-rw-r--r--   0        0        0     1226 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/rf-20mm-type1.json
+-rw-r--r--   0        0        0      450 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/tuya-16x24.json
+-rw-r--r--   0        0        0      227 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/tuya2-shield.json
+-rw-r--r--   0        0        0     1308 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/tuya2.json
+-rw-r--r--   0        0        0      229 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/tuya2l-shield.json
+-rw-r--r--   0        0        0      909 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/tuya2l.json
+-rw-r--r--   0        0        0      341 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/__init__.py
+-rw-r--r--   0        0        0     4324 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/base.py
+-rw-r--r--   0        0        0     1120 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/circle.py
+-rw-r--r--   0        0        0     1268 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/fill_style.py
+-rw-r--r--   0        0        0     2268 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/group.py
+-rw-r--r--   0        0        0      182 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/label/__init__.py
+-rw-r--r--   0        0        0     1706 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/label/block.py
+-rw-r--r--   0        0        0      543 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/label/io_line.py
+-rw-r--r--   0        0        0     3306 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/label/label.py
+-rw-r--r--   0        0        0     1082 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/rect.py
+-rw-r--r--   0        0        0      833 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/text.py
+-rw-r--r--   0        0        0     2003 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/utils.py
+-rw-r--r--   0        0        0      119 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/variant/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/variant/features.py
+-rw-r--r--   0        0        0     6271 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/variant/parts.py
+-rw-r--r--   0        0        0      319 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/variant/section.py
+-rw-r--r--   0        0        0     8502 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/variant/writer.py
+-rw-r--r--   0        0        0     8765 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/vector.py
+-rw-r--r--   0        0        0      546 2023-05-29 14:14:22.601899 boardgen-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5427 1970-01-01 00:00:00.000000 boardgen-0.6.2/PKG-INFO
```

### Comparing `boardgen-0.6.1/LICENSE` & `boardgen-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/README.md` & `boardgen-0.6.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
   list  List boards/templates/etc
 ```
 
 ### Board definitions
 
 Writing board definitions means putting a .JSON file to a directory and specifying this directory using the `--boards` option.
 
-Boardgen is meant to be used with PlatformIO-style board definition files. An example of such a board can be found [here (libretuya/boards/wr3.json)](https://github.com/kuba2k2/libretuya/blob/master/boards/wr3.json).
+Boardgen is meant to be used with PlatformIO-style board definition files. An example of such a board can be found [here (libretiny/boards/wr3.json)](https://github.com/kuba2k2/libretiny/blob/master/boards/wr3.json).
 
 Note that the board manifest uses `"_base"` definitions. These are merged recursively with the manifest, and this result is expected to produce a complete file.
 
 Apart from PlatformIO default variables (such as `build`, `debug`, `upload` or `name`, `url` and `vendor`) the board definition contains a [`Pcb`](boardgen/models/pcb.py) object.
 
 ### Templates
 
@@ -134,8 +134,8 @@
   - 1st stop color
   - 2nd stop position
   - 2nd stop color
 - `width`: stroke width (not used for "fill")
 
 ## Support
 
-As this project is just a quick solution that'll be used in [LibreTuya](https://github.com/kuba2k2/libretuya) for generating pinouts, it's not really well documented. If you find this project interesting and need any help using it, feel free to open an issue and I'll try to provide more examples and info on how to use it.
+As this project is just a quick solution that'll be used in [LibreTiny](https://github.com/kuba2k2/libretiny) for generating pinouts, it's not really well documented. If you find this project interesting and need any help using it, feel free to open an issue and I'll try to provide more examples and info on how to use it.
```

### Comparing `boardgen-0.6.1/boardgen/cli.py` & `boardgen-0.6.2/boardgen/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
     ctx.invoke(variant, boards=boards, output=output, subdir=subdir)
 
 
 @cli.command()
 @click.option("--no-docs", "-D", is_flag=True, help="Write variant files only")
 @click.pass_context
 def ltci(ctx, no_docs: bool):
-    """Generate board files for LibreTuya CI"""
+    """Generate board files for LibreTiny CI"""
     if not isfile("families.json"):
         print("Run this command in LT root directory")
         exit(1)
     boards = load_boards(["all"])
 
     if not no_docs:
         ctx.invoke(draw, boards=boards, output="boards/", subdir=True)
```

### Comparing `boardgen-0.6.1/boardgen/core/cache.py` & `boardgen-0.6.2/boardgen/core/cache.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/core/core.py` & `boardgen-0.6.2/boardgen/core/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from ..vector import V
 from .cache import CoreCache
 from .getters import CoreGetters
 
 
 class Core(CoreCache, CoreGetters):
     shape_ctors: dict[ShapeType, type]
-    is_libretuya: bool = False
+    is_libretiny: bool = False
 
     _dir_base: str
     _dirs_boards: list[str]
     _dirs_shapes: list[str]
     _dirs_templates: list[str]
     _file_presets: str
     _file_roles: str
@@ -52,15 +52,15 @@
         self._file_flash = join(self._dir_base, "flash.json")
         self.shape_ctors = {
             ShapeType.RECT: Rect,
             ShapeType.CIRCLE: Circle,
             ShapeType.SUBSHAPE: ShapeGroup,
             ShapeType.TEXT: Text,
         }
-        self.is_libretuya = isfile(
+        self.is_libretiny = isfile(
             join(dirname(__file__), "..", "..", "..", "..", "platform.json")
         ) or isfile("families.json")
 
     @property
     def version(self) -> str | None:
         pyproject = join(dirname(__file__), "..", "..", "pyproject.toml")
         if isfile(pyproject):
```

### Comparing `boardgen-0.6.1/boardgen/core/getters.py` & `boardgen-0.6.2/boardgen/core/getters.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/mixins.py` & `boardgen-0.6.2/boardgen/mixins.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/models/board.py` & `boardgen-0.6.2/boardgen/models/board.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/models/enums.py` & `boardgen-0.6.2/boardgen/models/enums.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/models/flash_region.py` & `boardgen-0.6.2/boardgen/models/flash_region.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/models/pcb.py` & `boardgen-0.6.2/boardgen/models/pcb.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/models/role.py` & `boardgen-0.6.2/boardgen/models/role.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/readme/parts.py` & `boardgen-0.6.2/boardgen/readme/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/readme/writer.py` & `boardgen-0.6.2/boardgen/readme/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,26 +79,26 @@
             link = self.get_link(board.doc.fccid, f"https://fccid.io/{board.doc.fccid}")
             rows.append(["FCC ID", link])
         self.add_table(header, *rows)
 
         # Usage
         self.add_heading("Usage", 2)
         self.add_text("**Board code:**", f"`{board.id}`")
-        if self.core.is_libretuya:
+        if self.core.is_libretiny:
             self.add_text("In `platformio.ini`:")
             code = [
                 f"[env:{board.id}]",
-                "platform = libretuya",
+                "platform = libretiny",
                 f"board = {board.id}",
                 "framework = arduino",
             ]
             self.add_code(code, lang="ini")
             self.add_text("In ESPHome YAML:")
             code = [
-                "libretuya:",
+                "libretiny:",
                 "  board: " + board.id,
                 "  framework:",
                 "    version: dev",
             ]
             self.add_code(code, lang="yaml")
 
         # Pinout
```

### Comparing `boardgen-0.6.1/boardgen/res/flash.json` & `boardgen-0.6.2/boardgen/res/flash.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'tuya'": "'Tuya Storage'"}*

```diff
@@ -16,10 +16,11 @@
     "param1": "Param 1",
     "param2": "Param 2",
     "part_table": "Partition Table",
     "rdp": "RDP",
     "rf": "RF Data",
     "system": "System Data",
     "tlv": "TLV Store",
+    "tuya": "Tuya Storage",
     "unknown": "Unknown",
     "userdata": "User Data"
 }
```

### Comparing `boardgen-0.6.1/boardgen/res/presets.json` & `boardgen-0.6.2/boardgen/res/presets.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/roles.json` & `boardgen-0.6.2/boardgen/res/roles.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/labels_horz5_2mm.json` & `boardgen-0.6.2/boardgen/res/shapes/labels_horz5_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/labels_horz6_2mm.json` & `boardgen-0.6.2/boardgen/res/shapes/labels_horz6_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/labels_horz7_2mm.json` & `boardgen-0.6.2/boardgen/res/shapes/labels_horz7_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/labels_horz8_2mm.json` & `boardgen-0.6.2/boardgen/res/shapes/labels_horz8_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/pads_horz5_2mm.json` & `boardgen-0.6.2/boardgen/res/shapes/pads_horz5_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/pads_horz6_2mm.json` & `boardgen-0.6.2/boardgen/res/shapes/pads_horz6_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json` & `boardgen-0.6.2/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json` & `boardgen-0.6.2/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json` & `boardgen-0.6.2/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json` & `boardgen-0.6.2/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json` & `boardgen-0.6.2/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json` & `boardgen-0.6.2/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/shapes/tuya2-pcb.json` & `boardgen-0.6.2/boardgen/res/shapes/tuya2-pcb.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/templates/custom-20x24-22.json` & `boardgen-0.6.2/boardgen/res/templates/custom-20x24-22.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/templates/esp12e-21.json` & `boardgen-0.6.2/boardgen/res/templates/esp12e-21.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/templates/esp12e-22.json` & `boardgen-0.6.2/boardgen/res/templates/esp12e-22.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/templates/esp12s.json` & `boardgen-0.6.2/boardgen/res/templates/esp12s.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/templates/rf-15mm-type1.json` & `boardgen-0.6.2/boardgen/res/templates/rf-15mm-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/templates/rf-16mm-type1.json` & `boardgen-0.6.2/boardgen/res/templates/rf-16mm-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/templates/rf-20mm-type1.json` & `boardgen-0.6.2/boardgen/res/templates/rf-20mm-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/templates/tuya2.json` & `boardgen-0.6.2/boardgen/res/templates/tuya2.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/res/templates/tuya2l.json` & `boardgen-0.6.2/boardgen/res/templates/tuya2l.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/shapes/base.py` & `boardgen-0.6.2/boardgen/shapes/base.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/shapes/circle.py` & `boardgen-0.6.2/boardgen/shapes/circle.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/shapes/fill_style.py` & `boardgen-0.6.2/boardgen/shapes/fill_style.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/shapes/group.py` & `boardgen-0.6.2/boardgen/shapes/group.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/shapes/label/block.py` & `boardgen-0.6.2/boardgen/shapes/label/block.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/shapes/label/io_line.py` & `boardgen-0.6.2/boardgen/shapes/label/io_line.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/shapes/label/label.py` & `boardgen-0.6.2/boardgen/shapes/label/label.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/shapes/rect.py` & `boardgen-0.6.2/boardgen/shapes/rect.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/shapes/text.py` & `boardgen-0.6.2/boardgen/shapes/text.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/utils.py` & `boardgen-0.6.2/boardgen/utils.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/variant/parts.py` & `boardgen-0.6.2/boardgen/variant/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/variant/writer.py` & `boardgen-0.6.2/boardgen/variant/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/boardgen/vector.py` & `boardgen-0.6.2/boardgen/vector.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.1/pyproject.toml` & `boardgen-0.6.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boardgen"
-version = "0.6.1"
+version = "0.6.2"
 description = "Board pinout diagram generator"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `boardgen-0.6.1/PKG-INFO` & `boardgen-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boardgen
-Version: 0.6.1
+Version: 0.6.2
 Summary: Board pinout diagram generator
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -59,15 +59,15 @@
   list  List boards/templates/etc
 ```
 
 ### Board definitions
 
 Writing board definitions means putting a .JSON file to a directory and specifying this directory using the `--boards` option.
 
-Boardgen is meant to be used with PlatformIO-style board definition files. An example of such a board can be found [here (libretuya/boards/wr3.json)](https://github.com/kuba2k2/libretuya/blob/master/boards/wr3.json).
+Boardgen is meant to be used with PlatformIO-style board definition files. An example of such a board can be found [here (libretiny/boards/wr3.json)](https://github.com/kuba2k2/libretiny/blob/master/boards/wr3.json).
 
 Note that the board manifest uses `"_base"` definitions. These are merged recursively with the manifest, and this result is expected to produce a complete file.
 
 Apart from PlatformIO default variables (such as `build`, `debug`, `upload` or `name`, `url` and `vendor`) the board definition contains a [`Pcb`](boardgen/models/pcb.py) object.
 
 ### Templates
 
@@ -153,9 +153,9 @@
   - 1st stop color
   - 2nd stop position
   - 2nd stop color
 - `width`: stroke width (not used for "fill")
 
 ## Support
 
-As this project is just a quick solution that'll be used in [LibreTuya](https://github.com/kuba2k2/libretuya) for generating pinouts, it's not really well documented. If you find this project interesting and need any help using it, feel free to open an issue and I'll try to provide more examples and info on how to use it.
+As this project is just a quick solution that'll be used in [LibreTiny](https://github.com/kuba2k2/libretiny) for generating pinouts, it's not really well documented. If you find this project interesting and need any help using it, feel free to open an issue and I'll try to provide more examples and info on how to use it.
```

