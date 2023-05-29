# Comparing `tmp/streamlitopencvplayer-1.1.0.tar.gz` & `tmp/streamlitopencvplayer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.1.0.tar", last modified: Thu May 25 21:45:59 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.2.0.tar", last modified: Mon May 29 13:26:48 2023, max compression
```

## Comparing `streamlitopencvplayer-1.1.0.tar` & `streamlitopencvplayer-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 21:45:59.585264 streamlitopencvplayer-1.1.0/
--rw-rw-rw-   0        0        0      324 2023-05-25 21:45:59.583263 streamlitopencvplayer-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      985 2023-05-10 09:24:37.000000 streamlitopencvplayer-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 21:45:59.586263 streamlitopencvplayer-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-05-25 21:45:30.000000 streamlitopencvplayer-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 21:45:59.555587 streamlitopencvplayer-1.1.0/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     7352 2023-05-25 21:45:15.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-05-25 21:45:59.571777 streamlitopencvplayer-1.1.0/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      324 2023-05-25 21:45:59.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-25 21:45:59.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 21:45:59.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-25 21:45:59.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 21:45:59.578264 streamlitopencvplayer-1.1.0/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.1.0/test/__init__.py
--rw-rw-rw-   0        0        0      818 2023-05-25 21:34:02.000000 streamlitopencvplayer-1.1.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:26:48.883677 streamlitopencvplayer-1.2.0/
+-rw-rw-rw-   0        0        0      419 2023-05-29 13:26:48.882677 streamlitopencvplayer-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 13:26:48.884676 streamlitopencvplayer-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-05-29 13:26:28.000000 streamlitopencvplayer-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:26:48.850693 streamlitopencvplayer-1.2.0/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     7668 2023-05-29 13:11:21.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:26:48.869680 streamlitopencvplayer-1.2.0/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-05-29 13:26:48.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-05-29 13:26:48.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 13:26:48.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-29 13:26:48.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 13:26:48.877680 streamlitopencvplayer-1.2.0/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.0/test/__init__.py
+-rw-rw-rw-   0        0        0      818 2023-05-25 21:34:02.000000 streamlitopencvplayer-1.2.0/test/test.py
```

### Comparing `streamlitopencvplayer-1.1.0/setup.py` & `streamlitopencvplayer-1.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.0' 
+VERSION = '1.2.0' 
 DESCRIPTION = 'Streamlit Opencv player'
-LONG_DESCRIPTION = 'Streamlit Opencv player'
+LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer", 
         version=VERSION,
         author="Nafaa Bougraine",
```

### Comparing `streamlitopencvplayer-1.1.0/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.2.0/streamlitopencvplayer/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 if 'frames' not in st.session_state:
     st.session_state['frames'] = []
 
 # Use a callback to display the current value of the slider when changed
 
 
 def display_value():
-    st.session_state['counter'] = st.session_state.myslider
+    if 'myslider' in st.session_state:
+        st.session_state['counter'] = st.session_state.myslider
 
 # Function to display video in the Streamlit app
 
 
 def display_video(video_path, alerts_dict, alerts, data):
     # Open the video file
     cap = cv2.VideoCapture(video_path)
@@ -49,33 +50,33 @@
         pause = container_2.button('⏸')
 
     with col2:
         widget = st.empty()
         # Create a Streamlit slider for navigating the video
         widget.slider("", min_value=0, max_value=int(
             cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], key="myslider", on_change=display_value)
-        st.session_state['counter'] = st.session_state.myslider
+        if 'myslider'  in st.session_state:
+            st.session_state['counter'] = st.session_state.myslider
     with col3:
         st.write('')
         st.write('')
         replay = st.button("↻")
     with col4:
         st.write('')
         st.write('')
         plus = st.button("➕")
     with col5:
         st.write('')
         st.write('')
         minus = st.button("➖")
-    if minus:
-        st.session_state['counter'] = st.session_state['counter']-1
-        # the first frame
+
     if replay:
         st.session_state['counter'] = 0
         st.session_state['frames'] = []
+        resume = False
     if selected_rows:
         selected_rows = grid_return["selected_rows"][0]["Alerts"]
 
         if plus:
             st.session_state['counter'] = st.session_state['counter']+1
         elif minus:
             st.session_state['counter'] = st.session_state['counter']-1
@@ -96,15 +97,16 @@
                 st.session_state['frames'].append(frames)
             else:
                 break
         cap.release()
     # back to the first frame if the video is finished
     if st.session_state['counter'] == len(st.session_state['frames']):
         st.session_state['counter'] = 0
-        del st.session_state.myslider
+        if 'myslider' in st.session_state:
+            del st.session_state.myslider
     stframe.image(st.session_state['frames']
                   [st.session_state['counter']], caption='', width=450)
     try:
         while st.session_state['counter'] < len(st.session_state['frames']):
             if not resume:
                 if i < len(data):
                     if st.session_state['counter'] == int(alerts[i]*fps):
@@ -129,38 +131,42 @@
                     st.session_state['frames'][st.session_state['counter']], caption='', width=500)
                 time.sleep(0.08)
                 st.session_state['counter'] += 1
                 # update slider value
 
                 frame_num = widget.slider("", min_value=0, max_value=int(
                     cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
-
-                if st.session_state.myslider > frame_num:
-                    del st.session_state.myslider
-                    # st.session_state.clear()
-                    st.session_state['counter'] = frame_num
-                    #st.session_state['counter'] = 0
-                    resume = True
-                    # st.experimental_rerun() #remove cache
-                    break
+                if 'myslider' in st.session_state:
+                    if st.session_state.myslider > frame_num:
+                        del st.session_state.myslider
+                        #st.session_state.clear()
+                        st.session_state['counter'] = frame_num
+                        #st.session_state['counter'] = 0
+                        resume = True
+                        #st.experimental_rerun() #remove cache
+                    
 
                 if pause:
                     resume = True
                     break
                 if plus:
                     resume = True
                     break
                 if minus:
                     st.session_state['counter'] -= 1
                     resume = True
                     break
+                if replay:
+                    st.session_state['counter'] = 0
+                    st.session_state['frames'] = []
                     # back to the first frame if the video is finished
                 if st.session_state['counter'] == len(st.session_state['frames']):
                     st.session_state['counter'] = 0
-                    del st.session_state.myslider
+                    if 'myslider'  in st.session_state:
+                        del st.session_state.myslider
                 st.session_state['counter'] = frame_num
     except Exception as e:
         st.write('')
     if resume:
         container_2.empty()
         pause = container_2.button('▶')
         resume = False
@@ -168,14 +174,14 @@
 
 def main():
 
     my_dict = {"Alerts": [43, 64]}
     alerts = [43, 64]
     data = [[[10, 100, 290, 200], 0.82, 0, "Class 0"],
             [[55, 22, 100, 120], 0.9, 1, "Class 1"]]
-    video_path = "https://cvlogger.blob.core.windows.net/clientsample/1678352121.8713963_1678352127.8713963.webm?se=2023-05-25T22%3A37%3A17Z&sp=r&sv=2021-08-06&sr=b&sig=Ev%2BgYuVoa00p82rLRBm%2ByqwN3ubvk%2Bb%2BI57Zp7zpWSU%3D"
+    video_path = "https://cvlogger.blob.core.windows.net/clientsample/1678352121.8713963_1678352127.8713963.webm?se=2023-05-29T14%3A09%3A37Z&sp=r&sv=2021-08-06&sr=b&sig=y2dF5a%2BUN7inLzOHJgOLmECl7h9iOHFH5dP8BsIF9Bc%3D"
     if video_path is not None:
         display_video(video_path, my_dict, alerts, data)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `streamlitopencvplayer-1.1.0/test/test.py` & `streamlitopencvplayer-1.2.0/test/test.py`

 * *Files identical despite different names*

