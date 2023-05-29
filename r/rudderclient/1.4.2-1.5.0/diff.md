# Comparing `tmp/rudderclient-1.4.2.tar.gz` & `tmp/rudderclient-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudderclient-1.4.2.tar", last modified: Thu May 25 12:23:00 2023, max compression
+gzip compressed data, was "rudderclient-1.5.0.tar", last modified: Mon May 29 14:30:57 2023, max compression
```

## Comparing `rudderclient-1.4.2.tar` & `rudderclient-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 12:23:00.458890 rudderclient-1.4.2/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1069 2023-05-17 06:37:36.000000 rudderclient-1.4.2/LICENSE
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1968 2023-05-25 12:23:00.458890 rudderclient-1.4.2/PKG-INFO
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      224 2023-05-22 12:05:46.000000 rudderclient-1.4.2/README.md
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      681 2023-05-25 12:22:20.000000 rudderclient-1.4.2/pyproject.toml
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       38 2023-05-25 12:23:00.458890 rudderclient-1.4.2/setup.cfg
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 12:23:00.458890 rudderclient-1.4.2/src/
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 12:23:00.458890 rudderclient-1.4.2/src/rudderclient/
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 12:23:00.458890 rudderclient-1.4.2/src/rudderclient/aws/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     2384 2023-05-25 12:20:59.000000 rudderclient-1.4.2/src/rudderclient/aws/requests.py
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 12:23:00.458890 rudderclient-1.4.2/src/rudderclient/gcp/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 09:45:20.000000 rudderclient-1.4.2/src/rudderclient/gcp/__init__.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1256 2023-05-25 09:35:18.000000 rudderclient-1.4.2/src/rudderclient/gcp/auth.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      381 2023-05-23 12:23:14.000000 rudderclient-1.4.2/src/rudderclient/gcp/http_requests.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      448 2023-05-25 09:35:18.000000 rudderclient-1.4.2/src/rudderclient/gcp/pubsub.py
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 12:23:00.458890 rudderclient-1.4.2/src/rudderclient/tools/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     5118 2023-05-23 09:45:20.000000 rudderclient-1.4.2/src/rudderclient/tools/send_account_email.py
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 12:23:00.458890 rudderclient-1.4.2/src/rudderclient.egg-info/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1968 2023-05-25 12:23:00.000000 rudderclient-1.4.2/src/rudderclient.egg-info/PKG-INFO
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      440 2023-05-25 12:23:00.000000 rudderclient-1.4.2/src/rudderclient.egg-info/SOURCES.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        1 2023-05-25 12:23:00.000000 rudderclient-1.4.2/src/rudderclient.egg-info/dependency_links.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       28 2023-05-25 12:23:00.000000 rudderclient-1.4.2/src/rudderclient.egg-info/requires.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       13 2023-05-25 12:23:00.000000 rudderclient-1.4.2/src/rudderclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.176339 rudderclient-1.5.0/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-05-29 14:30:26.000000 rudderclient-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-29 14:30:57.176339 rudderclient-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-05-29 14:30:26.000000 rudderclient-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)      940 2023-05-29 14:30:46.000000 rudderclient-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-05-29 14:30:57.176339 rudderclient-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.172338 rudderclient-1.5.0/src/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.172338 rudderclient-1.5.0/src/rudderclient/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.174338 rudderclient-1.5.0/src/rudderclient/aws/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/aws/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5274 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/aws/requests.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.174338 rudderclient-1.5.0/src/rudderclient/gcp/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2747 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/gcp/auth.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1087 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/gcp/http_requests.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      943 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/gcp/pubsub.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.175339 rudderclient-1.5.0/src/rudderclient/request/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/request/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/request/exceptions.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.175339 rudderclient-1.5.0/src/rudderclient/tools/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/tools/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5491 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/tools/send_account_email.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.173339 rudderclient-1.5.0/src/rudderclient.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-29 14:30:57.000000 rudderclient-1.5.0/src/rudderclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      629 2023-05-29 14:30:57.000000 rudderclient-1.5.0/src/rudderclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-05-29 14:30:57.000000 rudderclient-1.5.0/src/rudderclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-05-29 14:30:57.000000 rudderclient-1.5.0/src/rudderclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       22 2023-05-29 14:30:57.000000 rudderclient-1.5.0/src/rudderclient.egg-info/top_level.txt
```

### Comparing `rudderclient-1.4.2/LICENSE` & `rudderclient-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rudderclient-1.4.2/PKG-INFO` & `rudderclient-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.4.2
+Version: 1.5.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.4.2/src/rudderclient/tools/send_account_email.py` & `rudderclient-1.5.0/src/rudderclient/tools/send_account_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Email sending library.
 
-This library provides an easy way to send customizable emails with Python. 
+This library provides an easy way to send customizable emails with Python.
 It supports various kinds of attachments like images and PDF files.
 
 Functions:
 ----------
 get_image(file_path):
     Returns a MIMEImage object from a file path.
 
 get_html(file_path, replacements):
     Returns a string from a file, replacing placeholders with actual values.
 
 get_attachment(file_path, filename, _subtype):
     Returns a MIMEApplication object from a file path, filename, and MIME subtype.
 
-send_email(SMTP_USERNAME, SMTP_PASSWORD, FROM, TO, SUBJECT, NAME, EMAIL, 
+send_email(SMTP_USERNAME, SMTP_PASSWORD, FROM, TO, SUBJECT, NAME, EMAIL,
            PLATFORM='', ACCESS_URL='', PASSWORD='', FIRST_STEPS_FILE=None,
-           ERROR=False):
+           ERROR=False, ATTACHMENTS_PATH='', HTML_TEMPLATE_PATH=''):
     Sends an email using SMTP with the provided parameters.
 
     Parameters:
     ----------
     SMTP_USERNAME: str
         Username for the SMTP server.
     SMTP_PASSWORD: str
@@ -42,117 +42,143 @@
         The access URL, used in the email body.
     PASSWORD: str, optional
         The recipient's password, used in the email body.
     FIRST_STEPS_FILE: str, optional
         The file path of a PDF file to be attached to the email.
     ERROR: bool, optional
         Indicates if the email is an error email. If true, it changes the email template.
+    ATTACHMENTS_PATH: str
+        Path to the email attachments.
+    HTML_TEMPLATE_PATH: str
+        Path to the HTML template file.
 
     Raises:
     -------
     Exception:
         If there is an error reading the images, processing the email template, or sending the email.
 """
 
+
 import logging
 from email.mime.image import MIMEImage
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.mime.application import MIMEApplication
-from pathlib import Path
 from smtplib import SMTP
 import os
 
 # Configure logging
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+logging.basicConfig(
+    level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
+)
 
-# Working directory
-WORKING_DIRECTORY = Path("./email_attach")
 # AWS Config
-EMAIL_HOST = 'email-smtp.us-east-1.amazonaws.com'
+EMAIL_HOST = "email-smtp.us-east-1.amazonaws.com"
 EMAIL_PORT = 587
-ATTACHMENT_PATH = WORKING_DIRECTORY / "attachments"
 
 
 def get_image(file_path):
-    with open(file_path, 'rb') as f:
-        return MIMEImage(f.read())
+    try:
+        with open(file_path, "rb") as f:
+            return MIMEImage(f.read())
+    except FileNotFoundError:
+        logging.info(f"Image file not found: {file_path}")
+        return None
 
 
 def get_html(file_path, replacements):
     try:
-        with open(file_path, 'r') as file:
+        with open(file_path, "r") as file:
             filedata = file.read()
 
         for key, val in replacements.items():
             filedata = filedata.replace(key, val)
 
         return filedata
     except Exception as e:
         logging.error(f"Error processing the email template: {e}")
         raise
 
 
-def get_attachment(file_path, filename, _subtype):
-    with open(file_path, 'rb') as f:
-        attach = MIMEApplication(f.read(), _subtype=_subtype)
-        attach.add_header('Content-Disposition', 'attachment', filename=str(filename))
+def get_attachment(file_path, filename):
+    with open(file_path, "rb") as f:
+        ext = filename.split(".")[-1]
+        attach = MIMEApplication(f.read(), _subtype=ext)
+        attach.add_header(
+            "Content-Disposition", "attachment", filename=str(filename)
+        )
         return attach
-    
-def send_email(SMTP_USERNAME, SMTP_PASSWORD, FROM, TO, SUBJECT, NAME, EMAIL, 
-               PLATFORM='', ACCESS_URL='', PASSWORD='', FIRST_STEPS_FILE=None,
-               ERROR=False):
+
+
+def send_email(
+    SMTP_USERNAME,
+    SMTP_PASSWORD,
+    FROM,
+    TO,
+    SUBJECT,
+    NAME,
+    EMAIL,
+    PLATFORM="",
+    ACCESS_URL="",
+    PASSWORD="",
+    ATTACHMENTS_PATH="",
+    HTML_TEMPLATE_PATH="",
+):
     # AWS Config
     EMAIL_HOST_USER = SMTP_USERNAME
     EMAIL_HOST_PASSWORD = SMTP_PASSWORD
 
-    msg = MIMEMultipart('alternative')
-    msg['Subject'] = SUBJECT
-    msg['From'] = FROM
-    msg['To'] = TO
+    msg = MIMEMultipart("alternative")
+    msg["Subject"] = SUBJECT
+    msg["From"] = FROM
+    msg["To"] = TO
 
     # Attach Image
-    try:
-        logo_image = get_image(f'{ATTACHMENT_PATH}/logo.png')
-        logo_image.add_header('Content-Disposition', 'attachment', filename="logo.png")
-        logo_image.add_header('Content-ID', '<logo.png>')
+    logo_image = get_image(os.path.join(ATTACHMENTS_PATH, "logo.png"))
+    if logo_image:
+        logo_image.add_header(
+            "Content-Disposition", "attachment", filename="logo.png"
+        )
+        logo_image.add_header("Content-ID", "<logo.png>")
         msg.attach(logo_image)
 
+    try:
+        # Attach all files in ATTACHMENTS_PATH
+        for filename in os.listdir(ATTACHMENTS_PATH):
+            if filename != "logo.png":
+                full_file_path = os.path.join(ATTACHMENTS_PATH, filename)
+                attach = get_attachment(full_file_path, filename)
+                msg.attach(attach)
     except Exception as e:
-        logging.error(f"Error reading the images: {e}")
+        logging.error(f"Error attaching files: {e}")
         raise
 
-    # Attach optional attachments
-    if FIRST_STEPS_FILE:
-        attach = get_attachment(FIRST_STEPS_FILE, 'first_steps.pdf', 'pdf')
-        msg.attach(attach)
-    
     # Adapt html and txt to user
-    EMAIL_TEMPLATE_HTML = WORKING_DIRECTORY / ("error_email_template.html" if ERROR else "email_template.html")
     replacements = {
-        '{{ EMAIL }}': EMAIL,
-        '{{ NAME }}': NAME,
-        '{{ PLATFORM }}': PLATFORM,
-        '{{ ACCESS_URL }}': ACCESS_URL,
-        '{{ PASSWORD }}': PASSWORD,
-        '{{ COMPANY_NAME }}': "RealNaut",
-        '{{ COMPANY_ADDRESS }}': "Calle de Arturo Soria, 122, 28043 Madrid",
-        '{{ COMPANY_WEB }}': "www.realnaut.com"
+        "{{ EMAIL }}": EMAIL,
+        "{{ NAME }}": NAME,
+        "{{ PLATFORM }}": PLATFORM,
+        "{{ ACCESS_URL }}": ACCESS_URL,
+        "{{ PASSWORD }}": PASSWORD,
+        "{{ COMPANY_NAME }}": "RealNaut",
+        "{{ COMPANY_ADDRESS }}": "Calle de Arturo Soria, 122, 28043 Madrid",
+        "{{ COMPANY_WEB }}": "www.realnaut.com",
     }
 
     try:
-        filedata = get_html(EMAIL_TEMPLATE_HTML, replacements)
+        filedata = get_html(HTML_TEMPLATE_PATH, replacements)
     except Exception as e:
         logging.error(f"Error processing the email template: {e}")
         raise
 
-    msg.attach(MIMEText(filedata, 'html'))
+    msg.attach(MIMEText(filedata, "html"))
 
     # Send Email
     try:
+        logging.info("Attempting to send email...")
         with SMTP(host=EMAIL_HOST, port=EMAIL_PORT) as server:
             server.starttls()
             server.login(EMAIL_HOST_USER, EMAIL_HOST_PASSWORD)
             server.send_message(msg)
 
         logging.info(f"Email sent to {TO}")
     except Exception as e:
```

### Comparing `rudderclient-1.4.2/src/rudderclient.egg-info/PKG-INFO` & `rudderclient-1.5.0/src/rudderclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.4.2
+Version: 1.5.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

