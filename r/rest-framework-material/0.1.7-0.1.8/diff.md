# Comparing `tmp/rest_framework_material-0.1.7.tar.gz` & `tmp/rest_framework_material-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_material-0.1.7.tar", max compression
+gzip compressed data, was "rest_framework_material-0.1.8.tar", max compression
```

## Comparing `rest_framework_material-0.1.7.tar` & `rest_framework_material-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-21 17:36:10.988103 rest_framework_material-0.1.7/LICENSE
--rw-r--r--   0        0        0      637 2023-04-29 18:13:11.272014 rest_framework_material-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      749 2023-04-21 17:40:45.269789 rest_framework_material-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_material-0.1.7/rest_framework_material/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_material-0.1.7/rest_framework_material/admin.py
--rw-r--r--   0        0        0      248 2023-04-21 17:38:09.789518 rest_framework_material-0.1.7/rest_framework_material/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_material-0.1.7/rest_framework_material/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_material-0.1.7/rest_framework_material/models.py
--rw-r--r--   0        0        0    23044 2023-04-29 07:01:05.243695 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1181 2023-04-21 17:25:31.881402 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      682 2023-04-22 06:32:18.842409 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     3618 2023-04-24 06:09:24.194418 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1638 2023-04-29 07:07:20.918701 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      731 2023-04-29 07:07:37.667061 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_material-0.1.7/rest_framework_material/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_material-0.1.7/rest_framework_material/views.py
--rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 rest_framework_material-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-21 17:36:10.988103 rest_framework_material-0.1.8/LICENSE
+-rw-r--r--   0        0        0      637 2023-05-29 12:49:28.397280 rest_framework_material-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      754 2023-05-29 12:56:42.163758 rest_framework_material-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_material-0.1.8/rest_framework_material/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_material-0.1.8/rest_framework_material/admin.py
+-rw-r--r--   0        0        0      248 2023-04-21 17:38:09.789518 rest_framework_material-0.1.8/rest_framework_material/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_material-0.1.8/rest_framework_material/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_material-0.1.8/rest_framework_material/models.py
+-rw-r--r--   0        0        0    23044 2023-04-29 07:01:05.243695 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1183 2023-05-29 12:02:27.335562 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      682 2023-04-22 06:32:18.842409 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      878 2023-05-29 12:05:50.845274 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1579 2023-05-29 11:45:25.739927 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1194 2023-05-29 11:45:41.917043 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1511 2023-05-29 12:05:59.274119 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1232 2023-05-29 12:06:07.100461 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1266 2023-05-29 11:45:54.449056 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      840 2023-05-29 11:44:17.621348 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     3617 2023-05-29 11:46:11.504738 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1656 2023-05-29 11:38:06.884750 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      731 2023-04-29 07:07:37.667061 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      309 2023-05-29 11:41:05.911073 rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_material-0.1.8/rest_framework_material/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_material-0.1.8/rest_framework_material/views.py
+-rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 rest_framework_material-0.1.8/PKG-INFO
```

### Comparing `rest_framework_material-0.1.7/LICENSE` & `rest_framework_material-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.7/pyproject.toml` & `rest_framework_material-0.1.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-material"
-version = "0.1.7"
+version = "0.1.8"
 description = "Redesign of the browsable api of Django REST Framework using MD Bootstrap"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_material"}]
 homepage = "https://github.com/youzarsiph/rest-framework-material/"
 repository = "https://github.com/youzarsiph/rest-framework-material/"
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/api.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/filters/base.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/filters/base.html`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
           data-mdb-dismiss="modal"
           aria-label="Close"
         ></button>
       </div>
       <div class="modal-body">
         <div class="d-grid gap-4">
           {% for element in elements %}
-          <div>{{ element }}</div>
+            <div>{{ element }}</div>
           {% endfor %}
           <button
             type="button"
             class="btn btn-lg btn-secondary"
             data-mdb-dismiss="modal"
           >
             <strong
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/filters/ordering.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/filters/search.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/checkbox.html`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     {% if field.help_text %}
       <small class="d-block text-muted">{{ field.help_text|safe }}</small>
     {% endif %}
 
     {% if field.errors %}
       <div class="mt-3"></div>
       {% for error in field.errors %}
-        <div role="alert" class="alert alert-warning mb-3">
-          <p>{{ error }}</p>
+        <div role="alert" class="alert alert-danger mb-3">
+          <p class="mb-0">{{ error }}</p>
         </div>
       {% endfor %}
     {% endif %}
   </div>
 </div>
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,14 @@
     {% if field.help_text %}
       <small class="d-block text-muted">{{ field.help_text|safe }}</small>
     {% endif %}
 
     {% if field.errors %}
       <div class="mt-3"></div>
       {% for error in field.errors %}
-        <div role="alert" class="alert alert-warning mb-3">
-          <p>{{ error }}</p>
+        <div role="alert" class="alert alert-danger mb-3">
+          <p class="mb-0">{{ error }}</p>
         </div>
       {% endfor %}
     {% endif %}
   </div>
 </div>
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/input.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/input.html`

 * *Files 12% similar despite different names*

```diff
@@ -23,13 +23,13 @@
     {% if field.help_text %}
       <small class="d-block text-muted">{{ field.help_text|safe }}</small>
     {% endif %}
 
     {% if field.errors %}
       <div class="mt-3"></div>
       {% for error in field.errors %}
-        <div role="alert" class="alert alert-warning mb-3">
-          <p>{{ error }}</p>
+        <div role="alert" class="alert alert-danger mb-3">
+          <p class="mb-0">{{ error }}</p>
         </div>
       {% endfor %}
     {% endif %}
 </div>
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/radio.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/radio.html`

 * *Files 1% similar despite different names*

```diff
@@ -44,13 +44,13 @@
     {% if field.help_text %}
       <small class="d-block text-muted">{{ field.help_text|safe }}</small>
     {% endif %}
 
     {% if field.errors %}
       <div class="mt-3"></div>
       {% for error in field.errors %}
-        <div role="alert" class="alert alert-warning mb-3">
-          <p>{{ error }}</p>
+        <div role="alert" class="alert alert-danger mb-3">
+          <p class="mb-0">{{ error }}</p>
         </div>
       {% endfor %}
     {% endif %}
 </div>
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/select.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/select.html`

 * *Files 18% similar despite different names*

```diff
@@ -26,13 +26,13 @@
   {% if field.help_text %}
     <small class="d-block text-muted">{{ field.help_text|safe }}</small>
   {% endif %}
 
   {% if field.errors %}
     <div class="mt-3"></div>
     {% for error in field.errors %}
-      <div role="alert" class="alert alert-warning mb-3">
-        <p>{{ error }}</p>
+      <div role="alert" class="alert alert-danger mb-3">
+        <p class="mb-0">{{ error }}</p>
       </div>
     {% endfor %}
   {% endif %}
 </div>
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html`

 * *Files 6% similar despite different names*

```diff
@@ -29,13 +29,13 @@
   {% if field.help_text %}
     <small class="d-block text-muted">{{ field.help_text|safe }}</small>
   {% endif %}
 
   {% if field.errors %}
     <div class="mt-3"></div>
     {% for error in field.errors %}
-      <div role="alert" class="alert alert-warning mb-3">
-        <p>{{ error }}</p>
+      <div role="alert" class="alert alert-danger mb-3">
+        <p class="mb-0">{{ error }}</p>
       </div>
     {% endfor %}
   {% endif %}
 </div>
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/horizontal/textarea.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/horizontal/textarea.html`

 * *Files 3% similar despite different names*

```diff
@@ -14,13 +14,13 @@
   {% if field.help_text %}
     <small class="d-block text-muted">{{ field.help_text|safe }}</small>
   {% endif %}
 
   {% if field.errors %}
     <div class="mt-3"></div>
     {% for error in field.errors %}
-      <div role="alert" class="alert alert-warning mb-3">
-        <p>{{ error }}</p>
+      <div role="alert" class="alert alert-danger mb-3">
+        <p class="mb-0">{{ error }}</p>
       </div>
     {% endfor %}
   {% endif %}
 </div>
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/login.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/login.html`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                     {{ form.password.errors|striptags }}
                   </small>
                 {% endif %}
               </div>
 
               {% if form.non_field_errors %}
                 {% for error in form.non_field_errors %}
-                  <div class="alert alert-warning" role="alert">{{ error }}</div>
+                  <div class="alert alert-danger" role="alert">{{ error }}</div>
                 {% endfor %}
               {% endif %}
 
               <button type="submit" class="btn btn-lg btn-primary w-100">
                 <strong class="d-flex align-items-center justify-content-center gap-3">
                   <i class="bi bi-box-arrow-in-right"></i>
                   {% translate "Login" %}
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/pagination/numbers.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/pagination/numbers.html`

 * *Files 4% similar despite different names*

```diff
@@ -88,16 +88,17 @@
 00000570: 3d22 7472 7565 223e 2672 6171 756f 3b3c  ="true">&raquo;<
 00000580: 2f73 7061 6e3e 0a20 2020 2020 2020 203c  /span>.        <
 00000590: 2f61 3e0a 2020 2020 2020 3c2f 6c69 3e0a  /a>.      </li>.
 000005a0: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
 000005b0: 2020 2020 203c 6c69 2063 6c61 7373 3d22       <li class="
 000005c0: 7061 6765 2d69 7465 6d20 6469 7361 626c  page-item disabl
 000005d0: 6564 223e 0a20 2020 2020 2020 203c 6120  ed">.        <a 
-000005e0: 6872 6566 3d22 2322 2061 7269 612d 6c61  href="#" aria-la
-000005f0: 6265 6c3d 224e 6578 7422 3e0a 2020 2020  bel="Next">.    
-00000600: 2020 2020 2020 3c73 7061 6e20 6172 6961        <span aria
-00000610: 2d68 6964 6465 6e3d 2274 7275 6522 3e26  -hidden="true">&
-00000620: 7261 7175 6f3b 3c2f 7370 616e 3e0a 2020  raquo;</span>.  
-00000630: 2020 2020 2020 3c2f 613e 0a20 2020 2020        </a>.     
-00000640: 203c 2f6c 693e 0a20 2020 207b 2520 656e   </li>.    {% en
-00000650: 6469 6620 257d 0a20 203c 2f6f 6c3e 0a3c  dif %}.  </ol>.<
-00000660: 2f6e 6176 3e0a                           /nav>.
+000005e0: 636c 6173 733d 2270 6167 652d 6c69 6e6b  class="page-link
+000005f0: 2220 6872 6566 3d22 2322 2061 7269 612d  " href="#" aria-
+00000600: 6c61 6265 6c3d 224e 6578 7422 3e0a 2020  label="Next">.  
+00000610: 2020 2020 2020 2020 3c73 7061 6e20 6172          <span ar
+00000620: 6961 2d68 6964 6465 6e3d 2274 7275 6522  ia-hidden="true"
+00000630: 3e26 7261 7175 6f3b 3c2f 7370 616e 3e0a  >&raquo;</span>.
+00000640: 2020 2020 2020 2020 3c2f 613e 0a20 2020          </a>.   
+00000650: 2020 203c 2f6c 693e 0a20 2020 207b 2520     </li>.    {% 
+00000660: 656e 6469 6620 257d 0a20 203c 2f6f 6c3e  endif %}.  </ol>
+00000670: 0a3c 2f6e 6176 3e0a                      .</nav>.
```

### Comparing `rest_framework_material-0.1.7/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_material-0.1.8/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.7/PKG-INFO` & `rest_framework_material-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-material
-Version: 0.1.7
+Version: 0.1.8
 Summary: Redesign of the browsable api of Django REST Framework using MD Bootstrap
 Home-page: https://github.com/youzarsiph/rest-framework-material/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,19 +15,19 @@
 Requires-Dist: django (>=4.2,<5.0)
 Requires-Dist: djangorestframework (>=3.14,<4.0)
 Project-URL: Repository, https://github.com/youzarsiph/rest-framework-material/
 Description-Content-Type: text/markdown
 
 # rest-framework-material
 
-Redesign of the browsable api of Django REST Framework using MD Bootstrap
+Redesign of the browsable API of Django REST Framework using MD Bootstrap.
 
-## Get started
+The project aims to improve the look and feel of the API.
 
-To get started with rest-framework-material:
+## Get started
 
 Install the package:
 
 ```bash
 pip install rest-framework-material
 ```
 
@@ -55,9 +55,9 @@
 urlpatterns = [
     ...
     path('auth/', include('rest_framework.urls')),
     ...
 ]
 ```
 
-I hope you that you find this useful.
+I hope you find this useful.
```

