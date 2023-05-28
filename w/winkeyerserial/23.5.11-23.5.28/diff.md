# Comparing `tmp/winkeyerserial-23.5.11.tar.gz` & `tmp/winkeyerserial-23.5.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winkeyerserial-23.5.11.tar", last modified: Thu May 11 19:55:09 2023, max compression
+gzip compressed data, was "winkeyerserial-23.5.28.tar", last modified: Sun May 28 23:51:33 2023, max compression
```

## Comparing `winkeyerserial-23.5.11.tar` & `winkeyerserial-23.5.28.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-11 19:55:09.792730 winkeyerserial-23.5.11/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2021-04-26 00:57:26.000000 winkeyerserial-23.5.11/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2905 2023-05-11 19:55:09.791730 winkeyerserial-23.5.11/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2110 2023-05-11 19:54:52.000000 winkeyerserial-23.5.11/README.md
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1093 2023-05-11 19:52:32.000000 winkeyerserial-23.5.11/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-11 19:55:09.792730 winkeyerserial-23.5.11/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-11 19:55:09.790730 winkeyerserial-23.5.11/winkeyerserial/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-13 06:27:07.000000 winkeyerserial-23.5.11/winkeyerserial/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-01-13 06:27:07.000000 winkeyerserial-23.5.11/winkeyerserial/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15176 2023-05-11 19:47:47.000000 winkeyerserial-23.5.11/winkeyerserial/__main__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13458 2023-02-17 21:44:58.000000 winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1631 2023-02-17 21:44:22.000000 winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4652 2023-02-17 21:44:37.000000 winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      235 2023-02-17 21:46:11.000000 winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7773 2023-01-13 06:27:07.000000 winkeyerserial-23.5.11/winkeyerserial/main.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-11 19:55:09.791730 winkeyerserial-23.5.11/winkeyerserial.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2905 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      554 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       15 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       24 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/top_level.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-28 23:51:33.946216 winkeyerserial-23.5.28/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2021-04-26 00:57:26.000000 winkeyerserial-23.5.28/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2905 2023-05-28 23:51:33.945216 winkeyerserial-23.5.28/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2110 2023-05-11 19:54:52.000000 winkeyerserial-23.5.28/README.md
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1093 2023-05-28 23:18:09.000000 winkeyerserial-23.5.28/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-28 23:51:33.946216 winkeyerserial-23.5.28/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-28 23:51:33.933216 winkeyerserial-23.5.28/winkeyerserial/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-13 06:27:07.000000 winkeyerserial-23.5.28/winkeyerserial/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-01-13 06:27:07.000000 winkeyerserial-23.5.28/winkeyerserial/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15890 2023-05-28 23:49:39.000000 winkeyerserial-23.5.28/winkeyerserial/__main__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13458 2023-02-17 21:44:58.000000 winkeyerserial-23.5.28/winkeyerserial/k6gte-winkeyerserial-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1631 2023-02-17 21:44:22.000000 winkeyerserial-23.5.28/winkeyerserial/k6gte-winkeyerserial-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4652 2023-02-17 21:44:37.000000 winkeyerserial-23.5.28/winkeyerserial/k6gte-winkeyerserial-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      235 2023-02-17 21:46:11.000000 winkeyerserial-23.5.28/winkeyerserial/k6gte-winkeyerserial.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8578 2023-05-28 23:37:57.000000 winkeyerserial-23.5.28/winkeyerserial/main.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-28 23:51:33.943216 winkeyerserial-23.5.28/winkeyerserial.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2905 2023-05-28 23:51:33.000000 winkeyerserial-23.5.28/winkeyerserial.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      554 2023-05-28 23:51:33.000000 winkeyerserial-23.5.28/winkeyerserial.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-28 23:51:33.000000 winkeyerserial-23.5.28/winkeyerserial.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-28 23:51:33.000000 winkeyerserial-23.5.28/winkeyerserial.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       15 2023-05-28 23:51:33.000000 winkeyerserial-23.5.28/winkeyerserial.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       24 2023-05-28 23:51:33.000000 winkeyerserial-23.5.28/winkeyerserial.egg-info/top_level.txt
```

### Comparing `winkeyerserial-23.5.11/LICENSE` & `winkeyerserial-23.5.28/LICENSE`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.5.11/PKG-INFO` & `winkeyerserial-23.5.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winkeyerserial
-Version: 23.5.11
+Version: 23.5.28
 Summary: Talk to K1EL winkeyer
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/PyWinKeyerSerial
 Project-URL: Bug Tracker, https://github.com/mbridak/PyWinKeyerSerial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `winkeyerserial-23.5.11/README.md` & `winkeyerserial-23.5.28/README.md`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.5.11/pyproject.toml` & `winkeyerserial-23.5.28/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "winkeyerserial" 
-version = "23.5.11"
+version = "23.5.28"
 description = "Talk to K1EL winkeyer"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `winkeyerserial-23.5.11/winkeyerserial/JetBrainsMono-Regular.ttf` & `winkeyerserial-23.5.28/winkeyerserial/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.5.11/winkeyerserial/__main__.py` & `winkeyerserial-23.5.28/winkeyerserial/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -252,24 +252,26 @@
         command = b"\x07"  # have the winkeyer return the pot speed setting
         self.port.write(command)
 
     def host_close(self):
         """
         Sends the close command to winkeyer
         """
-        command = b"\x00\x03"
-        self.port.write(command)
+        if hasattr(self.port, "write"):
+            command = b"\x00\x03"
+            self.port.write(command)
 
     def setspeed(self, speed):
         """
         Sets winkeyer speed. I believe valid speeds are from 5 to brainmelt
         """
-        command = chr(2) + chr(int(speed))
-        self.port.write(command.encode())
-        self.spinBox_speed.setValue(int(speed))
+        if hasattr(self.port, "write"):
+            command = chr(2) + chr(int(speed))
+            self.port.write(command.encode())
+            self.spinBox_speed.setValue(int(speed))
 
     def potspeed(self, speed):
         """
         The pot speed value is the 6 LSB of the returned byte.
         It has the 2 MSB of the byte set to 10
         """
         self.setspeed(speed - 123)
@@ -281,93 +283,105 @@
         self.setspeed(self.spinBox_speed.value())
 
     def setmode(self):
         """
         Basically tells the device 'Hey, well be expecting you to
         transform letters into boop-ity boop stuff.'
         """
-        command = b"\x0e\x44"
-        self.port.write(command)
+        if hasattr(self.port, "write"):
+            command = b"\x0e\x44"
+            self.port.write(command)
 
     def sendblended(self, msg):
         """
         a way to glue togetther two characters to send a prosign.
         """
-        command = b"\x1b" + msg.upper().encode()
-        self.port.write(command)
+        if hasattr(self.port, "write"):
+            command = b"\x1b" + msg.upper().encode()
+            self.port.write(command)
 
     def send(self, msg):
         """
         Basic string in, Morse out of the device.
         """
-        command = msg.upper().encode()
-        self.port.write(command)
+        if hasattr(self.port, "write"):
+            command = msg.upper().encode()
+            self.port.write(command)
 
     def send_backspace(self):
         """
         Erases a character from the end of the winkeyer buffer if it has not been sent already.
         """
-        command = b"\x08"
-        self.port.write(command)
+        if hasattr(self.port, "write"):
+            command = b"\x08"
+            self.port.write(command)
 
     def tuneon(self):
         """
         Keydown and hold it.
         """
-        command = b"\x0b\x01"
-        self.port.write(command)
+        if hasattr(self.port, "write"):
+            command = b"\x0b\x01"
+            self.port.write(command)
 
     def tuneoff(self):
         """
         Stop the keydown
         """
-        command = b"\x0b\x00"
-        self.port.write(command)
+        if hasattr(self.port, "write"):
+            command = b"\x0b\x00"
+            self.port.write(command)
 
     def sendmsg1(self):
         """
         This and the following just pull text from the fields next to the button and sends it.
         """
-        local_message = self.msg1.text()
-        self.port.write(local_message.upper().encode())
+        if hasattr(self.port, "write"):
+            local_message = self.msg1.text()
+            self.port.write(local_message.upper().encode())
 
     def sendmsg2(self):
         """
         This and the following just pull text from the fields next to the button and sends it.
         """
-        local_message = self.msg2.text()
-        self.port.write(local_message.upper().encode())
+        if hasattr(self.port, "write"):
+            local_message = self.msg2.text()
+            self.port.write(local_message.upper().encode())
 
     def sendmsg3(self):
         """
         This and the following just pull text from the fields next to the button and sends it.
         """
-        local_message = self.msg3.text()
-        self.port.write(local_message.upper().encode())
+        if hasattr(self.port, "write"):
+            local_message = self.msg3.text()
+            self.port.write(local_message.upper().encode())
 
     def sendmsg4(self):
         """
         This and the following just pull text from the fields next to the button and sends it.
         """
-        local_message = self.msg4.text()
-        self.port.write(local_message.upper().encode())
+        if hasattr(self.port, "write"):
+            local_message = self.msg4.text()
+            self.port.write(local_message.upper().encode())
 
     def sendmsg5(self):
         """
         This and the following just pull text from the fields next to the button and sends it.
         """
-        local_message = self.msg5.text()
-        self.port.write(local_message.upper().encode())
+        if hasattr(self.port, "write"):
+            local_message = self.msg5.text()
+            self.port.write(local_message.upper().encode())
 
     def sendmsg6(self):
         """
         This and the following just pull text from the fields next to the button and sends it.
         """
-        local_message = self.msg6.text()
-        self.port.write(local_message.upper().encode())
+        if hasattr(self.port, "write"):
+            local_message = self.msg6.text()
+            self.port.write(local_message.upper().encode())
 
     def handle_text_change(self):
         """
         This is a poorly handled function where it sends text you type in the big box to the keyer.
         But hey, you get what you pay for. If you can do better then have at it.
         Oh and send a pull request when your done.
         """
@@ -405,20 +419,20 @@
         This is so hackish, it's a bit embarassing.
         This should be handled with slots and signals.
         But.... It works.
         """
         global MESSAGE
         sss = MESSAGE
         MESSAGE = ""
-        if sss:
+        if sss and hasattr(self.port, "write"):
             self.port.write(sss.upper().encode())
 
 
 app = QtWidgets.QApplication(sys.argv)
-app.setStyle("Fusion")
+app.setStyle("Adwaita-Dark")
 PATH = os.path.dirname(pkgutil.get_loader("winkeyerserial").get_filename())
 families = load_fonts_from_dir(PATH)
 logging.info(families)
 keyer = WinKeyer()
 keyer.show()
 keyer.host_init()
 if keyer.port:
```

### Comparing `winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-128.png` & `winkeyerserial-23.5.28/winkeyerserial/k6gte-winkeyerserial-128.png`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-32.png` & `winkeyerserial-23.5.28/winkeyerserial/k6gte-winkeyerserial-32.png`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-64.png` & `winkeyerserial-23.5.28/winkeyerserial/k6gte-winkeyerserial-64.png`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.5.11/winkeyerserial/main.ui` & `winkeyerserial-23.5.28/winkeyerserial/main.ui`

 * *Files 4% similar despite different names*

#### Comparing `winkeyerserial-23.5.11/winkeyerserial/main.ui` & `winkeyerserial-23.5.28/winkeyerserial/main.ui`

```diff
@@ -2,23 +2,23 @@
 <ui version="4.0">
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>371</width>
-        <height>502</height>
+        <width>579</width>
+        <height>594</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>K6GTE winkeyerserial</string>
     </property>
     <widget class="QWidget" name="centralwidget">
-      <layout class="QGridLayout" name="gridLayout" rowstretch="0,0,0,0,0,0,0,0,0,0,0,0">
+      <layout class="QGridLayout" name="gridLayout" rowstretch="0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0">
         <property name="leftMargin">
           <number>15</number>
         </property>
         <property name="topMargin">
           <number>15</number>
         </property>
         <property name="rightMargin">
@@ -29,27 +29,15 @@
         </property>
         <property name="horizontalSpacing">
           <number>10</number>
         </property>
         <property name="verticalSpacing">
           <number>4</number>
         </property>
-        <item row="0" column="0">
-          <widget class="QLabel" name="label">
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-            <property name="text">
-              <string>Sent Text</string>
-            </property>
-          </widget>
-        </item>
-        <item row="3" column="0" colspan="3">
+        <item row="3" column="1" colspan="4">
           <widget class="QPlainTextEdit" name="inputbox">
             <property name="maximumSize">
               <size>
                 <width>16777215</width>
                 <height>153</height>
               </size>
             </property>
@@ -57,247 +45,283 @@
               <font>
                 <family>JetBrains Mono</family>
               </font>
             </property>
           </widget>
         </item>
         <item row="2" column="1">
-          <widget class="QLabel" name="label_3">
+          <widget class="QLabel" name="label_2">
             <property name="font">
               <font>
                 <family>JetBrains Mono</family>
               </font>
             </property>
             <property name="text">
-              <string>Speed:</string>
-            </property>
-            <property name="alignment">
-              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+              <string>Free text input</string>
             </property>
           </widget>
         </item>
-        <item row="2" column="2">
+        <item row="2" column="4">
           <widget class="QSpinBox" name="spinBox_speed">
             <property name="font">
               <font>
                 <family>JetBrains Mono</family>
               </font>
             </property>
             <property name="minimum">
               <number>5</number>
             </property>
             <property name="maximum">
               <number>35</number>
             </property>
           </widget>
         </item>
-        <item row="0" column="1" colspan="2">
-          <widget class="QComboBox" name="comboBox_device">
-            <property name="sizePolicy">
-              <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-                <horstretch>0</horstretch>
-                <verstretch>0</verstretch>
-              </sizepolicy>
-            </property>
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-            <property name="currentText">
-              <string/>
-            </property>
-          </widget>
-        </item>
-        <item row="1" column="0" colspan="3">
-          <widget class="QPlainTextEdit" name="outputbox">
-            <property name="maximumSize">
-              <size>
-                <width>16777215</width>
-                <height>112</height>
-              </size>
-            </property>
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-          </widget>
-        </item>
-        <item row="2" column="0">
-          <widget class="QLabel" name="label_2">
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-            <property name="text">
-              <string>Free text input</string>
-            </property>
-          </widget>
-        </item>
-        <item row="4" column="2">
-          <widget class="QPushButton" name="sendmsg1_button">
-            <property name="maximumSize">
-              <size>
-                <width>70</width>
-                <height>16777215</height>
-              </size>
-            </property>
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-            <property name="text">
-              <string>msg 1</string>
-            </property>
-          </widget>
-        </item>
-        <item row="5" column="2">
-          <widget class="QPushButton" name="sendmsg2_button">
-            <property name="maximumSize">
-              <size>
-                <width>70</width>
-                <height>16777215</height>
-              </size>
-            </property>
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-            <property name="text">
-              <string>msg 2</string>
-            </property>
-          </widget>
-        </item>
-        <item row="6" column="2">
-          <widget class="QPushButton" name="sendmsg3_button">
-            <property name="maximumSize">
-              <size>
-                <width>70</width>
-                <height>16777215</height>
-              </size>
-            </property>
+        <item row="0" column="1">
+          <widget class="QLabel" name="label">
             <property name="font">
               <font>
                 <family>JetBrains Mono</family>
               </font>
             </property>
             <property name="text">
-              <string>msg 3</string>
+              <string>Sent Text</string>
             </property>
           </widget>
         </item>
-        <item row="9" column="2">
-          <widget class="QPushButton" name="sendmsg4_button">
-            <property name="maximumSize">
-              <size>
-                <width>70</width>
-                <height>16777215</height>
-              </size>
-            </property>
+        <item row="2" column="3">
+          <widget class="QLabel" name="label_3">
             <property name="font">
               <font>
                 <family>JetBrains Mono</family>
               </font>
             </property>
             <property name="text">
-              <string>msg 4</string>
-            </property>
-          </widget>
-        </item>
-        <item row="10" column="2">
-          <widget class="QPushButton" name="sendmsg5_button">
-            <property name="maximumSize">
-              <size>
-                <width>70</width>
-                <height>16777215</height>
-              </size>
-            </property>
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
+              <string>Speed:</string>
             </property>
-            <property name="text">
-              <string>msg 5</string>
+            <property name="alignment">
+              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
             </property>
           </widget>
         </item>
-        <item row="11" column="2">
-          <widget class="QPushButton" name="sendmsg6_button">
+        <item row="1" column="1" colspan="4">
+          <widget class="QPlainTextEdit" name="outputbox">
             <property name="maximumSize">
               <size>
-                <width>70</width>
-                <height>16777215</height>
+                <width>16777215</width>
+                <height>112</height>
               </size>
             </property>
             <property name="font">
               <font>
                 <family>JetBrains Mono</family>
               </font>
             </property>
-            <property name="text">
-              <string>msg 6</string>
-            </property>
-          </widget>
-        </item>
-        <item row="4" column="0" colspan="2">
-          <widget class="QLineEdit" name="msg1">
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-          </widget>
-        </item>
-        <item row="5" column="0" colspan="2">
-          <widget class="QLineEdit" name="msg2">
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
           </widget>
         </item>
-        <item row="6" column="0" colspan="2">
-          <widget class="QLineEdit" name="msg3">
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-          </widget>
+        <item row="15" column="1" colspan="4">
+          <layout class="QHBoxLayout" name="horizontalLayout_6">
+            <item>
+              <widget class="QLineEdit" name="msg6">
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="sendmsg6_button">
+                <property name="maximumSize">
+                  <size>
+                    <width>70</width>
+                    <height>16777215</height>
+                  </size>
+                </property>
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+                <property name="text">
+                  <string>msg 6</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item row="12" column="1" colspan="4">
+          <layout class="QHBoxLayout" name="horizontalLayout_5">
+            <item>
+              <widget class="QLineEdit" name="msg5">
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="sendmsg5_button">
+                <property name="maximumSize">
+                  <size>
+                    <width>70</width>
+                    <height>16777215</height>
+                  </size>
+                </property>
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+                <property name="text">
+                  <string>msg 5</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item row="11" column="1" colspan="4">
+          <layout class="QHBoxLayout" name="horizontalLayout_4">
+            <item>
+              <widget class="QLineEdit" name="msg4">
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="sendmsg4_button">
+                <property name="maximumSize">
+                  <size>
+                    <width>70</width>
+                    <height>16777215</height>
+                  </size>
+                </property>
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+                <property name="text">
+                  <string>msg 4</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item row="9" column="1" colspan="4">
+          <layout class="QHBoxLayout" name="horizontalLayout_3">
+            <item>
+              <widget class="QLineEdit" name="msg3">
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="sendmsg3_button">
+                <property name="maximumSize">
+                  <size>
+                    <width>70</width>
+                    <height>16777215</height>
+                  </size>
+                </property>
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+                <property name="text">
+                  <string>msg 3</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item row="8" column="1" colspan="4">
+          <layout class="QHBoxLayout" name="horizontalLayout_2">
+            <item>
+              <widget class="QLineEdit" name="msg2">
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="sendmsg2_button">
+                <property name="maximumSize">
+                  <size>
+                    <width>70</width>
+                    <height>16777215</height>
+                  </size>
+                </property>
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+                <property name="text">
+                  <string>msg 2</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item row="4" column="1" colspan="4">
+          <layout class="QHBoxLayout" name="horizontalLayout">
+            <item>
+              <widget class="QLineEdit" name="msg1">
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="sendmsg1_button">
+                <property name="maximumSize">
+                  <size>
+                    <width>70</width>
+                    <height>16777215</height>
+                  </size>
+                </property>
+                <property name="font">
+                  <font>
+                    <family>JetBrains Mono</family>
+                  </font>
+                </property>
+                <property name="text">
+                  <string>msg 1</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
         </item>
-        <item row="9" column="0" colspan="2">
-          <widget class="QLineEdit" name="msg4">
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
+        <item row="0" column="2" colspan="3">
+          <widget class="QComboBox" name="comboBox_device">
+            <property name="sizePolicy">
+              <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+                <horstretch>0</horstretch>
+                <verstretch>0</verstretch>
+              </sizepolicy>
             </property>
-          </widget>
-        </item>
-        <item row="10" column="0" colspan="2">
-          <widget class="QLineEdit" name="msg5">
             <property name="font">
               <font>
                 <family>JetBrains Mono</family>
               </font>
             </property>
-          </widget>
-        </item>
-        <item row="11" column="0" colspan="2">
-          <widget class="QLineEdit" name="msg6">
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
+            <property name="currentText">
+              <string/>
             </property>
           </widget>
         </item>
       </layout>
     </widget>
   </widget>
   <resources/>
```

### Comparing `winkeyerserial-23.5.11/winkeyerserial.egg-info/PKG-INFO` & `winkeyerserial-23.5.28/winkeyerserial.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winkeyerserial
-Version: 23.5.11
+Version: 23.5.28
 Summary: Talk to K1EL winkeyer
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/PyWinKeyerSerial
 Project-URL: Bug Tracker, https://github.com/mbridak/PyWinKeyerSerial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `winkeyerserial-23.5.11/winkeyerserial.egg-info/SOURCES.txt` & `winkeyerserial-23.5.28/winkeyerserial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

