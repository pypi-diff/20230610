# Comparing `tmp/tkintertools-dev-2.6.3.tar.gz` & `tmp/tkintertools-dev-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-dev-2.6.3.tar", last modified: Mon Jun  5 17:10:00 2023, max compression
+gzip compressed data, was "tkintertools-dev-2.6.4.tar", last modified: Sat Jun 10 16:31:18 2023, max compression
```

## Comparing `tkintertools-dev-2.6.3.tar` & `tkintertools-dev-2.6.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:10:00.511235 tkintertools-dev-2.6.3/
--rw-rw-rw-   0        0        0     7548 2023-05-27 20:59:02.000000 tkintertools-dev-2.6.3/LICENSE
--rw-rw-rw-   0        0        0    28175 2023-06-05 17:10:00.509223 tkintertools-dev-2.6.3/PKG-INFO
--rw-rw-rw-   0        0        0    27670 2023-06-05 16:18:37.000000 tkintertools-dev-2.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 17:10:00.512236 tkintertools-dev-2.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-05-30 16:20:05.000000 tkintertools-dev-2.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:10:00.498001 tkintertools-dev-2.6.3/tkintertools/
--rw-rw-rw-   0        0        0     2922 2023-06-05 17:07:12.000000 tkintertools-dev-2.6.3/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    60866 2023-06-05 13:14:52.000000 tkintertools-dev-2.6.3/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     2136 2023-06-05 17:00:41.000000 tkintertools-dev-2.6.3/tkintertools/constants.py
--rw-rw-rw-   0        0        0    14759 2023-06-05 13:09:11.000000 tkintertools-dev-2.6.3/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:10:00.505011 tkintertools-dev-2.6.3/tkintertools_dev.egg-info/
--rw-rw-rw-   0        0        0    28175 2023-06-05 17:10:00.000000 tkintertools-dev-2.6.3/tkintertools_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-05 17:10:00.000000 tkintertools-dev-2.6.3/tkintertools_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:10:00.000000 tkintertools-dev-2.6.3/tkintertools_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 17:10:00.000000 tkintertools-dev-2.6.3/tkintertools_dev.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 16:31:18.703807 tkintertools-dev-2.6.4/
+-rw-rw-rw-   0        0        0     7548 2023-05-27 20:59:02.000000 tkintertools-dev-2.6.4/LICENSE
+-rw-rw-rw-   0        0        0    28017 2023-06-10 16:31:18.701772 tkintertools-dev-2.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0    27512 2023-06-10 16:21:28.000000 tkintertools-dev-2.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-10 16:31:18.704774 tkintertools-dev-2.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-06-10 06:50:22.000000 tkintertools-dev-2.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:31:18.690328 tkintertools-dev-2.6.4/tkintertools/
+-rw-rw-rw-   0        0        0     2352 2023-06-10 12:13:26.000000 tkintertools-dev-2.6.4/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    62557 2023-06-10 12:15:00.000000 tkintertools-dev-2.6.4/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     2066 2023-06-10 13:59:58.000000 tkintertools-dev-2.6.4/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    18105 2023-06-10 15:12:51.000000 tkintertools-dev-2.6.4/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:31:18.700770 tkintertools-dev-2.6.4/tkintertools_dev.egg-info/
+-rw-rw-rw-   0        0        0    28017 2023-06-10 16:31:18.000000 tkintertools-dev-2.6.4/tkintertools_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-10 16:31:18.000000 tkintertools-dev-2.6.4/tkintertools_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 16:31:18.000000 tkintertools-dev-2.6.4/tkintertools_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-10 16:31:18.000000 tkintertools-dev-2.6.4/tkintertools_dev.egg-info/top_level.txt
```

### Comparing `tkintertools-dev-2.6.3/LICENSE` & `tkintertools-dev-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tkintertools-dev-2.6.3/PKG-INFO` & `tkintertools-dev-2.6.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: tkintertools-dev
-Version: 2.6.3
+Version: 2.6.4
 Summary: An auxiliary module of the tkinder module
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
-        src="./tkintertools.png" />
+        src="tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
-        <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
+        <a href="tkintertools/__init__.py">
+            <img src="https://img.shields.io/badge/Version-2.6.4(dev)-blue" alt="latest version" />
         </a>
-        <a href="./LICENSE">
+        <a href="LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
-        <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/06/06-orange" alt="ChangeLog" />
+        <a href="CHANGELOG.md">
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/11-orange" alt="ChangeLog" />
         </a>
-        <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
+        <a href="TODO.md">
+            <img src="https://img.shields.io/badge/ToDos-14-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
+            <img src="https://img.shields.io/badge/Downloads-4k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
@@ -46,152 +46,144 @@
         <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
     </p>
 </div>
 
 Installation/模块安装
------------------------
+--------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/30
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/07
 
 ```
-pip install tkintertools==2.6.2
-```
+pip install tkintertools==2.6.3
 或者
-```
 pip install tkintertools
 ```
 
-这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
-稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
+这个是目前的最新稳定版，比较稳定，bug （可能）没有那么多，推荐使用这个。  
+关于稳定版有 Issue 的话，我会去查看并尝试解决 Issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.3
-* Release Date/发布日期 : 2023/06/06
+* Version/版本 : 2.6.4
+* Release Date/发布日期 : 2023/06/11
 
 ```
-pip install tkintertools-dev==2.6.3
+pip install tkintertools-dev==2.6.4
+或者
+pip install tkintertools-dev
 ```
 
-这个是我正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
-开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
-
-News/最新功能
-------------
-
-最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
-同时修复一些bug，优化了一部分代码，提升了一部分性能。
+这个是我正在开发的版本，可能有新功能，bug 也可能会比较多，但也可能会比原来的版本更加稳定。  
+大家可以在 Issue 中提出一些建议，我会适当采纳一些并在开发版本中更改或实现。
 
-通过以下代码来使用3d绘图功能：
+**特别注意**
+* 开发版仅作示例，各函数或类的API并非最终确定结果，直接使用开发版可能导致后续无法与正式版兼容！
+* 若要使用开发版，请先卸载正式版后再进行pip安装，再次使用正式版时也是一样，先卸载开发版再安装正式版！
+* 需要 **Python3.8** 及更高版本才能运行 tkintertools！
 
-```python
-from tkintertools import tools_3d as t3d
-import tkintertools.tools_3d as t3d
-# 两种引入方式都可以
-```
+<a name="news">News/最新功能</a>
+------------
 
-子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+最新版的 tkintertools **开发版**(2.6.4-dev)新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
 
-目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
-以下是一个使用3d绘图的示例：
+在 Windows 系统下运行下面的示例程序时，其拥有以下功能：
+* 按住鼠标左键拖动可以旋转这多个几何体；
+* 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
+* 按“=”和“-”键分别可以放大和缩小几何体的大小；
+* 滚动鼠标中键可以放大和缩小画面。
 
-在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
-x、y 和 z 轴分别是红色、绿色和蓝色的线。
+下面是示例程序的效果图：
 
-![3d绘图](./docs/images/3d.png)
+![news.png](news.png)
 
 <details><summary><b>源代码</b></summary>
 
 ```python
-import random
-import tkinter
+from tkinter import Event
 
 import tkintertools as tkt
 from tkintertools import tools_3d as t3d
 
-root = tkt.Tk('tools_3d', 1280, 720)
-canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+root = tkt.Tk('tool_3d', 1280, 720)
+cv3d = t3d.Canvas_3D(root, 1280, 720, 0, 0)
 
-geos = []  # type: list[t3d.Geometry]
-origin = t3d.Point(canvas, [0, 0, 0], size=5)  # 原点
-axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'),  # 创建坐标轴
-        t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3, fill='green'),
-        t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
-
-for _ in range(8):
-    # 创建正方体
-    cube = t3d.Cuboid(
-        canvas, *random.sample(range(-200, 200), 3), *random.sample(range(50, 100), 3))
-    geos.append(cube)
-    # 创建四面体
-    x, y, z = random.sample(range(-200, 200), 3)
-    tetr = t3d.Tetrahedron(
-        canvas, *[[x+random.randint(-100, 100), y+random.randint(-100, 100), z+random.randint(-100, 100)] for _ in range(4)])
-    geos.append(tetr)
+origin = t3d.Point(cv3d, [0, 0, 0])  # 原点
+k = -100, 0, 100
+geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white', color_down='yellow', color_left='red',
+                   color_right='orange', color_front='blue', color_back='green') for a in k for b in k for c in k]
+cv3d.space_sort()
 
 
 def translate(event, flag=False, _cache=[]):
-    # type: (tkinter.Event, bool, list[float]) -> None
+    # type: (Event, bool, list[float]) -> None
     """ 平移事件 """
     if flag:
         _cache[:] = [event.x, event.y]
         return
-    dx = (event.x - _cache[0]) / 6
-    dy = (event.y - _cache[1]) / 6
+    dx = (event.x - _cache[0])
+    dy = (event.y - _cache[1])
     _cache[:] = [event.x, event.y]
-    for axis in axes:
-        axis.translate(0, 6*dx, 6*dy)
-        axis.update()
     for geo in geos:
         geo.translate(0, dx, dy)
         geo.update()
-    origin.translate(0, 6*dx, 6*dy)
+    origin.translate(0, dx, dy)
     origin.update()
+    cv3d.space_sort()
 
 
-def rotate(event, flag=False, _cache=[]):  # type: (tkinter.Event, bool, list[float]) -> None
+def rotate(event, flag=False, _cache=[]):
+    # type: (Event, bool, list[float]) -> None
     """ 旋转事件 """
     if flag:
         _cache[:] = [event.x, event.y]
         return
-    dy = (event.x - _cache[0]) / 200
-    dx = (_cache[1] - event.y) / 200
+    dy = (event.x - _cache[0]) / 100
+    dx = (_cache[1] - event.y) / 100
     _cache[:] = [event.x, event.y]
-    for axis in axes:
-        axis.rotate(0, 6*dx, 6*dy, center=origin.coords)
-        axis.update()
-    for geo in geos:
-        geo.rotate(0, dx, dy, center=origin.coords)
-        geo.update()
+    for item in geos:
+        item.rotate(0, dx, dy, center=origin.coords)
+        item.update()
+    cv3d.space_sort()
 
 
-def scale(event):  # type: (tkinter.Event) -> None
+def scale(event):  # type: (Event) -> None
     """ 缩放事件 """
-    k = 1.01 if event.delta > 0 else 0.99
+    k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1
     for geo in geos:
         geo.scale(k, k, k)
         geo.update()
+    cv3d.space_sort()
+
+
+def scale_center(event):  # type: (Event) -> None
+    """ 中心缩放事件 """
+    k = 1.05 if event.delta > 0 else 0.95
+    for geo in geos:
+        geo.scale(k, k, k, center=origin.coords)
+        geo.update()
+    cv3d.space_sort()
 
 
 root.bind('<Button-1>', lambda event: rotate(event, True))
 root.bind('<B1-Motion>', rotate)
 root.bind('<Button-3>', lambda event: translate(event, True))
 root.bind('<B3-Motion>', translate)
-root.bind('<MouseWheel>', scale)
+root.bind('<Any-Key>', scale)
+root.bind('<MouseWheel>', scale_center)
 root.mainloop()
 ```
 
 </details>
 
-更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+更多更新信息请见：[CHANGELOG.md](CHANGELOG.md)
 
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
@@ -204,30 +196,29 @@
 * 虚拟的控件在文本输入和显示的功能上存在一些缺陷（这个缺陷不是很明显，但强迫症就有点难受了，比如我）
 
 tkintertools 模块还具有一些特色的功能：
 
 * 利用 tkinter 和 tkintertools 创建的程序，在高分辨率的情况下，tkintertools 的会更加清晰（这点对于笔记本用户很友好，比如我）
 * 可以迅速实现渐变色的效果
 * 窗口缩放，所有的控件的大小跟着缩放（当然，也可以设置为不跟随缩放）
-
-注意：需要 **Python3.7** 及更高版本才能运行 tkintertools！
+* 子模块 tools_3d 可以是满足简单的 3D 绘图需求
 
 Provides/模块功能
 -------------------
 
 Here, only the more distinctive features will be listed  
 这里只会列举出比较具有特色的功能
 
 ### Customizable widgets/可自定义的控件
 
 tkintertools 模块的控件拥有许多参数供我们设置，比如圆角的半径、文本和边框以及控件内部的颜色，关联事件等等。  
 这里要说明的是，每个控件可以设置的关联事件不止一种，在鼠标经过控件时可以绑定事件，鼠标点击控件也可以，鼠标点击后松开也行等等。  
 文本和边框以及控件的填充色也是类似的，在鼠标经过控件、点击控件、点击后松开都可以设定颜色。  
 文本类控件还能够从右边逐步输入文本，文本输入提示符也可以不是单调无趣的竖线，可以是其他的，比如下划线等。  
-最后，大家可以看一下 [test.py](./test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
+最后，大家可以看一下 [test.py](test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
 
 ### Automatically control size/自动控制大小
 
 tkintertools 中的控件，其大小和形状可以随着窗口的变化而成比例地变化，不仅仅是控件中的文本，Canvas 绘制的图形也会随之变动，更让人兴奋的是，png 类型的图片也会随之成比例地缩放！当然，你也可以设定参数让其不随之变动，也可以设定参数使其在缩放的时候保持横纵方向的比例。  
 总之，很方便，很舒适！
 
 ### Easily move widgets/轻松移动控件
@@ -243,27 +234,35 @@
 见 [DPI 级别设置函数](#DPI)
 
 ### Detailed type hints/详细的类型提示
 
 参考 [PEP 526](https://peps.python.org/pep-0526/)、[PEP 586](https://peps.python.org/pep-0586/)、[PEP 604](https://peps.python.org/pep-0604/) 和 [PEP 612](https://peps.python.org/pep-0612/)，我采用了最兼容的方式去实现详细的类型提示，可适用 IDE 有 VScode、Pycharm 等。  
 那什么是类型提示呢？话不多说，直接看图就行：
 
-![type_hint.png](docs/images/type_hint_vscode.png)
+![type_hint.png](readme_res/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
-[test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
+[test.py](test.py) 在 Windows 系统（**Windows10**）上运行的界面如下：
+
+![test_windows10.png](readme_res/test_windows10.png)
 
-![test_win32.png](docs/images/test_win32.png)
+[test.py](test.py) 在 Linux 系统（**Ubuntu22.04**）上运行的界面如下：
 
-[test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
+![test_linux.png](readme_res/test_linux.png)
 
-![test_linux.png](docs/images/test_linux.png)
+[test.py](test.py) 在 Windows 系统（**Windows11**）上运行的界面如下(智能控制圆角半径)：
+
+![test_windows11.png](readme_res/test_windows11.png)
+
+### 3D Drawing/3D绘图
+
+见 [News/最新功能](#news)
 
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
@@ -284,15 +283,15 @@
 ### Virtual Canvas Widget/虚拟画布控件
 
 1. `Label`: 标签控件
 
     标签控件的功能和`tkinter.Label`的功能类似，但更加的多元化  
     下面是`Label`控件的外观：  
 
-    ![LabelTest.png](docs/images/LabelTest.png)
+    ![LabelTest.png](readme_res/LabelTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
@@ -319,15 +318,15 @@
     </details>
 
 2. `Button`: 按钮控件
 
     按钮控件相较于`tkinter.Button`，其自由度更高，`tkinter.Button`只有在按下的时候才能触发绑定的关联事件，而`Button`却可以在鼠标移至按钮上方时、鼠标按下时、鼠标松开时都可以绑定关联事件  
     下面是`Button`控件的外观：
 
-    ![ButtonTest.png](docs/images/ButtonTest.png)
+    ![ButtonTest.png](readme_res/ButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
@@ -354,15 +353,15 @@
     </details>
 
 3. `CheckButton`: 复选框控件
 
     复选框控件相对于`tkinter`原生的`tkinter.CheckButton`在使用方面更加地简单，同时颜值也上升了不少  
     下面是`CheckButton`控件的外观：
 
-    ![CheckButtonTest.png](docs/images/CheckButtonTest.png)
+    ![CheckButtonTest.png](readme_res/CheckButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
@@ -390,15 +389,15 @@
     </details>
 
 4. `Entry`: 输入框控件
 
     输入框控件可以轻松地设置输入的文本位置（靠左、居中和靠右），同时，它可以在鼠标移至输入框上方、鼠标未在输入框上方两种状态显示不同的默认文本  
     下面是`Entry`控件的外观：
 
-    ![EntryTest.png](docs/images/EntryTest.png)
+    ![EntryTest.png](readme_res/EntryTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
@@ -436,15 +435,15 @@
     </details>
 
 5. `Text`: 文本框控件
 
     文本框类似于输入框，这里就不再赘述  
     下面是`Text`控件的外观：
 
-    ![TextTest.png](docs/images/TextTest.png)
+    ![TextTest.png](readme_res/TextTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
@@ -472,15 +471,15 @@
     </details>
 
 6. `Progressbar`: 进度条控件
 
     进度条控件相比`tkinter.ttk.Progressbar`，外观上的自由度较大  
     下面是`Progressbar`控件的外观：
 
-    ![ProgressbarTest.png](docs/images/ProgressbarTest.png)
+    ![ProgressbarTest.png](readme_res/ProgressbarTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
@@ -534,15 +533,15 @@
 
 ### Tool Function/工具函数
 
 1. `move`: <a name="move">移动函数</a>
 
     移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！
 
-    ![MoveTest.gif](docs/images/MoveTest.gif)
+    ![MoveTest.gif](readme_res/MoveTest.gif)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
@@ -588,17 +587,17 @@
     `right`  : "        tkintertools"</pre>
 
 3. `color`: <a name="Gradient">颜色函数</a>
 
     颜色函数可以轻松求出一个颜色到另外一个颜色的过渡颜色，因此可以轻松得到渐变色的效果，同时，改变传入的参数还可以得到传入颜色的对比色  
     第二张图是 test.py 在图像测试中绘制的图案
 
-    ![ColorTest.png](docs/images/ColorTest.png)
+    ![ColorTest.png](readme_res/ColorTest.png)
 
-    ![Test_Draw.png](docs/images/Test_Draw.png)
+    ![Test_Draw.png](readme_res/Test_Draw.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
@@ -621,26 +620,26 @@
 
     </details>
 
 4. `askfont`: 字体选择对话框
 
     `askfont`函数可以打开默认的字体选择窗口，这个窗口虽然是默认的，但它实际上无法在`tkinter`中打开，因为`tkinter`并没有对应的 API 能够做到这一点。但是，`tkintertools`调用并封装了原生的 tcl 的命令，使得字体选择框能够被我们使用。
 
-    <p><img width="540px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/font.png" alt="font.png" /></p>
+    ![font.png](readme_res/font.png)
 
 5. `SetProcessDpiAwareness`: <a name="DPI">DPI 级别设置函数</a>
 
     这个函数实际上只是对函数`ctypes.WinDLL('shcore').SetProcessDpiAwareness`的一个简单包装，其值可为 0、1 和 2，分别代表程序 DPI 的不同级别，那么缩放效果也就不同，`tkintertools`选择的值是 1，但程序默认值实际为 0  
     下面是未执行这个函数的效果
     
-    ![SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+    ![SetProcessDpiAwareness_0.png](readme_res/SetProcessDpiAwareness_0.png)
 
     <p>下面是执行了这个函数的效果</p>
 
-    ![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
+    ![SetProcessDpiAwareness_1.png](readme_res/SetProcessDpiAwareness_1.png)
 
     从上面的两张图中可以很明显的看出第一张很模糊，第二张很清晰，这就是 DPI 级别不同的原因，不过这一点在屏幕缩放比不是 100% 的时候才会出现  
     大家对上面的图肯定很熟悉，这不就是 IDLE 吗！？对，这个的问题的解决办法也是来自于 IDLE 的源代码 [pyshell.py line 18~20]  
     注意：该函数在程序的不同位置执行的效果不一样！一般用在`mainloop`之前，但`tkintertools`已经在`mainloop`函数中嵌入了该函数，无需再设置一次 DPI 级别，此函数是为了原生`tkinter`程序用的。
 
 Examples/实战示例
 ----------------
@@ -654,52 +653,51 @@
 * 文章链接: https://xiaokang2022.blog.csdn.net/article/details/128561339
 * 代码仓库: https://gitcode.net/weixin_62651706/todolist
 * 程序下载(含打包好的程序和源代码): https://wwc.lanzoum.com/iyxL30kpkcbe
 * 推荐指数: 👍
 
 这个案例使用了 tkintertools-v2.5.7 版本（新版已无法兼容），含有一些 bug，大量采用了 tkintertools 的控件，取得了比较好的界面效果。体现了 tkintertools 模块与 tkinter 模块相比在颜值上的碾压性！
 
-<p>
-    <img width="720px" src="https://img-blog.csdnimg.cn/img_convert/dc1a598c3f082253c1ebc7bbca0b98ce.gif" alt="todolist.png"/>
-    <img width="720px" src="https://img-blog.csdnimg.cn/img_convert/7f34451deda1af13712a9edcb37f20b4.gif" alt="todolist.png"/>
-</p>
+![todolist.gif](https://img-blog.csdnimg.cn/img_convert/dc1a598c3f082253c1ebc7bbca0b98ce.gif)
+
+![todolist.gif](https://img-blog.csdnimg.cn/img_convert/7f34451deda1af13712a9edcb37f20b4.gif)
 
 ### 中国象棋游戏
 
 * 文章链接: https://xiaokang2022.blog.csdn.net/article/details/128852029
 * 代码仓库: https://gitcode.net/weixin_62651706/chess
 * 程序下载(含打包好的程序和源代码): https://wwc.lanzoum.com/iwgp00mlewpa
 * 推荐指数: 👍👍
 
 注意：源代码有解压密码，解压密码在链接文章中，请仔细查找！  
 这个案例使用了 tkintertools-v2.5.9.5 版本（新版已无法兼容）, 含有少量 bug，部分 UI 采用了 tkintertools，部分 UI 采用了 tkinter，属于混合使用。体现了 tkintertools 模块对 tkinter 模块的兼容性！
 
-<p>
-    <img height="640px" src="https://img-blog.csdnimg.cn/43df0568d4b34078a443a098b67c126a.png" alt="chess.png"/>
-    <img height="640px" src="https://img-blog.csdnimg.cn/fc768093715d47d7b14bea015a921e3d.png" alt="chess.png"/>
-</p>
+![chess.png](https://img-blog.csdnimg.cn/43df0568d4b34078a443a098b67c126a.png)
+
+![chess.png](https://img-blog.csdnimg.cn/fc768093715d47d7b14bea015a921e3d.png)
 
 ### 简易登录界面
 
 * 文章链接: 暂无
 * 代码仓库: https://gitcode.net/weixin_62651706/tester
 * 程序下载: 暂无
 * 推荐指数: 👍👍👍
 
 这个案例使用了最新稳定版的 tkintertools-v2.6.0，界面非常稳定，几乎没有 bug，完全采用 tkintertools 的控件，颜值很高，界面非常流畅。体现了 tkintertools 模块与 tkinter 模块相比在性能上的优越性！
 
-![exam3_1.png](docs/examples/exam3_1.png)
-![exam3_2.png](docs/examples/exam3_2.png)
+![exam3_1.png](readme_res/exam3_1.png)
+
+![exam3_2.png](readme_res/exam3_2.png)
 
 More/更多
 ---------
 
 > GitHub:  
 > https://github.com/Xiaokang2022/tkintertools
 
-> GitCode(Mirror/镜像):  
-> https://gitcode.net/weixin_62651706/tkintertools
-
 > Gitee(Mirror/镜像):  
 > https://gitee.com/xiaokang-2022/tkintertools
 
-还有更多内容请在 [源代码](./tkintertools/) 中探索！
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
+
+还有更多内容请在 [源代码](tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,96 +1,94 @@
-Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.3 Summary: An
+Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.4 Summary: An
 auxiliary module of the tkinder module Home-page: https://github.com/
 Xiaokang2022/tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2
 (MulanPSL-2.0) Classifier: Operating System :: OS Independent Description-
 Content-Type: text/markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
-Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
-``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
+* Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/07 ``` pip
+install tkintertools==2.6.3 æè pip install tkintertools ```
 è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
-æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
-issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/06
-``` pip install tkintertools-dev==2.6.3 ```
-è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
-å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
-ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-News/ææ°åè½ -----------
--
-ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
-åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
-éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
-tools_3d as t3d import tkintertools.tools_3d as t3d #
-ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
-tools_3d.py)
-ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
-ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
-å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
-xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
-images/3d.png) æºä»£ç  ```python import random import tkinter import
-tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
-('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
-# type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
-åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
-åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
-fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
-for _ in range(8): # åå»ºæ­£æ¹ä½ cube = t3d.Cuboid( canvas, *random.sample
-(range(-200, 200), 3), *random.sample(range(50, 100), 3)) geos.append(cube) #
-åå»ºåé¢ä½ x, y, z = random.sample(range(-200, 200), 3) tetr =
-t3d.Tetrahedron( canvas, *[[x+random.randint(-100, 100), y+random.randint(-100,
-100), z+random.randint(-100, 100)] for _ in range(4)]) geos.append(tetr) def
-translate(event, flag=False, _cache=[]): # type: (tkinter.Event, bool, list
-[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x, event.y]
-return dx = (event.x - _cache[0]) / 6 dy = (event.y - _cache[1]) / 6 _cache[:
-] = [event.x, event.y] for axis in axes: axis.translate(0, 6*dx, 6*dy)
-axis.update() for geo in geos: geo.translate(0, dx, dy) geo.update()
-origin.translate(0, 6*dx, 6*dy) origin.update() def rotate(event, flag=False,
-_cache=[]): # type: (tkinter.Event, bool, list[float]) -> None """ æè½¬äºä»¶
-""" if flag: _cache[:] = [event.x, event.y] return dy = (event.x - _cache[0]) /
-200 dx = (_cache[1] - event.y) / 200 _cache[:] = [event.x, event.y] for axis in
-axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
-geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
-(event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
-event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
+ï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã å³äºç¨³å®çæ Issue
+çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ### Development version/
+å¼åçæ¬ * Version/çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/11
+``` pip install tkintertools-dev==2.6.4 æè pip install tkintertools-dev ```
+è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼å¯è½ææ°åè½ï¼bug
+ä¹å¯è½ä¼æ¯è¾å¤ï¼ä½ä¹å¯è½ä¼æ¯åæ¥ççæ¬æ´å ç¨³å®ã
+å¤§å®¶å¯ä»¥å¨ Issue
+ä¸­æåºä¸äºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
+**ç¹å«æ³¨æ** *
+å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»çAPIå¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸æ­£å¼çå¼å®¹ï¼
+*
+è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½æ­£å¼çååè¿è¡pipå®è£ï¼åæ¬¡ä½¿ç¨æ­£å¼çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£æ­£å¼çï¼
+* éè¦ **Python3.8** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼ News/
+ææ°åè½ ------------ ææ°çç tkintertools **å¼åç**(2.6.4-
+dev)æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
+å¨ Windows ç³»ç»ä¸è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
+* æä½é¼ æ å·¦é®æå¨å¯ä»¥æè½¬è¿å¤ä¸ªå ä½ä½ï¼ *
+æä½é¼ æ å³é®æå¨å¯ä»¥ç§»å¨è¿äºå ä½ä½å¨ç©ºé´ä¸­çä½ç½®ï¼ *
+æâ=âåâ-âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼ *
+æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ã
+ä¸é¢æ¯ç¤ºä¾ç¨åºçææå¾ï¼ ![news.png](news.png) æºä»£ç  ```python
+from tkinter import Event import tkintertools as tkt from tkintertools import
+tools_3d as t3d root = tkt.Tk('tool_3d', 1280, 720) cv3d = t3d.Canvas_3D(root,
+1280, 720, 0, 0) origin = t3d.Point(cv3d, [0, 0, 0]) # åç¹ k = -100, 0, 100
+geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white',
+color_down='yellow', color_left='red', color_right='orange',
+color_front='blue', color_back='green') for a in k for b in k for c in k]
+cv3d.space_sort() def translate(event, flag=False, _cache=[]): # type: (Event,
+bool, list[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x,
+event.y] return dx = (event.x - _cache[0]) dy = (event.y - _cache[1]) _cache[:
+] = [event.x, event.y] for geo in geos: geo.translate(0, dx, dy) geo.update()
+origin.translate(0, dx, dy) origin.update() cv3d.space_sort() def rotate(event,
+flag=False, _cache=[]): # type: (Event, bool, list[float]) -> None """
+æè½¬äºä»¶ """ if flag: _cache[:] = [event.x, event.y] return dy = (event.x -
+_cache[0]) / 100 dx = (_cache[1] - event.y) / 100 _cache[:] = [event.x,
+event.y] for item in geos: item.rotate(0, dx, dy, center=origin.coords)
+item.update() cv3d.space_sort() def scale(event): # type: (Event) -> None """
+ç¼©æ¾äºä»¶ """ k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym
+== 'minus' else 1 for geo in geos: geo.scale(k, k, k) geo.update()
+cv3d.space_sort() def scale_center(event): # type: (Event) -> None """
+ä¸­å¿ç¼©æ¾äºä»¶ """ k = 1.05 if event.delta > 0 else 0.95 for geo in geos:
+geo.scale(k, k, k, center=origin.coords) geo.update() cv3d.space_sort()
 root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
 root.bind('', lambda event: translate(event, True)) root.bind('', translate)
-root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
-[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
-- tkintertools æ¯ä¸æ¬¾åºäº tkinter
+root.bind('', scale) root.bind('', scale_center) root.mainloop() ```
+æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼[CHANGELOG.md](CHANGELOG.md) Description/
+æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
 ä½åæ¶ä¹äº§çäºä¸äºç¼ºç¹ï¼ * èæçæ§ä»¶æ æ³è·åç¦ç¹ *
 èæçæ§ä»¶å¨ææ¬è¾å¥åæ¾ç¤ºçåè½ä¸å­å¨ä¸äºç¼ºé·ï¼è¿ä¸ªç¼ºé·ä¸æ¯å¾ææ¾ï¼ä½å¼ºè¿«çå°±æç¹é¾åäºï¼æ¯å¦æï¼
 tkintertools æ¨¡åè¿å·æä¸äºç¹è²çåè½ï¼ * å©ç¨ tkinter å
 tkintertools åå»ºçç¨åºï¼å¨é«åè¾¨ççæåµä¸ï¼tkintertools
 çä¼æ´å æ¸æ°ï¼è¿ç¹å¯¹äºç¬è®°æ¬ç¨æ·å¾åå¥½ï¼æ¯å¦æï¼ *
 å¯ä»¥è¿éå®ç°æ¸åè²çææ *
 çªå£ç¼©æ¾ï¼ææçæ§ä»¶çå¤§å°è·çç¼©æ¾ï¼å½ç¶ï¼ä¹å¯ä»¥è®¾ç½®ä¸ºä¸è·éç¼©æ¾ï¼
-æ³¨æï¼éè¦ **Python3.7** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼
-Provides/æ¨¡ååè½ ------------------- Here, only the more distinctive
-features will be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ###
-Customizable widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
+* å­æ¨¡å tools_3d å¯ä»¥æ¯æ»¡è¶³ç®åç 3D ç»å¾éæ± Provides/
+æ¨¡ååè½ ------------------- Here, only the more distinctive features will
+be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ### Customizable
+widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
 æ¨¡åçæ§ä»¶æ¥æè®¸å¤åæ°ä¾æä»¬è®¾ç½®ï¼æ¯å¦åè§çåå¾ãææ¬åè¾¹æ¡ä»¥åæ§ä»¶åé¨çé¢è²ï¼å³èäºä»¶ç­ç­ã
 è¿éè¦è¯´æçæ¯ï¼æ¯ä¸ªæ§ä»¶å¯ä»¥è®¾ç½®çå³èäºä»¶ä¸æ­¢ä¸ç§ï¼å¨é¼ æ ç»è¿æ§ä»¶æ¶å¯ä»¥ç»å®äºä»¶ï¼é¼ æ ç¹å»æ§ä»¶ä¹å¯ä»¥ï¼é¼ æ ç¹å»åæ¾å¼ä¹è¡ç­ç­ã
 ææ¬åè¾¹æ¡ä»¥åæ§ä»¶çå¡«åè²ä¹æ¯ç±»ä¼¼çï¼å¨é¼ æ ç»è¿æ§ä»¶ãç¹å»æ§ä»¶ãç¹å»åæ¾å¼é½å¯ä»¥è®¾å®é¢è²ã
 ææ¬ç±»æ§ä»¶è¿è½å¤ä»å³è¾¹éæ­¥è¾å¥ææ¬ï¼ææ¬è¾å¥æç¤ºç¬¦ä¹å¯ä»¥ä¸æ¯åè°æ è¶£çç«çº¿ï¼å¯ä»¥æ¯å¶ä»çï¼æ¯å¦ä¸åçº¿ç­ã
-æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](./test.py)
+æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](test.py)
 æä»¶éé¢çç¤ºä¾ï¼è¿ä¸ªç¤ºä¾å±ç¤ºäº tkintertools
 æ¨¡åçç»å¤§é¨ååè½ï¼ç¤ºä¾ä¸­æ´æéèç âå¤å½©åå¹»â
 å½©èå¦ï¼ ### Automatically control size/èªå¨æ§å¶å¤§å° tkintertools
 ä¸­çæ§ä»¶ï¼å¶å¤§å°åå½¢ç¶å¯ä»¥éççªå£çååèææ¯ä¾å°ååï¼ä¸ä»ä»æ¯æ§ä»¶ä¸­çææ¬ï¼Canvas
 ç»å¶çå¾å½¢ä¹ä¼éä¹åå¨ï¼æ´è®©äººå´å¥çæ¯ï¼png
 ç±»åçå¾çä¹ä¼éä¹ææ¯ä¾å°ç¼©æ¾ï¼å½ç¶ï¼ä½ ä¹å¯ä»¥è®¾å®åæ°è®©å¶ä¸éä¹åå¨ï¼ä¹å¯ä»¥è®¾å®åæ°ä½¿å¶å¨ç¼©æ¾çæ¶åä¿ææ¨ªçºµæ¹åçæ¯ä¾ã
 æ»ä¹ï¼å¾æ¹ä¾¿ï¼å¾èéï¼ ### Easily move widgets/è½»æ¾ç§»å¨æ§ä»¶
@@ -99,70 +97,73 @@
 çº§å«è®¾ç½®å½æ°](#DPI) ### Detailed type hints/è¯¦ç»çç±»åæç¤º åè
 [PEP 526](https://peps.python.org/pep-0526/)ã[PEP 586](https://
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
 é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
-[type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
+[type_hint.png](readme_res/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
-tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
-(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
-images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
-internal class and function in the module will be described in detail here
+tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](test.py) å¨
+Windows ç³»ç»ï¼**Windows10**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ !
+[test_windows10.png](readme_res/test_windows10.png) [test.py](test.py) å¨
+Linux ç³»ç»ï¼**Ubuntu22.04**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png]
+(readme_res/test_linux.png) [test.py](test.py) å¨ Windows
+ç³»ç»ï¼**Windows11**ï¼ä¸è¿è¡ççé¢å¦ä¸(æºè½æ§å¶åè§åå¾)ï¼
+![test_windows11.png](readme_res/test_windows11.png) ### 3D Drawing/3Dç»å¾
+è§ [News/ææ°åè½](#news) Contents/æ¨¡ååå®¹ ------------------- Each
+non internal class and function in the module will be described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
-ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](docs/images/LabelTest.png)
+ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](readme_res/LabelTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
 tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
 tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
 tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
-ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](docs/images/
+ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](readme_res/
 ButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk
 ('ButtonTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful
 (x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
 """ for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
 100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
 (canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
 (canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
 (canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
 å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
-ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](docs/images/
+ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](readme_res/
 CheckButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root =
 tkt.Tk('CheckButtonTest', 500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0)
 def colorful(x, y, width, height): # type: (int, int, int, int) -> None """
 Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(40, 190, 420, 50) tkt.CheckButton(canvas, 50, 50, 30,
 text='NormalCheckButton', value=True) tkt.CheckButton(canvas, 50, 100, 30,
 text='DisableCheckButton', value=True).set_live(False) tkt.CheckButton(canvas,
 50, 150, 30, radius=10, text='RoundCornerCheckButton') tkt.CheckButton(canvas,
 50, 200, 30, radius=15, text='TransparentCheckButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
-ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](docs/images/EntryTest.png)
+ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](readme_res/EntryTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
 400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
 100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
 (canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
@@ -173,29 +174,29 @@
 radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
 35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
 tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
 justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
 text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
 root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
-ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](docs/images/TextTest.png)
+ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](readme_res/TextTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
 for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
 Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
 (Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
 text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
 radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
-ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](docs/images/
+ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](readme_res/
 ProgressbarTest.png) æºä»£ç  ```python import tkintertools as tkt root =
 tkt.Tk('ProgressbarTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0)
 def colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None
 """ Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(30, 290, 440, 50) tkt.Progressbar(canvas, 50, 50, 400, 30)
 tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667) tkt.Progressbar(canvas,
@@ -213,15 +214,15 @@
 å¨å¾æå¾å¥½çæ¯æï¼ä»éæå°éä»£ç å³å¯å®ç°å¨å¾çæ¾ç¤ºï¼è¿å¯ä»¥è®¾ç½®å¨å¾æ¾ç¤ºçéåº¦ï¼æ­¤å¤ï¼å¯¹
 png
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
-![MoveTest.gif](docs/images/MoveTest.gif) æºä»£ç  ```python import
+![MoveTest.gif](readme_res/MoveTest.gif) æºä»£ç  ```python import
 tkintertools as tkt root = tkt.Tk('MoveTest', 500, 500) canvas = tkt.Canvas
 (root, 500, 500, 0, 0) rect = canvas.create_rectangle(50, 350, 150, 450) def
 move_window(switch=[True]): # type: (list[bool]) -> None tkt.move(root, None,
 1000 if switch[0] else -1000, 0, 800, mode='flat') switch[0] = not switch[0]
 def move_button(switch=[True]) -> None: # type: (list[bool]) -> None tkt.move
 (canvas, button, 200 if switch[0] else -200, 0, 500, mode='rebound') switch[0]
 = not switch[0] def move_rect(switch=[True]): # type: (list[bool]) -> None
@@ -235,36 +236,35 @@
 å¦ï¼å¾å°ä¸ä¸ª 20 é¿åº¦çå­ç¬¦ä¸² âtkintertoolsâ
     `left`   : "tkintertools        "
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
 ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡ ![ColorTest.png]
-(docs/images/ColorTest.png) ![Test_Draw.png](docs/images/Test_Draw.png)
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
-height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
-tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
-y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
+(readme_res/ColorTest.png) ![Test_Draw.png](readme_res/Test_Draw.png) æºä»£ç 
+```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500, 500)
+canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width, height): #
+type: (int, int, int, int) -> None """ Gradient colors """ for i in range
+(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 = tkt.color
+(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i, y+height,
+fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
 outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
 `askfont`: å­ä½éæ©å¯¹è¯æ¡
 `askfont`å½æ°å¯ä»¥æå¼é»è®¤çå­ä½éæ©çªå£ï¼è¿ä¸ªçªå£è½ç¶æ¯é»è®¤çï¼ä½å®å®éä¸æ æ³å¨`tkinter`ä¸­æå¼ï¼å ä¸º`tkinter`å¹¶æ²¡æå¯¹åºç
 API è½å¤åå°è¿ä¸ç¹ãä½æ¯ï¼`tkintertools`è°ç¨å¹¶å°è£äºåçç
-tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
-[font.png]
-5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
+tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã ![font.png]
+(readme_res/font.png) 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
 è¿ä¸ªå½æ°å®éä¸åªæ¯å¯¹å½æ°`ctypes.WinDLL
 ('shcore').SetProcessDpiAwareness`çä¸ä¸ªç®ååè£ï¼å¶å¼å¯ä¸º 0ã1
 å 2ï¼åå«ä»£è¡¨ç¨åº DPI
 çä¸åçº§å«ï¼é£ä¹ç¼©æ¾ææä¹å°±ä¸åï¼`tkintertools`éæ©çå¼æ¯
 1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ !
-[SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+[SetProcessDpiAwareness_0.png](readme_res/SetProcessDpiAwareness_0.png)
 ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
-![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
+![SetProcessDpiAwareness_1.png](readme_res/SetProcessDpiAwareness_1.png)
 ä»ä¸é¢çä¸¤å¼ å¾ä¸­å¯ä»¥å¾ææ¾ççåºç¬¬ä¸å¼ å¾æ¨¡ç³ï¼ç¬¬äºå¼ å¾æ¸æ°ï¼è¿å°±æ¯
 DPI çº§å«ä¸åçåå ï¼ä¸è¿è¿ä¸ç¹å¨å±å¹ç¼©æ¾æ¯ä¸æ¯ 100%
 çæ¶åæä¼åºç° å¤§å®¶å¯¹ä¸é¢çå¾è¯å®å¾çæï¼è¿ä¸å°±æ¯ IDLE
 åï¼ï¼å¯¹ï¼è¿ä¸ªçé®é¢çè§£å³åæ³ä¹æ¯æ¥èªäº IDLE çæºä»£ç 
 [pyshell.py line 18~20]
 æ³¨æï¼è¯¥å½æ°å¨ç¨åºçä¸åä½ç½®æ§è¡çææä¸ä¸æ ·ï¼ä¸è¬ç¨å¨`mainloop`ä¹åï¼ä½`tkintertools`å·²ç»å¨`mainloop`å½æ°ä¸­åµå¥äºè¯¥å½æ°ï¼æ éåè®¾ç½®ä¸æ¬¡
 DPI çº§å«ï¼æ­¤å½æ°æ¯ä¸ºäºåç`tkinter`ç¨åºç¨çã Examples/
@@ -276,30 +276,33 @@
 bugï¼åªéè¿éè¦æ¹è¿ï¼ ### ä»»å¡æ¸åå°å·¥å· * æç« é¾æ¥: https:
 //xiaokang2022.blog.csdn.net/article/details/128561339 * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/todolist * ç¨åºä¸è½½
 (å«æåå¥½çç¨åºåæºä»£ç ): https://wwc.lanzoum.com/iyxL30kpkcbe *
 æ¨èææ°: ð è¿ä¸ªæ¡ä¾ä½¿ç¨äº tkintertools-v2.5.7
 çæ¬ï¼æ°çå·²æ æ³å¼å®¹ï¼ï¼å«æä¸äº bugï¼å¤§ééç¨äº
 tkintertools çæ§ä»¶ï¼åå¾äºæ¯è¾å¥½ççé¢ææãä½ç°äº
-tkintertools æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨é¢å¼ä¸çç¢¾åæ§ï¼
-[todolist.png] [todolist.png]
-### ä¸­å½è±¡æ£æ¸¸æ * æç« é¾æ¥: https://xiaokang2022.blog.csdn.net/
-article/details/128852029 * ä»£ç ä»åº: https://gitcode.net/weixin_62651706/
-chess * ç¨åºä¸è½½(å«æåå¥½çç¨åºåæºä»£ç ): https://
-wwc.lanzoum.com/iwgp00mlewpa * æ¨èææ°: ðð
+tkintertools æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨é¢å¼ä¸çç¢¾åæ§ï¼ !
+[todolist.gif](https://img-blog.csdnimg.cn/img_convert/
+dc1a598c3f082253c1ebc7bbca0b98ce.gif) ![todolist.gif](https://img-
+blog.csdnimg.cn/img_convert/7f34451deda1af13712a9edcb37f20b4.gif) ###
+ä¸­å½è±¡æ£æ¸¸æ * æç« é¾æ¥: https://xiaokang2022.blog.csdn.net/article/
+details/128852029 * ä»£ç ä»åº: https://gitcode.net/weixin_62651706/chess *
+ç¨åºä¸è½½(å«æåå¥½çç¨åºåæºä»£ç ): https://wwc.lanzoum.com/
+iwgp00mlewpa * æ¨èææ°: ðð
 æ³¨æï¼æºä»£ç æè§£åå¯ç ï¼è§£åå¯ç å¨é¾æ¥æç« ä¸­ï¼è¯·ä»ç»æ¥æ¾ï¼
 è¿ä¸ªæ¡ä¾ä½¿ç¨äº tkintertools-v2.5.9.5 çæ¬ï¼æ°çå·²æ æ³å¼å®¹ï¼,
 å«æå°é bugï¼é¨å UI éç¨äº tkintertoolsï¼é¨å UI éç¨äº
 tkinterï¼å±äºæ··åä½¿ç¨ãä½ç°äº tkintertools æ¨¡åå¯¹ tkinter
-æ¨¡åçå¼å®¹æ§ï¼
-[chess.png] [chess.png]
-### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
-gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
-ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
+æ¨¡åçå¼å®¹æ§ï¼ ![chess.png](https://img-blog.csdnimg.cn/
+43df0568d4b34078a443a098b67c126a.png) ![chess.png](https://img-blog.csdnimg.cn/
+fc768093715d47d7b14bea015a921e3d.png) ### ç®æç»å½çé¢ * æç« é¾æ¥:
+ææ  * ä»£ç ä»åº: https://gitcode.net/weixin_62651706/tester *
+ç¨åºä¸è½½: ææ  * æ¨èææ°: ððð
+è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
-æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
-examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
------- > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
-(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
-(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
-è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png]
+(readme_res/exam3_1.png) ![exam3_2.png](readme_res/exam3_2.png) More/æ´å¤ ---
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > Gitee(Mirror/
+éå): > https://gitee.com/xiaokang-2022/tkintertools > GitCode(Mirror/
+éå): > https://gitcode.net/weixin_62651706/tkintertools
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](tkintertools/) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools-dev-2.6.3/README.md` & `tkintertools-dev-2.6.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
-        src="./tkintertools.png" />
+        src="tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
-        <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
+        <a href="tkintertools/__init__.py">
+            <img src="https://img.shields.io/badge/Version-2.6.4(dev)-blue" alt="latest version" />
         </a>
-        <a href="./LICENSE">
+        <a href="LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
-        <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/06/06-orange" alt="ChangeLog" />
+        <a href="CHANGELOG.md">
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/11-orange" alt="ChangeLog" />
         </a>
-        <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
+        <a href="TODO.md">
+            <img src="https://img.shields.io/badge/ToDos-14-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
+            <img src="https://img.shields.io/badge/Downloads-4k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
@@ -32,152 +32,144 @@
         <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
     </p>
 </div>
 
 Installation/模块安装
------------------------
+--------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/30
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/07
 
 ```
-pip install tkintertools==2.6.2
-```
+pip install tkintertools==2.6.3
 或者
-```
 pip install tkintertools
 ```
 
-这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
-稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
+这个是目前的最新稳定版，比较稳定，bug （可能）没有那么多，推荐使用这个。  
+关于稳定版有 Issue 的话，我会去查看并尝试解决 Issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.3
-* Release Date/发布日期 : 2023/06/06
+* Version/版本 : 2.6.4
+* Release Date/发布日期 : 2023/06/11
 
 ```
-pip install tkintertools-dev==2.6.3
+pip install tkintertools-dev==2.6.4
+或者
+pip install tkintertools-dev
 ```
 
-这个是我正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
-开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
-
-News/最新功能
-------------
-
-最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
-同时修复一些bug，优化了一部分代码，提升了一部分性能。
+这个是我正在开发的版本，可能有新功能，bug 也可能会比较多，但也可能会比原来的版本更加稳定。  
+大家可以在 Issue 中提出一些建议，我会适当采纳一些并在开发版本中更改或实现。
 
-通过以下代码来使用3d绘图功能：
+**特别注意**
+* 开发版仅作示例，各函数或类的API并非最终确定结果，直接使用开发版可能导致后续无法与正式版兼容！
+* 若要使用开发版，请先卸载正式版后再进行pip安装，再次使用正式版时也是一样，先卸载开发版再安装正式版！
+* 需要 **Python3.8** 及更高版本才能运行 tkintertools！
 
-```python
-from tkintertools import tools_3d as t3d
-import tkintertools.tools_3d as t3d
-# 两种引入方式都可以
-```
+<a name="news">News/最新功能</a>
+------------
 
-子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+最新版的 tkintertools **开发版**(2.6.4-dev)新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
 
-目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
-以下是一个使用3d绘图的示例：
+在 Windows 系统下运行下面的示例程序时，其拥有以下功能：
+* 按住鼠标左键拖动可以旋转这多个几何体；
+* 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
+* 按“=”和“-”键分别可以放大和缩小几何体的大小；
+* 滚动鼠标中键可以放大和缩小画面。
 
-在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
-x、y 和 z 轴分别是红色、绿色和蓝色的线。
+下面是示例程序的效果图：
 
-![3d绘图](./docs/images/3d.png)
+![news.png](news.png)
 
 <details><summary><b>源代码</b></summary>
 
 ```python
-import random
-import tkinter
+from tkinter import Event
 
 import tkintertools as tkt
 from tkintertools import tools_3d as t3d
 
-root = tkt.Tk('tools_3d', 1280, 720)
-canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+root = tkt.Tk('tool_3d', 1280, 720)
+cv3d = t3d.Canvas_3D(root, 1280, 720, 0, 0)
 
-geos = []  # type: list[t3d.Geometry]
-origin = t3d.Point(canvas, [0, 0, 0], size=5)  # 原点
-axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'),  # 创建坐标轴
-        t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3, fill='green'),
-        t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
-
-for _ in range(8):
-    # 创建正方体
-    cube = t3d.Cuboid(
-        canvas, *random.sample(range(-200, 200), 3), *random.sample(range(50, 100), 3))
-    geos.append(cube)
-    # 创建四面体
-    x, y, z = random.sample(range(-200, 200), 3)
-    tetr = t3d.Tetrahedron(
-        canvas, *[[x+random.randint(-100, 100), y+random.randint(-100, 100), z+random.randint(-100, 100)] for _ in range(4)])
-    geos.append(tetr)
+origin = t3d.Point(cv3d, [0, 0, 0])  # 原点
+k = -100, 0, 100
+geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white', color_down='yellow', color_left='red',
+                   color_right='orange', color_front='blue', color_back='green') for a in k for b in k for c in k]
+cv3d.space_sort()
 
 
 def translate(event, flag=False, _cache=[]):
-    # type: (tkinter.Event, bool, list[float]) -> None
+    # type: (Event, bool, list[float]) -> None
     """ 平移事件 """
     if flag:
         _cache[:] = [event.x, event.y]
         return
-    dx = (event.x - _cache[0]) / 6
-    dy = (event.y - _cache[1]) / 6
+    dx = (event.x - _cache[0])
+    dy = (event.y - _cache[1])
     _cache[:] = [event.x, event.y]
-    for axis in axes:
-        axis.translate(0, 6*dx, 6*dy)
-        axis.update()
     for geo in geos:
         geo.translate(0, dx, dy)
         geo.update()
-    origin.translate(0, 6*dx, 6*dy)
+    origin.translate(0, dx, dy)
     origin.update()
+    cv3d.space_sort()
 
 
-def rotate(event, flag=False, _cache=[]):  # type: (tkinter.Event, bool, list[float]) -> None
+def rotate(event, flag=False, _cache=[]):
+    # type: (Event, bool, list[float]) -> None
     """ 旋转事件 """
     if flag:
         _cache[:] = [event.x, event.y]
         return
-    dy = (event.x - _cache[0]) / 200
-    dx = (_cache[1] - event.y) / 200
+    dy = (event.x - _cache[0]) / 100
+    dx = (_cache[1] - event.y) / 100
     _cache[:] = [event.x, event.y]
-    for axis in axes:
-        axis.rotate(0, 6*dx, 6*dy, center=origin.coords)
-        axis.update()
-    for geo in geos:
-        geo.rotate(0, dx, dy, center=origin.coords)
-        geo.update()
+    for item in geos:
+        item.rotate(0, dx, dy, center=origin.coords)
+        item.update()
+    cv3d.space_sort()
 
 
-def scale(event):  # type: (tkinter.Event) -> None
+def scale(event):  # type: (Event) -> None
     """ 缩放事件 """
-    k = 1.01 if event.delta > 0 else 0.99
+    k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1
     for geo in geos:
         geo.scale(k, k, k)
         geo.update()
+    cv3d.space_sort()
+
+
+def scale_center(event):  # type: (Event) -> None
+    """ 中心缩放事件 """
+    k = 1.05 if event.delta > 0 else 0.95
+    for geo in geos:
+        geo.scale(k, k, k, center=origin.coords)
+        geo.update()
+    cv3d.space_sort()
 
 
 root.bind('<Button-1>', lambda event: rotate(event, True))
 root.bind('<B1-Motion>', rotate)
 root.bind('<Button-3>', lambda event: translate(event, True))
 root.bind('<B3-Motion>', translate)
-root.bind('<MouseWheel>', scale)
+root.bind('<Any-Key>', scale)
+root.bind('<MouseWheel>', scale_center)
 root.mainloop()
 ```
 
 </details>
 
-更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+更多更新信息请见：[CHANGELOG.md](CHANGELOG.md)
 
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
@@ -190,30 +182,29 @@
 * 虚拟的控件在文本输入和显示的功能上存在一些缺陷（这个缺陷不是很明显，但强迫症就有点难受了，比如我）
 
 tkintertools 模块还具有一些特色的功能：
 
 * 利用 tkinter 和 tkintertools 创建的程序，在高分辨率的情况下，tkintertools 的会更加清晰（这点对于笔记本用户很友好，比如我）
 * 可以迅速实现渐变色的效果
 * 窗口缩放，所有的控件的大小跟着缩放（当然，也可以设置为不跟随缩放）
-
-注意：需要 **Python3.7** 及更高版本才能运行 tkintertools！
+* 子模块 tools_3d 可以是满足简单的 3D 绘图需求
 
 Provides/模块功能
 -------------------
 
 Here, only the more distinctive features will be listed  
 这里只会列举出比较具有特色的功能
 
 ### Customizable widgets/可自定义的控件
 
 tkintertools 模块的控件拥有许多参数供我们设置，比如圆角的半径、文本和边框以及控件内部的颜色，关联事件等等。  
 这里要说明的是，每个控件可以设置的关联事件不止一种，在鼠标经过控件时可以绑定事件，鼠标点击控件也可以，鼠标点击后松开也行等等。  
 文本和边框以及控件的填充色也是类似的，在鼠标经过控件、点击控件、点击后松开都可以设定颜色。  
 文本类控件还能够从右边逐步输入文本，文本输入提示符也可以不是单调无趣的竖线，可以是其他的，比如下划线等。  
-最后，大家可以看一下 [test.py](./test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
+最后，大家可以看一下 [test.py](test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
 
 ### Automatically control size/自动控制大小
 
 tkintertools 中的控件，其大小和形状可以随着窗口的变化而成比例地变化，不仅仅是控件中的文本，Canvas 绘制的图形也会随之变动，更让人兴奋的是，png 类型的图片也会随之成比例地缩放！当然，你也可以设定参数让其不随之变动，也可以设定参数使其在缩放的时候保持横纵方向的比例。  
 总之，很方便，很舒适！
 
 ### Easily move widgets/轻松移动控件
@@ -229,27 +220,35 @@
 见 [DPI 级别设置函数](#DPI)
 
 ### Detailed type hints/详细的类型提示
 
 参考 [PEP 526](https://peps.python.org/pep-0526/)、[PEP 586](https://peps.python.org/pep-0586/)、[PEP 604](https://peps.python.org/pep-0604/) 和 [PEP 612](https://peps.python.org/pep-0612/)，我采用了最兼容的方式去实现详细的类型提示，可适用 IDE 有 VScode、Pycharm 等。  
 那什么是类型提示呢？话不多说，直接看图就行：
 
-![type_hint.png](docs/images/type_hint_vscode.png)
+![type_hint.png](readme_res/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
-[test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
+[test.py](test.py) 在 Windows 系统（**Windows10**）上运行的界面如下：
+
+![test_windows10.png](readme_res/test_windows10.png)
 
-![test_win32.png](docs/images/test_win32.png)
+[test.py](test.py) 在 Linux 系统（**Ubuntu22.04**）上运行的界面如下：
 
-[test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
+![test_linux.png](readme_res/test_linux.png)
 
-![test_linux.png](docs/images/test_linux.png)
+[test.py](test.py) 在 Windows 系统（**Windows11**）上运行的界面如下(智能控制圆角半径)：
+
+![test_windows11.png](readme_res/test_windows11.png)
+
+### 3D Drawing/3D绘图
+
+见 [News/最新功能](#news)
 
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
@@ -270,15 +269,15 @@
 ### Virtual Canvas Widget/虚拟画布控件
 
 1. `Label`: 标签控件
 
     标签控件的功能和`tkinter.Label`的功能类似，但更加的多元化  
     下面是`Label`控件的外观：  
 
-    ![LabelTest.png](docs/images/LabelTest.png)
+    ![LabelTest.png](readme_res/LabelTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
@@ -305,15 +304,15 @@
     </details>
 
 2. `Button`: 按钮控件
 
     按钮控件相较于`tkinter.Button`，其自由度更高，`tkinter.Button`只有在按下的时候才能触发绑定的关联事件，而`Button`却可以在鼠标移至按钮上方时、鼠标按下时、鼠标松开时都可以绑定关联事件  
     下面是`Button`控件的外观：
 
-    ![ButtonTest.png](docs/images/ButtonTest.png)
+    ![ButtonTest.png](readme_res/ButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
@@ -340,15 +339,15 @@
     </details>
 
 3. `CheckButton`: 复选框控件
 
     复选框控件相对于`tkinter`原生的`tkinter.CheckButton`在使用方面更加地简单，同时颜值也上升了不少  
     下面是`CheckButton`控件的外观：
 
-    ![CheckButtonTest.png](docs/images/CheckButtonTest.png)
+    ![CheckButtonTest.png](readme_res/CheckButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
@@ -376,15 +375,15 @@
     </details>
 
 4. `Entry`: 输入框控件
 
     输入框控件可以轻松地设置输入的文本位置（靠左、居中和靠右），同时，它可以在鼠标移至输入框上方、鼠标未在输入框上方两种状态显示不同的默认文本  
     下面是`Entry`控件的外观：
 
-    ![EntryTest.png](docs/images/EntryTest.png)
+    ![EntryTest.png](readme_res/EntryTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
@@ -422,15 +421,15 @@
     </details>
 
 5. `Text`: 文本框控件
 
     文本框类似于输入框，这里就不再赘述  
     下面是`Text`控件的外观：
 
-    ![TextTest.png](docs/images/TextTest.png)
+    ![TextTest.png](readme_res/TextTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
@@ -458,15 +457,15 @@
     </details>
 
 6. `Progressbar`: 进度条控件
 
     进度条控件相比`tkinter.ttk.Progressbar`，外观上的自由度较大  
     下面是`Progressbar`控件的外观：
 
-    ![ProgressbarTest.png](docs/images/ProgressbarTest.png)
+    ![ProgressbarTest.png](readme_res/ProgressbarTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
@@ -520,15 +519,15 @@
 
 ### Tool Function/工具函数
 
 1. `move`: <a name="move">移动函数</a>
 
     移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！
 
-    ![MoveTest.gif](docs/images/MoveTest.gif)
+    ![MoveTest.gif](readme_res/MoveTest.gif)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
@@ -574,17 +573,17 @@
     `right`  : "        tkintertools"</pre>
 
 3. `color`: <a name="Gradient">颜色函数</a>
 
     颜色函数可以轻松求出一个颜色到另外一个颜色的过渡颜色，因此可以轻松得到渐变色的效果，同时，改变传入的参数还可以得到传入颜色的对比色  
     第二张图是 test.py 在图像测试中绘制的图案
 
-    ![ColorTest.png](docs/images/ColorTest.png)
+    ![ColorTest.png](readme_res/ColorTest.png)
 
-    ![Test_Draw.png](docs/images/Test_Draw.png)
+    ![Test_Draw.png](readme_res/Test_Draw.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
@@ -607,26 +606,26 @@
 
     </details>
 
 4. `askfont`: 字体选择对话框
 
     `askfont`函数可以打开默认的字体选择窗口，这个窗口虽然是默认的，但它实际上无法在`tkinter`中打开，因为`tkinter`并没有对应的 API 能够做到这一点。但是，`tkintertools`调用并封装了原生的 tcl 的命令，使得字体选择框能够被我们使用。
 
-    <p><img width="540px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/font.png" alt="font.png" /></p>
+    ![font.png](readme_res/font.png)
 
 5. `SetProcessDpiAwareness`: <a name="DPI">DPI 级别设置函数</a>
 
     这个函数实际上只是对函数`ctypes.WinDLL('shcore').SetProcessDpiAwareness`的一个简单包装，其值可为 0、1 和 2，分别代表程序 DPI 的不同级别，那么缩放效果也就不同，`tkintertools`选择的值是 1，但程序默认值实际为 0  
     下面是未执行这个函数的效果
     
-    ![SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+    ![SetProcessDpiAwareness_0.png](readme_res/SetProcessDpiAwareness_0.png)
 
     <p>下面是执行了这个函数的效果</p>
 
-    ![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
+    ![SetProcessDpiAwareness_1.png](readme_res/SetProcessDpiAwareness_1.png)
 
     从上面的两张图中可以很明显的看出第一张很模糊，第二张很清晰，这就是 DPI 级别不同的原因，不过这一点在屏幕缩放比不是 100% 的时候才会出现  
     大家对上面的图肯定很熟悉，这不就是 IDLE 吗！？对，这个的问题的解决办法也是来自于 IDLE 的源代码 [pyshell.py line 18~20]  
     注意：该函数在程序的不同位置执行的效果不一样！一般用在`mainloop`之前，但`tkintertools`已经在`mainloop`函数中嵌入了该函数，无需再设置一次 DPI 级别，此函数是为了原生`tkinter`程序用的。
 
 Examples/实战示例
 ----------------
@@ -640,52 +639,51 @@
 * 文章链接: https://xiaokang2022.blog.csdn.net/article/details/128561339
 * 代码仓库: https://gitcode.net/weixin_62651706/todolist
 * 程序下载(含打包好的程序和源代码): https://wwc.lanzoum.com/iyxL30kpkcbe
 * 推荐指数: 👍
 
 这个案例使用了 tkintertools-v2.5.7 版本（新版已无法兼容），含有一些 bug，大量采用了 tkintertools 的控件，取得了比较好的界面效果。体现了 tkintertools 模块与 tkinter 模块相比在颜值上的碾压性！
 
-<p>
-    <img width="720px" src="https://img-blog.csdnimg.cn/img_convert/dc1a598c3f082253c1ebc7bbca0b98ce.gif" alt="todolist.png"/>
-    <img width="720px" src="https://img-blog.csdnimg.cn/img_convert/7f34451deda1af13712a9edcb37f20b4.gif" alt="todolist.png"/>
-</p>
+![todolist.gif](https://img-blog.csdnimg.cn/img_convert/dc1a598c3f082253c1ebc7bbca0b98ce.gif)
+
+![todolist.gif](https://img-blog.csdnimg.cn/img_convert/7f34451deda1af13712a9edcb37f20b4.gif)
 
 ### 中国象棋游戏
 
 * 文章链接: https://xiaokang2022.blog.csdn.net/article/details/128852029
 * 代码仓库: https://gitcode.net/weixin_62651706/chess
 * 程序下载(含打包好的程序和源代码): https://wwc.lanzoum.com/iwgp00mlewpa
 * 推荐指数: 👍👍
 
 注意：源代码有解压密码，解压密码在链接文章中，请仔细查找！  
 这个案例使用了 tkintertools-v2.5.9.5 版本（新版已无法兼容）, 含有少量 bug，部分 UI 采用了 tkintertools，部分 UI 采用了 tkinter，属于混合使用。体现了 tkintertools 模块对 tkinter 模块的兼容性！
 
-<p>
-    <img height="640px" src="https://img-blog.csdnimg.cn/43df0568d4b34078a443a098b67c126a.png" alt="chess.png"/>
-    <img height="640px" src="https://img-blog.csdnimg.cn/fc768093715d47d7b14bea015a921e3d.png" alt="chess.png"/>
-</p>
+![chess.png](https://img-blog.csdnimg.cn/43df0568d4b34078a443a098b67c126a.png)
+
+![chess.png](https://img-blog.csdnimg.cn/fc768093715d47d7b14bea015a921e3d.png)
 
 ### 简易登录界面
 
 * 文章链接: 暂无
 * 代码仓库: https://gitcode.net/weixin_62651706/tester
 * 程序下载: 暂无
 * 推荐指数: 👍👍👍
 
 这个案例使用了最新稳定版的 tkintertools-v2.6.0，界面非常稳定，几乎没有 bug，完全采用 tkintertools 的控件，颜值很高，界面非常流畅。体现了 tkintertools 模块与 tkinter 模块相比在性能上的优越性！
 
-![exam3_1.png](docs/examples/exam3_1.png)
-![exam3_2.png](docs/examples/exam3_2.png)
+![exam3_1.png](readme_res/exam3_1.png)
+
+![exam3_2.png](readme_res/exam3_2.png)
 
 More/更多
 ---------
 
 > GitHub:  
 > https://github.com/Xiaokang2022/tkintertools
 
-> GitCode(Mirror/镜像):  
-> https://gitcode.net/weixin_62651706/tkintertools
-
 > Gitee(Mirror/镜像):  
 > https://gitee.com/xiaokang-2022/tkintertools
 
-还有更多内容请在 [源代码](./tkintertools/) 中探索！
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
+
+还有更多内容请在 [源代码](tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,89 +1,87 @@
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
-Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
-``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
+* Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/07 ``` pip
+install tkintertools==2.6.3 æè pip install tkintertools ```
 è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
-æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
-issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/06
-``` pip install tkintertools-dev==2.6.3 ```
-è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
-å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
-ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-News/ææ°åè½ -----------
--
-ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
-åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
-éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
-tools_3d as t3d import tkintertools.tools_3d as t3d #
-ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
-tools_3d.py)
-ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
-ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
-å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
-xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
-images/3d.png) æºä»£ç  ```python import random import tkinter import
-tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
-('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
-# type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
-åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
-åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
-fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
-for _ in range(8): # åå»ºæ­£æ¹ä½ cube = t3d.Cuboid( canvas, *random.sample
-(range(-200, 200), 3), *random.sample(range(50, 100), 3)) geos.append(cube) #
-åå»ºåé¢ä½ x, y, z = random.sample(range(-200, 200), 3) tetr =
-t3d.Tetrahedron( canvas, *[[x+random.randint(-100, 100), y+random.randint(-100,
-100), z+random.randint(-100, 100)] for _ in range(4)]) geos.append(tetr) def
-translate(event, flag=False, _cache=[]): # type: (tkinter.Event, bool, list
-[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x, event.y]
-return dx = (event.x - _cache[0]) / 6 dy = (event.y - _cache[1]) / 6 _cache[:
-] = [event.x, event.y] for axis in axes: axis.translate(0, 6*dx, 6*dy)
-axis.update() for geo in geos: geo.translate(0, dx, dy) geo.update()
-origin.translate(0, 6*dx, 6*dy) origin.update() def rotate(event, flag=False,
-_cache=[]): # type: (tkinter.Event, bool, list[float]) -> None """ æè½¬äºä»¶
-""" if flag: _cache[:] = [event.x, event.y] return dy = (event.x - _cache[0]) /
-200 dx = (_cache[1] - event.y) / 200 _cache[:] = [event.x, event.y] for axis in
-axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
-geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
-(event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
-event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
+ï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã å³äºç¨³å®çæ Issue
+çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ### Development version/
+å¼åçæ¬ * Version/çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/11
+``` pip install tkintertools-dev==2.6.4 æè pip install tkintertools-dev ```
+è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼å¯è½ææ°åè½ï¼bug
+ä¹å¯è½ä¼æ¯è¾å¤ï¼ä½ä¹å¯è½ä¼æ¯åæ¥ççæ¬æ´å ç¨³å®ã
+å¤§å®¶å¯ä»¥å¨ Issue
+ä¸­æåºä¸äºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
+**ç¹å«æ³¨æ** *
+å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»çAPIå¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸æ­£å¼çå¼å®¹ï¼
+*
+è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½æ­£å¼çååè¿è¡pipå®è£ï¼åæ¬¡ä½¿ç¨æ­£å¼çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£æ­£å¼çï¼
+* éè¦ **Python3.8** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼ News/
+ææ°åè½ ------------ ææ°çç tkintertools **å¼åç**(2.6.4-
+dev)æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
+å¨ Windows ç³»ç»ä¸è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
+* æä½é¼ æ å·¦é®æå¨å¯ä»¥æè½¬è¿å¤ä¸ªå ä½ä½ï¼ *
+æä½é¼ æ å³é®æå¨å¯ä»¥ç§»å¨è¿äºå ä½ä½å¨ç©ºé´ä¸­çä½ç½®ï¼ *
+æâ=âåâ-âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼ *
+æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ã
+ä¸é¢æ¯ç¤ºä¾ç¨åºçææå¾ï¼ ![news.png](news.png) æºä»£ç  ```python
+from tkinter import Event import tkintertools as tkt from tkintertools import
+tools_3d as t3d root = tkt.Tk('tool_3d', 1280, 720) cv3d = t3d.Canvas_3D(root,
+1280, 720, 0, 0) origin = t3d.Point(cv3d, [0, 0, 0]) # åç¹ k = -100, 0, 100
+geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white',
+color_down='yellow', color_left='red', color_right='orange',
+color_front='blue', color_back='green') for a in k for b in k for c in k]
+cv3d.space_sort() def translate(event, flag=False, _cache=[]): # type: (Event,
+bool, list[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x,
+event.y] return dx = (event.x - _cache[0]) dy = (event.y - _cache[1]) _cache[:
+] = [event.x, event.y] for geo in geos: geo.translate(0, dx, dy) geo.update()
+origin.translate(0, dx, dy) origin.update() cv3d.space_sort() def rotate(event,
+flag=False, _cache=[]): # type: (Event, bool, list[float]) -> None """
+æè½¬äºä»¶ """ if flag: _cache[:] = [event.x, event.y] return dy = (event.x -
+_cache[0]) / 100 dx = (_cache[1] - event.y) / 100 _cache[:] = [event.x,
+event.y] for item in geos: item.rotate(0, dx, dy, center=origin.coords)
+item.update() cv3d.space_sort() def scale(event): # type: (Event) -> None """
+ç¼©æ¾äºä»¶ """ k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym
+== 'minus' else 1 for geo in geos: geo.scale(k, k, k) geo.update()
+cv3d.space_sort() def scale_center(event): # type: (Event) -> None """
+ä¸­å¿ç¼©æ¾äºä»¶ """ k = 1.05 if event.delta > 0 else 0.95 for geo in geos:
+geo.scale(k, k, k, center=origin.coords) geo.update() cv3d.space_sort()
 root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
 root.bind('', lambda event: translate(event, True)) root.bind('', translate)
-root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
-[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
-- tkintertools æ¯ä¸æ¬¾åºäº tkinter
+root.bind('', scale) root.bind('', scale_center) root.mainloop() ```
+æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼[CHANGELOG.md](CHANGELOG.md) Description/
+æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
 ä½åæ¶ä¹äº§çäºä¸äºç¼ºç¹ï¼ * èæçæ§ä»¶æ æ³è·åç¦ç¹ *
 èæçæ§ä»¶å¨ææ¬è¾å¥åæ¾ç¤ºçåè½ä¸å­å¨ä¸äºç¼ºé·ï¼è¿ä¸ªç¼ºé·ä¸æ¯å¾ææ¾ï¼ä½å¼ºè¿«çå°±æç¹é¾åäºï¼æ¯å¦æï¼
 tkintertools æ¨¡åè¿å·æä¸äºç¹è²çåè½ï¼ * å©ç¨ tkinter å
 tkintertools åå»ºçç¨åºï¼å¨é«åè¾¨ççæåµä¸ï¼tkintertools
 çä¼æ´å æ¸æ°ï¼è¿ç¹å¯¹äºç¬è®°æ¬ç¨æ·å¾åå¥½ï¼æ¯å¦æï¼ *
 å¯ä»¥è¿éå®ç°æ¸åè²çææ *
 çªå£ç¼©æ¾ï¼ææçæ§ä»¶çå¤§å°è·çç¼©æ¾ï¼å½ç¶ï¼ä¹å¯ä»¥è®¾ç½®ä¸ºä¸è·éç¼©æ¾ï¼
-æ³¨æï¼éè¦ **Python3.7** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼
-Provides/æ¨¡ååè½ ------------------- Here, only the more distinctive
-features will be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ###
-Customizable widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
+* å­æ¨¡å tools_3d å¯ä»¥æ¯æ»¡è¶³ç®åç 3D ç»å¾éæ± Provides/
+æ¨¡ååè½ ------------------- Here, only the more distinctive features will
+be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ### Customizable
+widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
 æ¨¡åçæ§ä»¶æ¥æè®¸å¤åæ°ä¾æä»¬è®¾ç½®ï¼æ¯å¦åè§çåå¾ãææ¬åè¾¹æ¡ä»¥åæ§ä»¶åé¨çé¢è²ï¼å³èäºä»¶ç­ç­ã
 è¿éè¦è¯´æçæ¯ï¼æ¯ä¸ªæ§ä»¶å¯ä»¥è®¾ç½®çå³èäºä»¶ä¸æ­¢ä¸ç§ï¼å¨é¼ æ ç»è¿æ§ä»¶æ¶å¯ä»¥ç»å®äºä»¶ï¼é¼ æ ç¹å»æ§ä»¶ä¹å¯ä»¥ï¼é¼ æ ç¹å»åæ¾å¼ä¹è¡ç­ç­ã
 ææ¬åè¾¹æ¡ä»¥åæ§ä»¶çå¡«åè²ä¹æ¯ç±»ä¼¼çï¼å¨é¼ æ ç»è¿æ§ä»¶ãç¹å»æ§ä»¶ãç¹å»åæ¾å¼é½å¯ä»¥è®¾å®é¢è²ã
 ææ¬ç±»æ§ä»¶è¿è½å¤ä»å³è¾¹éæ­¥è¾å¥ææ¬ï¼ææ¬è¾å¥æç¤ºç¬¦ä¹å¯ä»¥ä¸æ¯åè°æ è¶£çç«çº¿ï¼å¯ä»¥æ¯å¶ä»çï¼æ¯å¦ä¸åçº¿ç­ã
-æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](./test.py)
+æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](test.py)
 æä»¶éé¢çç¤ºä¾ï¼è¿ä¸ªç¤ºä¾å±ç¤ºäº tkintertools
 æ¨¡åçç»å¤§é¨ååè½ï¼ç¤ºä¾ä¸­æ´æéèç âå¤å½©åå¹»â
 å½©èå¦ï¼ ### Automatically control size/èªå¨æ§å¶å¤§å° tkintertools
 ä¸­çæ§ä»¶ï¼å¶å¤§å°åå½¢ç¶å¯ä»¥éççªå£çååèææ¯ä¾å°ååï¼ä¸ä»ä»æ¯æ§ä»¶ä¸­çææ¬ï¼Canvas
 ç»å¶çå¾å½¢ä¹ä¼éä¹åå¨ï¼æ´è®©äººå´å¥çæ¯ï¼png
 ç±»åçå¾çä¹ä¼éä¹ææ¯ä¾å°ç¼©æ¾ï¼å½ç¶ï¼ä½ ä¹å¯ä»¥è®¾å®åæ°è®©å¶ä¸éä¹åå¨ï¼ä¹å¯ä»¥è®¾å®åæ°ä½¿å¶å¨ç¼©æ¾çæ¶åä¿ææ¨ªçºµæ¹åçæ¯ä¾ã
 æ»ä¹ï¼å¾æ¹ä¾¿ï¼å¾èéï¼ ### Easily move widgets/è½»æ¾ç§»å¨æ§ä»¶
@@ -92,70 +90,73 @@
 çº§å«è®¾ç½®å½æ°](#DPI) ### Detailed type hints/è¯¦ç»çç±»åæç¤º åè
 [PEP 526](https://peps.python.org/pep-0526/)ã[PEP 586](https://
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
 é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
-[type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
+[type_hint.png](readme_res/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
-tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
-(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
-images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
-internal class and function in the module will be described in detail here
+tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](test.py) å¨
+Windows ç³»ç»ï¼**Windows10**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ !
+[test_windows10.png](readme_res/test_windows10.png) [test.py](test.py) å¨
+Linux ç³»ç»ï¼**Ubuntu22.04**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png]
+(readme_res/test_linux.png) [test.py](test.py) å¨ Windows
+ç³»ç»ï¼**Windows11**ï¼ä¸è¿è¡ççé¢å¦ä¸(æºè½æ§å¶åè§åå¾)ï¼
+![test_windows11.png](readme_res/test_windows11.png) ### 3D Drawing/3Dç»å¾
+è§ [News/ææ°åè½](#news) Contents/æ¨¡ååå®¹ ------------------- Each
+non internal class and function in the module will be described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
-ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](docs/images/LabelTest.png)
+ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](readme_res/LabelTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
 tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
 tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
 tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
-ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](docs/images/
+ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](readme_res/
 ButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk
 ('ButtonTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful
 (x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
 """ for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
 100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
 (canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
 (canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
 (canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
 å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
-ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](docs/images/
+ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](readme_res/
 CheckButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root =
 tkt.Tk('CheckButtonTest', 500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0)
 def colorful(x, y, width, height): # type: (int, int, int, int) -> None """
 Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(40, 190, 420, 50) tkt.CheckButton(canvas, 50, 50, 30,
 text='NormalCheckButton', value=True) tkt.CheckButton(canvas, 50, 100, 30,
 text='DisableCheckButton', value=True).set_live(False) tkt.CheckButton(canvas,
 50, 150, 30, radius=10, text='RoundCornerCheckButton') tkt.CheckButton(canvas,
 50, 200, 30, radius=15, text='TransparentCheckButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
-ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](docs/images/EntryTest.png)
+ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](readme_res/EntryTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
 400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
 100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
 (canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
@@ -166,29 +167,29 @@
 radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
 35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
 tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
 justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
 text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
 root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
-ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](docs/images/TextTest.png)
+ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](readme_res/TextTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
 for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
 Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
 (Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
 text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
 radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
-ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](docs/images/
+ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](readme_res/
 ProgressbarTest.png) æºä»£ç  ```python import tkintertools as tkt root =
 tkt.Tk('ProgressbarTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0)
 def colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None
 """ Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(30, 290, 440, 50) tkt.Progressbar(canvas, 50, 50, 400, 30)
 tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667) tkt.Progressbar(canvas,
@@ -206,15 +207,15 @@
 å¨å¾æå¾å¥½çæ¯æï¼ä»éæå°éä»£ç å³å¯å®ç°å¨å¾çæ¾ç¤ºï¼è¿å¯ä»¥è®¾ç½®å¨å¾æ¾ç¤ºçéåº¦ï¼æ­¤å¤ï¼å¯¹
 png
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
-![MoveTest.gif](docs/images/MoveTest.gif) æºä»£ç  ```python import
+![MoveTest.gif](readme_res/MoveTest.gif) æºä»£ç  ```python import
 tkintertools as tkt root = tkt.Tk('MoveTest', 500, 500) canvas = tkt.Canvas
 (root, 500, 500, 0, 0) rect = canvas.create_rectangle(50, 350, 150, 450) def
 move_window(switch=[True]): # type: (list[bool]) -> None tkt.move(root, None,
 1000 if switch[0] else -1000, 0, 800, mode='flat') switch[0] = not switch[0]
 def move_button(switch=[True]) -> None: # type: (list[bool]) -> None tkt.move
 (canvas, button, 200 if switch[0] else -200, 0, 500, mode='rebound') switch[0]
 = not switch[0] def move_rect(switch=[True]): # type: (list[bool]) -> None
@@ -228,36 +229,35 @@
 å¦ï¼å¾å°ä¸ä¸ª 20 é¿åº¦çå­ç¬¦ä¸² âtkintertoolsâ
     `left`   : "tkintertools        "
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
 ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡ ![ColorTest.png]
-(docs/images/ColorTest.png) ![Test_Draw.png](docs/images/Test_Draw.png)
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
-height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
-tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
-y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
+(readme_res/ColorTest.png) ![Test_Draw.png](readme_res/Test_Draw.png) æºä»£ç 
+```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500, 500)
+canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width, height): #
+type: (int, int, int, int) -> None """ Gradient colors """ for i in range
+(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 = tkt.color
+(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i, y+height,
+fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
 outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
 `askfont`: å­ä½éæ©å¯¹è¯æ¡
 `askfont`å½æ°å¯ä»¥æå¼é»è®¤çå­ä½éæ©çªå£ï¼è¿ä¸ªçªå£è½ç¶æ¯é»è®¤çï¼ä½å®å®éä¸æ æ³å¨`tkinter`ä¸­æå¼ï¼å ä¸º`tkinter`å¹¶æ²¡æå¯¹åºç
 API è½å¤åå°è¿ä¸ç¹ãä½æ¯ï¼`tkintertools`è°ç¨å¹¶å°è£äºåçç
-tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
-[font.png]
-5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
+tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã ![font.png]
+(readme_res/font.png) 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
 è¿ä¸ªå½æ°å®éä¸åªæ¯å¯¹å½æ°`ctypes.WinDLL
 ('shcore').SetProcessDpiAwareness`çä¸ä¸ªç®ååè£ï¼å¶å¼å¯ä¸º 0ã1
 å 2ï¼åå«ä»£è¡¨ç¨åº DPI
 çä¸åçº§å«ï¼é£ä¹ç¼©æ¾ææä¹å°±ä¸åï¼`tkintertools`éæ©çå¼æ¯
 1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ !
-[SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+[SetProcessDpiAwareness_0.png](readme_res/SetProcessDpiAwareness_0.png)
 ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
-![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
+![SetProcessDpiAwareness_1.png](readme_res/SetProcessDpiAwareness_1.png)
 ä»ä¸é¢çä¸¤å¼ å¾ä¸­å¯ä»¥å¾ææ¾ççåºç¬¬ä¸å¼ å¾æ¨¡ç³ï¼ç¬¬äºå¼ å¾æ¸æ°ï¼è¿å°±æ¯
 DPI çº§å«ä¸åçåå ï¼ä¸è¿è¿ä¸ç¹å¨å±å¹ç¼©æ¾æ¯ä¸æ¯ 100%
 çæ¶åæä¼åºç° å¤§å®¶å¯¹ä¸é¢çå¾è¯å®å¾çæï¼è¿ä¸å°±æ¯ IDLE
 åï¼ï¼å¯¹ï¼è¿ä¸ªçé®é¢çè§£å³åæ³ä¹æ¯æ¥èªäº IDLE çæºä»£ç 
 [pyshell.py line 18~20]
 æ³¨æï¼è¯¥å½æ°å¨ç¨åºçä¸åä½ç½®æ§è¡çææä¸ä¸æ ·ï¼ä¸è¬ç¨å¨`mainloop`ä¹åï¼ä½`tkintertools`å·²ç»å¨`mainloop`å½æ°ä¸­åµå¥äºè¯¥å½æ°ï¼æ éåè®¾ç½®ä¸æ¬¡
 DPI çº§å«ï¼æ­¤å½æ°æ¯ä¸ºäºåç`tkinter`ç¨åºç¨çã Examples/
@@ -269,30 +269,33 @@
 bugï¼åªéè¿éè¦æ¹è¿ï¼ ### ä»»å¡æ¸åå°å·¥å· * æç« é¾æ¥: https:
 //xiaokang2022.blog.csdn.net/article/details/128561339 * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/todolist * ç¨åºä¸è½½
 (å«æåå¥½çç¨åºåæºä»£ç ): https://wwc.lanzoum.com/iyxL30kpkcbe *
 æ¨èææ°: ð è¿ä¸ªæ¡ä¾ä½¿ç¨äº tkintertools-v2.5.7
 çæ¬ï¼æ°çå·²æ æ³å¼å®¹ï¼ï¼å«æä¸äº bugï¼å¤§ééç¨äº
 tkintertools çæ§ä»¶ï¼åå¾äºæ¯è¾å¥½ççé¢ææãä½ç°äº
-tkintertools æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨é¢å¼ä¸çç¢¾åæ§ï¼
-[todolist.png] [todolist.png]
-### ä¸­å½è±¡æ£æ¸¸æ * æç« é¾æ¥: https://xiaokang2022.blog.csdn.net/
-article/details/128852029 * ä»£ç ä»åº: https://gitcode.net/weixin_62651706/
-chess * ç¨åºä¸è½½(å«æåå¥½çç¨åºåæºä»£ç ): https://
-wwc.lanzoum.com/iwgp00mlewpa * æ¨èææ°: ðð
+tkintertools æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨é¢å¼ä¸çç¢¾åæ§ï¼ !
+[todolist.gif](https://img-blog.csdnimg.cn/img_convert/
+dc1a598c3f082253c1ebc7bbca0b98ce.gif) ![todolist.gif](https://img-
+blog.csdnimg.cn/img_convert/7f34451deda1af13712a9edcb37f20b4.gif) ###
+ä¸­å½è±¡æ£æ¸¸æ * æç« é¾æ¥: https://xiaokang2022.blog.csdn.net/article/
+details/128852029 * ä»£ç ä»åº: https://gitcode.net/weixin_62651706/chess *
+ç¨åºä¸è½½(å«æåå¥½çç¨åºåæºä»£ç ): https://wwc.lanzoum.com/
+iwgp00mlewpa * æ¨èææ°: ðð
 æ³¨æï¼æºä»£ç æè§£åå¯ç ï¼è§£åå¯ç å¨é¾æ¥æç« ä¸­ï¼è¯·ä»ç»æ¥æ¾ï¼
 è¿ä¸ªæ¡ä¾ä½¿ç¨äº tkintertools-v2.5.9.5 çæ¬ï¼æ°çå·²æ æ³å¼å®¹ï¼,
 å«æå°é bugï¼é¨å UI éç¨äº tkintertoolsï¼é¨å UI éç¨äº
 tkinterï¼å±äºæ··åä½¿ç¨ãä½ç°äº tkintertools æ¨¡åå¯¹ tkinter
-æ¨¡åçå¼å®¹æ§ï¼
-[chess.png] [chess.png]
-### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
-gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
-ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
+æ¨¡åçå¼å®¹æ§ï¼ ![chess.png](https://img-blog.csdnimg.cn/
+43df0568d4b34078a443a098b67c126a.png) ![chess.png](https://img-blog.csdnimg.cn/
+fc768093715d47d7b14bea015a921e3d.png) ### ç®æç»å½çé¢ * æç« é¾æ¥:
+ææ  * ä»£ç ä»åº: https://gitcode.net/weixin_62651706/tester *
+ç¨åºä¸è½½: ææ  * æ¨èææ°: ððð
+è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
-æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
-examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
------- > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
-(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
-(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
-è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png]
+(readme_res/exam3_1.png) ![exam3_2.png](readme_res/exam3_2.png) More/æ´å¤ ---
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > Gitee(Mirror/
+éå): > https://gitee.com/xiaokang-2022/tkintertools > GitCode(Mirror/
+éå): > https://gitcode.net/weixin_62651706/tkintertools
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](tkintertools/) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools-dev-2.6.3/setup.py` & `tkintertools-dev-2.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ 上传 pypi """
 
 import setuptools
 
 
 setuptools.setup(
     name='tkintertools-dev',
-    version="2.6.3",
+    version="2.6.4",
     author='Xiaokang2022',
     license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
     description='An auxiliary module of the tkinder module',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Xiaokang2022/tkintertools',
```

### Comparing `tkintertools-dev-2.6.3/tkintertools/__main__.py` & `tkintertools-dev-2.6.4/tkintertools/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """ Main File """
 
 import math  # 数学支持
 import sys  # DPI 兼容
 import tkinter  # 基础模块
 from fractions import Fraction  # 图片缩放
-from typing import Any, Callable, Generator, Iterable  # 类型提示
-
-try:  # NOTE: 为了兼容 Python3.7，从 typing_extensions 引入 Literal 而不是 typing
-    from typing_extensions import Literal
-except ImportError:
-    pass
+from typing import Any, Callable, Generator, Iterable, Literal, overload
+# 类型提示
 
 if sys.platform == 'win32':  # 仅在 Windows 平台下支持设置 DPI 级别
     from ctypes import WinDLL
 else:
     WinDLL = None
 
 from .constants import *
@@ -45,16 +41,16 @@
         if type(self) == Tk:  # NOTE:方便后面的 Toplevel 类继承
             tkinter.Tk.__init__(self, **kw)
 
         self.width = [100, 1]  # type: list[int]  # [初始宽度, 当前宽度]
         self.height = [100, 1]  # type: list[int]  # [初始高度, 当前高度]
         self._canvas = []  # type: list[Canvas]  # 子画布列表
 
-        if width and height:
-            if x is not None and y is not None:  # BUG: 可能需要修改
+        if width is not None and height is not None:
+            if x is not None and y is not None:
                 self.geometry('%dx%d+%d+%d' % (width, height, x, y))
             else:
                 self.geometry('%dx%d' % (width, height))
 
         self.title(title if title else None)
         self.protocol('WM_DELETE_WINDOW', shutdown if shutdown else None)
         self.bind('<Configure>', lambda _: self.__zoom())  # 开启窗口缩放检测
@@ -74,15 +70,15 @@
         for canvas in self._canvas:
             if canvas.expand and canvas._lock:
                 canvas.zoom(width/self.width[1], height/self.height[1])
 
         self.width[1], self.height[1] = width, height  # 更新窗口当前的宽高值
 
     def wm_geometry(self, newGeometry=None):  # type: (str | None) -> str | None
-        # 重写: 添加修改初始宽高值的功能并兼容不同的DPI缩放
+        # override: 添加修改初始宽高值的功能并兼容不同的DPI缩放
         if newGeometry:
             width, height, _width, _height, * \
                 _ = map(int, (newGeometry+'+0+0').replace('+', 'x').split('x'))
             self.width, self.height = [width]*2, [height]*2
             geometry = '%dx%d+%d+%d' % (width, height, _width, _height)
             if not _:
                 geometry = geometry.split('+')[0]
@@ -198,19 +194,27 @@
         self.bind('<ButtonRelease-1>', self.__release)  # 绑定鼠标左键松开
         self.bind('<<Paste>>', lambda _: self.__paste())  # 绑定粘贴快捷键
 
     def widget(self):  # type: () -> tuple[BaseWidget]
         """ 返回`Canvas`类的`BaseWidget`元组 """
         return tuple(self._widget)
 
+    @overload
+    def lock(self, value):  # type: (bool) -> None
+        ...
+
+    @overload
+    def lock(self):  # type: () -> None
+        ...
+
     def lock(self, value=None):  # type: (bool | None) -> bool | None
         """
-        设置画布锁\n
+        设置或者查询画布锁\n
         ---
-        `value`: 布尔值，True则可操作，False反之，None则返回当前值\n
+        `value`: 布尔值，True则可操作，False反之，无参数或参数为None则返回当前值\n
         """
         if value is None:
             return self._lock
         self._lock = value
         if value and self.expand:
             self.zoom()
 
@@ -321,48 +325,48 @@
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, TextWidget):
                     if widget.paste():
                         return
 
     def create_text(self, *args, **kw):  # type: (...) -> tkinter._CanvasItemId
-        # 重写：添加对 text 类型的 _CanvasItemId 的字体大小的控制
+        # override: 添加对 text 类型的 _CanvasItemId 的字体大小的控制
         font = kw.get('font')
         if not font:
             kw['font'] = FONT, SIZE
         elif isinstance(font, str):
             kw['font'] = font, SIZE
         item = tkinter.Canvas.create_text(self, *args, **kw)
         self._font[item] = list(kw['font'])
         return item
 
     def create_image(self, *args, **kw):  # type: (...) -> tkinter._CanvasItemId
-        # 重写：添加对 image 类型的 _CanvasItemId 的图像大小的控制
+        # override: 添加对 image 类型的 _CanvasItemId 的图像大小的控制
         item = tkinter.Canvas.create_image(self, *args, **kw)
         self._image[item] = [kw.get('image'), None]
         return item
 
     def itemconfigure(
         self,
         tagOrId,  # type: str | tkinter._CanvasItemId
         **kw
     ):  # type: (...) -> dict[str, tuple[str, str, str, str, str]] | None
-        # 重写：创建空 image 的 _CanvasItemId 时漏去对图像大小的控制
+        # override: 创建空 image 的 _CanvasItemId 时漏去对图像大小的控制
         if type(kw.get('image')) == PhotoImage:
             self._image[tagOrId] = [kw.get('image'), None]
         return tkinter.Canvas.itemconfigure(self, tagOrId, **kw)
 
     def place(self, *args, **kw):  # type: (...) -> None  # BUG: 缩放就会恢复原样
-        # 重写：增加一些特定功能
+        # override: 增加一些特定功能
         self.width[0] = kw.get('wdith', self.width[0])
         self.height[0] = kw.get('height', self.height[0])
         return tkinter.Canvas.place(self, *args, **kw)
 
     def destroy(self):  # type: () -> None
-        # 重写：兼容
+        # override: 兼容
         self.master._canvas.remove(self)
         for widget in self.widget():
             widget.destroy()
         return tkinter.Canvas.destroy(self)
 
 
 class BaseWidget:
@@ -518,18 +522,27 @@
 
         if type(font) != str:
             font = list(font)
             font[1] = int(font[1]*math.sqrt(canvas.rx*canvas.ry))
             canvas._font[self.text][1] = font[1]
             canvas.itemconfigure(self.text, font=font)
 
-    # type: (Literal['normal', 'touch', 'click', 'disabled'] | None) -> None
+    @overload
+    def state(self, mode):
+        # type: (Literal['normal', 'touch', 'click', 'disabled']) -> None
+        ...
+
+    @overload
+    def state(self):  # type: () -> None
+        ...
+
     def state(self, mode=None):
+        # type: (Literal['normal', 'touch', 'click', 'disabled'] | None) -> None
         """
-        mode 参数为 None 时仅更新控件，否则改变虚拟控件的外观\n
+        mode参数为None或者无参数时仅更新控件，否则改变虚拟控件的外观\n
         ---
         `normal`: 正常状态\n
         `touch`: 鼠标触碰时的状态\n
         `click`: 鼠标按下时的状态\n
         `disabled`: 禁用状态\n
         """
         if mode:
@@ -606,14 +619,22 @@
         改变控件的位置（以控件左上角为基准）\n
         ---
         `x`: 改变到的横坐标（单位：像素）\n
         `y`: 改变到的纵坐标\n
         """
         self.move(x - self.x1, y - self.y1)
 
+    @overload
+    def configure(self, **kw):  # type: (...) -> None
+        ...
+
+    @overload
+    def configure(self, *args):  # type: (...) -> str | tuple
+        ...
+
     def configure(self, *args, **kw):  # type: (...) -> str | tuple | None
         """
         修改或查询原有参数的值，可供修改或查询的参数有\n
         1. 所有控件: `color_text`、`color_fill`、`color_outline`
         2. 非文本控件: `text`\n
         注意：颜色修改不会立即生效，可通过鼠标经过生效，或者调用 state 方法立即刷新状态！
         """
@@ -662,21 +683,29 @@
             self.master.delete(self._text)
         if isinstance(self, Progressbar):
             self.master.delete(self.bar)
 
         self.master.delete(self.image)
         self.master.delete(self.text)
 
-    def set_live(self, boolean=None):  # type: (bool | None) -> bool | None
+    @overload
+    def set_live(self, value):  # type: (bool) -> None
+        ...
+
+    @overload
+    def set_live(self):  # type: () -> bool
+        ...
+
+    def set_live(self, value=None):  # type: (bool | None) -> bool | None
         """ 设定或查询live值 """
-        if boolean is None:
+        if value is None:
             return self.live
         else:
-            self.live = boolean
-            if boolean:
+            self.live = value
+            if value:
                 self.state('normal')
             else:
                 self.state('disabled')
 
 
 class TextWidget(BaseWidget):
     """ 内部类：文本类控件基类 """
@@ -1016,15 +1045,15 @@
                 self._value[0] = self._value[0][1:]
                 self.master.itemconfigure(self.text, text=self._value[0])
             else:
                 break
 
 
 class Text(TextWidget):
-    """ 创建一个透明的虚拟文本框，用于输入多行文本和显示多行文本（只读模式）"""
+    """ 创建一个透明的虚拟文本框，用于输入多行文本和显示多行文本 """
 
     def __init__(
         self,
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
@@ -1153,15 +1182,15 @@
             _ = self.value.rsplit('\n', 1)[-1]
             self.master.itemconfigure(self._text, text=_)
 
             # 内容未超出框的大小
             if self.value == self.master.itemcget(self.text, 'text'):
                 _pos = self.master.bbox(self._text)
                 self.master.move(self._text, 0, _pos[1] - _pos[3])
-                # NOTE: 为了兼容Python3.7/3.8,放弃使用str.removesuffix方法，以temp取而代之
+                # NOTE: 为了兼容Python3.8,放弃使用str.removesuffix方法，以temp取而代之
                 temp = self.value[:-
                                   len(_)] if self.value.endswith(_) else self.value
                 __ = temp[:-('\n' in self.value)]
             else:  # 内容已经超出框框的大小啦
                 text = self.master.itemcget(self.text, 'text')
                 temp = self.value[:-len(text)
                                   ] if self.value.endswith(text) else self.value
@@ -1337,23 +1366,55 @@
 
     def __new__(cls, *args, **kw):
         if not cls._instance:
             cls._instance = object.__new__(cls)
         return cls._instance
 
 
+@overload
+def move(
+    master,  # type: Tk | Canvas | tkinter.Misc | tkinter.BaseWidget | None
+    widget,  # type: Canvas | BaseWidget | tkinter.BaseWidget
+    dx,  # type: int
+    dy,  # type: int
+    times,  # type: int
+    *,
+    mode,  # type: Literal['smooth', 'rebound', 'flat']
+    frames=FRAMES,  # type: int
+    end=None,  # type: Callable | None
+    _ind=0  # type: int
+):  # type: (...) -> None
+    ...
+
+
+@overload
+def move(
+    master,  # type: Tk | Canvas | tkinter.Misc | tkinter.BaseWidget | None
+    widget,  # type: Canvas | BaseWidget | tkinter.BaseWidget
+    dx,  # type: int
+    dy,  # type: int
+    times,  # type: int
+    *,
+    mode,  # type: tuple[Callable[[float], float], float, float]
+    frames=FRAMES,  # type: int
+    end=None,  # type: Callable | None
+    _ind=0  # type: int
+):  # type: (...) -> None
+    ...
+
+
 def move(
     master,  # type: Tk | Canvas | tkinter.Misc | tkinter.BaseWidget | None
     widget,  # type: Canvas | BaseWidget | tkinter.BaseWidget
     dx,  # type: int
     dy,  # type: int
     times,  # type: int
     *,
-    # type: tuple[Callable[[float], float], float, float] | Literal['smooth', 'rebound', 'flat']  # NOTE
     mode,
+    # type: tuple[Callable[[float], float], float, float] | Literal['smooth', 'rebound', 'flat']
     frames=FRAMES,  # type: int
     end=None,  # type: Callable | None
     _ind=0  # type: int
 ):  # type: (...) -> None
     """
     ### 移动函数
     以特定方式移动由 Place 布局的某个控件或某些控件的集合或图像\n
@@ -1424,14 +1485,30 @@
     elif position == 'right':  # 靠右
         return string+length*' '
     else:  # 居中
         length, key = divmod(length, 2)
         return ' '*length+string+(length+key)*' '
 
 
+@overload
+def color(
+    color,  # type: Iterable[str]
+    proportion=1.  # type: float
+):  # type: (...) -> str
+    ...
+
+
+@overload
+def color(
+    color,  # type: str
+    proportion=1.  # type: float
+):  # type: (...) -> str
+    ...
+
+
 def color(
     color,  # type: Iterable[str] | str
     proportion=1.  # type: float
 ):  # type: (...) -> str
     """
     ### 颜色函数
     按一定比例给出已有 RGB 颜色字符串的渐变 RGB 颜色字符串，或颜色的对比色\n
```

### Comparing `tkintertools-dev-2.6.3/tkintertools/constants.py` & `tkintertools-dev-2.6.4/tkintertools/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 FRAMES = 60
 """ Default move frame rate """
 
 TICK = '✓'
 """ Default checkbox symbol """
 
 
-CFG_3D = 500, None, None
-""" Default 3D configuration """
+CAMERA_DISTANCE = 1000
+""" Default 3D camera distance """
 
 
 COLOR_POINT_FILL = '#000000'
 """ Default point fill color """
 
 COLOR_POINT_OUTLINE = '#000000'
 """ Default point outline color """
@@ -88,10 +88,8 @@
 LINE_WDITH = 1
 """ Default line width """
 
 SIDE_WIDTH = 1
 """ Default side width """
 
 
-if __name__ == '__main__':
-    print(', '.join(name for name in globals()
-          if '__' not in name and name.isupper()))
+__all__ = [name for name in globals() if name.isupper()]
```

### Comparing `tkintertools-dev-2.6.3/tkintertools/tools_3d.py` & `tkintertools-dev-2.6.4/tkintertools/tools_3d.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,95 +4,155 @@
 import statistics  # 数据统计
 from typing import Iterable  # 类型提示
 
 from .__main__ import Canvas, Tk, Toplevel  # 继承和类型提示
 from .constants import *
 
 
+def translate(coords, dx=0, dy=0, dz=0):
+    # type: (list[float], float, float, float) -> None
+    """
+    ### 平移
+    将一个空间三维中的点进行平移\n
+    ---
+    `coords`: 被平移点的空间坐标列表\n
+    `dx`: x方向位移\n
+    `dy`: y方向位移\n
+    `dz`: z方向位移\n
+    """
+    coords[0] += dx
+    coords[1] += dy
+    coords[2] += dz
+
+
+def rotate(coords, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+    # type: (list[float], float, float, float, ..., Iterable[float]) -> None
+    """
+    ### 旋转
+    将一个空间三维中的点以另一个点为旋转中心进行旋转\n
+    ---
+    `coords`: 被旋转点的空间坐标列表\n
+    `dx`: x方向旋转弧度\n
+    `dy`: y方向旋转弧度\n
+    `dz`: z方向旋转弧度\n
+    `center`: 旋转中心的空间坐标列表\n
+    """
+    sx, sy, sz = math.sin(dx), math.sin(dy), math.sin(dz)
+    cx, cy, cz = math.cos(dx), math.cos(dy), math.cos(dz)
+
+    matrix = [[cz*cy, cz*sy*sx-sz*cx, cz*sy*cx+sz*sx],
+              [sz*cy, sz*sy*sx+cz*cx, sz*sy*cx-cz*sx],
+              [-sy,   cy*sx,          cy*cx]]
+
+    for i in range(3):
+        matrix[0][i] = center[i] + \
+            sum(matrix[i][j]*(coords[j]-center[j]) for j in range(3))
+
+    coords[:] = matrix[0]
+
+
+def scale(coords, kx=1, ky=1, kz=1, *, center=None):
+    # type: (list[float], float, float, float, ..., Iterable[float] | None) -> None
+    """
+    ### 缩放
+    将一个空间三维中的点以另一个点为缩放中心进行位置缩放\n
+    ---
+    `coords`: 被缩放点的空间坐标列表\n
+    `dx`: x方向缩放比例\n
+    `dy`: y方向缩放比例\n
+    `dz`: z方向缩放比例\n
+    `center`: 缩放中心的空间坐标列表\n
+    """
+    for i, k in zip(range(3), (kx, ky, kz)):
+        coords[i] += (coords[i] - center[i]) * (k - 1)
+
+
 class Canvas_3D(Canvas):
     """ 3D画布，支持3d绘图 """
 
     def __init__(
         self,
         master,  # type: Tk | Toplevel
         width,  # type: int
         height,  # type: int
         x=None,  # type: int | None
         y=None,  # type: int | None
         *,
         lock=True,  # type: bool
         expand=True,  # type: bool
         keep=True,  # type: bool
-        cfg_3d=CFG_3D,  # type: Iterable[float, float | None, float | None]
+        camera_distance=CAMERA_DISTANCE,  # type: float
+        dx=None,  # type: float | None
+        dy=None,  # type: float | None
         **kw
     ):  # type: (...) -> None
         """
         `master`: 父控件\n
         `width`: 画布宽度\n
         `height`: 画布高度\n
         `x`: 画布左上角的横坐标\n
         `y`: 画布左上角的纵坐标\n
         `lock`: 画布内控件的功能锁，False 时功能暂时失效\n
         `expand`: 画布内控件是否能缩放\n
         `keep`: 画布比例是否保持不变\n
-        `cfg_3d`: 3d绘图的配置，一个包含三个值的列表，[相机距离，横坐标偏移，纵坐标偏移]，默认值相机距离500，图像居中\n
+        `camera_distance`: 3d绘图时相机与原点的距离，默认值为1000\n
+        `dx`: 画面在横坐标方向的偏移，None表示居中\n
+        `dy`: 画面在纵坐标方向的偏移，None表示居中\n
         `**kw`: 与 tkinter.Canvas 类的参数相同\n
         """
         Canvas.__init__(self, master, width, height, x, y,
-                        lock=lock, expand=expand, keep=keep)
-        self.distance = cfg_3d[0]
-        self.dx = width / 2 if cfg_3d[1] is None else cfg_3d[1]
-        self.dy = height / 2 if cfg_3d[2] is None else cfg_3d[2]
-        self._items_3d = []  # type: list[Point | Line | Side | Geometry]
+                        lock=lock, expand=expand, keep=keep, **kw)
+        self.distance = camera_distance
+        self.dx = width / 2 if dx is None else dx
+        self.dy = height / 2 if dy is None else dy
+        self._items_3d = []  # type: list[Point | Line | Side]
+        self._geos = []  # type: list[Geometry]
 
-    def items_3d(self):  # type: () -> tuple[Point | Line | Side | Geometry]
+    def items_3d(self):  # type: () -> tuple[Point | Line | Side]
         """ 返回`Canvas_3d`类的`items_3d`元组 """
         return tuple(self._items_3d)
 
+    def geos(self):  # type: () -> tuple[Geometry]
+        """ 返回`Canvas_3d`类的`geos`元组 """
+        return tuple(self._geos)
+
+    def space_sort(self):  # type: () -> None
+        """ 空间位置排序 """
+        items = [item for item in self._items_3d]
+        items.sort(key=lambda item: item.camera_distance())
+        for item in items:
+            self.lower(item.item)
+
 
-class _Point:
+class _Point():
     """ 点 """
 
     def __init__(self, coords):  # type: (list[float]) -> None
         self.coords = coords  # 利用列表引用
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """ 平移 """
-        self.coords[0] += dx
-        self.coords[1] += dy
-        self.coords[2] += dz
+        translate(self.coords, dx, dy, dz)
 
     def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
         """ 旋转 """
-        sx, sy, sz = math.sin(dx), math.sin(dy), math.sin(dz)
-        cx, cy, cz = math.cos(dx), math.cos(dy), math.cos(dz)
-
-        matrix = [[cz*cy, cz*sy*sx-sz*cx, cz*sy*cx+sz*sx],
-                  [sz*cy, sz*sy*sx+cz*cx, sz*sy*cx-cz*sx],
-                  [-sy,   cy*sx,          cy*cx]]
-
-        for i in range(3):
-            matrix[0][i] = center[i] + \
-                sum(matrix[i][j]*(self.coords[j]-center[j]) for j in range(3))
-
-        self.coords[:] = matrix[0]
+        rotate(self.coords, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         """ 缩放 """
-        for i, k in zip(range(3), (kx, ky, kz)):
-            self.coords[i] += (self.coords[i] - center[i]) * (k - 1)
+        scale(self.coords, kx, ky, kz, center=center)
 
     def project(self, distance):  # type: (float) -> list[float]
         """ 投影 """
         try:
             k = distance/(distance - self.coords[0])
         except ZeroDivisionError:
-            return [distance, distance]
+            return [distance*10, distance*10]
         return [self.coords[1]*k, self.coords[2]*k]
 
 
 class _Line:
     """ 线 """
 
     def __init__(
@@ -101,30 +161,30 @@
         point2,  # type: list[float]
     ):  # type: (...) -> None
         self.coords = [point1, point2]
         self.points = [_Point(point) for point in self.coords]
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """ 平移 """
-        for point in self.points:
-            point.translate(dx, dy, dz)
+        for coord in self.coords:
+            translate(coord, dx, dy, dz)
 
     def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
         """ 旋转 """
-        for point in self.points:
-            point.rotate(dx, dy, dz, center=center)
+        for coord in self.coords:
+            rotate(coord, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         """ 缩放 """
         if center is None:
             center = [statistics.mean(axis) for axis in zip(*self.coords)]
-        for point in self.points:
-            point.scale(kx, ky, kz, center=center)
+        for coord in self.coords:
+            scale(coord, kx, ky, kz, center=center)
 
     def project(self, distance):  # type: (float) -> list[list[float]]
         """ 投影 """
         return [point.project(distance) for point in self.points]
 
 
 class _Side:
@@ -133,30 +193,30 @@
     def __init__(self, *points):  # type: (list[float]) -> None
         self.coords = list(points)
         self.lines = [_Line(points[ind-1], points[ind])
                       for ind in range(len(points))]
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """ 平移 """
-        for point in set(point for line in self.lines for point in line.points):
-            point.translate(dx, dy, dz)
+        for coord in self.coords:
+            translate(coord, dx, dy, dz)
 
     def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
         """ 旋转 """
-        for point in set(point for line in self.lines for point in line.points):
-            point.rotate(dx, dy, dz, center=center)
+        for coord in self.coords:
+            rotate(coord, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         """ 缩放 """
         if center is None:
             center = [statistics.mean(axis) for axis in zip(*self.coords)]
-        for point in set(point for line in self.lines for point in line.points):
-            point.scale(kx, ky, kz, center=center)
+        for coord in self.coords:
+            scale(coord, kx, ky, kz, center=center)
 
     def project(self, distance):  # type: (float) -> list[list[list[float]]]
         """ 投影 """
         return [line.project(distance) for line in self.lines]
 
 
 class Point(_Point):
@@ -195,14 +255,18 @@
         x, y = self.project(self.canvas.distance)
         kx, ky = self.canvas.rx, self.canvas.ry
         x += self.canvas.dx
         y += self.canvas.dy
         self.canvas.coords(
             self.item, (x-self.size)*kx, (y-self.size)*ky, (x+self.size)*kx, (y+self.size)*ky)
 
+    def camera_distance(self):  # type: () -> float
+        """ 与相机距离 """
+        return math.hypot(self.canvas.distance-self.coords[0], self.coords[1], self.coords[2])
+
 
 class Line(_Line):
     """ 线 """
 
     def __init__(
         self,
         canvas,  # type: Canvas_3D
@@ -233,14 +297,18 @@
         data = self.project(self.canvas.distance)
         for point in data:
             point[0] += self.canvas.dx
             point[1] += self.canvas.dy
         self.canvas.coords(
             self.item, *[coord*(ky if i else kx) for point in data for i, coord in enumerate(point)])
 
+    def camera_distance(self):  # type: () -> float
+        """ 与相机距离 """
+        return statistics.mean(math.hypot(self.canvas.distance-coord[0], coord[1], coord[2]) for coord in self.coords)
+
 
 class Side(_Side):
     """ 面 """
 
     def __init__(
         self,
         canvas,  # type: Canvas_3D
@@ -258,81 +326,90 @@
         """
         _Side.__init__(self, *points)
         canvas._items_3d.append(self)
         self.canvas = canvas
         self.width = width
         self.fill = fill
         self.outline = outline
-        self.item = canvas.create_polygon(-1, -1, -1, -1,
-                                          width=width, fill=fill, outline=outline)
+        self.item = canvas.create_polygon(
+            -1, -1, -1, -1, width=width, fill=fill, outline=outline)
         self.update()
 
     def update(self) -> None:
         """ 更新 """
         kx, ky = self.canvas.rx, self.canvas.ry
         data = self.project(self.canvas.distance)
         for line in data:
             for point in line:
                 point[0] += self.canvas.dx
                 point[1] += self.canvas.dy
         self.canvas.coords(
             self.item, *[coord*(ky if i else kx) for line in data for point in line for i, coord in enumerate(point)])
 
+    def camera_distance(self):  # type: () -> float
+        """ 与相机距离 """
+        return statistics.mean(math.hypot(self.canvas.distance-coord[0], coord[1], coord[2]) for coord in self.coords)
+
 
 class Geometry:
     """ 几何体 """
 
     def __init__(self, canvas, *sides):  # type: (Canvas_3D, _Side) -> None
         """
         `canvas`: 显示的画布\n
         `sides`: 平面类`Side`\n
         """
-        canvas._items_3d.append(self)
+        canvas._geos.append(self)
         self.canvas = canvas
         self.coords = []  # type: list[list[float]]
         self.sides = []  # type: list[Side]
         if sides:
             self.append(*sides)
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """
         平移\n
         `dx`: x轴方向位移距离\n
         `dy`: y轴方向位移距离\n
         `dz`: z轴方向位移距离\n
         """
-        for point in set(point for side in self.sides for line in side.lines for point in line.points):
-            point.translate(dx, dy, dz)
+        coords = [coord for side in self.sides for coord in side.coords]
+        for ind, coord in enumerate(coords):
+            if coord not in coords[:ind]:
+                translate(coord, dx, dy, dz)
 
     def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
         """
         旋转\n
         `dx`: 绕x轴方向旋转角度\n
         `dy`: 绕y轴方向旋转角度\n
         `dz`: 绕z轴方向旋转角度\n
         `center`: 旋转中心\n
         """
-        for point in set(point for side in self.sides for line in side.lines for point in line.points):
-            point.rotate(dx, dy, dz, center=center)
+        coords = [coord for side in self.sides for coord in side.coords]
+        for ind, coord in enumerate(coords):
+            if coord not in coords[:ind]:
+                rotate(coord, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         """
         缩放\n
         `kx`: x轴方向缩放比例\n
         `ky`: y轴方向缩放比例\n
         `kz`: z轴方向缩放比例\n
         `center`: 缩放中心，默认为几何中心\n
         """
-        if center is None:
-            # NOTE: 对凹面几何体无效
+        if center is None:  # NOTE: 对凹面几何体无效
             center = [statistics.mean(axis) for axis in zip(*self.coords)]
-        for point in set(point for side in self.sides for line in side.lines for point in line.points):
-            point.scale(kx, ky, kz, center=center)
+        coords = [coord for side in self.sides for coord in side.coords]
+        for ind, coord in enumerate(coords):
+            if coord not in coords[:ind]:
+                scale(coord, kx, ky, kz, center=center)
 
     def update(self):  # type: () -> None
         """ 更新几何体 """
         for side in self.sides:
             side.update()
 
     def append(self, *sides):  # type: (Side) -> None
@@ -356,64 +433,87 @@
         canvas,  # type: Canvas_3D
         x,  # type: float
         y,  # type: float
         z,  # type: float
         length,  # type: float
         width,  # type: float
         height,  # type: float
+        *,
+        color_up='',  # type: str
+        color_down='',  # type: str
+        color_left='',  # type: str
+        color_right='',  # type: str
+        color_front='',  # type: str
+        color_back='',  # type: str
     ):  # type: (...) -> None
         """
         `canvas`: 父画布\n
         `x`: 左上角x坐标\n
         `y`: 左上角y坐标\n
         `z`: 左上角z坐标\n
         `length`: 长度\n
         `width`: 宽度\n
         `height`: 高度\n
+        `color_up`: 上表面颜色\n
+        `color_down`: 下表面颜色\n
+        `color_left`: 左侧面颜色\n
+        `color_right`: 右侧面颜色\n
+        `color_front`: 正面颜色\n
+        `color_back`: 后面颜色\n
         """
         self.canvas = canvas
         self.coords = [[x+l, y+w, z+h]
                        for l in (0, length)
                        for w in (0, width)
                        for h in (0, height)]
         self.sides = [
             Side(canvas, self.coords[0], self.coords[1],
-                 self.coords[3], self.coords[2]),
+                 self.coords[3], self.coords[2], fill=color_back),
             Side(canvas, self.coords[0], self.coords[1],
-                 self.coords[5], self.coords[4]),
+                 self.coords[5], self.coords[4], fill=color_left),
             Side(canvas, self.coords[0], self.coords[2],
-                 self.coords[6], self.coords[4]),
+                 self.coords[6], self.coords[4], fill=color_up),
             Side(canvas, self.coords[1], self.coords[3],
-                 self.coords[7], self.coords[5]),
+                 self.coords[7], self.coords[5], fill=color_down),
             Side(canvas, self.coords[2], self.coords[3],
-                 self.coords[7], self.coords[6]),
+                 self.coords[7], self.coords[6], fill=color_right),
             Side(canvas, self.coords[4], self.coords[5],
-                 self.coords[7], self.coords[6]),
+                 self.coords[7], self.coords[6], fill=color_front),
         ]
 
 
 class Tetrahedron(Geometry):
     """ 四面体 """
 
     def __init__(
         self,
         canvas,  # type: Canvas_3D
         p1,  # type: Iterable[float]
         p2,  # type: Iterable[float]
         p3,  # type: Iterable[float]
         p4,  # type: Iterable[float]
+        *,
+        colors=('',)*4  # type: Iterable[str]
     ):  # type: (...) -> None
         """
         `canvas`: 父画布\n
         `p1`: 第一个顶点\n
         `p2`: 第二个顶点\n
         `p3`: 第三个顶点\n
         `p4`: 第四个顶点\n
+        `colors`: 颜色序列\n
         """
         self.canvas = canvas
         self.coords = [list(p1), list(p2), list(p3), list(p4)]
         self.sides = [
-            Side(canvas, self.coords[0], self.coords[1], self.coords[2]),
-            Side(canvas, self.coords[0], self.coords[1], self.coords[3]),
-            Side(canvas, self.coords[0], self.coords[2], self.coords[3]),
-            Side(canvas, self.coords[1], self.coords[2], self.coords[3]),
+            Side(canvas, self.coords[0], self.coords[1],
+                 self.coords[2], fill=colors[0]),
+            Side(canvas, self.coords[0], self.coords[1],
+                 self.coords[3], fill=colors[1]),
+            Side(canvas, self.coords[0], self.coords[2],
+                 self.coords[3], fill=colors[2]),
+            Side(canvas, self.coords[1], self.coords[2],
+                 self.coords[3], fill=colors[3]),
         ]
+
+
+__all__ = [name for name in globals() if '__' not in name]
```

### Comparing `tkintertools-dev-2.6.3/tkintertools_dev.egg-info/PKG-INFO` & `tkintertools-dev-2.6.4/tkintertools_dev.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: tkintertools-dev
-Version: 2.6.3
+Version: 2.6.4
 Summary: An auxiliary module of the tkinder module
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
-        src="./tkintertools.png" />
+        src="tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
-        <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
+        <a href="tkintertools/__init__.py">
+            <img src="https://img.shields.io/badge/Version-2.6.4(dev)-blue" alt="latest version" />
         </a>
-        <a href="./LICENSE">
+        <a href="LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
-        <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/06/06-orange" alt="ChangeLog" />
+        <a href="CHANGELOG.md">
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/11-orange" alt="ChangeLog" />
         </a>
-        <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
+        <a href="TODO.md">
+            <img src="https://img.shields.io/badge/ToDos-14-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
+            <img src="https://img.shields.io/badge/Downloads-4k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
@@ -46,152 +46,144 @@
         <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
     </p>
 </div>
 
 Installation/模块安装
------------------------
+--------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/30
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/07
 
 ```
-pip install tkintertools==2.6.2
-```
+pip install tkintertools==2.6.3
 或者
-```
 pip install tkintertools
 ```
 
-这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
-稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
+这个是目前的最新稳定版，比较稳定，bug （可能）没有那么多，推荐使用这个。  
+关于稳定版有 Issue 的话，我会去查看并尝试解决 Issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.3
-* Release Date/发布日期 : 2023/06/06
+* Version/版本 : 2.6.4
+* Release Date/发布日期 : 2023/06/11
 
 ```
-pip install tkintertools-dev==2.6.3
+pip install tkintertools-dev==2.6.4
+或者
+pip install tkintertools-dev
 ```
 
-这个是我正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
-开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
-
-News/最新功能
-------------
-
-最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
-同时修复一些bug，优化了一部分代码，提升了一部分性能。
+这个是我正在开发的版本，可能有新功能，bug 也可能会比较多，但也可能会比原来的版本更加稳定。  
+大家可以在 Issue 中提出一些建议，我会适当采纳一些并在开发版本中更改或实现。
 
-通过以下代码来使用3d绘图功能：
+**特别注意**
+* 开发版仅作示例，各函数或类的API并非最终确定结果，直接使用开发版可能导致后续无法与正式版兼容！
+* 若要使用开发版，请先卸载正式版后再进行pip安装，再次使用正式版时也是一样，先卸载开发版再安装正式版！
+* 需要 **Python3.8** 及更高版本才能运行 tkintertools！
 
-```python
-from tkintertools import tools_3d as t3d
-import tkintertools.tools_3d as t3d
-# 两种引入方式都可以
-```
+<a name="news">News/最新功能</a>
+------------
 
-子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+最新版的 tkintertools **开发版**(2.6.4-dev)新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
 
-目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
-以下是一个使用3d绘图的示例：
+在 Windows 系统下运行下面的示例程序时，其拥有以下功能：
+* 按住鼠标左键拖动可以旋转这多个几何体；
+* 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
+* 按“=”和“-”键分别可以放大和缩小几何体的大小；
+* 滚动鼠标中键可以放大和缩小画面。
 
-在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
-x、y 和 z 轴分别是红色、绿色和蓝色的线。
+下面是示例程序的效果图：
 
-![3d绘图](./docs/images/3d.png)
+![news.png](news.png)
 
 <details><summary><b>源代码</b></summary>
 
 ```python
-import random
-import tkinter
+from tkinter import Event
 
 import tkintertools as tkt
 from tkintertools import tools_3d as t3d
 
-root = tkt.Tk('tools_3d', 1280, 720)
-canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+root = tkt.Tk('tool_3d', 1280, 720)
+cv3d = t3d.Canvas_3D(root, 1280, 720, 0, 0)
 
-geos = []  # type: list[t3d.Geometry]
-origin = t3d.Point(canvas, [0, 0, 0], size=5)  # 原点
-axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'),  # 创建坐标轴
-        t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3, fill='green'),
-        t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
-
-for _ in range(8):
-    # 创建正方体
-    cube = t3d.Cuboid(
-        canvas, *random.sample(range(-200, 200), 3), *random.sample(range(50, 100), 3))
-    geos.append(cube)
-    # 创建四面体
-    x, y, z = random.sample(range(-200, 200), 3)
-    tetr = t3d.Tetrahedron(
-        canvas, *[[x+random.randint(-100, 100), y+random.randint(-100, 100), z+random.randint(-100, 100)] for _ in range(4)])
-    geos.append(tetr)
+origin = t3d.Point(cv3d, [0, 0, 0])  # 原点
+k = -100, 0, 100
+geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white', color_down='yellow', color_left='red',
+                   color_right='orange', color_front='blue', color_back='green') for a in k for b in k for c in k]
+cv3d.space_sort()
 
 
 def translate(event, flag=False, _cache=[]):
-    # type: (tkinter.Event, bool, list[float]) -> None
+    # type: (Event, bool, list[float]) -> None
     """ 平移事件 """
     if flag:
         _cache[:] = [event.x, event.y]
         return
-    dx = (event.x - _cache[0]) / 6
-    dy = (event.y - _cache[1]) / 6
+    dx = (event.x - _cache[0])
+    dy = (event.y - _cache[1])
     _cache[:] = [event.x, event.y]
-    for axis in axes:
-        axis.translate(0, 6*dx, 6*dy)
-        axis.update()
     for geo in geos:
         geo.translate(0, dx, dy)
         geo.update()
-    origin.translate(0, 6*dx, 6*dy)
+    origin.translate(0, dx, dy)
     origin.update()
+    cv3d.space_sort()
 
 
-def rotate(event, flag=False, _cache=[]):  # type: (tkinter.Event, bool, list[float]) -> None
+def rotate(event, flag=False, _cache=[]):
+    # type: (Event, bool, list[float]) -> None
     """ 旋转事件 """
     if flag:
         _cache[:] = [event.x, event.y]
         return
-    dy = (event.x - _cache[0]) / 200
-    dx = (_cache[1] - event.y) / 200
+    dy = (event.x - _cache[0]) / 100
+    dx = (_cache[1] - event.y) / 100
     _cache[:] = [event.x, event.y]
-    for axis in axes:
-        axis.rotate(0, 6*dx, 6*dy, center=origin.coords)
-        axis.update()
-    for geo in geos:
-        geo.rotate(0, dx, dy, center=origin.coords)
-        geo.update()
+    for item in geos:
+        item.rotate(0, dx, dy, center=origin.coords)
+        item.update()
+    cv3d.space_sort()
 
 
-def scale(event):  # type: (tkinter.Event) -> None
+def scale(event):  # type: (Event) -> None
     """ 缩放事件 """
-    k = 1.01 if event.delta > 0 else 0.99
+    k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1
     for geo in geos:
         geo.scale(k, k, k)
         geo.update()
+    cv3d.space_sort()
+
+
+def scale_center(event):  # type: (Event) -> None
+    """ 中心缩放事件 """
+    k = 1.05 if event.delta > 0 else 0.95
+    for geo in geos:
+        geo.scale(k, k, k, center=origin.coords)
+        geo.update()
+    cv3d.space_sort()
 
 
 root.bind('<Button-1>', lambda event: rotate(event, True))
 root.bind('<B1-Motion>', rotate)
 root.bind('<Button-3>', lambda event: translate(event, True))
 root.bind('<B3-Motion>', translate)
-root.bind('<MouseWheel>', scale)
+root.bind('<Any-Key>', scale)
+root.bind('<MouseWheel>', scale_center)
 root.mainloop()
 ```
 
 </details>
 
-更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+更多更新信息请见：[CHANGELOG.md](CHANGELOG.md)
 
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
@@ -204,30 +196,29 @@
 * 虚拟的控件在文本输入和显示的功能上存在一些缺陷（这个缺陷不是很明显，但强迫症就有点难受了，比如我）
 
 tkintertools 模块还具有一些特色的功能：
 
 * 利用 tkinter 和 tkintertools 创建的程序，在高分辨率的情况下，tkintertools 的会更加清晰（这点对于笔记本用户很友好，比如我）
 * 可以迅速实现渐变色的效果
 * 窗口缩放，所有的控件的大小跟着缩放（当然，也可以设置为不跟随缩放）
-
-注意：需要 **Python3.7** 及更高版本才能运行 tkintertools！
+* 子模块 tools_3d 可以是满足简单的 3D 绘图需求
 
 Provides/模块功能
 -------------------
 
 Here, only the more distinctive features will be listed  
 这里只会列举出比较具有特色的功能
 
 ### Customizable widgets/可自定义的控件
 
 tkintertools 模块的控件拥有许多参数供我们设置，比如圆角的半径、文本和边框以及控件内部的颜色，关联事件等等。  
 这里要说明的是，每个控件可以设置的关联事件不止一种，在鼠标经过控件时可以绑定事件，鼠标点击控件也可以，鼠标点击后松开也行等等。  
 文本和边框以及控件的填充色也是类似的，在鼠标经过控件、点击控件、点击后松开都可以设定颜色。  
 文本类控件还能够从右边逐步输入文本，文本输入提示符也可以不是单调无趣的竖线，可以是其他的，比如下划线等。  
-最后，大家可以看一下 [test.py](./test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
+最后，大家可以看一下 [test.py](test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
 
 ### Automatically control size/自动控制大小
 
 tkintertools 中的控件，其大小和形状可以随着窗口的变化而成比例地变化，不仅仅是控件中的文本，Canvas 绘制的图形也会随之变动，更让人兴奋的是，png 类型的图片也会随之成比例地缩放！当然，你也可以设定参数让其不随之变动，也可以设定参数使其在缩放的时候保持横纵方向的比例。  
 总之，很方便，很舒适！
 
 ### Easily move widgets/轻松移动控件
@@ -243,27 +234,35 @@
 见 [DPI 级别设置函数](#DPI)
 
 ### Detailed type hints/详细的类型提示
 
 参考 [PEP 526](https://peps.python.org/pep-0526/)、[PEP 586](https://peps.python.org/pep-0586/)、[PEP 604](https://peps.python.org/pep-0604/) 和 [PEP 612](https://peps.python.org/pep-0612/)，我采用了最兼容的方式去实现详细的类型提示，可适用 IDE 有 VScode、Pycharm 等。  
 那什么是类型提示呢？话不多说，直接看图就行：
 
-![type_hint.png](docs/images/type_hint_vscode.png)
+![type_hint.png](readme_res/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
-[test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
+[test.py](test.py) 在 Windows 系统（**Windows10**）上运行的界面如下：
+
+![test_windows10.png](readme_res/test_windows10.png)
 
-![test_win32.png](docs/images/test_win32.png)
+[test.py](test.py) 在 Linux 系统（**Ubuntu22.04**）上运行的界面如下：
 
-[test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
+![test_linux.png](readme_res/test_linux.png)
 
-![test_linux.png](docs/images/test_linux.png)
+[test.py](test.py) 在 Windows 系统（**Windows11**）上运行的界面如下(智能控制圆角半径)：
+
+![test_windows11.png](readme_res/test_windows11.png)
+
+### 3D Drawing/3D绘图
+
+见 [News/最新功能](#news)
 
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
@@ -284,15 +283,15 @@
 ### Virtual Canvas Widget/虚拟画布控件
 
 1. `Label`: 标签控件
 
     标签控件的功能和`tkinter.Label`的功能类似，但更加的多元化  
     下面是`Label`控件的外观：  
 
-    ![LabelTest.png](docs/images/LabelTest.png)
+    ![LabelTest.png](readme_res/LabelTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
@@ -319,15 +318,15 @@
     </details>
 
 2. `Button`: 按钮控件
 
     按钮控件相较于`tkinter.Button`，其自由度更高，`tkinter.Button`只有在按下的时候才能触发绑定的关联事件，而`Button`却可以在鼠标移至按钮上方时、鼠标按下时、鼠标松开时都可以绑定关联事件  
     下面是`Button`控件的外观：
 
-    ![ButtonTest.png](docs/images/ButtonTest.png)
+    ![ButtonTest.png](readme_res/ButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
@@ -354,15 +353,15 @@
     </details>
 
 3. `CheckButton`: 复选框控件
 
     复选框控件相对于`tkinter`原生的`tkinter.CheckButton`在使用方面更加地简单，同时颜值也上升了不少  
     下面是`CheckButton`控件的外观：
 
-    ![CheckButtonTest.png](docs/images/CheckButtonTest.png)
+    ![CheckButtonTest.png](readme_res/CheckButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
@@ -390,15 +389,15 @@
     </details>
 
 4. `Entry`: 输入框控件
 
     输入框控件可以轻松地设置输入的文本位置（靠左、居中和靠右），同时，它可以在鼠标移至输入框上方、鼠标未在输入框上方两种状态显示不同的默认文本  
     下面是`Entry`控件的外观：
 
-    ![EntryTest.png](docs/images/EntryTest.png)
+    ![EntryTest.png](readme_res/EntryTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
@@ -436,15 +435,15 @@
     </details>
 
 5. `Text`: 文本框控件
 
     文本框类似于输入框，这里就不再赘述  
     下面是`Text`控件的外观：
 
-    ![TextTest.png](docs/images/TextTest.png)
+    ![TextTest.png](readme_res/TextTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
@@ -472,15 +471,15 @@
     </details>
 
 6. `Progressbar`: 进度条控件
 
     进度条控件相比`tkinter.ttk.Progressbar`，外观上的自由度较大  
     下面是`Progressbar`控件的外观：
 
-    ![ProgressbarTest.png](docs/images/ProgressbarTest.png)
+    ![ProgressbarTest.png](readme_res/ProgressbarTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
@@ -534,15 +533,15 @@
 
 ### Tool Function/工具函数
 
 1. `move`: <a name="move">移动函数</a>
 
     移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！
 
-    ![MoveTest.gif](docs/images/MoveTest.gif)
+    ![MoveTest.gif](readme_res/MoveTest.gif)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
@@ -588,17 +587,17 @@
     `right`  : "        tkintertools"</pre>
 
 3. `color`: <a name="Gradient">颜色函数</a>
 
     颜色函数可以轻松求出一个颜色到另外一个颜色的过渡颜色，因此可以轻松得到渐变色的效果，同时，改变传入的参数还可以得到传入颜色的对比色  
     第二张图是 test.py 在图像测试中绘制的图案
 
-    ![ColorTest.png](docs/images/ColorTest.png)
+    ![ColorTest.png](readme_res/ColorTest.png)
 
-    ![Test_Draw.png](docs/images/Test_Draw.png)
+    ![Test_Draw.png](readme_res/Test_Draw.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
@@ -621,26 +620,26 @@
 
     </details>
 
 4. `askfont`: 字体选择对话框
 
     `askfont`函数可以打开默认的字体选择窗口，这个窗口虽然是默认的，但它实际上无法在`tkinter`中打开，因为`tkinter`并没有对应的 API 能够做到这一点。但是，`tkintertools`调用并封装了原生的 tcl 的命令，使得字体选择框能够被我们使用。
 
-    <p><img width="540px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/font.png" alt="font.png" /></p>
+    ![font.png](readme_res/font.png)
 
 5. `SetProcessDpiAwareness`: <a name="DPI">DPI 级别设置函数</a>
 
     这个函数实际上只是对函数`ctypes.WinDLL('shcore').SetProcessDpiAwareness`的一个简单包装，其值可为 0、1 和 2，分别代表程序 DPI 的不同级别，那么缩放效果也就不同，`tkintertools`选择的值是 1，但程序默认值实际为 0  
     下面是未执行这个函数的效果
     
-    ![SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+    ![SetProcessDpiAwareness_0.png](readme_res/SetProcessDpiAwareness_0.png)
 
     <p>下面是执行了这个函数的效果</p>
 
-    ![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
+    ![SetProcessDpiAwareness_1.png](readme_res/SetProcessDpiAwareness_1.png)
 
     从上面的两张图中可以很明显的看出第一张很模糊，第二张很清晰，这就是 DPI 级别不同的原因，不过这一点在屏幕缩放比不是 100% 的时候才会出现  
     大家对上面的图肯定很熟悉，这不就是 IDLE 吗！？对，这个的问题的解决办法也是来自于 IDLE 的源代码 [pyshell.py line 18~20]  
     注意：该函数在程序的不同位置执行的效果不一样！一般用在`mainloop`之前，但`tkintertools`已经在`mainloop`函数中嵌入了该函数，无需再设置一次 DPI 级别，此函数是为了原生`tkinter`程序用的。
 
 Examples/实战示例
 ----------------
@@ -654,52 +653,51 @@
 * 文章链接: https://xiaokang2022.blog.csdn.net/article/details/128561339
 * 代码仓库: https://gitcode.net/weixin_62651706/todolist
 * 程序下载(含打包好的程序和源代码): https://wwc.lanzoum.com/iyxL30kpkcbe
 * 推荐指数: 👍
 
 这个案例使用了 tkintertools-v2.5.7 版本（新版已无法兼容），含有一些 bug，大量采用了 tkintertools 的控件，取得了比较好的界面效果。体现了 tkintertools 模块与 tkinter 模块相比在颜值上的碾压性！
 
-<p>
-    <img width="720px" src="https://img-blog.csdnimg.cn/img_convert/dc1a598c3f082253c1ebc7bbca0b98ce.gif" alt="todolist.png"/>
-    <img width="720px" src="https://img-blog.csdnimg.cn/img_convert/7f34451deda1af13712a9edcb37f20b4.gif" alt="todolist.png"/>
-</p>
+![todolist.gif](https://img-blog.csdnimg.cn/img_convert/dc1a598c3f082253c1ebc7bbca0b98ce.gif)
+
+![todolist.gif](https://img-blog.csdnimg.cn/img_convert/7f34451deda1af13712a9edcb37f20b4.gif)
 
 ### 中国象棋游戏
 
 * 文章链接: https://xiaokang2022.blog.csdn.net/article/details/128852029
 * 代码仓库: https://gitcode.net/weixin_62651706/chess
 * 程序下载(含打包好的程序和源代码): https://wwc.lanzoum.com/iwgp00mlewpa
 * 推荐指数: 👍👍
 
 注意：源代码有解压密码，解压密码在链接文章中，请仔细查找！  
 这个案例使用了 tkintertools-v2.5.9.5 版本（新版已无法兼容）, 含有少量 bug，部分 UI 采用了 tkintertools，部分 UI 采用了 tkinter，属于混合使用。体现了 tkintertools 模块对 tkinter 模块的兼容性！
 
-<p>
-    <img height="640px" src="https://img-blog.csdnimg.cn/43df0568d4b34078a443a098b67c126a.png" alt="chess.png"/>
-    <img height="640px" src="https://img-blog.csdnimg.cn/fc768093715d47d7b14bea015a921e3d.png" alt="chess.png"/>
-</p>
+![chess.png](https://img-blog.csdnimg.cn/43df0568d4b34078a443a098b67c126a.png)
+
+![chess.png](https://img-blog.csdnimg.cn/fc768093715d47d7b14bea015a921e3d.png)
 
 ### 简易登录界面
 
 * 文章链接: 暂无
 * 代码仓库: https://gitcode.net/weixin_62651706/tester
 * 程序下载: 暂无
 * 推荐指数: 👍👍👍
 
 这个案例使用了最新稳定版的 tkintertools-v2.6.0，界面非常稳定，几乎没有 bug，完全采用 tkintertools 的控件，颜值很高，界面非常流畅。体现了 tkintertools 模块与 tkinter 模块相比在性能上的优越性！
 
-![exam3_1.png](docs/examples/exam3_1.png)
-![exam3_2.png](docs/examples/exam3_2.png)
+![exam3_1.png](readme_res/exam3_1.png)
+
+![exam3_2.png](readme_res/exam3_2.png)
 
 More/更多
 ---------
 
 > GitHub:  
 > https://github.com/Xiaokang2022/tkintertools
 
-> GitCode(Mirror/镜像):  
-> https://gitcode.net/weixin_62651706/tkintertools
-
 > Gitee(Mirror/镜像):  
 > https://gitee.com/xiaokang-2022/tkintertools
 
-还有更多内容请在 [源代码](./tkintertools/) 中探索！
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
+
+还有更多内容请在 [源代码](tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,96 +1,94 @@
-Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.3 Summary: An
+Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.4 Summary: An
 auxiliary module of the tkinder module Home-page: https://github.com/
 Xiaokang2022/tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2
 (MulanPSL-2.0) Classifier: Operating System :: OS Independent Description-
 Content-Type: text/markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
-Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
-``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
+* Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/07 ``` pip
+install tkintertools==2.6.3 æè pip install tkintertools ```
 è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
-æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
-issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/06
-``` pip install tkintertools-dev==2.6.3 ```
-è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
-å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
-ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-News/ææ°åè½ -----------
--
-ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
-åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
-éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
-tools_3d as t3d import tkintertools.tools_3d as t3d #
-ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
-tools_3d.py)
-ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
-ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
-å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
-xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
-images/3d.png) æºä»£ç  ```python import random import tkinter import
-tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
-('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
-# type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
-åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
-åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
-fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
-for _ in range(8): # åå»ºæ­£æ¹ä½ cube = t3d.Cuboid( canvas, *random.sample
-(range(-200, 200), 3), *random.sample(range(50, 100), 3)) geos.append(cube) #
-åå»ºåé¢ä½ x, y, z = random.sample(range(-200, 200), 3) tetr =
-t3d.Tetrahedron( canvas, *[[x+random.randint(-100, 100), y+random.randint(-100,
-100), z+random.randint(-100, 100)] for _ in range(4)]) geos.append(tetr) def
-translate(event, flag=False, _cache=[]): # type: (tkinter.Event, bool, list
-[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x, event.y]
-return dx = (event.x - _cache[0]) / 6 dy = (event.y - _cache[1]) / 6 _cache[:
-] = [event.x, event.y] for axis in axes: axis.translate(0, 6*dx, 6*dy)
-axis.update() for geo in geos: geo.translate(0, dx, dy) geo.update()
-origin.translate(0, 6*dx, 6*dy) origin.update() def rotate(event, flag=False,
-_cache=[]): # type: (tkinter.Event, bool, list[float]) -> None """ æè½¬äºä»¶
-""" if flag: _cache[:] = [event.x, event.y] return dy = (event.x - _cache[0]) /
-200 dx = (_cache[1] - event.y) / 200 _cache[:] = [event.x, event.y] for axis in
-axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
-geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
-(event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
-event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
+ï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã å³äºç¨³å®çæ Issue
+çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ### Development version/
+å¼åçæ¬ * Version/çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/11
+``` pip install tkintertools-dev==2.6.4 æè pip install tkintertools-dev ```
+è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼å¯è½ææ°åè½ï¼bug
+ä¹å¯è½ä¼æ¯è¾å¤ï¼ä½ä¹å¯è½ä¼æ¯åæ¥ççæ¬æ´å ç¨³å®ã
+å¤§å®¶å¯ä»¥å¨ Issue
+ä¸­æåºä¸äºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
+**ç¹å«æ³¨æ** *
+å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»çAPIå¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸æ­£å¼çå¼å®¹ï¼
+*
+è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½æ­£å¼çååè¿è¡pipå®è£ï¼åæ¬¡ä½¿ç¨æ­£å¼çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£æ­£å¼çï¼
+* éè¦ **Python3.8** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼ News/
+ææ°åè½ ------------ ææ°çç tkintertools **å¼åç**(2.6.4-
+dev)æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
+å¨ Windows ç³»ç»ä¸è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
+* æä½é¼ æ å·¦é®æå¨å¯ä»¥æè½¬è¿å¤ä¸ªå ä½ä½ï¼ *
+æä½é¼ æ å³é®æå¨å¯ä»¥ç§»å¨è¿äºå ä½ä½å¨ç©ºé´ä¸­çä½ç½®ï¼ *
+æâ=âåâ-âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼ *
+æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ã
+ä¸é¢æ¯ç¤ºä¾ç¨åºçææå¾ï¼ ![news.png](news.png) æºä»£ç  ```python
+from tkinter import Event import tkintertools as tkt from tkintertools import
+tools_3d as t3d root = tkt.Tk('tool_3d', 1280, 720) cv3d = t3d.Canvas_3D(root,
+1280, 720, 0, 0) origin = t3d.Point(cv3d, [0, 0, 0]) # åç¹ k = -100, 0, 100
+geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white',
+color_down='yellow', color_left='red', color_right='orange',
+color_front='blue', color_back='green') for a in k for b in k for c in k]
+cv3d.space_sort() def translate(event, flag=False, _cache=[]): # type: (Event,
+bool, list[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x,
+event.y] return dx = (event.x - _cache[0]) dy = (event.y - _cache[1]) _cache[:
+] = [event.x, event.y] for geo in geos: geo.translate(0, dx, dy) geo.update()
+origin.translate(0, dx, dy) origin.update() cv3d.space_sort() def rotate(event,
+flag=False, _cache=[]): # type: (Event, bool, list[float]) -> None """
+æè½¬äºä»¶ """ if flag: _cache[:] = [event.x, event.y] return dy = (event.x -
+_cache[0]) / 100 dx = (_cache[1] - event.y) / 100 _cache[:] = [event.x,
+event.y] for item in geos: item.rotate(0, dx, dy, center=origin.coords)
+item.update() cv3d.space_sort() def scale(event): # type: (Event) -> None """
+ç¼©æ¾äºä»¶ """ k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym
+== 'minus' else 1 for geo in geos: geo.scale(k, k, k) geo.update()
+cv3d.space_sort() def scale_center(event): # type: (Event) -> None """
+ä¸­å¿ç¼©æ¾äºä»¶ """ k = 1.05 if event.delta > 0 else 0.95 for geo in geos:
+geo.scale(k, k, k, center=origin.coords) geo.update() cv3d.space_sort()
 root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
 root.bind('', lambda event: translate(event, True)) root.bind('', translate)
-root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
-[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
-- tkintertools æ¯ä¸æ¬¾åºäº tkinter
+root.bind('', scale) root.bind('', scale_center) root.mainloop() ```
+æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼[CHANGELOG.md](CHANGELOG.md) Description/
+æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
 ä½åæ¶ä¹äº§çäºä¸äºç¼ºç¹ï¼ * èæçæ§ä»¶æ æ³è·åç¦ç¹ *
 èæçæ§ä»¶å¨ææ¬è¾å¥åæ¾ç¤ºçåè½ä¸å­å¨ä¸äºç¼ºé·ï¼è¿ä¸ªç¼ºé·ä¸æ¯å¾ææ¾ï¼ä½å¼ºè¿«çå°±æç¹é¾åäºï¼æ¯å¦æï¼
 tkintertools æ¨¡åè¿å·æä¸äºç¹è²çåè½ï¼ * å©ç¨ tkinter å
 tkintertools åå»ºçç¨åºï¼å¨é«åè¾¨ççæåµä¸ï¼tkintertools
 çä¼æ´å æ¸æ°ï¼è¿ç¹å¯¹äºç¬è®°æ¬ç¨æ·å¾åå¥½ï¼æ¯å¦æï¼ *
 å¯ä»¥è¿éå®ç°æ¸åè²çææ *
 çªå£ç¼©æ¾ï¼ææçæ§ä»¶çå¤§å°è·çç¼©æ¾ï¼å½ç¶ï¼ä¹å¯ä»¥è®¾ç½®ä¸ºä¸è·éç¼©æ¾ï¼
-æ³¨æï¼éè¦ **Python3.7** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼
-Provides/æ¨¡ååè½ ------------------- Here, only the more distinctive
-features will be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ###
-Customizable widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
+* å­æ¨¡å tools_3d å¯ä»¥æ¯æ»¡è¶³ç®åç 3D ç»å¾éæ± Provides/
+æ¨¡ååè½ ------------------- Here, only the more distinctive features will
+be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ### Customizable
+widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
 æ¨¡åçæ§ä»¶æ¥æè®¸å¤åæ°ä¾æä»¬è®¾ç½®ï¼æ¯å¦åè§çåå¾ãææ¬åè¾¹æ¡ä»¥åæ§ä»¶åé¨çé¢è²ï¼å³èäºä»¶ç­ç­ã
 è¿éè¦è¯´æçæ¯ï¼æ¯ä¸ªæ§ä»¶å¯ä»¥è®¾ç½®çå³èäºä»¶ä¸æ­¢ä¸ç§ï¼å¨é¼ æ ç»è¿æ§ä»¶æ¶å¯ä»¥ç»å®äºä»¶ï¼é¼ æ ç¹å»æ§ä»¶ä¹å¯ä»¥ï¼é¼ æ ç¹å»åæ¾å¼ä¹è¡ç­ç­ã
 ææ¬åè¾¹æ¡ä»¥åæ§ä»¶çå¡«åè²ä¹æ¯ç±»ä¼¼çï¼å¨é¼ æ ç»è¿æ§ä»¶ãç¹å»æ§ä»¶ãç¹å»åæ¾å¼é½å¯ä»¥è®¾å®é¢è²ã
 ææ¬ç±»æ§ä»¶è¿è½å¤ä»å³è¾¹éæ­¥è¾å¥ææ¬ï¼ææ¬è¾å¥æç¤ºç¬¦ä¹å¯ä»¥ä¸æ¯åè°æ è¶£çç«çº¿ï¼å¯ä»¥æ¯å¶ä»çï¼æ¯å¦ä¸åçº¿ç­ã
-æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](./test.py)
+æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](test.py)
 æä»¶éé¢çç¤ºä¾ï¼è¿ä¸ªç¤ºä¾å±ç¤ºäº tkintertools
 æ¨¡åçç»å¤§é¨ååè½ï¼ç¤ºä¾ä¸­æ´æéèç âå¤å½©åå¹»â
 å½©èå¦ï¼ ### Automatically control size/èªå¨æ§å¶å¤§å° tkintertools
 ä¸­çæ§ä»¶ï¼å¶å¤§å°åå½¢ç¶å¯ä»¥éççªå£çååèææ¯ä¾å°ååï¼ä¸ä»ä»æ¯æ§ä»¶ä¸­çææ¬ï¼Canvas
 ç»å¶çå¾å½¢ä¹ä¼éä¹åå¨ï¼æ´è®©äººå´å¥çæ¯ï¼png
 ç±»åçå¾çä¹ä¼éä¹ææ¯ä¾å°ç¼©æ¾ï¼å½ç¶ï¼ä½ ä¹å¯ä»¥è®¾å®åæ°è®©å¶ä¸éä¹åå¨ï¼ä¹å¯ä»¥è®¾å®åæ°ä½¿å¶å¨ç¼©æ¾çæ¶åä¿ææ¨ªçºµæ¹åçæ¯ä¾ã
 æ»ä¹ï¼å¾æ¹ä¾¿ï¼å¾èéï¼ ### Easily move widgets/è½»æ¾ç§»å¨æ§ä»¶
@@ -99,70 +97,73 @@
 çº§å«è®¾ç½®å½æ°](#DPI) ### Detailed type hints/è¯¦ç»çç±»åæç¤º åè
 [PEP 526](https://peps.python.org/pep-0526/)ã[PEP 586](https://
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
 é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
-[type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
+[type_hint.png](readme_res/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
-tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
-(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
-images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
-internal class and function in the module will be described in detail here
+tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](test.py) å¨
+Windows ç³»ç»ï¼**Windows10**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ !
+[test_windows10.png](readme_res/test_windows10.png) [test.py](test.py) å¨
+Linux ç³»ç»ï¼**Ubuntu22.04**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png]
+(readme_res/test_linux.png) [test.py](test.py) å¨ Windows
+ç³»ç»ï¼**Windows11**ï¼ä¸è¿è¡ççé¢å¦ä¸(æºè½æ§å¶åè§åå¾)ï¼
+![test_windows11.png](readme_res/test_windows11.png) ### 3D Drawing/3Dç»å¾
+è§ [News/ææ°åè½](#news) Contents/æ¨¡ååå®¹ ------------------- Each
+non internal class and function in the module will be described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
-ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](docs/images/LabelTest.png)
+ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](readme_res/LabelTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
 tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
 tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
 tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
-ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](docs/images/
+ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](readme_res/
 ButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk
 ('ButtonTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful
 (x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
 """ for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
 100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
 (canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
 (canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
 (canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
 å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
-ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](docs/images/
+ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](readme_res/
 CheckButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root =
 tkt.Tk('CheckButtonTest', 500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0)
 def colorful(x, y, width, height): # type: (int, int, int, int) -> None """
 Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(40, 190, 420, 50) tkt.CheckButton(canvas, 50, 50, 30,
 text='NormalCheckButton', value=True) tkt.CheckButton(canvas, 50, 100, 30,
 text='DisableCheckButton', value=True).set_live(False) tkt.CheckButton(canvas,
 50, 150, 30, radius=10, text='RoundCornerCheckButton') tkt.CheckButton(canvas,
 50, 200, 30, radius=15, text='TransparentCheckButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
-ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](docs/images/EntryTest.png)
+ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](readme_res/EntryTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
 400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
 100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
 (canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
@@ -173,29 +174,29 @@
 radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
 35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
 tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
 justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
 text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
 root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
-ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](docs/images/TextTest.png)
+ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](readme_res/TextTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
 for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
 Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
 (Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
 text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
 radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
-ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](docs/images/
+ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](readme_res/
 ProgressbarTest.png) æºä»£ç  ```python import tkintertools as tkt root =
 tkt.Tk('ProgressbarTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0)
 def colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None
 """ Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(30, 290, 440, 50) tkt.Progressbar(canvas, 50, 50, 400, 30)
 tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667) tkt.Progressbar(canvas,
@@ -213,15 +214,15 @@
 å¨å¾æå¾å¥½çæ¯æï¼ä»éæå°éä»£ç å³å¯å®ç°å¨å¾çæ¾ç¤ºï¼è¿å¯ä»¥è®¾ç½®å¨å¾æ¾ç¤ºçéåº¦ï¼æ­¤å¤ï¼å¯¹
 png
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
-![MoveTest.gif](docs/images/MoveTest.gif) æºä»£ç  ```python import
+![MoveTest.gif](readme_res/MoveTest.gif) æºä»£ç  ```python import
 tkintertools as tkt root = tkt.Tk('MoveTest', 500, 500) canvas = tkt.Canvas
 (root, 500, 500, 0, 0) rect = canvas.create_rectangle(50, 350, 150, 450) def
 move_window(switch=[True]): # type: (list[bool]) -> None tkt.move(root, None,
 1000 if switch[0] else -1000, 0, 800, mode='flat') switch[0] = not switch[0]
 def move_button(switch=[True]) -> None: # type: (list[bool]) -> None tkt.move
 (canvas, button, 200 if switch[0] else -200, 0, 500, mode='rebound') switch[0]
 = not switch[0] def move_rect(switch=[True]): # type: (list[bool]) -> None
@@ -235,36 +236,35 @@
 å¦ï¼å¾å°ä¸ä¸ª 20 é¿åº¦çå­ç¬¦ä¸² âtkintertoolsâ
     `left`   : "tkintertools        "
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
 ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡ ![ColorTest.png]
-(docs/images/ColorTest.png) ![Test_Draw.png](docs/images/Test_Draw.png)
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
-height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
-tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
-y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
+(readme_res/ColorTest.png) ![Test_Draw.png](readme_res/Test_Draw.png) æºä»£ç 
+```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500, 500)
+canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width, height): #
+type: (int, int, int, int) -> None """ Gradient colors """ for i in range
+(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 = tkt.color
+(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i, y+height,
+fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
 outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
 `askfont`: å­ä½éæ©å¯¹è¯æ¡
 `askfont`å½æ°å¯ä»¥æå¼é»è®¤çå­ä½éæ©çªå£ï¼è¿ä¸ªçªå£è½ç¶æ¯é»è®¤çï¼ä½å®å®éä¸æ æ³å¨`tkinter`ä¸­æå¼ï¼å ä¸º`tkinter`å¹¶æ²¡æå¯¹åºç
 API è½å¤åå°è¿ä¸ç¹ãä½æ¯ï¼`tkintertools`è°ç¨å¹¶å°è£äºåçç
-tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
-[font.png]
-5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
+tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã ![font.png]
+(readme_res/font.png) 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
 è¿ä¸ªå½æ°å®éä¸åªæ¯å¯¹å½æ°`ctypes.WinDLL
 ('shcore').SetProcessDpiAwareness`çä¸ä¸ªç®ååè£ï¼å¶å¼å¯ä¸º 0ã1
 å 2ï¼åå«ä»£è¡¨ç¨åº DPI
 çä¸åçº§å«ï¼é£ä¹ç¼©æ¾ææä¹å°±ä¸åï¼`tkintertools`éæ©çå¼æ¯
 1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ !
-[SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+[SetProcessDpiAwareness_0.png](readme_res/SetProcessDpiAwareness_0.png)
 ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
-![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
+![SetProcessDpiAwareness_1.png](readme_res/SetProcessDpiAwareness_1.png)
 ä»ä¸é¢çä¸¤å¼ å¾ä¸­å¯ä»¥å¾ææ¾ççåºç¬¬ä¸å¼ å¾æ¨¡ç³ï¼ç¬¬äºå¼ å¾æ¸æ°ï¼è¿å°±æ¯
 DPI çº§å«ä¸åçåå ï¼ä¸è¿è¿ä¸ç¹å¨å±å¹ç¼©æ¾æ¯ä¸æ¯ 100%
 çæ¶åæä¼åºç° å¤§å®¶å¯¹ä¸é¢çå¾è¯å®å¾çæï¼è¿ä¸å°±æ¯ IDLE
 åï¼ï¼å¯¹ï¼è¿ä¸ªçé®é¢çè§£å³åæ³ä¹æ¯æ¥èªäº IDLE çæºä»£ç 
 [pyshell.py line 18~20]
 æ³¨æï¼è¯¥å½æ°å¨ç¨åºçä¸åä½ç½®æ§è¡çææä¸ä¸æ ·ï¼ä¸è¬ç¨å¨`mainloop`ä¹åï¼ä½`tkintertools`å·²ç»å¨`mainloop`å½æ°ä¸­åµå¥äºè¯¥å½æ°ï¼æ éåè®¾ç½®ä¸æ¬¡
 DPI çº§å«ï¼æ­¤å½æ°æ¯ä¸ºäºåç`tkinter`ç¨åºç¨çã Examples/
@@ -276,30 +276,33 @@
 bugï¼åªéè¿éè¦æ¹è¿ï¼ ### ä»»å¡æ¸åå°å·¥å· * æç« é¾æ¥: https:
 //xiaokang2022.blog.csdn.net/article/details/128561339 * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/todolist * ç¨åºä¸è½½
 (å«æåå¥½çç¨åºåæºä»£ç ): https://wwc.lanzoum.com/iyxL30kpkcbe *
 æ¨èææ°: ð è¿ä¸ªæ¡ä¾ä½¿ç¨äº tkintertools-v2.5.7
 çæ¬ï¼æ°çå·²æ æ³å¼å®¹ï¼ï¼å«æä¸äº bugï¼å¤§ééç¨äº
 tkintertools çæ§ä»¶ï¼åå¾äºæ¯è¾å¥½ççé¢ææãä½ç°äº
-tkintertools æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨é¢å¼ä¸çç¢¾åæ§ï¼
-[todolist.png] [todolist.png]
-### ä¸­å½è±¡æ£æ¸¸æ * æç« é¾æ¥: https://xiaokang2022.blog.csdn.net/
-article/details/128852029 * ä»£ç ä»åº: https://gitcode.net/weixin_62651706/
-chess * ç¨åºä¸è½½(å«æåå¥½çç¨åºåæºä»£ç ): https://
-wwc.lanzoum.com/iwgp00mlewpa * æ¨èææ°: ðð
+tkintertools æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨é¢å¼ä¸çç¢¾åæ§ï¼ !
+[todolist.gif](https://img-blog.csdnimg.cn/img_convert/
+dc1a598c3f082253c1ebc7bbca0b98ce.gif) ![todolist.gif](https://img-
+blog.csdnimg.cn/img_convert/7f34451deda1af13712a9edcb37f20b4.gif) ###
+ä¸­å½è±¡æ£æ¸¸æ * æç« é¾æ¥: https://xiaokang2022.blog.csdn.net/article/
+details/128852029 * ä»£ç ä»åº: https://gitcode.net/weixin_62651706/chess *
+ç¨åºä¸è½½(å«æåå¥½çç¨åºåæºä»£ç ): https://wwc.lanzoum.com/
+iwgp00mlewpa * æ¨èææ°: ðð
 æ³¨æï¼æºä»£ç æè§£åå¯ç ï¼è§£åå¯ç å¨é¾æ¥æç« ä¸­ï¼è¯·ä»ç»æ¥æ¾ï¼
 è¿ä¸ªæ¡ä¾ä½¿ç¨äº tkintertools-v2.5.9.5 çæ¬ï¼æ°çå·²æ æ³å¼å®¹ï¼,
 å«æå°é bugï¼é¨å UI éç¨äº tkintertoolsï¼é¨å UI éç¨äº
 tkinterï¼å±äºæ··åä½¿ç¨ãä½ç°äº tkintertools æ¨¡åå¯¹ tkinter
-æ¨¡åçå¼å®¹æ§ï¼
-[chess.png] [chess.png]
-### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
-gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
-ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
+æ¨¡åçå¼å®¹æ§ï¼ ![chess.png](https://img-blog.csdnimg.cn/
+43df0568d4b34078a443a098b67c126a.png) ![chess.png](https://img-blog.csdnimg.cn/
+fc768093715d47d7b14bea015a921e3d.png) ### ç®æç»å½çé¢ * æç« é¾æ¥:
+ææ  * ä»£ç ä»åº: https://gitcode.net/weixin_62651706/tester *
+ç¨åºä¸è½½: ææ  * æ¨èææ°: ððð
+è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
-æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
-examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
------- > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
-(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
-(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
-è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png]
+(readme_res/exam3_1.png) ![exam3_2.png](readme_res/exam3_2.png) More/æ´å¤ ---
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > Gitee(Mirror/
+éå): > https://gitee.com/xiaokang-2022/tkintertools > GitCode(Mirror/
+éå): > https://gitcode.net/weixin_62651706/tkintertools
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](tkintertools/) ä¸­æ¢ç´¢ï¼
```

