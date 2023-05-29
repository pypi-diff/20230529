# Comparing `tmp/u0_stitcher-0.1.4.tar.gz` & `tmp/u0_stitcher-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "u0_stitcher-0.1.4.tar", last modified: Fri May 26 02:35:12 2023, max compression
+gzip compressed data, was "u0_stitcher-0.1.5.tar", last modified: Mon May 29 09:34:58 2023, max compression
```

## Comparing `u0_stitcher-0.1.4.tar` & `u0_stitcher-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-26 02:35:12.579029 u0_stitcher-0.1.4/
--rw-r--r--   0 u03013112   (502) staff       (20)     4254 2023-05-26 02:35:12.578881 u0_stitcher-0.1.4/PKG-INFO
--rw-r--r--   0 u03013112   (502) staff       (20)     3167 2023-05-25 09:48:10.000000 u0_stitcher-0.1.4/README.md
--rw-r--r--   0 u03013112   (502) staff       (20)       38 2023-05-26 02:35:12.579078 u0_stitcher-0.1.4/setup.cfg
--rw-r--r--   0 u03013112   (502) staff       (20)      865 2023-05-26 02:33:56.000000 u0_stitcher-0.1.4/setup.py
-drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-26 02:35:12.577654 u0_stitcher-0.1.4/u0_stitcher/
--rw-r--r--   0 u03013112   (502) staff       (20)       46 2023-05-25 08:29:16.000000 u0_stitcher-0.1.4/u0_stitcher/__init__.py
--rw-r--r--   0 u03013112   (502) staff       (20)      163 2023-05-25 09:15:53.000000 u0_stitcher-0.1.4/u0_stitcher/errors.py
--rw-r--r--   0 u03013112   (502) staff       (20)     4466 2023-05-25 11:37:38.000000 u0_stitcher-0.1.4/u0_stitcher/fisheye2Equirectangular.py
--rw-r--r--   0 u03013112   (502) staff       (20)    10771 2023-05-25 07:51:21.000000 u0_stitcher-0.1.4/u0_stitcher/stitchEasy3.py
--rw-r--r--   0 u03013112   (502) staff       (20)    12166 2023-05-25 11:49:35.000000 u0_stitcher-0.1.4/u0_stitcher/stitcher.py
-drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-26 02:35:12.578646 u0_stitcher-0.1.4/u0_stitcher.egg-info/
--rw-r--r--   0 u03013112   (502) staff       (20)     4254 2023-05-26 02:35:12.000000 u0_stitcher-0.1.4/u0_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 u03013112   (502) staff       (20)      328 2023-05-26 02:35:12.000000 u0_stitcher-0.1.4/u0_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 u03013112   (502) staff       (20)        1 2023-05-26 02:35:12.000000 u0_stitcher-0.1.4/u0_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 u03013112   (502) staff       (20)       20 2023-05-26 02:35:12.000000 u0_stitcher-0.1.4/u0_stitcher.egg-info/requires.txt
--rw-r--r--   0 u03013112   (502) staff       (20)       12 2023-05-26 02:35:12.000000 u0_stitcher-0.1.4/u0_stitcher.egg-info/top_level.txt
+drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-29 09:34:58.805980 u0_stitcher-0.1.5/
+-rw-r--r--   0 u03013112   (502) staff       (20)     3790 2023-05-29 09:34:58.805846 u0_stitcher-0.1.5/PKG-INFO
+-rw-r--r--   0 u03013112   (502) staff       (20)     3167 2023-05-25 09:48:10.000000 u0_stitcher-0.1.5/README.md
+-rw-r--r--   0 u03013112   (502) staff       (20)       38 2023-05-29 09:34:58.806022 u0_stitcher-0.1.5/setup.cfg
+-rw-r--r--   0 u03013112   (502) staff       (20)      865 2023-05-29 09:33:23.000000 u0_stitcher-0.1.5/setup.py
+drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-29 09:34:58.804044 u0_stitcher-0.1.5/u0_stitcher/
+-rw-r--r--   0 u03013112   (502) staff       (20)       46 2023-05-25 08:29:16.000000 u0_stitcher-0.1.5/u0_stitcher/__init__.py
+-rw-r--r--   0 u03013112   (502) staff       (20)      163 2023-05-25 09:15:53.000000 u0_stitcher-0.1.5/u0_stitcher/errors.py
+-rw-r--r--   0 u03013112   (502) staff       (20)     4466 2023-05-25 11:37:38.000000 u0_stitcher-0.1.5/u0_stitcher/fisheye2Equirectangular.py
+-rw-r--r--   0 u03013112   (502) staff       (20)    10883 2023-05-29 08:50:20.000000 u0_stitcher-0.1.5/u0_stitcher/stitchEasy3.py
+-rw-r--r--   0 u03013112   (502) staff       (20)    13180 2023-05-29 09:31:46.000000 u0_stitcher-0.1.5/u0_stitcher/stitcher.py
+drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-29 09:34:58.805619 u0_stitcher-0.1.5/u0_stitcher.egg-info/
+-rw-r--r--   0 u03013112   (502) staff       (20)     3790 2023-05-29 09:34:58.000000 u0_stitcher-0.1.5/u0_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 u03013112   (502) staff       (20)      328 2023-05-29 09:34:58.000000 u0_stitcher-0.1.5/u0_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 u03013112   (502) staff       (20)        1 2023-05-29 09:34:58.000000 u0_stitcher-0.1.5/u0_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 u03013112   (502) staff       (20)       20 2023-05-29 09:34:58.000000 u0_stitcher-0.1.5/u0_stitcher.egg-info/requires.txt
+-rw-r--r--   0 u03013112   (502) staff       (20)       12 2023-05-29 09:34:58.000000 u0_stitcher-0.1.5/u0_stitcher.egg-info/top_level.txt
```

### Comparing `u0_stitcher-0.1.4/PKG-INFO` & `u0_stitcher-0.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 Metadata-Version: 2.1
 Name: u0_stitcher
-Version: 0.1.4
+Version: 0.1.5
 Summary: stitcher for two fisheye camera
 Home-page: https://github.com/u03013112/pano
 Author: u03013112
 Author-email: u03013112@hotmail.com
-License: UNKNOWN
-Description: # pano
-        
-        全景图像拼接
-        
-        原本是想解决网络遥控车的视角太小，不能有效观察周围情况问题，找到了广角镜头。
-        后来发现竟然可以用两个超过180°的摄像头拼接全景图片。
-        
-        但是在网上没有找到效果好的实时全景传输项目，所以自己做一个。
-        
-        我理解的全景图片生成应该主要是3个步骤
-        1、把图片摊平，这个步骤的学名未知。可能是将鱼眼原图（等角图片）展开成等距图片。
-        2、将两个鱼眼镜头的等距图分成3份，并进行水平拼接
-        3、拼接图按照给定的角度在还原成等角图
-        
-        为了可以做到即时（30FPS），需要尽可能的提高效率。
-        目前最大的效率瓶颈是在拼接上。
-        
-        ## 调研拼接3张水平图片效率  
-        
-        技术上打算采用opencv 的 stitcher，先试试看。
-        
-        `opencv 用 4.X 吧，尽量用新一点的东西。`
-        
-        ## 2023-05-24 进展
-        
-        目前的拼接还是完全自己写的，原因是所有第三方提供的方案均不能有效的对我的图片进行拼接。
-        可能是我的参数有问题，但是我的需求相对简单并且我对拼接效率有要求，所以就自己写了。
-        
-        写的过程还是挺顺利的，由于我的摄像头是背靠背绑在一起的，所以他们的水平同步和角度偏差是不大的，所以我放弃了拼接时进行旋转和扭曲。
-        拼接中对图片只有平移，这对图片首尾相连还是很有帮助的。
-        
-        目前拼接的图片效果还是不错的，拼接效率上没有测试，从代码上看起来，应该是足够高效的。
-        
-        ## 封装思路
-        
-        为了更加模块化，封装思路如下：
-        1、贯彻单视频流方案，虽然涉及拼装切分，单比起双倍的编码和解码，还是要好很多的。所以输入的视频流是两个摄像头的拼接视频流。
-        横向拼接，分辨率一致，帧率一致，编码一致，码率一致。
-        这里可以简化成输入两张（一张）图片，视频流的处理还是放到视频流的相关模块中。
-        2、校准主副镜头，由于目前的两个摄像头都是usb摄像头，usb的可插拔等特性导致，每次启动时，主副镜头的顺序都可能不一致，所以需要校准。
-        3、校准主副镜头的图像，即圆心+半径。这里由于是超级广角，所以图像是一个圆，但是随着镜头的物理位置不稳定，需要进行校准。这里会强制要求两个图片的半径一致，即获得的等距投影图分辨率一致。
-        4、拼接矫正，尝试用等距投影进行拼接。
-        以上校准全部保存校准结果至本地文件，当本地文件不存在，强制要求校准，否则不需要校准。如果有必要可以随时进行校准。
-        5、拼接输入图片，这是一个全流程，输入一张图片（横向拼接原图输入），输出一张图片（等距投影拼接）。
-        
-        暂时封装成一个类。
-        
-        ## 2023-05-25 进展
-        
-        基础功能完成，在比较合适的图片上表现还是挺好的，但是在一些特殊情况，比如校准时的距离与实际视频距离有较大变化的情况下，拼接效果就不好了。
-        
-        所以可能需要手动或者自动进行不断的校准。
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+
+# pano
+
+全景图像拼接
+
+原本是想解决网络遥控车的视角太小，不能有效观察周围情况问题，找到了广角镜头。
+后来发现竟然可以用两个超过180°的摄像头拼接全景图片。
+
+但是在网上没有找到效果好的实时全景传输项目，所以自己做一个。
+
+我理解的全景图片生成应该主要是3个步骤
+1、把图片摊平，这个步骤的学名未知。可能是将鱼眼原图（等角图片）展开成等距图片。
+2、将两个鱼眼镜头的等距图分成3份，并进行水平拼接
+3、拼接图按照给定的角度在还原成等角图
+
+为了可以做到即时（30FPS），需要尽可能的提高效率。
+目前最大的效率瓶颈是在拼接上。
+
+## 调研拼接3张水平图片效率  
+
+技术上打算采用opencv 的 stitcher，先试试看。
+
+`opencv 用 4.X 吧，尽量用新一点的东西。`
+
+## 2023-05-24 进展
+
+目前的拼接还是完全自己写的，原因是所有第三方提供的方案均不能有效的对我的图片进行拼接。
+可能是我的参数有问题，但是我的需求相对简单并且我对拼接效率有要求，所以就自己写了。
+
+写的过程还是挺顺利的，由于我的摄像头是背靠背绑在一起的，所以他们的水平同步和角度偏差是不大的，所以我放弃了拼接时进行旋转和扭曲。
+拼接中对图片只有平移，这对图片首尾相连还是很有帮助的。
+
+目前拼接的图片效果还是不错的，拼接效率上没有测试，从代码上看起来，应该是足够高效的。
+
+## 封装思路
+
+为了更加模块化，封装思路如下：
+1、贯彻单视频流方案，虽然涉及拼装切分，单比起双倍的编码和解码，还是要好很多的。所以输入的视频流是两个摄像头的拼接视频流。
+横向拼接，分辨率一致，帧率一致，编码一致，码率一致。
+这里可以简化成输入两张（一张）图片，视频流的处理还是放到视频流的相关模块中。
+2、校准主副镜头，由于目前的两个摄像头都是usb摄像头，usb的可插拔等特性导致，每次启动时，主副镜头的顺序都可能不一致，所以需要校准。
+3、校准主副镜头的图像，即圆心+半径。这里由于是超级广角，所以图像是一个圆，但是随着镜头的物理位置不稳定，需要进行校准。这里会强制要求两个图片的半径一致，即获得的等距投影图分辨率一致。
+4、拼接矫正，尝试用等距投影进行拼接。
+以上校准全部保存校准结果至本地文件，当本地文件不存在，强制要求校准，否则不需要校准。如果有必要可以随时进行校准。
+5、拼接输入图片，这是一个全流程，输入一张图片（横向拼接原图输入），输出一张图片（等距投影拼接）。
+
+暂时封装成一个类。
+
+## 2023-05-25 进展
+
+基础功能完成，在比较合适的图片上表现还是挺好的，但是在一些特殊情况，比如校准时的距离与实际视频距离有较大变化的情况下，拼接效果就不好了。
+
+所以可能需要手动或者自动进行不断的校准。
```

### Comparing `u0_stitcher-0.1.4/README.md` & `u0_stitcher-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `u0_stitcher-0.1.4/setup.py` & `u0_stitcher-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="u0_stitcher",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         'numpy',
         'opencv-python',
     ],
     author="u03013112",
     author_email="u03013112@hotmail.com",
```

### Comparing `u0_stitcher-0.1.4/u0_stitcher/fisheye2Equirectangular.py` & `u0_stitcher-0.1.5/u0_stitcher/fisheye2Equirectangular.py`

 * *Files identical despite different names*

### Comparing `u0_stitcher-0.1.4/u0_stitcher/stitchEasy3.py` & `u0_stitcher-0.1.5/u0_stitcher/stitchEasy3.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
     control_points1, control_points2 = get_control_points_flann(img2_right, img1)
     overlap_width1 = img2_right.shape[1] - int(min(control_points1, key=lambda x: x[0])[0]) + int(min(control_points2, key=lambda x: x[0])[0])
     # 计算 偏移均值left
     dv1 = np.mean(control_points1 - control_points2, axis=0)
 
     # 计算 img1 和 img2_left 的特征点
     control_points1, control_points2 = get_control_points_flann(img1, img2_left)
+    if len(control_points1) == 0 or len(control_points2) == 0:
+        raise Exception('没有找到特征点')
     overlap_width2 = img1.shape[1] - int(min(control_points1, key=lambda x: x[0])[0]) + int(min(control_points2, key=lambda x: x[0])[0])
     # 计算 偏移均值right
     dv2 = np.mean(control_points1 - control_points2, axis=0)
 
     # 尝试对 偏移均值left 和 偏移均值right 进行统一，最好是个轴对称，如果不是会很麻烦，需要调整两个摄像头的物理位置
     # 由于一个是img2_right 和 img1，另一个是 img1 和 img2_left，所以他们的dv[1]是相反数
     # 对dv[1]取平均值，再按照原来的符号赋值给dv[1]
```

### Comparing `u0_stitcher-0.1.4/u0_stitcher/stitcher.py` & `u0_stitcher-0.1.5/u0_stitcher/stitcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,50 +171,61 @@
         # 如果配置文件中没有圆心和半径的配置，那么就报错，调用者收到这个报错应该调用calibCircleCenter
         if 'img1' not in self.config:
             self.calibMainCamera()
         if 'img1CircleCenter' not in self.config or 'img2CircleCenter' not in self.config or 'imgCircleRadius' not in self.config:
             raise CircleCenterNotCalibratedException('请先校准圆心和半径，调用calibCircleCenter')
         
         # 将图片分开
-        img1 = img[:, :int(img.shape[1] / 2)]
-        img2 = img[:, int(img.shape[1] / 2):]
-        
-        img1Croped = crop_image(img1,(self.config['img1CircleCenter'][0],self.config['img1CircleCenter'][1],self.config['imgCircleRadius']))
-        img2Croped = crop_image(img2,(self.config['img2CircleCenter'][0],self.config['img2CircleCenter'][1],self.config['imgCircleRadius']))
-
+        if self.config['img1'] == 'left':
+            img1 = img[:, :int(img.shape[1] / 2)]
+            img2 = img[:, int(img.shape[1] / 2):]
+            img1Croped = crop_image(img1,(self.config['img1CircleCenter'][0],self.config['img1CircleCenter'][1],self.config['imgCircleRadius']))
+            img2Croped = crop_image(img2,(self.config['img2CircleCenter'][0],self.config['img2CircleCenter'][1],self.config['imgCircleRadius']))
+        else:
+            img1 = img[:, int(img.shape[1] / 2):]
+            img2 = img[:, :int(img.shape[1] / 2)]
+            img1Croped = crop_image(img1,(self.config['img2CircleCenter'][0],self.config['img2CircleCenter'][1],self.config['imgCircleRadius']))
+            img2Croped = crop_image(img2,(self.config['img1CircleCenter'][0],self.config['img1CircleCenter'][1],self.config['imgCircleRadius']))
 
         # 将两张方图分别做成等距投影
         img1EC = self.fisheye2Equirectangular(img1Croped)
         img2EC = self.fisheye2Equirectangular(img2Croped)
-
-        overlap_width1,overlap_width2,dh = stitch2(img1EC,img2EC)
-        # 写配置文件
-        self.config['overlap_width1'] = overlap_width1
-        self.config['overlap_width2'] = overlap_width2
-        self.config['dh'] = dh
-        self.writeConfig()
+        try:
+            overlap_width1,overlap_width2,dh = stitch2(img1EC,img2EC)
+        except Exception as e:
+            print(e)
+        else:
+            # 写配置文件
+            self.config['overlap_width1'] = overlap_width1
+            self.config['overlap_width2'] = overlap_width2
+            self.config['dh'] = dh
+            self.writeConfig()
 
     def stitch(self,img):
         # 进行判断，
         # 如果配置文件中没有img1，则默认左侧是img1
         # 如果配置文件中没有圆心和半径的配置，那么就报错，调用者收到这个报错应该调用calibCircleCenter
         if 'img1' not in self.config:
             self.calibMainCamera()
         if 'img1CircleCenter' not in self.config or 'img2CircleCenter' not in self.config or 'imgCircleRadius' not in self.config:
             raise CircleCenterNotCalibratedException('请先校准圆心和半径，调用calibCircleCenter')
         # 如果配置文件中没有overlap_width1，overlap_width2，dh的配置，那么就报错，调用者收到这个报错应该调用calibStitch
         if 'overlap_width1' not in self.config or 'overlap_width2' not in self.config or 'dh' not in self.config:
             raise StitchNotCalibratedException('请先校准拼接，调用calibStitch')
         # 将图片分开
-        img1 = img[:, :int(img.shape[1] / 2)]
-        img2 = img[:, int(img.shape[1] / 2):]
-
-        img1Croped = crop_image(img1,(self.config['img1CircleCenter'][0],self.config['img1CircleCenter'][1],self.config['imgCircleRadius']))
-        img2Croped = crop_image(img2,(self.config['img2CircleCenter'][0],self.config['img2CircleCenter'][1],self.config['imgCircleRadius']))
-
+        if self.config['img1'] == 'left':
+            img1 = img[:, :int(img.shape[1] / 2)]
+            img2 = img[:, int(img.shape[1] / 2):]
+            img1Croped = crop_image(img1,(self.config['img1CircleCenter'][0],self.config['img1CircleCenter'][1],self.config['imgCircleRadius']))
+            img2Croped = crop_image(img2,(self.config['img2CircleCenter'][0],self.config['img2CircleCenter'][1],self.config['imgCircleRadius']))
+        else:
+            img1 = img[:, int(img.shape[1] / 2):]
+            img2 = img[:, :int(img.shape[1] / 2)]
+            img1Croped = crop_image(img1,(self.config['img2CircleCenter'][0],self.config['img2CircleCenter'][1],self.config['imgCircleRadius']))
+            img2Croped = crop_image(img2,(self.config['img1CircleCenter'][0],self.config['img1CircleCenter'][1],self.config['imgCircleRadius']))
 
         # 将两张方图分别做成等距投影
         img1EC = self.fisheye2Equirectangular(img1Croped)
         img2EC = self.fisheye2Equirectangular(img2Croped)
 
         stitchedResult = stitch3(img1EC,img2EC,self.config['overlap_width1'],self.config['overlap_width2'],self.config['dh'])
```

### Comparing `u0_stitcher-0.1.4/u0_stitcher.egg-info/PKG-INFO` & `u0_stitcher-0.1.5/u0_stitcher.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 Metadata-Version: 2.1
 Name: u0-stitcher
-Version: 0.1.4
+Version: 0.1.5
 Summary: stitcher for two fisheye camera
 Home-page: https://github.com/u03013112/pano
 Author: u03013112
 Author-email: u03013112@hotmail.com
-License: UNKNOWN
-Description: # pano
-        
-        全景图像拼接
-        
-        原本是想解决网络遥控车的视角太小，不能有效观察周围情况问题，找到了广角镜头。
-        后来发现竟然可以用两个超过180°的摄像头拼接全景图片。
-        
-        但是在网上没有找到效果好的实时全景传输项目，所以自己做一个。
-        
-        我理解的全景图片生成应该主要是3个步骤
-        1、把图片摊平，这个步骤的学名未知。可能是将鱼眼原图（等角图片）展开成等距图片。
-        2、将两个鱼眼镜头的等距图分成3份，并进行水平拼接
-        3、拼接图按照给定的角度在还原成等角图
-        
-        为了可以做到即时（30FPS），需要尽可能的提高效率。
-        目前最大的效率瓶颈是在拼接上。
-        
-        ## 调研拼接3张水平图片效率  
-        
-        技术上打算采用opencv 的 stitcher，先试试看。
-        
-        `opencv 用 4.X 吧，尽量用新一点的东西。`
-        
-        ## 2023-05-24 进展
-        
-        目前的拼接还是完全自己写的，原因是所有第三方提供的方案均不能有效的对我的图片进行拼接。
-        可能是我的参数有问题，但是我的需求相对简单并且我对拼接效率有要求，所以就自己写了。
-        
-        写的过程还是挺顺利的，由于我的摄像头是背靠背绑在一起的，所以他们的水平同步和角度偏差是不大的，所以我放弃了拼接时进行旋转和扭曲。
-        拼接中对图片只有平移，这对图片首尾相连还是很有帮助的。
-        
-        目前拼接的图片效果还是不错的，拼接效率上没有测试，从代码上看起来，应该是足够高效的。
-        
-        ## 封装思路
-        
-        为了更加模块化，封装思路如下：
-        1、贯彻单视频流方案，虽然涉及拼装切分，单比起双倍的编码和解码，还是要好很多的。所以输入的视频流是两个摄像头的拼接视频流。
-        横向拼接，分辨率一致，帧率一致，编码一致，码率一致。
-        这里可以简化成输入两张（一张）图片，视频流的处理还是放到视频流的相关模块中。
-        2、校准主副镜头，由于目前的两个摄像头都是usb摄像头，usb的可插拔等特性导致，每次启动时，主副镜头的顺序都可能不一致，所以需要校准。
-        3、校准主副镜头的图像，即圆心+半径。这里由于是超级广角，所以图像是一个圆，但是随着镜头的物理位置不稳定，需要进行校准。这里会强制要求两个图片的半径一致，即获得的等距投影图分辨率一致。
-        4、拼接矫正，尝试用等距投影进行拼接。
-        以上校准全部保存校准结果至本地文件，当本地文件不存在，强制要求校准，否则不需要校准。如果有必要可以随时进行校准。
-        5、拼接输入图片，这是一个全流程，输入一张图片（横向拼接原图输入），输出一张图片（等距投影拼接）。
-        
-        暂时封装成一个类。
-        
-        ## 2023-05-25 进展
-        
-        基础功能完成，在比较合适的图片上表现还是挺好的，但是在一些特殊情况，比如校准时的距离与实际视频距离有较大变化的情况下，拼接效果就不好了。
-        
-        所以可能需要手动或者自动进行不断的校准。
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+
+# pano
+
+全景图像拼接
+
+原本是想解决网络遥控车的视角太小，不能有效观察周围情况问题，找到了广角镜头。
+后来发现竟然可以用两个超过180°的摄像头拼接全景图片。
+
+但是在网上没有找到效果好的实时全景传输项目，所以自己做一个。
+
+我理解的全景图片生成应该主要是3个步骤
+1、把图片摊平，这个步骤的学名未知。可能是将鱼眼原图（等角图片）展开成等距图片。
+2、将两个鱼眼镜头的等距图分成3份，并进行水平拼接
+3、拼接图按照给定的角度在还原成等角图
+
+为了可以做到即时（30FPS），需要尽可能的提高效率。
+目前最大的效率瓶颈是在拼接上。
+
+## 调研拼接3张水平图片效率  
+
+技术上打算采用opencv 的 stitcher，先试试看。
+
+`opencv 用 4.X 吧，尽量用新一点的东西。`
+
+## 2023-05-24 进展
+
+目前的拼接还是完全自己写的，原因是所有第三方提供的方案均不能有效的对我的图片进行拼接。
+可能是我的参数有问题，但是我的需求相对简单并且我对拼接效率有要求，所以就自己写了。
+
+写的过程还是挺顺利的，由于我的摄像头是背靠背绑在一起的，所以他们的水平同步和角度偏差是不大的，所以我放弃了拼接时进行旋转和扭曲。
+拼接中对图片只有平移，这对图片首尾相连还是很有帮助的。
+
+目前拼接的图片效果还是不错的，拼接效率上没有测试，从代码上看起来，应该是足够高效的。
+
+## 封装思路
+
+为了更加模块化，封装思路如下：
+1、贯彻单视频流方案，虽然涉及拼装切分，单比起双倍的编码和解码，还是要好很多的。所以输入的视频流是两个摄像头的拼接视频流。
+横向拼接，分辨率一致，帧率一致，编码一致，码率一致。
+这里可以简化成输入两张（一张）图片，视频流的处理还是放到视频流的相关模块中。
+2、校准主副镜头，由于目前的两个摄像头都是usb摄像头，usb的可插拔等特性导致，每次启动时，主副镜头的顺序都可能不一致，所以需要校准。
+3、校准主副镜头的图像，即圆心+半径。这里由于是超级广角，所以图像是一个圆，但是随着镜头的物理位置不稳定，需要进行校准。这里会强制要求两个图片的半径一致，即获得的等距投影图分辨率一致。
+4、拼接矫正，尝试用等距投影进行拼接。
+以上校准全部保存校准结果至本地文件，当本地文件不存在，强制要求校准，否则不需要校准。如果有必要可以随时进行校准。
+5、拼接输入图片，这是一个全流程，输入一张图片（横向拼接原图输入），输出一张图片（等距投影拼接）。
+
+暂时封装成一个类。
+
+## 2023-05-25 进展
+
+基础功能完成，在比较合适的图片上表现还是挺好的，但是在一些特殊情况，比如校准时的距离与实际视频距离有较大变化的情况下，拼接效果就不好了。
+
+所以可能需要手动或者自动进行不断的校准。
```

