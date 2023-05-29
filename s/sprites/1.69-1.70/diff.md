# Comparing `tmp/sprites-1.69.tar.gz` & `tmp/sprites-1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprites-1.69.tar", last modified: Fri May 26 12:45:22 2023, max compression
+gzip compressed data, was "sprites-1.70.tar", last modified: Mon May 29 09:32:11 2023, max compression
```

## Comparing `sprites-1.69.tar` & `sprites-1.70.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 12:45:22.658787 sprites-1.69/
--rw-rw-rw-   0        0        0     2099 2023-05-26 12:45:22.656787 sprites-1.69/PKG-INFO
--rw-rw-rw-   0        0        0     1001 2020-01-01 03:51:20.000000 sprites-1.69/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 12:45:22.661787 sprites-1.69/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-05-26 12:44:48.000000 sprites-1.69/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:45:22.618785 sprites-1.69/sprites/
--rw-rw-rw-   0        0        0  1439092 2023-05-11 01:04:21.000000 sprites-1.69/sprites/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:45:22.648786 sprites-1.69/sprites.egg-info/
--rw-rw-rw-   0        0        0     2099 2023-05-26 12:45:22.000000 sprites-1.69/sprites.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-26 12:45:22.000000 sprites-1.69/sprites.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 12:45:22.000000 sprites-1.69/sprites.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-26 12:45:16.000000 sprites-1.69/sprites.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-05-26 12:45:22.000000 sprites-1.69/sprites.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 12:45:22.000000 sprites-1.69/sprites.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 09:32:11.152691 sprites-1.70/
+-rw-rw-rw-   0        0        0     2099 2023-05-29 09:32:11.150691 sprites-1.70/PKG-INFO
+-rw-rw-rw-   0        0        0     1001 2023-05-29 09:32:05.000000 sprites-1.70/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 09:32:11.154692 sprites-1.70/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-05-29 09:30:55.000000 sprites-1.70/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:32:11.114689 sprites-1.70/sprites/
+-rw-rw-rw-   0        0        0  1438345 2023-05-29 06:20:09.000000 sprites-1.70/sprites/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:32:11.144691 sprites-1.70/sprites.egg-info/
+-rw-rw-rw-   0        0        0     2099 2023-05-29 09:32:10.000000 sprites-1.70/sprites.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-29 09:32:11.000000 sprites-1.70/sprites.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 09:32:10.000000 sprites-1.70/sprites.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-29 09:18:17.000000 sprites-1.70/sprites.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-05-29 09:32:10.000000 sprites-1.70/sprites.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-29 09:32:10.000000 sprites-1.70/sprites.egg-info/top_level.txt
```

### Comparing `sprites-1.69/PKG-INFO` & `sprites-1.70/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprites
-Version: 1.69
+Version: 1.70
 Summary: Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com
 Home-page: http://www.lixingqiu.com
 Author: lixingqiu
 Author-email: 406273900@qq.com
 License: MIT
 Description: ﻿# Python sprites module introduce
         
@@ -16,15 +16,15 @@
         ## Main application scenarios:
         1、Introduction to children's computer games and animation development.
         2、learn the ABC of Python game development.
         3、Python game crash.
         4、Getting started with Python for training institutions.
         5、Python experience courses and public welfare courses of training institutions.
         
-         
         
         more example,please conatct lixingqiu, wechat:scratch8,website:<http://www.lixingqiu.com>
         
         sprites module Developer: Li Xingqiu，email:406273900@qq.com,Pingxiang, Jiangxi, China.
+         
 Keywords: creative game pygame turtle animation sprite geometry math Elementary Mathematics Teaching
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `sprites-1.69/README.md` & `sprites-1.70/README.md`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 ## Main application scenarios:
 1、Introduction to children's computer games and animation development.
 2、learn the ABC of Python game development.
 3、Python game crash.
 4、Getting started with Python for training institutions.
 5、Python experience courses and public welfare courses of training institutions.
 
- 
 
 more example,please conatct lixingqiu, wechat:scratch8,website:<http://www.lixingqiu.com>
 
-sprites module Developer: Li Xingqiu，email:406273900@qq.com,Pingxiang, Jiangxi, China.
+sprites module Developer: Li Xingqiu，email:406273900@qq.com,Pingxiang, Jiangxi, China.
+
```

### Comparing `sprites-1.69/setup.py` & `sprites-1.70/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding='utf-8') as fh:
     long_d = fh.read()
 
 
 setup(name='sprites',
       long_description_content_type="text/markdown",
-      version = '1.69',
+      version = '1.70',
       description = 'Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com',
       long_description = long_d,      
       keywords = 'creative game pygame turtle animation sprite geometry math Elementary Mathematics Teaching',
       url = 'http://www.lixingqiu.com',
       wechat = 'scratch8',
       author ='lixingqiu',
       author_email = '406273900@qq.com',
```

### Comparing `sprites-1.69/sprites/__init__.py` & `sprites-1.70/sprites/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
    72. gettop：获取角色或项目编号的最顶y坐标。
    73. getbottom：获取角色或项目编号的最底y坐标。
    74. pixelcollide：像素碰撞方法。用于两个角色之间的像素级别碰撞。返回碰撞点的坐标及两个角色在这个点的像素值及重叠区域矩形。
    75. draggable：设置角色为可拖放。要取消只要设置ondrag方法的值为None即可。
    76. saveshape：保存当前造型为图片，只支持image类型的角色。
    77. coloroverlap：角色造型图片上的颜色重叠检测命令，属于像素级碰撞命令。
    78. collidecolor：碰到颜色命令
+   79. fill命令，填充命令，有三种模式，mode=0适合于填充凸多边形，mode=1适合于任意多边形，mode为2采用不同算法适合于任何多边形，速度较快。
    
    三. screen新增命令：
    
    在海龟画图中，屏幕的本质是继承自框架内的画布和滚动条。sprites模块中也一样，但是把屏幕放在了名为displayframe的框架中。
    当使用Screen()命令时,不加参数或参数1,则窗口还是和原来一样。displayframe组件就是tk组件(即窗口组件)。
    当使用Screen(2)时，新建的窗口会分为左右两大区，名称分别为leftframe和rightframe框架区。displayframe在leftframe区上面。
    当使用Screen(3)时，新建的窗口会分为上下两大区，名称分别为topframe和bottomframe区。displayframe在topframe区的左边。
@@ -176,15 +177,15 @@
    原因是绑定盒命令得到的是先前没有刷新的角色的坐标，这样获取的不是最新坐标，当然会导致程序出意外。
    4. 屏幕的update命令会重新渲染所有的角色，如果角色较多，反而会让程序运行更慢。
    5. 本模块给RawTurtle类增加了update方法，这样能单独渲染一个角色。本模块已经把屏幕的自动绘画延时设为0及速度也设为最快了。
    6. 其实Turtle模块可以支持png图片,但要像以下这样写:
    screen.addshape('scratch.png',Shape("image", screen._image('scratch.png')))
 """
 __author__ = 'lixingqiu'
-__date__ = '2023/5/3'
+__date__ = '2023/5/29'
 __blog__ = 'www.lixingqiu.com'
 
 import os
 import re
 import sys
 import math
 import glob
@@ -198,15 +199,15 @@
 from copy import deepcopy
 from tkinter import filedialog
 from tkinter import colorchooser
 from winsound import PlaySound,SND_ASYNC,SND_LOOP,SND_PURGE
 from PIL import ImageTk,ImageOps,Image,ImageGrab,ImageDraw,ImageFont,ImagePath,ImageColor
 from turtle import TK,_Root,ScrolledCanvas,_CFG ,TNavigator,Tbuffer,TPen,_Screen,Screen,Turtle,Vec2D, RawTurtle,TurtleScreenBase,Shape,TurtleScreen,_TurtleImage,TurtleGraphicsError 
 
-_VERSION = 1.69 # 增加foold_fill洪水填充函数,rotate_points单独函数， 增加了InputBox类和屏幕的inputbox方法及更多的内置造型图
+_VERSION = 1.70 
 _CFG['delay'] = 0
 # 定义资源文件夹
 _resfld = os.path.join(os.getcwd(),'res')
 if not os.path.exists(_resfld):os.mkdir(_resfld)
 
 class InputBox:
     def __init__(self,master,title='输入对话框',prompt='请输入字符:'):
@@ -303,15 +304,15 @@
     """
     array = np.array(im)   
     a =  array[:,:,3:]        # 提取透明通道所有值
     a = np.where(a>0,alpha,0) # 如果透明度大于0,则设为alpha,否则为0    
     array[:,:,3:] = a         # 把array的透明度全部改为a
     return Image.fromarray(array)
 
-# 重定义Tpen类的_reset方法,让精灵实例化时不落笔
+# 重定义Tpen类的_reset方法,让角色实例化时不落笔
 def TPen_reset(self, pencolor=_CFG["pencolor"],
                  fillcolor=_CFG["fillcolor"]):
     self._pensize = 1
     self._shown = False
     self._pencolor = pencolor
     self._fillcolor = fillcolor
     self._drawing = False
@@ -1576,15 +1577,15 @@
         y2 = y + A * (b-y)/d
         x3 = x2 - h * (b - y) / d
         y3 = y2 + h * (a - x) / d
         x4 = x2 + h * (b - y) / d
         y4 = y2 - h * (a - x) / d
         return [(x3,y3),(x4,y4)]
     
-def intersection_bak(item1,item2,combmode=0):   
+def __intersection_bak(item1,item2,combmode=0):   #  不要用这个函数，已废 
     """两个对象相交，仅支持点，直线，线段与圆
        item1与item2可表示：点，直线、线段、圆。
        本函数严格区分点，线段，直线的表示方法，我们默认以下规则：
        1.用二元组表示一个点，如(0,0)表示原点
        2.用在列表中的两个点表示线段，如[(0,0),(10,10)]表示从原点到(10,10)的线段。
        3.用在元组中的两个点表示经过两点的直线，如((0,0),(10,10))表示经过这两个点的直线。
        4.用点和半径表示圆，并用中括号括起来，如[(0,0),100]
@@ -2616,15 +2617,14 @@
             else:
                 cv.itemconfig(im,image='')
                 cv.delete(im)
     next_picture()
     
 effect = explode                   # 给爆炸效果函数名定义别名
 
-
 def _findframes(foldername):
     """本函数返回文件夹下面序列帧图,要求这些图片的文件名形式为
        0.png,1.png,2.png,3.png......
        返回所有图片列表。
     """
     exts = ['.png','.gif','.jpg','.jpeg']    
     for ext in exts:
@@ -2634,16 +2634,17 @@
         for index in range(len(files)):
             file = foldername + os.sep + str(index) + ext
             if os.path.exists(file):
                 frames.append(file)
 
         if frames!=[]:break
     return frames
+# 共154个从颜色单词到hex颜色映射
+tkcolors = {'lightpink': '#FFB6C1','light pink': '#FFB6C1', 'pink': '#FFC0CB', 'crimson': '#DC143C', 'lavenderblush': '#FFF0F5', 'palevioletred': '#DB7093', 'hotpink': '#FF69B4', 'deeppink': '#FF1493', 'mediumvioletred': '#C71585', 'orchid': '#DA70D6', 'thistle': '#D8BFD8', 'plum': '#DDA0DD', 'violet': '#EE82EE', 'magenta': '#FF00FF', 'fuchsia': '#FF00FF', 'darkmagenta': '#8B008B', 'purple': '#800080', 'mediumorchid': '#BA55D3', 'darkviolet': '#9400D3', 'darkorchid': '#9932CC', 'indigo': '#4B0082', 'blueviolet': '#8A2BE2', 'mediumpurple': '#9370DB', 'mediumslateblue': '#7B68EE', 'slateblue': '#6A5ACD', 'darkslateblue': '#483D8B', 'lavender': '#E6E6FA', 'ghostwhite': '#F8F8FF', 'blue': '#0000FF', 'mediumblue': '#0000CD', 'midnightblue': '#191970', 'darkblue': '#00008B', 'navy': '#000080', 'royalblue': '#4169E1', 'cornflowerblue': '#6495ED', 'lightsteelblue': '#B0C4DE', 'light steelblue': '#B0C4DE', 'lightslategray': '#778899',  'light slategray': '#778899','slategray': '#708090', 'dodgerblue': '#1E90FF', 'aliceblue': '#F0F8FF', 'steelblue': '#4682B4', 'lightskyblue': '#87CEFA', 'light skyblue': '#87CEFA','skyblue': '#87CEEB', 'deepskyblue': '#00BFFF', 'lightblue': '#ADD8E6', 'light blue': '#ADD8E6', 'powderblue': '#B0E0E6', 'cadetblue': '#5F9EA0', 'azure': '#F0FFFF', 'lightcyan': '#E0FFFF',  'light cyan': '#E0FFFF', 'paleturquoise': '#AFEEEE', 'cyan': '#00FFFF', 'aqua': '#00FFFF', 'darkturquoise': '#00CED1', 'darkslategray': '#2F4F4F', 'darkcyan': '#008B8B', 'teal': '#008080', 'mediumturquoise': '#48D1CC', 'lightseagreen': '#20B2AA', 'light seagreen': '#20B2AA', 'turquoise': '#40E0D0', 'aquamarine': '#7FFFD4', 'mediumaquamarine': '#66CDAA', 'mediumspringgreen': '#00FA9A', 'mintcream': '#F5FFFA', 'springgreen': '#00FF7F', 'mediumseagreen': '#3CB371', 'seagreen': '#2E8B57', 'honeydew': '#F0FFF0', 'lightgreen': '#90EE90', 'light green': '#90EE90', 'palegreen': '#98FB98', 'darkseagreen': '#8FBC8F', 'limegreen': '#32CD32', 'lime': '#00FF00', 'forestgreen': '#228B22', 'green': '#008000', 'darkgreen': '#006400', 'chartreuse': '#7FFF00', 'lawngreen': '#7CFC00', 'greenyellow': '#ADFF2F', 'darkolivegreen': '#556B2F', 'yellowgreen': '#9ACD32', 'olivedrab': '#6B8E23', 'beige': '#F5F5DC', 'lightgoldenrodyellow': '#FAFAD2', 'light goldenrodyellow': '#FAFAD2', 'ivory': '#FFFFF0', 'lightyellow': '#FFFFE0', 'light yellow': '#FFFFE0', 'yellow': '#FFFF00', 'olive': '#808000', 'darkkhaki': '#BDB76B', 'lemonchiffon': '#FFFACD', 'palegoldenrod': '#EEE8AA', 'khaki': '#F0E68C', 'gold': '#FFD700', 'cornsilk': '#FFF8DC', 'goldenrod': '#DAA520', 'darkgoldenrod': '#B8860B', 'floralwhite': '#FFFAF0', 'oldlace': '#FDF5E6', 'wheat': '#F5DEB3', 'moccasin': '#FFE4B5', 'orange': '#FFA500', 'papayawhip': '#FFEFD5', 'blanchedalmond': '#FFEBCD', 'navajowhite': '#FFDEAD', 'antiquewhite': '#FAEBD7', 'tan': '#D2B48C', 'burlywood': '#DEB887', 'bisque': '#FFE4C4', 'darkorange': '#FF8C00', 'linen': '#FAF0E6', 'peru': '#CD853F', 'peachpuff': '#FFDAB9', 'sandybrown': '#F4A460', 'chocolate': '#D2691E', 'saddlebrown': '#8B4513', 'seashell': '#FFF5EE', 'sienna': '#A0522D', 'lightsalmon': '#FFA07A', 'light salmon': '#FFA07A', 'coral': '#FF7F50', 'orangered': '#FF4500', 'darksalmon': '#E9967A', 'tomato': '#FF6347', 'mistyrose': '#FFE4E1', 'salmon': '#FA8072', 'snow': '#FFFAFA', 'lightcoral': '#F08080', 'light coral': '#F08080', 'rosybrown': '#BC8F8F', 'indianred': '#CD5C5C', 'red': '#FF0000', 'brown': '#A52A2A', 'firebrick': '#B22222', 'darkred': '#8B0000', 'maroon': '#800000', 'white': '#FFFFFF', 'whitesmoke': '#F5F5F5', 'gainsboro': '#DCDCDC', 'lightgrey': '#D3D3D3', 'light grey': '#D3D3D3','light gray': '#D3D3D3','silver': '#C0C0C0', 'darkgray': '#A9A9A9', 'gray': '#808080', 'dimgray': '#696969', 'black': '#000000'}
 
-tkcolors = {'lightpink': '#FFB6C1', 'pink': '#FFC0CB', 'crimson': '#DC143C', 'lavenderblush': '#FFF0F5', 'palevioletred': '#DB7093', 'hotpink': '#FF69B4', 'deeppink': '#FF1493', 'mediumvioletred': '#C71585', 'orchid': '#DA70D6', 'thistle': '#D8BFD8', 'plum': '#DDA0DD', 'violet': '#EE82EE', 'magenta': '#FF00FF', 'fuchsia': '#FF00FF', 'darkmagenta': '#8B008B', 'purple': '#800080', 'mediumorchid': '#BA55D3', 'darkviolet': '#9400D3', 'darkorchid': '#9932CC', 'indigo': '#4B0082', 'blueviolet': '#8A2BE2', 'mediumpurple': '#9370DB', 'mediumslateblue': '#7B68EE', 'slateblue': '#6A5ACD', 'darkslateblue': '#483D8B', 'lavender': '#E6E6FA', 'ghostwhite': '#F8F8FF', 'blue': '#0000FF', 'mediumblue': '#0000CD', 'midnightblue': '#191970', 'darkblue': '#00008B', 'navy': '#000080', 'royalblue': '#4169E1', 'cornflowerblue': '#6495ED', 'lightsteelblue': '#B0C4DE', 'lightslategray': '#778899', 'slategray': '#708090', 'dodgerblue': '#1E90FF', 'aliceblue': '#F0F8FF', 'steelblue': '#4682B4', 'lightskyblue': '#87CEFA', 'skyblue': '#87CEEB', 'deepskyblue': '#00BFFF', 'lightblue': '#ADD8E6', 'powderblue': '#B0E0E6', 'cadetblue': '#5F9EA0', 'azure': '#F0FFFF', 'lightcyan': '#E0FFFF', 'paleturquoise': '#AFEEEE', 'cyan': '#00FFFF', 'aqua': '#00FFFF', 'darkturquoise': '#00CED1', 'darkslategray': '#2F4F4F', 'darkcyan': '#008B8B', 'teal': '#008080', 'mediumturquoise': '#48D1CC', 'lightseagreen': '#20B2AA', 'turquoise': '#40E0D0', 'aquamarine': '#7FFFD4', 'mediumaquamarine': '#66CDAA', 'mediumspringgreen': '#00FA9A', 'mintcream': '#F5FFFA', 'springgreen': '#00FF7F', 'mediumseagreen': '#3CB371', 'seagreen': '#2E8B57', 'honeydew': '#F0FFF0', 'lightgreen': '#90EE90', 'palegreen': '#98FB98', 'darkseagreen': '#8FBC8F', 'limegreen': '#32CD32', 'lime': '#00FF00', 'forestgreen': '#228B22', 'green': '#008000', 'darkgreen': '#006400', 'chartreuse': '#7FFF00', 'lawngreen': '#7CFC00', 'greenyellow': '#ADFF2F', 'darkolivegreen': '#556B2F', 'yellowgreen': '#9ACD32', 'olivedrab': '#6B8E23', 'beige': '#F5F5DC', 'lightgoldenrodyellow': '#FAFAD2', 'ivory': '#FFFFF0', 'lightyellow': '#FFFFE0', 'yellow': '#FFFF00', 'olive': '#808000', 'darkkhaki': '#BDB76B', 'lemonchiffon': '#FFFACD', 'palegoldenrod': '#EEE8AA', 'khaki': '#F0E68C', 'gold': '#FFD700', 'cornsilk': '#FFF8DC', 'goldenrod': '#DAA520', 'darkgoldenrod': '#B8860B', 'floralwhite': '#FFFAF0', 'oldlace': '#FDF5E6', 'wheat': '#F5DEB3', 'moccasin': '#FFE4B5', 'orange': '#FFA500', 'papayawhip': '#FFEFD5', 'blanchedalmond': '#FFEBCD', 'navajowhite': '#FFDEAD', 'antiquewhite': '#FAEBD7', 'tan': '#D2B48C', 'burlywood': '#DEB887', 'bisque': '#FFE4C4', 'darkorange': '#FF8C00', 'linen': '#FAF0E6', 'peru': '#CD853F', 'peachpuff': '#FFDAB9', 'sandybrown': '#F4A460', 'chocolate': '#D2691E', 'saddlebrown': '#8B4513', 'seashell': '#FFF5EE', 'sienna': '#A0522D', 'lightsalmon': '#FFA07A', 'coral': '#FF7F50', 'orangered': '#FF4500', 'darksalmon': '#E9967A', 'tomato': '#FF6347', 'mistyrose': '#FFE4E1', 'salmon': '#FA8072', 'snow': '#FFFAFA', 'lightcoral': '#F08080', 'rosybrown': '#BC8F8F', 'indianred': '#CD5C5C', 'red': '#FF0000', 'brown': '#A52A2A', 'firebrick': '#B22222', 'darkred': '#8B0000', 'maroon': '#800000', 'white': '#FFFFFF', 'whitesmoke': '#F5F5F5', 'gainsboro': '#DCDCDC', 'lightgrey': '#D3D3D3', 'silver': '#C0C0C0', 'darkgray': '#A9A9A9', 'gray': '#808080', 'dimgray': '#696969', 'black': '#000000'}
 def convert_colorRGBA255(fillcolor):  # 把'red','#FF0000',(0.8,0.5,0.2)这样的转换成RGBA255形式,如'red' 转为 (255,0,0,255)
     screen = Screen()
     if screen._iscolorstring(fillcolor):     # 如果是合法的颜色字符串,则转换成RGBA255
         if not fillcolor.startswith('#'):         # 如果不是以#开头的
             fillcolor = tkcolors[fillcolor.lower()]  # 转换成以#开头的,通过查tkcolors字典
         fillcolor = ImageColor.getcolor(fillcolor, "RGB")
     else:                                        # 否则认为传入的是三元组
@@ -2662,16 +2663,15 @@
     height = screen.window_height()
     pos = pos[0],-pos[1]
     heading = [(1,0),(0,1),(-1,0),(0,-1)]  # 右下左上 4个方向   
     stack = [pos] # stack保存坐标
     cors = {}
     cors[pos] = 1
     counter = 0
-    while stack:
-        begin = time.time()
+    while stack:       
         x,y  = stack.pop()
         i = 0        
         while i < 4:
             counter += 1
             next_x = x + heading[i][0]
             next_y = y + heading[i][1]                 
             if (next_x ,next_y) in cors :
@@ -2683,16 +2683,15 @@
             if items or abs(next_x)>width/2 or abs(next_y)>height/2: # 如果发现了此点是边界                     
                  cors[(next_x,next_y)] = 2   # 轮廓点
                  i = i + 1                     
             else:
                  stack.append((next_x,next_y))
                  cors[(next_x,next_y)] = 1   #  图形内的点
                  x = next_x
-                 y = next_y       
-    #print('dfs函数运行所花时间:',time.time() - start_time,'执行次数:',counter)    
+                 y = next_y     
     return cors
     
 class Pointer:
     """用于辅助的Pointer类,它能像海龟一样移动,可以认为是无画笔的极简版海龟"""
     def __init__(self,pos=(0,0),angle=0):
         """
            初始化方法，pos:坐标,angle:角度
@@ -3045,19 +3044,17 @@
                  if  pixel2 == color:
                     collideflag = True
                     break
               if collideflag == True: break
         return collideflag
                 
     def _store(self,x,y):
-        self.clickpos = Vec2D(x,y)  # 单击点坐标       
-
-    
-    def ondraghook(self,x,y):
-        pass
+        self.clickpos = Vec2D(x,y)  # 单击点坐标
+        
+    def ondraghook(self,x,y):pass
     
     def drag(self,x,y):
         """拖动自己到鼠标指针的坐标"""
         self.ondrag(None)
         neu = Vec2D(x,y)
         self.drag_last_xy = self.pos()   # 角色上一次移动时的x,y坐标
         self.goto(self.pos() + (neu-self.clickpos))
@@ -4671,37 +4668,35 @@
 
     # 下面是为fill命令设计的几个方法
     def find_contours(self,pos,exclude=set()):  
         """从一个点开始查找轮廓，一定要是封闭区域。
            由于find_overlapping在canvas中的查找是以y轴向下为正,所以y值要取反。
            pos：列表或者元组表示的二维点坐标，如(10,20)
            exclude：查找重叠时要排除的item集。
-           这是一个测试版本。深度优先搜索算法,floodfill方法.
         """    
         cors = dfs(pos,exclude=exclude)  # 返回封装图形内所有点,包括边界点
         contours = [ (k[0],-k[1]) for k,v in cors.items() if v==2 ] # 边界点即轮廓点
         #print('边界点数量=',len(contours))
-        inners = [ (k[0],-k[1]) for k,v in cors.items() if v==1 ]
+        inners = [ (k[0],-k[1]) for k,v in cors.items() if v==1 ]  # 值是1则是内部点
         return contours,inners        # 返回边界点和内部点,
         # 下面代码准备作废
         # 需要对points里的点进行优化,如:同一线段上的点只要取两个端点即可,中间点要删除
         # 以下处理方法是查找折线的拐点,然后只保留points的第一个点,拐点集和points的最后一个点.
         knee_points = inflection_points(inners)      # 拐点集     
         knee_points.insert(0,inners[0])
         knee_points.append(inners[-1])
-        print(len(points),len(knee_points))
-        return inners
-        return knee_points
+        #print(len(points),len(knee_points))
+        return inners,knee_points
     
     def godot(self,x,y,diameter,fc):   #  去打点
         self.goto(x,y)        
         self.dot(diameter,fc)
         self.screen.update()
         
-    def fill_concave(self,x,y):
+    def fill_concave(self,x,y):        # fill命令模式为1调用的方法
         """以start为起点,查找封闭图形并进行填充,本函数是测试版本，
            请不要让start在封闭图形外,否则填充时间长导致无响应,并会出现意外!
            这是填充凹多边形版本,速度较慢。
         """
         fc = self.fillcolor()         # 填充颜色
         if isinstance(fc,tuple) and self.screen.colormode()==255:
             fc = int(fc[0]),int(fc[1]),int(fc[2])
@@ -4712,15 +4707,15 @@
         isd = self.isdown()            # 记录当前是否落笔的状态    
         self.penup()                   # 不管当前是否有无落笔,都要抬笔         
         [self.godot(x,y,1,fc) for x,y in contours+innters ]  # 用打点填充内部,速度慢        
         screen.tracer(tr,0)
         if isd:self.pendown()           # 如果填充前是落笔状态,则恢复
         return contours , innters
 
-    def fill_convex(self,x,y):
+    def fill_convex(self,x,y):        # fill命令模式为0调用的方法 
         """以start为起点,查找封闭图形并进行填充,本函数是测试版本，
            请不要让start在封闭图形外,否则填充时间长导致无响应,并会出现意外!
            这是填充凸多边形版本,速度稍快。        """
         fc = self.fillcolor()         # 填充颜色
         if isinstance(fc,tuple) and self.screen.colormode()==255:
             fc = int(fc[0]),int(fc[1]),int(fc[2])
         start = x,y
@@ -4737,15 +4732,15 @@
         self.goto(points[0]) 
         self.end_fill()
         screen.update()        
         screen.tracer(tr,0)
         if isd:self.pendown()           # 如果填充前是落笔状态,则恢复
         return  points,tuple()
         
-    def flood_fill(self,x,y): # 洪水填充函数
+    def flood_fill(self,x,y): # fill模式为2调用的方法
         """漫水填充方法要调用find_contours,cors2image与fill_area方法"""        
         start = x,y
         screen = self.getscreen()
         tr = screen.tracer()
         screen.tracer(0,0)
         # exds是要排除的item列表,(在用find_contour查找轮廓时要排除一些item
         pop = self._draw_bubble_turtle
@@ -4762,15 +4757,15 @@
         screen.tracer(tr,0)
         return contours,innters
           
     def fill(self,x,y,mode=2):
         """Sprite类的填充函数，x,y则是封闭图形内的一个点。
            mode:值为0,1,2，值为0时调用凸版，即fill_convex函数，适合于画的图形为凸多边形。
            值为1则调用凹版，即fill_concave函数，适合于任何封装图形，速度较慢，请耐心等待。
-           值为3时调用 flood_fill即洪水填充方法。"""            
+           值为3时调用 flood_fill即洪水填充方法，速度还行,注意不要在封闭图形外面填充,会导致无响应。"""            
         if mode==0:
             contours,innters = self.fill_convex(x,y)     # 凸
         elif mode==1:           
             contours,innters = self.fill_concave(x,y)    # 凹
         else:           
             contours,innters = self.flood_fill(x,y)      # 洪水填充
         return contours,innters
@@ -4809,14 +4804,15 @@
 # 定义类的别名
 Js  = Sprite
 Juese = Sprite
 角色 = Sprite
 精灵 = Sprite
 
 def fill(x,y,fillcolor='black',mode=2):  # 单独的填充命令,方便配合turtle模块使用
+    """单独的填充命令，为了让turtle能使用sprites中的fill，所以编写这个函数。它会建一个隐藏的角色用于fill"""
     if Turtle._screen is None:return    
     screen = Screen()            # 返回屏幕对象
     if not hasattr(screen,'_fill_sprite'):  # 第一次没这个属性,则建立专用于填充的角色
         screen._fill_sprite =  Sprite('blank',visible=False)
     screen._fill_sprite.fillcolor(fillcolor)
     contours,innters = screen._fill_sprite.fill(x,y,mode=mode)
     return contours,innters
@@ -5040,105 +5036,59 @@
        widget = TK.{0}(**kw)  # 说明用户自己写了master参数
     
     return widget
 """
 for wd,value in some_widgets.items():
     fc = widgets_function.format(wd,value)
     exec(fc)
-
     
 #print("Successful import sprites V" + str(_VERSION) + ",email:406273900@qq.com")
 
 if __name__ == "__main__":  
 
+    import turtle
     
-    def cangoto(i,j):
-        """返回是否能到达i,j位置"""
-        if i<rows and j<cols:
-            if maze[i][j]==0:
-                return True
-        return False
-
-    maze=[[1,1,1,1,1,1,1,1,1,1,1,1,1,1],
-          [1,0,0,0,1,1,0,0,0,1,0,0,0,1],
-          [1,0,1,0,0,0,0,1,0,1,0,1,0,1],
-          [1,0,1,0,1,1,1,1,0,1,0,1,0,1],
-          [1,0,1,0,0,0,0,0,0,1,1,1,0,1],
-          [1,0,1,1,1,1,1,1,1,1,0,0,0,1],
-          [1,0,1,0,0,0,0,0,0,0,0,1,0,1],
-          [1,0,0,0,1,1,1,0,1,0,1,1,0,1],
-          [1,0,1,0,1,0,1,0,1,0,1,0,0,1],
-          [1,0,1,0,1,0,1,0,1,1,1,1,0,1],
-          [1,0,1,0,0,0,1,0,0,1,0,0,0,1],
-          [1,1,1,1,1,1,1,1,1,1,1,1,1,1]]
-
-    cols = 14                           # 列数
-    rows = 12                           # 行数  
-
-    screen = Screen()
-    #screen.hide()
-    screen.tracer(0,0)
-    screen.setup(800,600)
-    screen.bgcolor('light cyan')
-    cat = Sprite(2)
-    cat.fd(100)
-    ball = Sprite(1)
-    ball.bk(200) 
-    ret = screen.inputbox('请输入','一些字符')
-    
-    bug = Sprite(shape='square')        # 新建方形对象
-    bug.shapesize(2.5)
-    cors = bug.draw_grid2(rows,cols)    # 画rows行,cols列,宽高各50的格子
-    bug.clear()                         # 清除所有格子
-    # 格子标为1的印上黑色正方形
-    for r in range(rows):
-        for c in range(cols):
-            if maze[r][c]==1:           # 如果这个位置是1 
-                bug.goto(cors[r][c])    # bug到达这个位置的坐标
-                bug.stamp()             # 印黑正方形
-    bug.shape('res/bug.png')            # bug 修改造型 
-    bug.scale(1)                        # 修正比例
-    bug.goto(cors[1][1])                # 到达起始点
-    bug.dest= False                     # 自定义属性
-    screen.update()
-    def walk_maze(r,c,endr,endc):       # 递归函数(深度搜索)  
-        """r,c:起点,endr,endc:终点"""
-        # 寻找所有可用的方向
-        for i,j in dirs:
-            if cangoto(r+i,c+j):        # 如果前面这一格是空
-                r += i
-                c += j
-                if bug.dest == False:   # 如果没到达目的地
-                   bug.goto(cors[r][c]);bug.wait(0.2)
-                maze[r][c] = 1
-                stack.append((r,c))                
-                if r==endr and c==endc: # 如果到达目的地了
-                    bug.dest = True                     
-                else:walk_maze(r,c,endr,endc)
-        else:       
-           if stack:
-               r,c = stack.pop()
-               if bug.dest == False:   # 如果没到达目的地
-                   bug.goto(cors[r][c]);bug.wait(0.2)
-               walk_maze(r,c,endr,endc)
-
-    r,c = 1,1                          # 起点
-    endr,endc = 10,12                  # 终点
-    txt2image('起','res/起点.png')     # 文字转图
-    txt2image('终','res/终点.png')     # 文字转图
-    dummy = Sprite(visible=False)
-    dummy.shape('res/起点.png')
-    dummy.goto(cors[r][c])
-    dummy.stamp()
-    dummy.shape('res/终点.png')
-    dummy.goto(cors[endr][endc])
-    dummy.stamp()
-    
-    stack = []
-    dirs = [(1,0),(0,1),(-1,0),(0,-1)]  # 4个方向
-    stack.append((r,c))                 # 起点添加到stack中
-    walk_maze(r,c,endr,endc)
-
-    screen.mainloop()
-
- 
+    ysb = ['red','orange','yellow','green','cyan',
+           'blue','purple','pink','brown','lime']
+    screen = turtle.Screen()    
+    screen.xy_grid()
+    screen.setup(480,720)
+    turtle.shape('blank')
+    turtle.hideturtle()
+    turtle.goto(0,100)
+    turtle.pd()
+    turtle.pensize(2)
+    turtle.circle(100)    
+    turtle.penup()
+    fill(50,150,mode=0)      # 在（50，150）坐标开始填充，模式为2
+    fill(-50,150,fillcolor='red',mode=2)      # 在（50，150）坐标开始填充，模式为2
+    fill(50,250,fillcolor='blue',mode=2)      # 在（50，150）坐标开始填充，模式为2
+    fill(-50,250,fillcolor='green',mode=2)      # 在（50，150）坐标开始填充，模式为2
+    ft = ('黑体',14,'normal')
+    s = '请画封闭图形，然后单击右键填充'
+    turtle.home();turtle.write(s,align='center',font=ft)
+    
+    spacekey = Key('space')           # 实例化空格键
+    leftkey = Mouse()                 # 实例化鼠标左键
+    rightkey = Mouse(3)               # 实例化鼠标右键
+    turtle.ht()                       # 隐藏海龟
+    turtle.pensize(4)
+    turtle.pencolor('red')
+    screen.listen()                   # 监听按键检测
+    screen.colormode(255)
+    while True:
+        turtle.goto(mouse_pos())
+        if spacekey.isdownup():         # 如果按空格键,更换画笔颜色
+            turtle.pencolor(random.choice(ysb))
+        if leftkey.down():              # 如果单击左键,则落笔 
+            turtle.pendown()
+        else:
+            turtle.penup()              # 否则抬笔
+        if rightkey.isdownup():         # 如果单击右键并松开,则填充
+            fx,fy = rightkey.pos
+            r  = random.randint(0,255)
+            g  = random.randint(0,255)
+            b  = random.randint(0,255)
+            fill(fx,fy,fillcolor=(r,g,b),mode=2) # 默认模式为2,共有0,1,2共有3种模式,请自行尝试
+            
+        screen.update()
```

### Comparing `sprites-1.69/sprites.egg-info/PKG-INFO` & `sprites-1.70/sprites.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprites
-Version: 1.69
+Version: 1.70
 Summary: Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com
 Home-page: http://www.lixingqiu.com
 Author: lixingqiu
 Author-email: 406273900@qq.com
 License: MIT
 Description: ﻿# Python sprites module introduce
         
@@ -16,15 +16,15 @@
         ## Main application scenarios:
         1、Introduction to children's computer games and animation development.
         2、learn the ABC of Python game development.
         3、Python game crash.
         4、Getting started with Python for training institutions.
         5、Python experience courses and public welfare courses of training institutions.
         
-         
         
         more example,please conatct lixingqiu, wechat:scratch8,website:<http://www.lixingqiu.com>
         
         sprites module Developer: Li Xingqiu，email:406273900@qq.com,Pingxiang, Jiangxi, China.
+         
 Keywords: creative game pygame turtle animation sprite geometry math Elementary Mathematics Teaching
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

