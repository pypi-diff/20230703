# Comparing `tmp/tkintertools-2.6.6.dev0.tar.gz` & `tmp/tkintertools-2.6.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.6.dev0.tar", last modified: Thu Jun 29 09:43:34 2023, max compression
+gzip compressed data, was "tkintertools-2.6.7.dev0.tar", last modified: Mon Jul  3 07:32:36 2023, max compression
```

## Comparing `tkintertools-2.6.6.dev0.tar` & `tkintertools-2.6.7.dev0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 09:43:34.023952 tkintertools-2.6.6.dev0/
--rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.6.dev0/LICENSE.txt
--rw-rw-rw-   0        0        0     9062 2023-06-29 09:43:34.022947 tkintertools-2.6.6.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     8428 2023-06-29 09:04:12.000000 tkintertools-2.6.6.dev0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 09:43:34.023952 tkintertools-2.6.6.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-06-29 06:36:36.000000 tkintertools-2.6.6.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:43:34.010671 tkintertools-2.6.6.dev0/tkintertools/
--rw-rw-rw-   0        0        0     2863 2023-06-29 07:57:18.000000 tkintertools-2.6.6.dev0/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    62351 2023-06-28 20:32:13.000000 tkintertools-2.6.6.dev0/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     1999 2023-06-16 16:48:27.000000 tkintertools-2.6.6.dev0/tkintertools/constants.py
--rw-rw-rw-   0        0        0    21734 2023-06-29 07:51:40.000000 tkintertools-2.6.6.dev0/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:43:34.020749 tkintertools-2.6.6.dev0/tkintertools.egg-info/
--rw-rw-rw-   0        0        0     9062 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 07:32:36.042061 tkintertools-2.6.7.dev0/
+-rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.7.dev0/LICENSE.txt
+-rw-rw-rw-   0        0        0     9269 2023-07-03 07:32:36.041061 tkintertools-2.6.7.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     8635 2023-07-03 07:30:27.000000 tkintertools-2.6.7.dev0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 07:32:36.042061 tkintertools-2.6.7.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2023-07-03 07:26:30.000000 tkintertools-2.6.7.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 07:32:36.034789 tkintertools-2.6.7.dev0/tkintertools/
+-rw-rw-rw-   0        0        0     2335 2023-07-03 06:46:57.000000 tkintertools-2.6.7.dev0/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    63639 2023-07-03 07:09:55.000000 tkintertools-2.6.7.dev0/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     2514 2023-07-03 06:06:54.000000 tkintertools-2.6.7.dev0/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    23455 2023-07-03 06:38:55.000000 tkintertools-2.6.7.dev0/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-07-03 07:32:36.040063 tkintertools-2.6.7.dev0/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0     9269 2023-07-03 07:32:35.000000 tkintertools-2.6.7.dev0/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-03 07:32:35.000000 tkintertools-2.6.7.dev0/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 07:32:35.000000 tkintertools-2.6.7.dev0/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 07:32:35.000000 tkintertools-2.6.7.dev0/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.6.dev0/LICENSE.txt` & `tkintertools-2.6.7.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.6.dev0/PKG-INFO` & `tkintertools-2.6.7.dev0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.6.dev0
+Version: 2.6.7.dev0
 Summary: An auxiliary module of the tkinter module.
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 Maintainer: Xiaokang2022
 Maintainer-email: 2951256653@qq.com
 License: MulanPSL-2.0
@@ -23,66 +23,66 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/06/29-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/03-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
-[![Wiki](https://img.shields.io/badge/Wiki-15-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
+[![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
 [![Insights](https://repobeats.axiom.co/api/embed/ab8fae686a5a96f91fa71c40c53c189310924f5e.svg)](https://github.com/Xiaokang2022/tkintertools/pulse)
 
 </div>
 
 Install/模块安装👇
 -----------------
 
 ### Stable Version/稳定版本
 
-* Version/最新版本 : `2.6.5`
-* Release/发布日期 : 2023/06/17 (UTC+08)
+* Version/最新版本 : `2.6.6`
+* Release/发布日期 : 2023/07/01 (UTC+08)
 
 这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。  
 稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.5
+pip install tkintertools==2.6.6
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.6.dev`
-* Release/发布日期 : 2023/06/29 (UTC+08)
+* Version/最新版本 : `2.6.7.dev0`
+* Release/发布日期 : 2023/07/03 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
 开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
 大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.6.dev
+pip install tkintertools==2.6.7.dev0
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
 
-目前稳定版在以下操作系统中已经测试通过:
+目前 **稳定版** 在以下操作系统中已经测试通过:
 
 ![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows)
 ![Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11)
 ![Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
 
 可能还有其他的操作系统也是可以运行 tkintertools 的，我没有进行更多的验证。  
 没有任何额外的依赖包（除了一般 Python 内置的 tkinter），但只支持以下 Python 版本:
@@ -92,66 +92,97 @@
 ![Python3.10.*](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
 ![Python3.11.*](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
-**最新版本: tkintertools-2.6.6.dev 开发版**
+### Release Notes/版本说明
+
+**最新版本: `tkintertools-v2.6.7.dev0`**
 
 > **Note**  
-> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！
+> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！  
+> tkintertools 的介绍和使用教程均在 Wiki 中，[点我传送](https://github.com/Xiaokang2022/tkintertools/wiki)
 
 下面是本次版本更新内容条目：
 
-- [X] 新增抽象类 `_3D_Object` 来作为类 `_Point`、`_Line` 和 `_Side` 的元基类；
-- [X] 优化了 3D 子模块中的参数传递，使用者不需要时刻保证 `list` 的传递性，且原来只能使用 `list` 类型的参数现在为 `Iterable` 类型；
-- [X] 3D 子模块中 3D 对象居中方式改变，相比原来性能提升了不少，代码量也减少了；
-- [X] 改正了部分错误的类型提示，完善了部分缺少的方法注释；
-- [X] 3D 子模块中原来用函数 `hypot` 计算两点间距离，现在直接用函数 `dist` 计算两点间欧几里得距离，提高性能；
-- [X] 3D 子模块中优化了类 `Point` 的控件位置显示，让其始终保持在最前；
-- [X] 3D 子模块的类 `Point` 及其父类 `_Point` 的参数 `point1` 和 `point2` 分别被重命名为 `point_start` 和 `point_end`；
-- [X] 3D 子模块的类 `Space` 的参数 `origin_color` 被更改为四个新的参数，分别是 `origin_size`、`origin_width`、`origin_fill` 和 `origin_outline`；
-- [X] 3D 子模块的类 `Canvas_3D` 和 `Space` 移除参数 `dx` 和 `dy`，画布默认视野保持居中，也就是说，现在它们的中心位置才是原来的左上角顶点；
+- [X] 新增常量 `ROTATE_CENTER`、`ORIGIN_COORDINATE`、`ORIGIN_SIZE`、`ORIGIN_WIDTH`、`ORIGIN_FILL` 和 `ORIGIN_OUTLINE`；
+- [X] 类 `Tk` 和 `Toplevel` 新增关键字参数 `alpha`、`toolwindow`、`topmost` 和 `transparentcolor`；
+- [X] 修复了类 `Text` 在使用鼠标滚轮滚动时会报错的 bug；
+- [X] 优化函数 `translate`、`rotate` 和 `scale` 内部的实现，提高了性能；
+- [X] 修改和完善了大量的不完整的文档注释；
+- [X] 将部分类的部分方法更改为保护方法；
+
+### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 滚动鼠标中键可以放大和缩小画面；
+* 这多个几何体会自动地旋转以及上下浮动；
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
-![news](news.png)
+![news](news.gif)
 
 <details><summary><b>点击查看源代码</b></summary>
 
 ```python
 import math  # 数学支持
 
 import tkintertools as tkt  # 引入基础模块
 from tkintertools import tools_3d as t3d  # 引入 3d 子模块
 
 root = tkt.Tk('3D', 1280, 720)  # 创建窗口
 space = t3d.Space(root, 1280, 720, 0, 0)  # 创建空间
-last_point = [0, 100*math.cos(-math.pi/3), 100*math.sin(-math.pi/3)]
-color_lst = ['red', 'orange', 'yellow', 'green', 'blue', 'purple']
-color_lst += color_lst
-
-for i in range(6):
-    rad = i*math.pi/3
-    next_point = [0, 100*math.cos(rad), 100*math.sin(rad)]
-    point_h2 = [0, 150*math.cos(rad), 150*math.sin(rad)]
-    t3d.Line(space, last_point, next_point, width=3, fill=color_lst[i])
-    t3d.Line(space, next_point, point_h2, width=3, fill=color_lst[i+1])
-    t3d.Point(space, last_point, size=20, fill=color_lst[i+2])
-    t3d.Point(space, point_h2, size=10, fill=color_lst[i+3])
-    last_point = next_point
 
-space.space_sort()  # 给它们的空间位置排序以正确显示
+for a in -100, 0, 100:
+    for b in -100, 0, 100:
+        for c in -100, 0, 100:
+            t3d.Cuboid(space, a-50, b-50, c-50, 100, 100, 100,  # 创建正方体
+                       color_up='white', color_down='yellow', color_left='red',
+                       color_right='orange', color_front='blue', color_back='green')
+
+
+def spin():
+    """ 自动旋转 """
+    for geo in space.geos():
+        geo.rotate(dz=0.01)
+
+
+def floating(value):
+    """ 上下浮动 """
+    for geo in space.geos():
+        geo.translate(dz=math.sin(value))
+
+
+def animation(value=0):
+    """ 形成动画 """
+    spin()
+    floating(value)
+    space.space_sort()  # 给它们的空间位置排序以正确显示
+    for geo in space.geos():
+        geo.update()
+    space.after(10, animation, value+math.pi/60)
+
+
+def scale(event):
+    """ 缩放事件 """
+    k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1  # 缩放比率
+    for geo in space.geos():  # 遍历所有的几何体（不包括基本 3D 对象）
+        geo.scale(k, k, k)  # 缩放
+        geo.update()  # 更新改对象的实际画面
+    space.space_sort()  # 空间前后位置排序
+
+
+animation()
+root.bind('<Key-equal>', scale)  # 绑定等号按键
+root.bind('<Key-minus>', scale)  # 绑定减号按键
 root.mainloop()  # 消息事件循环
 ```
 
 </details>
 
 More/更多👇
 -----------
```

### Comparing `tkintertools-2.6.6.dev0/README.md` & `tkintertools-2.6.7.dev0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,66 +5,66 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/06/29-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/03-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
-[![Wiki](https://img.shields.io/badge/Wiki-15-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
+[![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
 [![Insights](https://repobeats.axiom.co/api/embed/ab8fae686a5a96f91fa71c40c53c189310924f5e.svg)](https://github.com/Xiaokang2022/tkintertools/pulse)
 
 </div>
 
 Install/模块安装👇
 -----------------
 
 ### Stable Version/稳定版本
 
-* Version/最新版本 : `2.6.5`
-* Release/发布日期 : 2023/06/17 (UTC+08)
+* Version/最新版本 : `2.6.6`
+* Release/发布日期 : 2023/07/01 (UTC+08)
 
 这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。  
 稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.5
+pip install tkintertools==2.6.6
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.6.dev`
-* Release/发布日期 : 2023/06/29 (UTC+08)
+* Version/最新版本 : `2.6.7.dev0`
+* Release/发布日期 : 2023/07/03 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
 开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
 大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.6.dev
+pip install tkintertools==2.6.7.dev0
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
 
-目前稳定版在以下操作系统中已经测试通过:
+目前 **稳定版** 在以下操作系统中已经测试通过:
 
 ![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows)
 ![Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11)
 ![Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
 
 可能还有其他的操作系统也是可以运行 tkintertools 的，我没有进行更多的验证。  
 没有任何额外的依赖包（除了一般 Python 内置的 tkinter），但只支持以下 Python 版本:
@@ -74,66 +74,97 @@
 ![Python3.10.*](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
 ![Python3.11.*](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
-**最新版本: tkintertools-2.6.6.dev 开发版**
+### Release Notes/版本说明
+
+**最新版本: `tkintertools-v2.6.7.dev0`**
 
 > **Note**  
-> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！
+> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！  
+> tkintertools 的介绍和使用教程均在 Wiki 中，[点我传送](https://github.com/Xiaokang2022/tkintertools/wiki)
 
 下面是本次版本更新内容条目：
 
-- [X] 新增抽象类 `_3D_Object` 来作为类 `_Point`、`_Line` 和 `_Side` 的元基类；
-- [X] 优化了 3D 子模块中的参数传递，使用者不需要时刻保证 `list` 的传递性，且原来只能使用 `list` 类型的参数现在为 `Iterable` 类型；
-- [X] 3D 子模块中 3D 对象居中方式改变，相比原来性能提升了不少，代码量也减少了；
-- [X] 改正了部分错误的类型提示，完善了部分缺少的方法注释；
-- [X] 3D 子模块中原来用函数 `hypot` 计算两点间距离，现在直接用函数 `dist` 计算两点间欧几里得距离，提高性能；
-- [X] 3D 子模块中优化了类 `Point` 的控件位置显示，让其始终保持在最前；
-- [X] 3D 子模块的类 `Point` 及其父类 `_Point` 的参数 `point1` 和 `point2` 分别被重命名为 `point_start` 和 `point_end`；
-- [X] 3D 子模块的类 `Space` 的参数 `origin_color` 被更改为四个新的参数，分别是 `origin_size`、`origin_width`、`origin_fill` 和 `origin_outline`；
-- [X] 3D 子模块的类 `Canvas_3D` 和 `Space` 移除参数 `dx` 和 `dy`，画布默认视野保持居中，也就是说，现在它们的中心位置才是原来的左上角顶点；
+- [X] 新增常量 `ROTATE_CENTER`、`ORIGIN_COORDINATE`、`ORIGIN_SIZE`、`ORIGIN_WIDTH`、`ORIGIN_FILL` 和 `ORIGIN_OUTLINE`；
+- [X] 类 `Tk` 和 `Toplevel` 新增关键字参数 `alpha`、`toolwindow`、`topmost` 和 `transparentcolor`；
+- [X] 修复了类 `Text` 在使用鼠标滚轮滚动时会报错的 bug；
+- [X] 优化函数 `translate`、`rotate` 和 `scale` 内部的实现，提高了性能；
+- [X] 修改和完善了大量的不完整的文档注释；
+- [X] 将部分类的部分方法更改为保护方法；
+
+### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 滚动鼠标中键可以放大和缩小画面；
+* 这多个几何体会自动地旋转以及上下浮动；
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
-![news](news.png)
+![news](news.gif)
 
 <details><summary><b>点击查看源代码</b></summary>
 
 ```python
 import math  # 数学支持
 
 import tkintertools as tkt  # 引入基础模块
 from tkintertools import tools_3d as t3d  # 引入 3d 子模块
 
 root = tkt.Tk('3D', 1280, 720)  # 创建窗口
 space = t3d.Space(root, 1280, 720, 0, 0)  # 创建空间
-last_point = [0, 100*math.cos(-math.pi/3), 100*math.sin(-math.pi/3)]
-color_lst = ['red', 'orange', 'yellow', 'green', 'blue', 'purple']
-color_lst += color_lst
-
-for i in range(6):
-    rad = i*math.pi/3
-    next_point = [0, 100*math.cos(rad), 100*math.sin(rad)]
-    point_h2 = [0, 150*math.cos(rad), 150*math.sin(rad)]
-    t3d.Line(space, last_point, next_point, width=3, fill=color_lst[i])
-    t3d.Line(space, next_point, point_h2, width=3, fill=color_lst[i+1])
-    t3d.Point(space, last_point, size=20, fill=color_lst[i+2])
-    t3d.Point(space, point_h2, size=10, fill=color_lst[i+3])
-    last_point = next_point
 
-space.space_sort()  # 给它们的空间位置排序以正确显示
+for a in -100, 0, 100:
+    for b in -100, 0, 100:
+        for c in -100, 0, 100:
+            t3d.Cuboid(space, a-50, b-50, c-50, 100, 100, 100,  # 创建正方体
+                       color_up='white', color_down='yellow', color_left='red',
+                       color_right='orange', color_front='blue', color_back='green')
+
+
+def spin():
+    """ 自动旋转 """
+    for geo in space.geos():
+        geo.rotate(dz=0.01)
+
+
+def floating(value):
+    """ 上下浮动 """
+    for geo in space.geos():
+        geo.translate(dz=math.sin(value))
+
+
+def animation(value=0):
+    """ 形成动画 """
+    spin()
+    floating(value)
+    space.space_sort()  # 给它们的空间位置排序以正确显示
+    for geo in space.geos():
+        geo.update()
+    space.after(10, animation, value+math.pi/60)
+
+
+def scale(event):
+    """ 缩放事件 """
+    k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1  # 缩放比率
+    for geo in space.geos():  # 遍历所有的几何体（不包括基本 3D 对象）
+        geo.scale(k, k, k)  # 缩放
+        geo.update()  # 更新改对象的实际画面
+    space.space_sort()  # 空间前后位置排序
+
+
+animation()
+root.bind('<Key-equal>', scale)  # 绑定等号按键
+root.bind('<Key-minus>', scale)  # 绑定减号按键
 root.mainloop()  # 消息事件循环
 ```
 
 </details>
 
 More/更多👇
 -----------
```

### Comparing `tkintertools-2.6.6.dev0/tkintertools/__main__.py` & `tkintertools-2.6.7.dev0/tkintertools/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,96 @@
 """ Main File """
 
 import math  # 数学支持
-import sys  # DPI 兼容
+import sys  # DPI 适配
 import tkinter  # 基础模块
 from fractions import Fraction  # 图片缩放
-from typing import Any, Callable, Generator, Iterable, Literal, overload
-# 类型提示
+from typing import (Any, Callable, Generator, Iterable, Literal,  # 类型提示
+                    overload)
 
 if sys.platform == 'win32':  # 仅在 Windows 平台下支持设置 DPI 级别
     from ctypes import WinDLL
 else:
     WinDLL = None
 
 from .constants import *
 
 
 class Tk(tkinter.Tk):
-    """ 创建一个主窗口 """
+    """ 根窗口类 """
 
     def __init__(
         self,
         title=None,  # type: str | None
         width=None,  # type: int | None
         height=None,  # type: int | None
         x=None,  # type: int | None
         y=None,  # type: int | None
         *,
         shutdown=None,  # type: Callable | None
+        alpha=None,  # type: float | None
+        toolwindow=None,  # type: bool | None
+        topmost=None,  # type: bool | None
+        transparentcolor=None,  # type: str | None
         **kw
     ):  # type: (...) -> None
         """
-        `title`: 窗口标题\n
-        `width`: 窗口宽度\n
-        `height`: 窗口高度\n
-        `x`: 窗口左上角横坐标\n
-        `y`: 窗口左上角纵坐标\n
-        `shutdown`: 关闭窗口之前执行的函数，但会覆盖原关闭操作\n
-        `**kw`: 与 tkinter.Tk 类的参数相同\n
+        `title`: 窗口标题 \ 
+        `width`: 窗口宽度 \ 
+        `height`: 窗口高度 \ 
+        `x`: 窗口左上角横坐标 \ 
+        `y`: 窗口左上角纵坐标 \ 
+        `shutdown`: 关闭窗口之前执行的函数，但会覆盖原关闭操作 \ 
+        `alpha`: 窗口的透明度，取值在 0~1 之间，且 1 为不透明 \ 
+        `toolwindow`: 窗口是否为工具窗口 \ 
+        `topmost`: 窗口是否置顶，为布尔值 \ 
+        `transparentcolor`: 过滤掉该颜色 \ 
+        `**kw`: 与 tkinter.Tk 类的其他参数相同
         """
         if type(self) == Tk:  # NOTE:方便后面的 Toplevel 类继承
             tkinter.Tk.__init__(self, **kw)
 
         self.width = [100, 1]  # type: list[int]  # [初始宽度, 当前宽度]
         self.height = [100, 1]  # type: list[int]  # [初始高度, 当前高度]
         self._canvas = []  # type: list[Canvas]  # 子画布列表
 
         if width is not None and height is not None:
             if x is not None and y is not None:
                 self.geometry('%dx%d+%d+%d' % (width, height, x, y))
             else:
                 self.geometry('%dx%d' % (width, height))
 
-        self.title(title if title else None)
+        if title is not None:
+            self.title(title)
+        if alpha is not None:
+            self.attributes('-alpha', alpha)
+        if toolwindow is not None:
+            self.attributes('-toolwindow', toolwindow)
+        if topmost is not None:
+            self.attributes('-topmost', topmost)
+        if transparentcolor is not None:
+            self.attributes('-transparentcolor', transparentcolor)
         self.protocol('WM_DELETE_WINDOW', shutdown if shutdown else None)
-        self.bind('<Configure>', lambda _: self.__zoom())  # 开启窗口缩放检测
+        self.bind('<Configure>', lambda _: self._zoom())  # 开启窗口缩放检测
 
     def canvas(self):  # type: () -> tuple[Canvas]
-        """ 返回`Tk`类的`Canvas`元组 """
+        """ 返回 `Tk` 类全部的 `Canvas` 对象 """
         return tuple(self._canvas)
 
-    def __zoom(self):  # type: () -> None
-        """ 内部方法：缩放检测 """
+    def _zoom(self):  # type: () -> None
+        """ 缩放检测 """
         width, height = map(int, self.geometry().split('+')[0].split('x'))
         # NOTE: 此处必须用 geometry 方法，直接用 Event 或者 winfo 会有画面异常的 bug
 
         if width == self.width[1] and height == self.height[1]:  # 没有大小的改变
             return
 
         for canvas in self._canvas:
             if canvas.expand and canvas._lock:
-                canvas.zoom(width/self.width[1], height/self.height[1])
+                canvas._zoom(width/self.width[1], height/self.height[1])
 
         self.width[1], self.height[1] = width, height  # 更新窗口当前的宽高值
 
     def wm_geometry(self, newGeometry=None):  # type: (str | None) -> str | None
         # override: 添加修改初始宽高值的功能并兼容不同的DPI缩放
         if newGeometry:
             width, height, _width, _height, * \
@@ -84,62 +101,71 @@
                 geometry = geometry.split('+')[0]
             return tkinter.Tk.wm_geometry(self, geometry)
         geometry = tkinter.Tk.wm_geometry(self, newGeometry)
         width, height, _width, _height, * \
             _ = map(int, (geometry+'+0+0').replace('+', 'x').split('x'))
         return '%dx%d+%d+%d' % (width, height, _width, _height)
 
-    geometry = wm_geometry
+    geometry = wm_geometry  # 方法别名
 
     def mainloop(
         self,
         n=0,  # type: int
         *,
         dpi_awareness=1  # type: Literal[1, 2, 3]
     ):  # type: (...) -> None
         """
-        根（主）窗口的消息循环\n
-        `dpi_awareness`: 程序的DPI级别，值可以为0、1和2，程序默认为0，默认值为1
+        ### 消息循环
+        `dpi_awareness`: 程序的 DPI 级别，值可以为 0、1 和 2，程序默认为 0，默认值为 1
         """
         SetProcessDpiAwareness(dpi_awareness)
         return tkinter.Tk.mainloop(self, n)
 
 
 class Toplevel(tkinter.Toplevel, Tk):
-    """ 创建一个子窗口 """
+    """ 子窗口类 """
 
     def __init__(
         self,
         master=None,  # type: Tk | None
         title=None,  # type: str | None
         width=None,  # type: int | None
         height=None,  # type: int | None
         x=None,  # type: int | None
         y=None,  # type: int | None
         *,
         shutdown=None,  # type: Callable | None
+        alpha=None,  # type: float | None
+        toolwindow=None,  # type: bool | None
+        topmost=None,  # type: bool | None
+        transparentcolor=None,  # type: str | None
         **kw
     ):  # type: (...) -> None
         """
-        `master`: 父窗口\n
-        `title`: 窗口标题\n
-        `width`: 窗口宽度\n
-        `height`: 窗口高度\n
-        `x`: 窗口左上角横坐标\n
-        `y`: 窗口左上角纵坐标\n
-        `shutdown`: 关闭窗口之前执行的函数，但会覆盖关闭操作\n
-        `**kw`: 与 tkinter.Toplevel 类的参数相同\n
+        `master`: 父窗口 \ 
+        `title`: 窗口标题 \ 
+        `width`: 窗口宽度 \ 
+        `height`: 窗口高度 \ 
+        `x`: 窗口左上角横坐标 \ 
+        `y`: 窗口左上角纵坐标 \ 
+        `shutdown`: 关闭窗口之前执行的函数，但会覆盖关闭操作 \ 
+        `alpha`: 窗口的透明度，取值在 0~1 之间，且 1 为不透明 \ 
+        `toolwindow`: 窗口是否为工具窗口 \ 
+        `topmost`: 窗口是否置顶，为布尔值 \ 
+        `transparentcolor`: 过滤掉该颜色 \ 
+        `**kw`: 与 tkinter.Toplevel 类的参数相同
         """
         tkinter.Toplevel.__init__(self, master, **kw)
-        Tk.__init__(self, title, width, height, x, y, shutdown=shutdown, **kw)
-        self.focus_set()
+        Tk.__init__(self, title, width, height, x, y, shutdown=shutdown, alpha=alpha,
+                    toolwindow=toolwindow, topmost=topmost, transparentcolor=transparentcolor, **kw)
+        self.focus_set()  # 把焦点转移到该子窗口上来
 
 
 class Canvas(tkinter.Canvas):
-    """ 用于承载虚拟的画布控件，并处理部分绑定事件 """
+    """ 画布容器类 """
 
     def __init__(
         self,
         master,  # type: Tk | Toplevel
         width,  # type: int
         height,  # type: int
         x=None,  # type: int | None
@@ -147,23 +173,23 @@
         *,
         lock=True,  # type: bool
         expand=True,  # type: bool
         keep=False,  # type: bool
         **kw
     ):  # type: (...) -> None
         """
-        `master`: 父控件\n
-        `width`: 画布宽度\n
-        `height`: 画布高度\n
-        `x`: 画布左上角的横坐标\n
-        `y`: 画布左上角的纵坐标\n
-        `lock`: 画布内控件的功能锁，False 时功能暂时失效\n
-        `expand`: 画布内控件是否能缩放\n
-        `keep`: 画布比例是否保持不变\n
-        `**kw`: 与 tkinter.Canvas 类的参数相同\n
+        `master`: 父控件 \ 
+        `width`: 画布宽度 \ 
+        `height`: 画布高度 \ 
+        `x`: 画布左上角的横坐标 \ 
+        `y`: 画布左上角的纵坐标 \ 
+        `lock`: 画布内控件的功能锁，为 False 时功能暂时失效 \ 
+        `expand`: 画布内控件是否能缩放 \ 
+        `keep`: 画布比例是否保持不变 \ 
+        `**kw`: 与 tkinter.Canvas 类的参数相同
         """
         self.width = [width]*2  # [初始宽度, 当前宽度]
         self.height = [height]*2  # [初始高度, 当前高度]
         self._lock = lock
         self.expand = expand
         self.keep = keep
 
@@ -178,52 +204,50 @@
         tkinter.Canvas.__init__(
             self, master, width=width, height=height, highlightthickness=0, **kw)
 
         master._canvas.append(self)  # 将实例添加到 Tk 的画布列表中
         if x is not None and y is not None:
             self.place(x=x, y=y)
 
-        self.bind('<Motion>', self.__touch)  # 绑定鼠标触碰控件
-        self.bind('<Any-Key>', self.__input)  # 绑定键盘输入字符（和Ctrl+v的代码顺序不可错）
-        self.bind('<Button-1>', self.__click)  # 绑定鼠标左键按下
-        self.bind('<B1-Motion>', self.__click)  # 绑定鼠标左键按下移动
-        self.bind('<MouseWheel>', self.__mousewheel)  # 绑定鼠标滚轮滚动
-        self.bind('<ButtonRelease-1>', self.__release)  # 绑定鼠标左键松开
-        self.bind('<<Paste>>', lambda _: self.__paste())  # 绑定粘贴快捷键
+        self.bind('<Motion>', self._touch)  # 绑定鼠标触碰控件
+        self.bind('<Any-Key>', self._input)  # 绑定键盘输入字符（和Ctrl+v的代码顺序不可错）
+        self.bind('<Button-1>', self._click)  # 绑定鼠标左键按下
+        self.bind('<B1-Motion>', self._click)  # 绑定鼠标左键按下移动
+        self.bind('<MouseWheel>', self._mousewheel)  # 绑定鼠标滚轮滚动
+        self.bind('<ButtonRelease-1>', self._release)  # 绑定鼠标左键松开
+        self.bind('<<Paste>>', lambda _: self._paste())  # 绑定粘贴快捷键
 
     def widget(self):  # type: () -> tuple[BaseWidget]
-        """ 返回`Canvas`类的`BaseWidget`元组 """
+        """ 返回 `Canvas` 类全部的 `BaseWidget` 对象 """
         return tuple(self._widget)
 
     @overload
     def lock(self, value):  # type: (bool) -> None
         ...
 
     @overload
     def lock(self):  # type: () -> None
         ...
 
     def lock(self, value=None):  # type: (bool | None) -> bool | None
         """
-        设置或者查询画布锁\n
-        ---
-        `value`: 布尔值，True则可操作，False反之，无参数或参数为None则返回当前值\n
+        ### 设置或查询画布锁的状态
+        `value`: 布尔值，为 True 则可操作，为 False 则反之，无参数或参数为 None 则返回当前值
         """
         if value is None:
             return self._lock
         self._lock = value
         if value and self.expand:
-            self.zoom()
+            self._zoom()
 
-    def zoom(self, rate_x=None, rate_y=None):  # type: (float | None, float | None) -> None
+    def _zoom(self, rate_x=None, rate_y=None):  # type: (float | None, float | None) -> None
         """
-        缩放画布及其内部的所有元素\n
-        ---
-        `rate_x`: 横向缩放比率，默认值表示自动更新缩放（根据窗口缩放程度）\n
-        `rate_y`: 纵向缩放比率，默认值同上\n
+        ### 缩放画布及其内部的所有元素
+        `rate_x`: 横向缩放比率，默认值表示自动更新缩放（根据窗口缩放程度） \ 
+        `rate_y`: 纵向缩放比率，默认值同上
         """
         if not rate_x:
             rate_x = self.master.width[1]/self.master.width[0]/self.rx
         if not rate_y:
             rate_y = self.master.height[1]/self.master.height[0]/self.ry
 
         rate_x_pos, rate_y_pos = rate_x, rate_y  # 避免受 keep 影响
@@ -265,67 +289,67 @@
 
         for item in self._image:  # 图像大小缩放（采用相对的绝对缩放）
             if self._image[item][0] and self._image[item][0].extension != 'gif':
                 self._image[item][1] = self._image[item][0].zoom(
                     temp_x*rate_x, temp_y*rate_y, 1.2)
                 self.itemconfigure(item, image=self._image[item][1])
 
-    def __touch(self, event, flag=True):  # type: (tkinter.Event, bool) -> None
-        """ 内部方法：鼠标触碰控件事件 """
+    def _touch(self, event, flag=True):  # type: (tkinter.Event, bool) -> None
+        """ 鼠标触碰控件事件 """
         if self._lock:
             for widget in self._widget[::-1]:
-                if widget.live and widget.touch(event) and flag:
+                if widget.live and widget._touch(event) and flag:
                     if isinstance(widget, TextWidget):
                         self.configure(cursor='xterm')
                     elif isinstance(widget, Button):
                         self.configure(cursor='hand2')
                     else:
                         self.configure(cursor='arrow')
                     flag = False
             if flag:
                 self.configure(cursor='arrow')
 
-    def __click(self, event):  # type: (tkinter.Event) -> None
-        """ 内部方法：鼠标左键按下事件 """
+    def _click(self, event):  # type: (tkinter.Event) -> None
+        """ 鼠标左键按下事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, (Button, TextWidget)):
-                    widget.click(event)  # NOTE: 无需 return，按下空白区域也有作用
+                    widget._click(event)  # NOTE: 无需 return，按下空白区域也有作用
                     self.focus_set()
 
-    def __release(self, event):  # type: (tkinter.Event) -> None
-        """ 内部方法：鼠标左键松开事件 """
+    def _release(self, event):  # type: (tkinter.Event) -> None
+        """ 鼠标左键松开事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, Button):
-                    if widget.touch(event):
-                        return widget.execute(event)
+                    if widget._touch(event):
+                        return widget._execute(event)
 
-    def __mousewheel(self, event):  # type: (tkinter.Event) -> None
-        """ 内部方法：鼠标滚轮滚动事件 """
+    def _mousewheel(self, event):  # type: (tkinter.Event) -> None
+        """ 鼠标滚轮滚动事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, Text):
-                    if widget.scroll(event):
+                    if widget._scroll(event):
                         return
 
-    def __input(self, event):  # type: (tkinter.Event) -> None
-        """ 内部方法：键盘输入字符事件 """
+    def _input(self, event):  # type: (tkinter.Event) -> None
+        """ 键盘输入字符事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, TextWidget):
-                    if widget.input(event):
+                    if widget._input(event):
                         return
 
-    def __paste(self):  # type: () -> None
-        """ 内部方法：快捷键粘贴事件 """
+    def _paste(self):  # type: () -> None
+        """ 快捷键粘贴事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, TextWidget):
-                    if widget.paste():
+                    if widget._paste():
                         return
 
     def create_text(self, *args, **kw):  # type: (...) -> tkinter._CanvasItemId
         # override: 添加对 text 类型的 _CanvasItemId 的字体大小的控制
         font = kw.get('font')
         if not font:
             kw['font'] = FONT, SIZE
@@ -354,23 +378,23 @@
     def place(self, *args, **kw):  # type: (...) -> None  # BUG: 缩放就会恢复原样
         # override: 增加一些特定功能
         self.width[0] = kw.get('wdith', self.width[0])
         self.height[0] = kw.get('height', self.height[0])
         return tkinter.Canvas.place(self, *args, **kw)
 
     def destroy(self):  # type: () -> None
-        # override: 兼容
+        # override: 兼容 tkinter
         self.master._canvas.remove(self)
         for widget in self.widget():
             widget.destroy()
         return tkinter.Canvas.destroy(self)
 
 
 class BaseWidget:
-    """ 内部类：虚拟画布控件基类 """
+    """ 虚拟画布控件基类 """
 
     def __init__(
         self,
         canvas,  # type:  Canvas
         x,  # type: float
         y,  # type: float
         width,  # type: float
@@ -383,49 +407,49 @@
         image,  # type: PhotoImage | None
         color_text,  # type: tuple[str, str, str]
         color_fill,  # type: tuple[str, str, str]
         color_outline  # type: tuple[str, str, str]
     ):  # type: (...) -> None
         """
         ### 标准参数
-        标准参数是所有控件都有的\n
+        标准参数是所有控件都有的 \n 
         ---
-        `canvas`: 父画布容器控件\n
-        `x`: 控件左上角的横坐标\n
-        `y`: 控件左上角的纵坐标\n
-        `width`: 控件的宽度\n
-        `height`: 控件的高度\n
-        `radius`: 控件圆角化半径\n
-        `text`: 控件显示的文本，对于文本控件而言，可以为一个元组：(默认文本, 鼠标触碰文本)\n
-        `justify`: 文本的对齐方式\n
-        `borderwidth`: 外框的宽度\n
-        `font`: 控件的字体设定 (字体, 大小, 样式)\n
-        `image`: 控件的背景（支持 png 类型，大小必须小于控件，否则会溢出）\n
-        `color_text`: 控件文本的颜色\n
-        `color_fill`: 控件内部的颜色\n
-        `color_outline`: 控件外框的颜色\n
+        `canvas`: 父画布容器控件 \ 
+        `x`: 控件左上角的横坐标 \ 
+        `y`: 控件左上角的纵坐标 \ 
+        `width`: 控件的宽度 \ 
+        `height`: 控件的高度 \ 
+        `radius`: 控件圆角化半径 \ 
+        `text`: 控件显示的文本，对于文本控件而言，可以为一个元组：(默认文本, 鼠标触碰文本) \ 
+        `justify`: 文本的对齐方式 \ 
+        `borderwidth`: 外框的宽度 \ 
+        `font`: 控件的字体设定 (字体, 大小, 样式) \ 
+        `image`: 控件的背景（支持 png 类型，大小必须小于控件，否则会溢出控件边框） \ 
+        `color_text`: 控件文本的颜色 \ 
+        `color_fill`: 控件内部的颜色 \ 
+        `color_outline`: 控件外框的颜色
         ---
         ### 特定参数
-        特定参数只有某些控件类才有\n
+        特定参数只有某些控件类才有 \n 
         ---
-        `command`: 按钮控件的关联函数\n
-        `show`: 文本控件的显示文本\n
-        `limit`: 文本控件的输入字数限制，为负数时表示没有字数限制\n
-        `read`: 文本控件的只读模式\n
-        `cursor`: 输入提示符的字符，默认为一竖线\n
+        `command`: 按钮控件的关联函数 \ 
+        `show`: 文本控件的显示文本 \ 
+        `limit`: 文本控件的输入字数限制，为负数时表示没有字数限制 \ 
+        `read`: 文本控件的只读模式 \ 
+        `cursor`: 文本控件输入提示符的字符，默认为一竖线
         ---
         ### 详细说明
-        1. 字体的值为一个包含两个或三个值的元组或者单个的字符串，共三种形式\n
+        1. 字体的值为一个包含两个或三个值的元组或者单个的字符串，共三种形式:
             * 形式一: `字体名称`
             * 形式二: `(字体名称, 字体大小)`
             * 形式三: `(字体名称, 字体大小, 字体样式)`
-        2. 颜色为一个包含三个或四个 RGB 颜色字符串的元组，共两种形式\n
+        2. 颜色为一个包含三个或四个 RGB 颜色字符串的元组，共两种形式:
             * 不使用禁用功能时: `(正常颜色, 触碰颜色, 交互颜色)`
             * 需使用禁用功能时: `(正常颜色, 触碰颜色, 交互颜色, 禁用颜色)`
-            * 特别地，进度条控件的参数`color_bar`为: `(底色, 进度条颜色)`
+            * 特别地，进度条控件的参数 `color_bar` 为: `(底色, 进度条颜色)`
         """
         self.master = canvas
         self.value = text
         self.justify = justify
         self.font = font
         self.photoimage = image
         self.color_text = list(color_text)
@@ -474,15 +498,16 @@
                 canvas.create_arc(
                     x+_w, y, x+width, y+d*canvas.ry, start=0, **kw),
                 canvas.create_arc(
                     x, y+_h, x+d*canvas.rx, y+height, start=180, **kw),
                 canvas.create_arc(
                     x+_w, y+_h, x+width, y+height, start=270, **kw)]
 
-            kw = {'extent': 100, 'style': 'arc', 'outline': color_outline[0]}
+            kw = {'extent': 100, 'style': tkinter.ARC,
+                  'outline': color_outline[0]}
             self.outside = [  # 虚拟控件外框
                 canvas.create_line(
                     _x, y, x+width-radius*canvas.rx, y, fill=color_outline[0], width=borderwidth),
                 canvas.create_line(
                     _x, y+height, x+width-radius*canvas.rx, y+height, fill=color_outline[0], width=borderwidth),
                 canvas.create_line(
                     x, _y, x, y+height-radius*canvas.ry, fill=color_outline[0], width=borderwidth),
@@ -528,22 +553,21 @@
         ...
 
     @overload
     def state(self):  # type: () -> None
         ...
 
     def state(self, mode=None):
-        # type: (Literal['normal', 'touch', 'click', 'disabled'] | None) -> None
+        # type: (Literal['normal', 'touch', 'click', 'disabled'] | None) -> str | None
         """
-        mode参数为None或者无参数时仅更新控件，否则改变虚拟控件的外观\n
+        ### 设置或查询控件的状态
+        参数 mode 为 None 或者无参数时仅更新控件，否则改变虚拟控件的外观 \n 
         ---
-        `normal`: 正常状态\n
-        `touch`: 鼠标触碰时的状态\n
-        `click`: 鼠标按下时的状态\n
-        `disabled`: 禁用状态\n
+        `mode`: 可以为下列值之一 normal（正常状态）、touch（鼠标触碰时的状态）、
+        click（鼠标按下时的状态）、disabled（禁用状态） 和 None（查询控件状态）
         """
         if mode:
             self._state, self.pre_state = mode, self._state
             if self._state == self.pre_state:  # 保持状态时直接跳过
                 return
 
         if self._state == 'normal':
@@ -580,18 +604,17 @@
                     self.rect, fill=self.color_fill[mode])
 
         if self.command_ex[self._state]:
             self.command_ex[self._state]()
 
     def move(self, dx, dy):  # type: (float, float) -> None
         """
-        移动控件的位置\n
-        ---
-        `dx`: 横向移动长度（单位：像素）\n
-        `dy`: 纵向移动长度\n
+        ### 移动控件的位置
+        `dx`: 横向移动长度 \ 
+        `dy`: 纵向移动长度
         """
         self.x1 += dx
         self.x2 += dx
         self.y1 += dy
         self.y2 += dy
 
         if self.radius:
@@ -608,34 +631,34 @@
         if isinstance(self, (Text, CheckButton)):
             self.master.move(self._text, dx, dy)
         if isinstance(self, Progressbar):
             self.master.move(self.bar, dx, dy)
 
     def moveto(self, x, y):  # type: (float, float) -> None
         """
-        改变控件的位置（以控件左上角为基准）\n
-        ---
-        `x`: 改变到的横坐标（单位：像素）\n
-        `y`: 改变到的纵坐标\n
+        ### 改变控件的位置（以控件左上角为基准）
+        `x`: 改变到的横坐标 \ 
+        `y`: 改变到的纵坐标
         """
         self.move(x - self.x1, y - self.y1)
 
     @overload
     def configure(self, **kw):  # type: (...) -> None
         ...
 
     @overload
     def configure(self, *args):  # type: (...) -> str | tuple
         ...
 
     def configure(self, *args, **kw):  # type: (...) -> str | tuple | None
         """
-        修改或查询原有参数的值，可供修改或查询的参数有\n
+        ### 修改或查询参数的值
+        可供修改或查询的参数有: 
         1. 所有控件: `color_text`、`color_fill`、`color_outline`
-        2. 非文本控件: `text`\n
+        2. 非文本控件: `text` \n 
         注意：颜色修改不会立即生效，可通过鼠标经过生效，或者调用 state 方法立即刷新状态！
         """
         if args:
             if args[0] == 'text':
                 if isinstance(self, CheckButton):
                     return self.master.itemcget(self._text, 'text')
                 return self.value
@@ -688,27 +711,30 @@
         ...
 
     @overload
     def set_live(self):  # type: () -> bool
         ...
 
     def set_live(self, value=None):  # type: (bool | None) -> bool | None
-        """ 设定或查询live值 """
+        """
+        ### 设置或查询控件的活跃状态
+        `value`: 可以为 bool 类型（设置当前值）或者 None（返回当前值）
+        """
         if value is None:
             return self.live
         else:
             self.live = value
             if value:
                 self.state('normal')
             else:
                 self.state('disabled')
 
 
 class TextWidget(BaseWidget):
-    """ 内部类：文本类控件基类 """
+    """ 虚拟文本类控件基类 """
 
     def __init__(
         self,
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
@@ -740,97 +766,97 @@
 
         # 提示光标 NOTE:位置顺序不可乱动，font不可乱改
         self._cursor = canvas.create_text(0, 0, fill=color_text[2], font=font)
         canvas._font[self._cursor][1] = canvas._font[self.text][1]
         font = canvas.itemcget(self.text, 'font')
         canvas.itemconfigure(self._cursor, font=font)
 
-    def touch_on(self):  # type: () -> None
-        """ 内部方法：鼠标悬停状态 """
+    def _touch_on(self):  # type: () -> None
+        """ 鼠标悬停状态 """
         if self._state != 'click':
             self.state('touch')
 
             if self.master.itemcget(self.text, 'text') == self._value[1]:
                 self.master.itemconfigure(self.text, text=self._value[2])
 
-    def touch_off(self):  # type: () -> None
-        """ 内部方法：鼠标离开状态 """
+    def _touch_off(self):  # type: () -> None
+        """ 鼠标离开状态 """
         if self._state != 'click':
             self.state('normal')
 
             if self.master.itemcget(self.text, 'text') == self._value[2]:
                 self.master.itemconfigure(self.text, text=self._value[1])
 
-    def click(self, event):  # type: (tkinter.Event) -> None
-        """ 内部方法：交互状态检测 """
+    def _click(self, event):  # type: (tkinter.Event) -> None
+        """ 交互状态检测 """
         if self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2:
             if self._state != 'click':
-                self.click_on()
+                self._click_on()
         else:
-            self.click_off()
+            self._click_off()
 
-    def touch(
+    def _touch(
         self,  # type: Entry | Text
         event  # type: tkinter.Event
     ):  # type: (...) -> bool
-        """ 内部方法：触碰状态检测 """
+        """ 触碰状态检测 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
-        self.touch_on() if condition else self.touch_off()
+        self._touch_on() if condition else self._touch_off()
         return condition
 
-    def cursor_flash(self):  # type: () -> None
-        """ 内部方法：鼠标光标闪烁 """
+    def _cursor_flash(self):  # type: () -> None
+        """ 鼠标光标闪烁 """
         if self.interval >= 300:
             self.interval, self.flag = 0, not self.flag
             if self.flag:
                 self.master.itemconfigure(self._cursor, text=self.icursor)
             else:
                 self.master.itemconfigure(self._cursor, text='')
 
         if self._state == 'click':
             self.interval += 10
-            self.master.after(10, self.cursor_flash)
+            self.master.after(10, self._cursor_flash)
         else:
             self.interval, self.flag = 300, False  # 恢复默认值
             self.master.itemconfigure(self._cursor, text='')
 
-    def cursor_update(self, text=' '):  # type: (str) -> None
-        """ 内部方法：鼠标光标更新 """
+    def _cursor_update(self, text=' '):  # type: (str) -> None
+        """ 鼠标光标更新 """
         self.interval, self.flag = 300, False  # 恢复默认值
         if isinstance(self, Entry):
             self.master.coords(self._cursor, self.master.bbox(
                 self.text)[2], self.y1+self.height * self.master.ry / 2)  # BUG
         elif isinstance(self, Text):
             _pos = self.master.bbox(self._text)
             self.master.coords(self._cursor, _pos[2], _pos[1])
         self.master.itemconfigure(
             self._cursor, text='' if not text else self.icursor)
 
-    def paste(self):  # type: () -> bool
-        """ 内部方法：快捷键粘贴 """
+    def _paste(self):  # type: () -> bool
+        """ 快捷键粘贴 """
         condition = self._state == 'click' and not getattr(self, 'show', None)
         if condition:
             self.append(self.master.clipboard_get())
         return condition
 
-    def clear(self):  # type: () -> None
-        """ 内部方法：清空文本类控件的内容 """
+    def _clear(self):  # type: () -> None
+        """ 清空文本类控件的内容 """
         if isinstance(self, Text):
             event = tkinter.Event()
             event.keysym = 'BackSpace'
-            self.click_on()
+            self._click_on()
             for _ in range(len(self.value)):
-                self.input(event, True)
-            self.click_off()
+                self._input(event, True)
+            self._click_off()
         else:
             self.value = self._value[0] = ''
             self.master.itemconfigure(self.text, text='')
 
     def get(self):  # type: () -> str
-        """ 内部方法：获取输入框的值 """
+        """ 获取输入框的值 """
         return self.value
 
     def set(self, value):  # type: (str) -> None
         """ 设置输入框的值 """
         self.value = self._value[0] = value
         self.master.itemconfigure(self.text, text=self._value[0])
 
@@ -842,15 +868,15 @@
         for s in value:
             event.char = s
             self.input(event, True)
         self.click_off()
 
 
 class Label(BaseWidget):
-    """ 创建一个虚拟的标签控件，用于显示少量文本 """
+    """ 虚拟标签控件 """
 
     def __init__(
         self,
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
@@ -865,23 +891,23 @@
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_BUTTON_OUTLINE  # type: tuple[str, str, str]
     ):  # type: (...) -> None
         BaseWidget.__init__(self, canvas, x, y, width, height, radius, text, justify,
                             borderwidth, font, image, color_text, color_fill, color_outline)
 
-    def touch(self, event):  # type: (tkinter.Event) -> bool
+    def _touch(self, event):  # type: (tkinter.Event) -> bool
         """ 触碰状态检测 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         self.state('touch' if condition else 'normal')
         return condition
 
 
 class Button(BaseWidget):
-    """ 创建一个虚拟的按钮，并执行关联函数 """
+    """ 虚拟按钮控件 """
 
     def __init__(
         self,
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
@@ -898,36 +924,36 @@
         color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_BUTTON_OUTLINE,  # type: tuple[str, str, str]
     ):  # type: (...) -> None
         BaseWidget.__init__(self, canvas, x, y, width, height, radius, text, justify,
                             borderwidth, font, image, color_text, color_fill, color_outline)
         self.command = command
 
-    def execute(self, event):  # type: (tkinter.Event) -> None
+    def _execute(self, event):  # type: (tkinter.Event) -> None
         """ 执行关联函数 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         if condition and self.command:
             self.command()
 
-    def click(self, event):  # type: (tkinter.Event) -> None
+    def _click(self, event):  # type: (tkinter.Event) -> None
         """ 交互状态检测 """
         if self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2:
             self.state('click')
         else:
             self.state('normal')
 
-    def touch(self, event):  # type: (tkinter.Event) -> bool
+    def _touch(self, event):  # type: (tkinter.Event) -> bool
         """ 触碰状态检测 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         self.state('touch' if condition else 'normal')
         return condition
 
 
 class CheckButton(Button):
-    """ 创建一个复选框 """
+    """ 虚拟复选框控件 """
 
     def __init__(
         self,
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         length,  # type: int
@@ -961,15 +987,15 @@
     def set(self, value):  # type: (bool) -> None
         """ 设置复选框状态 """
         self.value = TICK if value else ''
         self.master.itemconfigure(self.text, text=self.value)
 
 
 class Entry(TextWidget):
-    """ 创建一个虚拟的输入框控件，可输入单行少量字符，并获取这些字符 """
+    """ 虚拟输入框控件 """
 
     def __init__(
         self,
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
@@ -989,31 +1015,31 @@
         color_outline=COLOR_TEXT_OUTLINE  # type: tuple[str, str, str]
     ):  # type: (...) -> None
         TextWidget.__init__(self, canvas, x, y, width, height, radius, text, limit, justify,
                             cursor, borderwidth, font, image, color_text, color_fill, color_outline)
         self.master.itemconfigure(self.text, text=self._value[1])
         self.show = show
 
-    def click_on(self):  # type: () -> None
+    def _click_on(self):  # type: () -> None
         """ 控件获得焦点 """
         self.state('click')
         self.master.itemconfigure(self.text, text=self._value[0])
-        self.cursor_update('')
-        self.cursor_flash()
+        self._cursor_update('')
+        self._cursor_flash()
 
-    def click_off(self):  # type: () -> None
+    def _click_off(self):  # type: () -> None
         """ 控件失去焦点 """
         self.state('normal')
 
         if self.value == '':
             self.master.itemconfigure(self.text, text=self._value[1])
         else:
             self.master.itemconfigure(self.text, text=self._value[0])
 
-    def input(self, event, flag=False):  # type: (tkinter.Event, bool) -> None
+    def _input(self, event, flag=False):  # type: (tkinter.Event, bool) -> None
         """ 文本输入 """
         if self._state == 'click' or flag:
             if event.keysym == 'BackSpace':  # 按下退格键
                 self.value = self.value[:-1]
             elif len(self.value) == self.limit:  # 达到字数限制
                 return True
             elif len(event.char):
@@ -1025,31 +1051,31 @@
                 return True
 
             self._value[0] = len(  # 更新表面显示值
                 self.value) * self.show if self.show else self.value
 
             # 更新显示
             self.master.itemconfigure(self.text, text=self._value[0])
-            self.update_text()
-            self.cursor_update()
+            self._update_text()
+            self._cursor_update()
             return True
 
-    def update_text(self):  # type: () -> None
+    def _update_text(self):  # type: () -> None
         """ 更新控件 """
         while True:
             pos = self.master.bbox(self.text)
             if pos[2] > self.x2-self.radius-2 or pos[0] < self.x1+self.radius+1:
                 self._value[0] = self._value[0][1:]
                 self.master.itemconfigure(self.text, text=self._value[0])
             else:
                 break
 
 
 class Text(TextWidget):
-    """ 创建一个透明的虚拟文本框，用于输入多行文本和显示多行文本 """
+    """ 虚拟文本框控件 """
 
     def __init__(
         self,
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
@@ -1086,70 +1112,70 @@
 
         # 修改多行文本靠左显示
         self.master.coords(self.text, _x, y+radius+2)
         self.master.itemconfigure(
             self.text, text=self._value[1], anchor=_anchor)
         self.master.itemconfigure(self._cursor, anchor='n')
 
-    def click_on(self):  # type: () -> None
+    def _click_on(self):  # type: () -> None
         """ 控件获得焦点 """
         if not self.read:
             self.state('click')
             *__, _ = [''] + self._value[0].rsplit('\n', 1)
             self.master.itemconfigure(self.text, text=''.join(__))
             self.master.itemconfigure(self._text, text=_)
-            self.cursor_update('')
-            self.cursor_flash()
+            self._cursor_update('')
+            self._cursor_flash()
 
-    def click_off(self):  # type: () -> None
+    def _click_off(self):  # type: () -> None
         """ 控件失去焦点 """
         self.state('normal')
 
         if self.value == '':
             self.master.itemconfigure(self.text, text=self._value[1])
         else:
             *__, _ = [''] + self._value[0].rsplit('\n', 1)
             self.master.itemconfigure(self.text, text=''.join(__))
             self.master.itemconfigure(self._text, text=_)
 
-    def input(self, event, flag=False):  # type: (tkinter.Event, bool) -> bool
+    def _input(self, event, flag=False):  # type: (tkinter.Event, bool) -> bool
         """ 文本输入 """
         if self._state == 'click' or flag:
             if event.keysym == 'BackSpace':  # 按下退格键
-                self.input_backspace()
+                self._input_backspace()
             elif len(self.value) == self.limit:  # 达到字数限制
                 return True
             elif event.keysym == 'Tab':  # 按下Tab键
                 self.append(' '*4)
             elif event.keysym == 'Return' or event.char == '\n':  # 按下回车键
-                self.input_return()
+                self._input_return()
             elif event.char.isprintable() and event.char:  # 按下其他普通的键
                 _text = self.master.itemcget(self._text, 'text')
                 self.master.itemconfigure(self._text, text=_text+event.char)
                 _pos = self.master.bbox(self._text)
 
                 if _pos[2] > self.x2-self.radius-2 or _pos[0] < self.x1+self.radius+1:  # 文本溢出啦
                     self.master.itemconfigure(self._text, text=_text)
-                    self.input_return()
+                    self._input_return()
                     self.master.itemconfigure(self._text, text=event.char)
 
                 self.value += event.char
             else:
                 return True
 
-            self.cursor_update()
+            self._cursor_update()
 
             # 更新表面显示值
             text = self.master.itemcget(self.text, 'text')
             _text = self.master.itemcget(self._text, 'text')
             self._value[0] = text+'\n'+_text
 
             return True
 
-    def input_return(self):  # type: () -> None
+    def _input_return(self):  # type: () -> None
         """ 回车键功能 """
         self.value += '\n'
 
         # 相关数据获取
         text = self.master.itemcget(self.text, 'text')
         _text = self.master.itemcget(self._text, 'text')
         _pos = self.master.bbox(self._text)
@@ -1160,15 +1186,15 @@
             self.master.move(self._text, 0, _pos[3] - _pos[1])
             self.master.itemconfigure(
                 self.text, text=text+bool(text)*'\n'+_text)
         else:  # 文本框已经被填满了
             text = text.split('\n', 1)[-1]
             self.master.itemconfigure(self.text, text=text+'\n'+_text)
 
-    def input_backspace(self):  # type: () -> None
+    def _input_backspace(self):  # type: () -> None
         """ 退格键功能 """
         if not self.value:  # 没有内容，删个毛啊
             return
 
         _text = self.master.itemcget(self._text, 'text')
         self.value = self.value[:-1]
 
@@ -1191,17 +1217,21 @@
                 temp = self.value[:-len(text)
                                   ] if self.value.endswith(text) else self.value
                 temp2 = text[:len(_)] if text.endswith(_) else text
                 __ = temp[:-1].rsplit('\n', 1)[-1]+'\n'+temp2[:-1]
 
             self.master.itemconfigure(self.text, text=__)
 
+    def _scroll(self, event):  # type: (tkinter.Event) -> bool
+        """ 鼠标滚轮滚动 """
+        return False  # TODO: 暂未实现
+
 
 class Progressbar(BaseWidget):
-    """ 虚拟的进度条，可以直观的方式显示任务进度 """
+    """ 虚拟进度条控件 """
 
     def __init__(
         self,
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
@@ -1221,61 +1251,58 @@
             x, y, x, y+height, width=borderwidth, outline='', fill=color_bar[1])
 
         BaseWidget.__init__(self, canvas, x, y, width, height, 0, '0.00%', justify,
                             borderwidth, font, image, color_text, COLOR_NONE, color_outline)
 
         self.color_fill = list(color_bar)
 
-    def touch(self, event):  # type: (tkinter.Event) -> bool
+    def _touch(self, event):  # type: (tkinter.Event) -> bool
         """ 触碰状态检测 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         self.state('touch' if condition else 'normal')
         return condition
 
     def load(self, percentage):  # type: (float) -> None
         """
-        进度条加载，并更新外观\n
-        ---
-        `percentage`: 进度条的值，范围 0 ~ 1\n
+        ### 加载
+        `percentage`: 进度条的值，范围 0 ~ 1
         """
         percentage = 0 if percentage < 0 else 1 if percentage > 1 else percentage
         x2 = self.x1 + self.width * percentage * self.master.rx
         self.master.coords(self.bar, self.x1, self.y1, x2, self.y2)
         self.configure(text='%.2f%%' % (percentage * 100))
 
 
 class PhotoImage(tkinter.PhotoImage):
-    """ 生成图片并进行相应的一些处理 """
+    """ 图片类 """
 
     def __init__(
         self,
         file,  # type: str | bytes
         **kw
     ):  # type: (...) -> None
         """
-        初始化参数\n
-        ---
-        `file`: 图片文件的路径\n
-        `**kw`: 与 tkinter.PhotoImage 的参数相同\n
+        `file`: 图片文件的路径 \ 
+        `**kw`: 与 tkinter.PhotoImage 的参数相同
         """
         self.file = file  # 图片文件的路径
         self.extension = file.rsplit('.', 1)[-1]  # 文件扩展名
         self._item = {}  # type: dict[tkinter._CanvasItemId, Canvas | None]
 
         if self.extension == 'gif':  # 动态图片
             self.image = []  # type: list[tkinter.PhotoImage]
         else:  # 静态图片
             self.image = tkinter.PhotoImage.__init__(self, file=file, **kw)
 
     def parse(self, start=0):  # type: (int) -> Generator[int, None, None]
         """
         ### 解析动图
-        解析并得到动图的每一帧动画，该方法返回一个生成器\n
+        解析并得到动图的每一帧动画，该方法返回一个生成器 \n 
         ---
-        `start`: 动图解析的起始索引（帧数-1）\n
+        `start`: 动图解析的起始索引（帧数-1）
         """
         try:
             while True:
                 self.image.append(tkinter.PhotoImage(
                     file=self.file, format='gif -index %d' % start))
                 value = yield start  # 抛出索引
                 start += value if value else 1
@@ -1287,19 +1314,19 @@
         canvas,  # type: Canvas
         item,  # type: tkinter._CanvasItemId
         interval,  # type: int
         **kw
     ):  # type: (...) -> None
         """
         ### 播放动图
-        播放动图，设置 canvas.lock 为 False 会暂停\n
+        播放动图，设置 canvas.lock 为 False 会暂停 \n 
         ---
-        `canvas`: 播放动画的画布\n
-        `item`: 播放动画的 _CanvasItemId（create_text 的返回值）\n
-        `interval`: 每帧动画的间隔时间\n
+        `canvas`: 播放动画的画布 \ 
+        `item`: 播放动画的 _CanvasItemId（create_text 的返回值） \ 
+        `interval`: 每帧动画的间隔时间
         """
         if kw.get('_ind', None) is None:  # 初始化的判定
             self._item[item], kw['ind'] = canvas, -1
         if not self._item[item]:  # 终止播放的判定
             return
         if canvas._lock:  # 暂停播放的判定
             canvas.itemconfigure(item, image=self.image[kw['_ind']])
@@ -1310,36 +1337,36 @@
     def stop(
         self,
         item,  # type: tkinter._CanvasItemId
         clear=False  # type: bool
     ):  # type: (...) -> None
         """
         ### 终止播放
-        终止对应动图的播放，且无法重新播放\n
+        终止对应动图的播放，且无法重新播放 \n 
         ---
-        `item`: 播放动画的 _CanvasItemId（create_text 的返回值）\n
-        `clear`: 清除图片的标识, True 就清除图片\n
+        `item`: 播放动画的 _CanvasItemId（create_text 的返回值） \ 
+        `clear`: 清除图片的标识，为 True 就清除图片
         """
         self._item[item] = None
         if clear:  # 清除背景
             self._item[item].itemconfigure(item, image=None)
 
     def zoom(
         self,
         rate_x,  # type: float
         rate_y,  # type: float
         precision=None  # type: float | None
     ):  # type: (...) -> tkinter.PhotoImage
         """
         ### 缩放图片
-        不会缩放该图片对象本身，只是返回一个缩放后的图片对象\n
+        不会缩放该图片对象本身，只是返回一个缩放后的图片对象 \n 
         ---
-        `rate_x`: 横向缩放倍率\n
-        `rate_y`: 纵向缩放倍率\n
-        `precision`: 精度到小数点后的位数（推荐 1.2），越大运算就越慢（默认值代表绝对精确）\n
+        `rate_x`: 横向缩放倍率 \ 
+        `rate_y`: 纵向缩放倍率 \ 
+        `precision`: 精度到小数点后的位数（推荐 1.2），越大运算就越慢（默认值代表绝对精确）
         """
         if precision is not None:
             limit = round(10**precision)
             rate_x = Fraction(str(rate_x)).limit_denominator(limit)
             rate_y = Fraction(str(rate_y)).limit_denominator(limit)
             image = tkinter.PhotoImage.zoom(
                 self, rate_x.numerator, rate_y.numerator)
@@ -1352,15 +1379,15 @@
                     image.put('#%02X%02X%02X' % self.get(
                         int(x/rate_x), int(y/rate_y)), (x, y))
 
         return image
 
 
 class Singleton(object):
-    """ 单例模式类，用于继承 """
+    """ 单例模式类 """
 
     _instance = None
 
     def __new__(cls, *args, **kw):
         if not cls._instance:
             cls._instance = object.__new__(cls)
         return cls._instance
@@ -1409,23 +1436,24 @@
     # type: tuple[Callable[[float], float], float, float] | Literal['smooth', 'rebound', 'flat']
     frames=FRAMES,  # type: int
     end=None,  # type: Callable | None
     _ind=0  # type: int
 ):  # type: (...) -> None
     """
     ### 移动函数
-    以特定方式移动由 Place 布局的某个控件或某些控件的集合或图像\n
+    以特定方式移动由 Place 布局的某个控件或某些控件的集合或图像 \ 
+    或者按一定的函数规律来移动
     ---
-    `master`: 控件所在的父控件\n
-    `widget`: 要移动位置的控件\n
-    `dx`: 横向移动的距离（单位：像素）\n
-    `dy`: 纵向移动的距离（单位：像素）\n
-    `times`: 移动总时长（单位：毫秒）\n
-    `mode`: 移动速度模式，为 smooth（顺滑）、rebound（回弹）和 flat（平移）这三种，或者为元组 (函数, 起始值, 终止值) 的形式\n
-    `frames`: 帧数，越大移动就越流畅，但计算越慢（范围为 1 ~ 100）\n
+    `master`: 控件所在的父控件 \ 
+    `widget`: 要移动位置的控件 \ 
+    `dx`: 横向移动的距离（单位：像素） \ 
+    `dy`: 纵向移动的距离（单位：像素） \ 
+    `times`: 移动总时长（单位：毫秒） \ 
+    `mode`: 移动速度模式，为 smooth（顺滑）、rebound（回弹）和 flat（平移）这三种，或者为元组 (函数, 起始值, 终止值) 的形式 \ 
+    `frames`: 帧数，越大移动就越流畅，但计算越慢（范围为 1 ~ 100） \ 
     `end`: 移动结束时执行的函数
     """
     if _ind:  # 记忆值
         dis = mode
     elif mode == 'flat':  # 平滑模式
         return move(master, widget, dx, dy, times, mode=(lambda _: 1, 0, 1), frames=frames, end=end)
     elif mode == 'smooth':  # 流畅模式
@@ -1465,19 +1493,20 @@
 def text(
     length,  # type: int
     string,  # type: str
     position='center'  # type: Literal['left', 'center', 'right']
 ):  # type: (...) -> str
     """
     ### 文本对齐函数
-    可将目标字符串改为目标长度并居中对齐，ASCII 码字符算 1 个长度，中文及其他字符算 2 个\n
+    可将目标字符串改为目标长度并居中对齐 \ 
+    ASCII 字符算 1 个长度，中文及其他字符算 2 个
     ---
-    `length`: 目标长度\n
-    `string`: 要修改的字符串\n
-    `position`: 文本处于该长度范围的位置，可选 left（靠左）、center（居中）和 right（靠右）这三个值\n
+    `length`: 目标长度 \ 
+    `string`: 要修改的字符串 \ 
+    `position`: 文本处于该长度范围的位置，可选 left（靠左）、center（居中）和 right（靠右）这三个值
     """
     length -= sum(1 + (ord(i) >= 256) for i in string)  # 计算空格总个数
     if position == 'left':  # 靠左
         return ' '*length+string
     elif position == 'right':  # 靠右
         return string+length*' '
     else:  # 居中
@@ -1503,18 +1532,19 @@
 
 def color(
     color,  # type: Iterable[str] | str
     proportion=1.  # type: float
 ):  # type: (...) -> str
     """
     ### 颜色函数
-    按一定比例给出已有 RGB 颜色字符串的渐变 RGB 颜色字符串，或颜色的对比色\n
+    按一定比例给出已有 RGB 颜色字符串的渐变 RGB 颜色字符串 \ 
+    或者给出已有 RGB 颜色字符串的对比色
     ---
-    `color`: 颜色元组或列表 (初始颜色, 目标颜色)，或者一个颜色字符串（此时返回其对比色）\n
-    `proportion`: 改变比例（浮点数，范围为 0 ~ 1）\n
+    `color`: 颜色元组或列表 (初始颜色, 目标颜色)，或者一个颜色字符串（此时返回其对比色） \ 
+    `proportion`: 改变比例（浮点数，范围为 0 ~ 1）
     """
     rgb, _rgb = [[None]*3, [None]*3], 0
 
     if isinstance(color, str):  # 对比色的情况处理
         color = color, '#%06X' % (16777216-int(color[1:], 16))
 
     for i, c in enumerate(color):  # 解析颜色的 RGB
@@ -1532,20 +1562,20 @@
 def askfont(
     root,  # type: tkinter.Tk | tkinter.Canvas | Tk | Toplevel | Canvas
     bind=None,  # type: Callable[[str], Any] | None
     initfont=''  # type: tuple[str, int, str] | tuple[str, int] | str
 ):  # type: (...) -> None
     """
     ### 字体选择对话框
-    弹出选择字体的默认对话框窗口\n
-    注意：由于 tkinter 模块无法直接打开该窗口，所以此处添加了这个函数\n
+    弹出选择字体的默认对话框窗口 \ 
+    注意: 由于 tkinter 模块无法直接打开该窗口，所以此处添加了这个函数
     ---
-    `root`: 父容器控件\n
-    `bind`: 关联函数，有且仅有一个参数 font\n
-    `initfont`: 初始字体，格式为 font 参数默认格式\n
+    `root`: 父容器控件 \ 
+    `bind`: 关联函数，有且仅有一个参数 font \ 
+    `initfont`: 初始字体，格式为 font 参数默认格式
     """
     args = []
     if bind:
         args += ['-command', root.register(bind)]
     if initfont:
         if isinstance(initfont, tuple):
             initfont = ' '.join(str(i) for i in initfont)
@@ -1556,16 +1586,16 @@
 
 
 def SetProcessDpiAwareness(
     awareness=PROCESS_SYSTEM_DPI_AWARE  # type: Literal[0, 1, 2]
 ):  # type: (...) -> None
     """
     ### 设定程序 DPI 级别
-    设定窗口程序的 DPI 级别，让系统知道该如何对程序进行缩放，以提升高缩放倍数情况下的清晰度\n
-    注意：
+    设定窗口程序的 DPI 级别，让系统知道该如何对程序进行缩放，以提升高缩放倍数情况下的清晰度 \ 
+    注意: 
     * 此函数仅在 Windows 平台上生效！
     * tkintertools 程序已内置该功能，该函数不应在 tkintertools 程序中使用，而应该在 tkinter 程序中使用！
     ---
-    `awareness`: DPI 级别，值可以为 0、1 和 2，本来默认为 0，此处更改默认值为 1\n
+    `awareness`: DPI 级别，值可以为 0、1 和 2，本来默认为 0，此处更改默认值为 1
     """
     if WinDLL:
         WinDLL('shcore').SetProcessDpiAwareness(awareness)
```

### Comparing `tkintertools-2.6.6.dev0/tkintertools/constants.py` & `tkintertools-2.6.7.dev0/tkintertools/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """ All constants """
 
-import platform
+import platform  # Get information about the platform
+
+### System constants ###
+
 
 SYSTEM = platform.system()
 """ Operating System """
 
 PROCESS_SYSTEM_DPI_AWARE = 1
 """ Default DPI aware """
 
 
+### Color constants ###
+
+
 COLOR_BUTTON_FILL = '#E1E1E1', '#E5F1FB', '#CCE4F7', '#E0E0E0'
 """ Default button fill color """
 
 COLOR_BUTTON_OUTLINE = '#C0C0C0', '#288CDB', '#4884B4', '#D0D0D0'
 """ Default button outline color """
 
 COLOR_TEXT_FILL = '#FFFFFF', '#FFFFFF', '#FFFFFF', '#E0E0E0'
@@ -27,14 +33,17 @@
 COLOR_NONE = '', '', '', ''
 """ Default transparent color tuple """
 
 COLOR_BAR = '#E1E1E1', '#06b025'
 """ Default progress bar color """
 
 
+### Other constants ###
+
+
 BORDERWIDTH = 1
 """ Default widget borderwidth """
 
 CURSOR = '│'
 """ text cursor """
 
 FONT = 'Microsoft YaHei' if SYSTEM == 'Windows' else 'DejaVu Sans' if SYSTEM == 'linux' else 'Arial'
@@ -53,17 +62,22 @@
 FRAMES = 60
 """ Default move frame rate """
 
 TICK = '✓'
 """ Default checkbox symbol """
 
 
+### 3D constants ###
+
+
 CAMERA_DISTANCE = 1000
 """ Default 3D camera distance """
 
+ROTATE_CENTER = 0, 0, 0
+""" Default rotation center """
 
 COLOR_POINT_FILL = '#000000'
 """ Default point fill color """
 
 COLOR_POINT_OUTLINE = '#000000'
 """ Default point outline color """
 
@@ -84,9 +98,24 @@
 
 LINE_WDITH = 1
 """ Default line width """
 
 SIDE_WIDTH = 1
 """ Default side width """
 
+ORIGIN_COORDINATE = 0, 0, 0
+""" Default origin coordinate """
+
+ORIGIN_SIZE = POINT_SIZE
+""" Default origin size """
+
+ORIGIN_WIDTH = POINT_WIDTH
+""" Default origin width """
+
+ORIGIN_FILL = ''
+""" Default origin fill color """
+
+ORIGIN_OUTLINE = ''
+""" Default origin outline color """
+
 
-__all__ = [name for name in globals() if name.isupper()]
+all_constants = [name for name in globals() if name.isupper()]
```

### Comparing `tkintertools-2.6.6.dev0/tkintertools/tools_3d.py` & `tkintertools-2.6.7.dev0/tkintertools/tools_3d.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,77 +3,78 @@
 import math  # 数学支持
 import statistics  # 数据统计
 from abc import ABCMeta, abstractmethod  # 抽象类
 from tkinter import Event  # 类型提示
 from typing import Iterable  # 类型提示
 
 from .__main__ import Canvas, Tk, Toplevel  # 继承和类型提示
-from .constants import *
+from .constants import *  # 常量
 
 
-def translate(coords, dx=0, dy=0, dz=0):
+def translate(coordinate, dx=0, dy=0, dz=0):
     # type: (list[float], float, float, float) -> None
     """
     ### 平移
-    将一个空间三维中的点进行平移\n
+    将一个三维空间中的点进行平移 \n
     ---
-    `coords`: 被平移点的空间坐标列表\n
-    `dx`: x 方向位移\n
-    `dy`: y 方向位移\n
-    `dz`: z 方向位移\n
+    `coordinate`: 点的空间坐标 \ 
+    `dx`: x 方向位移长度 \ 
+    `dy`: y 方向位移长度 \ 
+    `dz`: z 方向位移长度
     """
-    coords[0] += dx
-    coords[1] += dy
-    coords[2] += dz
+    for i, delta in enumerate((dx, dy, dz)):
+        coordinate[i] += delta
 
 
-def rotate(coords, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
+def rotate(coordinate, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
     # type: (list[float], float, float, float, ..., Iterable[float]) -> None
     """
     ### 旋转
-    将一个空间三维中的点以另一个点为旋转中心进行旋转\n
+    将一个三维空间中的点以另一个点为旋转中心进行旋转 \n
     ---
-    `coords`: 被旋转点的空间坐标列表\n
-    `dx`: x 方向旋转弧度\n
-    `dy`: y 方向旋转弧度\n
-    `dz`: z 方向旋转弧度\n
-    `center`: 旋转中心的空间坐标列表\n
+    `coordinate`: 点的空间坐标 \ 
+    `dx`: x 方向旋转弧度 \ 
+    `dy`: y 方向旋转弧度 \ 
+    `dz`: z 方向旋转弧度 \ 
+    `center`: 旋转中心的空间坐标，默认值为元组 (0, 0, 0)
     """
     sx, sy, sz = math.sin(dx), math.sin(dy), math.sin(dz)
     cx, cy, cz = math.cos(dx), math.cos(dy), math.cos(dz)
 
-    matrix = [[cz*cy, cz*sy*sx-sz*cx, cz*sy*cx+sz*sx],
-              [sz*cy, sz*sy*sx+cz*cx, sz*sy*cx-cz*sx],
-              [-sy,   cy*sx,          cy*cx]]
+    matrix = [[cz * cy, cz * sy * sx - sz * cx, cz * sy * cx + sz * sx],
+              [sz * cy, sz * sy * sx + cz * cx, sz * sy * cx - cz * sx],
+              [-sy,     cy * sx,                cy * cx]]
 
-    for i in range(3):
-        matrix[0][i] = center[i] + \
-            sum(matrix[i][j]*(coords[j]-center[j]) for j in range(3))
+    for i, c_i in enumerate(center):
+        matrix[0][i] = c_i + sum(
+            matrix[i][j] * (coordinate[j] - c_j) for j, c_j in enumerate(center))
 
-    coords[:] = matrix[0]
+    coordinate[:] = matrix[0]
 
 
-def scale(coords, kx=1, ky=1, kz=1, *, center=None):
-    # type: (list[float], float, float, float, ..., Iterable[float] | None) -> None
+def scale(coordinate, kx=1, ky=1, kz=1, *, center):
+    # type: (list[float], float, float, float, ..., Iterable[float]) -> None
     """
     ### 缩放
-    将一个空间三维中的点以另一个点为缩放中心进行位置缩放\n
+    将一个三维空间中的点以另一个点为缩放中心进行缩放 \n
     ---
-    `coords`: 被缩放点的空间坐标列表\n
-    `dx`: x 方向缩放比例\n
-    `dy`: y 方向缩放比例\n
-    `dz`: z 方向缩放比例\n
-    `center`: 缩放中心的空间坐标列表\n
+    `coordinate`: 点的空间坐标 \ 
+    `kx`: x 方向缩放比例 \ 
+    `ky`: y 方向缩放比例 \ 
+    `kz`: z 方向缩放比例 \ 
+    `center`: 缩放中心的空间坐标
     """
-    for i, k in zip(range(3), (kx, ky, kz)):
-        coords[i] += (coords[i] - center[i]) * (k - 1)
+    if kx <= 0 or ky <= 0 or kz <= 0:  # 限制缩放比例的范围
+        raise ValueError('invalid scaling factor')
+    for i, k in enumerate((kx, ky, kz)):
+        coordinate[i] += (coordinate[i] - center[i]) * (k - 1)
 
 
 class Canvas_3D(Canvas):
-    """ 3D画布，支持3d绘图 """
+    """ 3D 画布基类 """
 
     def __init__(
         self,
         master,  # type: Tk | Toplevel
         width,  # type: int
         height,  # type: int
         x=None,  # type: int | None
@@ -82,52 +83,51 @@
         lock=True,  # type: bool
         expand=True,  # type: bool
         keep=True,  # type: bool
         camera_distance=CAMERA_DISTANCE,  # type: float
         **kw
     ):  # type: (...) -> None
         """
-        `master`: 父控件\n
-        `width`: 画布宽度\n
-        `height`: 画布高度\n
-        `x`: 画布左上角的横坐标\n
-        `y`: 画布左上角的纵坐标\n
-        `lock`: 画布内控件的功能锁，False 时功能暂时失效\n
-        `expand`: 画布内控件是否能缩放\n
-        `keep`: 画布比例是否保持不变\n
-        `camera_distance`: 3D 绘图时相机与原点的距离，默认值为 1000\n
-        `**kw`: 与 tkinter.Canvas 类的参数相同\n
+        `master`: 父控件 \ 
+        `width`: 画布宽度 \ 
+        `height`: 画布高度 \ 
+        `x`: 画布左上角的横坐标 \ 
+        `y`: 画布左上角的纵坐标 \ 
+        `lock`: 画布内控件的功能锁，为 False 时功能暂时失效 \ 
+        `expand`: 画布内控件是否能缩放 \ 
+        `keep`: 画布比例是否保持不变 \ 
+        `camera_distance`: 相机位置与原点间的距离，默认值为 1000 \ 
+        `**kw`: 与 tkinter.Canvas 类的参数相同
         """
-        Canvas.__init__(self, master, width, height, x, y,
-                        lock=lock, expand=expand, keep=keep, **kw)
+        Canvas.__init__(
+            self, master, width, height, x, y, lock=lock, expand=expand, keep=keep, **kw)
         self.distance = camera_distance
         self._items_3d = []  # type: list[Point | Line | Side]
         self._geos = []  # type: list[Geometry]
-        self.configure(  # 使画布视野居中
-            scrollregion=(-self.width[1]/2, -self.height[1]/2, self.width[1]/2, self.height[1]/2))
+        self._zoom()  # 更新画布视野
 
-    def zoom(self, rate_x=None, rate_y=None):  # type: (float | None, float | None) -> None
+    def _zoom(self, rate_x=None, rate_y=None):  # type: (float | None, float | None) -> None
         # override: 保持画布视野居中
-        Canvas.zoom(self, rate_x, rate_y)
-        half_width, half_height = self.width[1]/2, self.height[1]/2
-        self.configure(scrollregion=(-half_width, -
-                       half_height, half_width, half_height))
+        Canvas._zoom(self, rate_x, rate_y)
+        half_width, half_height = self.width[1] / 2, self.height[1] / 2
+        self.configure(
+            scrollregion=(-half_width, -half_height, half_width, half_height))
 
     def items_3d(self):  # type: () -> tuple[Point | Line | Side]
-        """ 返回 `Canvas_3d` 类的 `items_3d` 元组 """
+        """ 返回 `Canvas_3d` 类全部的基本 3D 对象 """
         return tuple(self._items_3d)
 
     def geos(self):  # type: () -> tuple[Geometry]
-        """ 返回 `Canvas_3d` 类的 `geos` 元组 """
+        """ 返回 `Canvas_3d` 类全部的几何体对象 """
         return tuple(self._geos)
 
     def space_sort(self):  # type: () -> None
-        """ 空间位置排序 """
-        self._items_3d.sort(key=lambda item: (
-            not isinstance(item, Point), item.camera_distance()))
+        """ 空间位置排序 """  # BUG: 在距离比较近的两个对象时，仍会显示不正确
+        self._items_3d.sort(
+            key=lambda item: (not isinstance(item, Point), item._camera_distance()))
         for item in self._items_3d:
             self.lower(item.item)
 
 
 class Space(Canvas_3D):
     """ 三维空间 """
 
@@ -139,88 +139,87 @@
         x=None,  # type: int | None
         y=None,  # type: int | None
         *,
         lock=True,  # type: bool
         expand=True,  # type: bool
         keep=True,  # type: bool
         camera_distance=CAMERA_DISTANCE,  # type: float
-        origin_size=POINT_SIZE,  # type: float
-        origin_width=POINT_WIDTH,  # type: float
-        origin_fill='',  # type: str
-        origin_outline='',  # type: str
+        origin_size=ORIGIN_SIZE,  # type: float
+        origin_width=ORIGIN_WIDTH,  # type: float
+        origin_fill=ORIGIN_FILL,  # type: str
+        origin_outline=ORIGIN_OUTLINE,  # type: str
         **kw
     ):  # type: (...) -> None
         """
-        `master`: 父控件\n
-        `width`: 画布宽度\n
-        `height`: 画布高度\n
-        `x`: 画布左上角的横坐标\n
-        `y`: 画布左上角的纵坐标\n
-        `lock`: 画布内控件的功能锁，False 时功能暂时失效\n
-        `expand`: 画布内控件是否能缩放\n
-        `keep`: 画布比例是否保持不变\n
-        `camera_distance`: 3D 绘图时相机与原点的距离，默认值为 1000\n
-        `origin_size`: 原点大小\n
-        `origin_width`: 原点轮廓宽度\n
-        `origin_fill`: 原点内部填充颜色\n
-        `origin_outline`: 原点轮廓颜色\n
-        `**kw`: 与 `tkinter.Canvas` 类的参数相同\n
-        """
-        Canvas_3D.__init__(self, master, width, height, x, y, lock=lock, expand=expand,
-                           keep=keep, camera_distance=camera_distance, **kw)
-        self._origin = Point(self, [0, 0, 0], size=origin_size, width=origin_width,
-                             fill=origin_fill, outline=origin_outline)
+        `master`: 父控件 \ 
+        `width`: 画布宽度 \ 
+        `height`: 画布高度 \ 
+        `x`: 画布左上角的横坐标 \ 
+        `y`: 画布左上角的纵坐标 \ 
+        `lock`: 画布内控件的功能锁，为 False 时功能暂时失效 \ 
+        `expand`: 画布内控件是否能缩放 \ 
+        `keep`: 画布比例是否保持不变 \ 
+        `camera_distance`: 相机位置与原点间的距离，默认值为 1000 \ 
+        `origin_size`: 原点大小，默认值为 1 \ 
+        `origin_width`: 原点轮廓宽度，默认值为 1 \ 
+        `origin_fill`: 原点填充颜色，默认为无色 \ 
+        `origin_outline`: 原点轮廓颜色，默认为无色 \ 
+        `**kw`: 与 tkinter.Canvas 类的参数相同
+        """
+        Canvas_3D.__init__(
+            self, master, width, height, x, y, lock=lock, expand=expand, keep=keep, camera_distance=camera_distance, **kw)
+        self._origin = Point(
+            self, ORIGIN_COORDINATE, size=origin_size, width=origin_width, fill=origin_fill, outline=origin_outline)
         self._items_3d.clear()
-        self.space_sort()
         self.bind('<B3-Motion>', self._translate)
         self.bind('<Button-3>', lambda _: self._translate(_, True))
         self.bind('<ButtonRelease-3>', lambda _: self._translate(_, False))
         self.bind('<B1-Motion>', self._rotate)
         self.bind('<Button-1>', lambda _: self._rotate(_, True))
         self.bind('<ButtonRelease-1>', lambda _: self._rotate(_, False))
         if SYSTEM == 'Linux':  # 兼容 Linux 系统
-            self.bind('<Button-4>', lambda _: self._zoom(_, True))
-            self.bind('<Button-5>', lambda _: self._zoom(_, False))
+            self.bind('<Button-4>', lambda _: self._scale(_, True))
+            self.bind('<Button-5>', lambda _: self._scale(_, False))
         else:
-            self.bind('<MouseWheel>', self._zoom)
+            self.bind('<MouseWheel>', self._scale)
 
-    def _translate(self, event, flag=None, cache=[]):
+    def _translate(self, event, flag=None, _cache=[]):
         # type: (Event, bool | None, list[float]) -> None
-        """ 平移视角 """
+        """ 平移事件 """
         if flag is True:  # 按下
-            cache[:] = [event.x, event.y]
+            _cache[:] = [event.x, event.y]
             return self.configure(cursor='fleur')
         elif flag is False:  # 松开
             return self.configure(cursor='arrow')
-        dx, dy = event.x-cache[0], event.y-cache[1]
-        cache[:] = [event.x, event.y]
+        dx, dy = event.x-_cache[0], event.y-_cache[1]
+        _cache[:] = [event.x, event.y]
         for item in self._items_3d+[self._origin]:
             item.translate(
                 0, dx*self.width[0]/self.width[1], dy*self.height[0]/self.height[1])
             item.update()
         self.space_sort()
 
-    def _rotate(self, event, flag=None, cache=[]):
+    def _rotate(self, event, flag=None, _cache=[]):
         # type: (Event, bool | None, list[float]) -> None
-        """ 旋转视角 """
+        """ 旋转事件 """
         if flag is True:
-            cache[:] = [event.x, event.y]
+            _cache[:] = [event.x, event.y]
             return self.configure(cursor='fleur')
         elif flag is False:
             return self.configure(cursor='arrow')
-        dx, dy = event.x-cache[0], event.y-cache[1]
-        cache[:] = [event.x, event.y]
+        dx, dy = event.x-_cache[0], event.y-_cache[1]
+        _cache[:] = [event.x, event.y]
         for item in self._items_3d:
             item.rotate(0, -2*dy/self.width[1]*math.tau, 2*dx /
                         self.height[1]*math.tau, center=self._origin.coords)
             item.update()
         self.space_sort()
 
-    def _zoom(self, event, flag=None):  # type: (Event, bool | None) -> None
-        """ 缩放视角 """
+    def _scale(self, event, flag=None):  # type: (Event, bool | None) -> None
+        """ 缩放事件 """
         if flag is not None:
             event.delta = flag
         k = 1.1 if event.delta > 0 else 0.9
         for item in self._items_3d:
             item.scale(k, k, k, center=self._origin.coords)
             item.update()
         self.space_sort()
@@ -228,130 +227,143 @@
 
 class _3D_Object(metaclass=ABCMeta):
     """ 3D 对象抽象元类 """
 
     @abstractmethod
     def translate(self, dx=0, dy=0, dz=0):
         """
-        平移\n
-        `dx`: x 轴方向位移距离\n
-        `dy`: y 轴方向位移距离\n
-        `dz`: z 轴方向位移距离\n
+        ### 平移
+        `dx`: x 方向位移长度 \ 
+        `dy`: y 方向位移长度 \ 
+        `dz`: z 方向位移长度
         """
 
     @abstractmethod
-    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
+    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
         """
-        旋转\n
-        `dx`: 绕x 轴方向旋转弧度\n
-        `dy`: 绕y 轴方向旋转弧度\n
-        `dz`: 绕z 轴方向旋转弧度\n
-        `center`: 旋转中心\n
+        ### 旋转
+        `dx`: x 方向旋转弧度 \ 
+        `dy`: y 方向旋转弧度 \ 
+        `dz`: z 方向旋转弧度 \ 
+        `center`: 旋转中心，默认为原点
         """
 
     @abstractmethod
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         """
-        缩放\n
-        `kx`: x 轴方向缩放比例\n
-        `ky`: y 轴方向缩放比例\n
-        `kz`: z 轴方向缩放比例\n
-        `center`: 缩放中心，默认为几何中心\n
+        ### 缩放
+        `kx`: x 方向缩放比例 \ 
+        `ky`: y 方向缩放比例 \ 
+        `kz`: z 方向缩放比例 \ 
+        `center`: 缩放中心，默认为几何中心
         """
 
     @abstractmethod
-    def project(self, distance):
+    def center(self):
+        """ 几何中心 """
+
+    @abstractmethod
+    def _project(self, distance):
         """
-        投影\n
-        `distance`: 对象与观察者的距离\n
+        ### 投影
+        `distance`: 对象与观察者的距离
         """
 
 
 class _Point(_3D_Object):
-    """ 点 """
+    """ 点（基类） """
 
     def __init__(self, coords):  # type: (list[float]) -> None
         self.coords = coords  # 利用列表引用
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         translate(self.coords, dx, dy, dz)
 
-    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
+    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
         # type: (float, float, float, ..., Iterable[float]) -> None
         rotate(self.coords, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         scale(self.coords, kx, ky, kz, center=center)
 
-    def project(self, distance):  # type: (float) -> list[float]
+    def center(self):  # type: () -> tuple[float, float, float]
+        return tuple(self.coords)
+
+    def _project(self, distance):  # type: (float) -> list[float]
         relative_dis = distance - self.coords[0]
         if relative_dis <= 1e-16:
-            return [float('INF')]*2  # BUG: 目前超出范围只能让其消失
+            return [float('inf')]*2  # BUG: 目前超出范围只能让其消失
         k = distance/relative_dis
         return [self.coords[1]*k, self.coords[2]*k]
 
 
 class _Line(_3D_Object):
-    """ 线 """
+    """ 线（基类） """
 
     def __init__(
         self,
         point_start,  # type: list[float]
         point_end,  # type: list[float]
     ):  # type: (...) -> None
         self.coords = [point_start, point_end]
         self.points = [_Point(point) for point in self.coords]
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         for coord in self.coords:
             translate(coord, dx, dy, dz)
 
-    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
+    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
         # type: (float, float, float, ..., Iterable[float]) -> None
         for coord in self.coords:
             rotate(coord, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         if center is None:
-            center = [statistics.mean(axis) for axis in zip(*self.coords)]
+            center = self.center()
         for coord in self.coords:
             scale(coord, kx, ky, kz, center=center)
 
-    def project(self, distance):  # type: (float) -> list[list[float]]
-        return [point.project(distance) for point in self.points]
+    def center(self):  # type: () -> tuple[float, float, float]
+        return tuple(statistics.mean(coords) for coords in zip(*self.coords))
+
+    def _project(self, distance):  # type: (float) -> list[list[float]]
+        return [point._project(distance) for point in self.points]
 
 
 class _Side(_3D_Object):
-    """ 面 """
+    """ 面（基类） """
 
     def __init__(self, *points):  # type: (list[float]) -> None
         self.coords = list(points)
         self.lines = [_Line(points[ind-1], points[ind])
                       for ind in range(len(points))]
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         for coord in self.coords:
             translate(coord, dx, dy, dz)
 
-    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
+    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
         # type: (float, float, float, ..., Iterable[float]) -> None
         for coord in self.coords:
             rotate(coord, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         if center is None:
-            center = [statistics.mean(axis) for axis in zip(*self.coords)]
+            center = self.center()
         for coord in self.coords:
             scale(coord, kx, ky, kz, center=center)
 
-    def project(self, distance):  # type: (float) -> list[list[list[float]]]
-        return [line.project(distance) for line in self.lines]
+    def center(self):  # type: () -> tuple[float, float, float]
+        return tuple(statistics.mean(coords) for coords in zip(*self.coords))
+
+    def _project(self, distance):  # type: (float) -> list[list[list[float]]]
+        return [line._project(distance) for line in self.lines]
 
 
 class Point(_Point):
     """ 点 """
 
     def __init__(
         self,
@@ -360,40 +372,41 @@
         *,
         size=POINT_SIZE,  # type: float
         width=POINT_WIDTH,  # type: float
         fill=COLOR_POINT_FILL,  # type: str
         outline=COLOR_POINT_OUTLINE,  # type: str
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布\n
-        `coords`: 点的空间坐标\n
-        `size`: 点的大小\n
-        `width`: 点轮廓的宽度\n
-        `fill`: 点内部的填充颜色\n
-        `outline`: 点轮廓的颜色\n
+        `canvas`: 父画布 \ 
+        `coords`: 点的空间坐标 \ 
+        `size`: 点的大小 \ 
+        `width`: 点轮廓的宽度 \ 
+        `fill`: 点内部的填充颜色 \ 
+        `outline`: 点轮廓的颜色
         """
         _Point.__init__(self, list(coords))
         canvas._items_3d.append(self)
         self.canvas = canvas
         self.size = size
         self.width = width
         self.fill = fill
         self.item = canvas.create_oval(
             -1, -1, -1, -1, fill=fill, outline=outline, width=width)
         self.update()
 
-    def update(self) -> None:
-        """ 更新 """
-        x, y = self.project(self.canvas.distance)
+    def update(self):  # type: () -> None
+        """ 更新对象的显示 """
+        x, y = self._project(self.canvas.distance)
         self.canvas.coords(self.item, (x-self.size)*self.canvas.rx, (y-self.size) *
                            self.canvas.ry, (x+self.size)*self.canvas.rx, (y+self.size)*self.canvas.ry)
 
-    def camera_distance(self):  # type: () -> float
+    def _camera_distance(self):  # type: () -> float
         """ 与相机距离 """
-        return math.dist([self.canvas.distance, 0, 0], self.coords)
+        sign = math.copysign(1, self.canvas.distance - self.coords[0])
+        return sign*math.dist([self.canvas.distance, 0, 0], self.coords)
 
 
 class Line(_Line):
     """ 线 """
 
     def __init__(
         self,
@@ -401,118 +414,146 @@
         point_start,  # type: Iterable[float]
         point_end,  # type: Iterable[float]
         *,
         width=LINE_WDITH,  # type: float
         fill=COLOR_LINE_FILL,  # type: str
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布\n
-        `point_start`: 起点坐标\n
-        `point_end`: 终点坐标\n
-        `width`: 线的宽度\n
-        `fill`: 线的颜色\n
+        `canvas`: 父画布 \ 
+        `point_start`: 起点坐标 \ 
+        `point_end`: 终点坐标 \ 
+        `width`: 线的宽度 \ 
+        `fill`: 线的颜色
         """
         _Line.__init__(self, list(point_start), list(point_end))
         canvas._items_3d.append(self)
         self.canvas = canvas
         self.width = width
         self.fill = fill
         self.item = canvas.create_line(-1, -1, -1, -1, width=width, fill=fill)
         self.update()
 
-    def update(self) -> None:
-        """ 更新 """
+    def update(self):  # type: () -> None
+        """ 更新对象的显示 """
         self.canvas.coords(self.item, *[coord*(self.canvas.ry if i else self.canvas.rx)
-                           for point in self.project(self.canvas.distance) for i, coord in enumerate(point)])
+                           for point in self._project(self.canvas.distance) for i, coord in enumerate(point)])
 
-    def camera_distance(self):  # type: () -> float
+    def _camera_distance(self):  # type: () -> float
         """ 与相机距离 """
-        return statistics.mean(math.dist([self.canvas.distance, 0, 0], coord) for coord in self.coords)
+        center = self.center()
+        sign = math.copysign(1, self.canvas.distance - center[0])
+        return sign*math.dist([self.canvas.distance, 0, 0], center)
 
 
 class Side(_Side):
     """ 面 """
 
     def __init__(
         self,
         canvas,  # type: Canvas_3D | Space
         *points,  # type: Iterable[float]
         width=SIDE_WIDTH,  # type: float
         fill=COLOR_SIDE_FILL,  # type: str
         outline=COLOR_SIDE_OUTLINE,  # type: str
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布\n
-        `points`: 各点的空间坐标\n
-        `width`: 面轮廓的宽度\n
-        `fill`: 面内部的填充颜色\n
-        `outline`: 面轮廓的颜色\n
+        `canvas`: 父画布 \ 
+        `points`: 各点的空间坐标 \ 
+        `width`: 面轮廓的宽度 \ 
+        `fill`: 面内部的填充颜色 \ 
+        `outline`: 面轮廓的颜色
         """
         _Side.__init__(self, *[list(point) for point in points])
         canvas._items_3d.append(self)
         self.canvas = canvas
         self.width = width
         self.fill = fill
         self.outline = outline
         self.item = canvas.create_polygon(
             -1, -1, -1, -1, width=width, fill=fill, outline=outline)
         self.update()
 
-    def update(self) -> None:
-        """ 更新 """
+    def update(self):  # type: () -> None
+        """ 更新对象的显示 """
         self.canvas.coords(self.item, *[coord*(self.canvas.ry if i else self.canvas.rx)
-                           for line in self.project(self.canvas.distance) for point in line for i, coord in enumerate(point)])
+                           for line in self._project(self.canvas.distance) for point in line for i, coord in enumerate(point)])
 
-    def camera_distance(self):  # type: () -> float
+    def _camera_distance(self):  # type: () -> float
         """ 与相机距离 """
-        return statistics.mean(math.dist([self.canvas.distance, 0, 0], coord) for coord in self.coords)
+        center = self.center()
+        sign = math.copysign(1, self.canvas.distance - center[0])
+        return sign*math.dist([self.canvas.distance, 0, 0], center)
 
 
 class Geometry:
     """ 几何体 """
 
     def __init__(
         self,
         canvas,  # type: Canvas_3D | Space
         *sides,  # type: Side
     ):  # type: (...) -> None
         """
-        `canvas`: 显示的画布\n
-        `sides`: 组成几何体的面\n
+        `canvas`: 父画布 \ 
+        `sides`: 组成几何体的面
         """
         canvas._geos.append(self)
         self.canvas = canvas
         self.sides = list(sides)
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
+        """
+        ### 平移
+        `dx`: x 方向位移长度 \ 
+        `dy`: y 方向位移长度 \ 
+        `dz`: z 方向位移长度
+        """
         for side in self.sides:
             side.translate(dx, dy, dz)
 
-    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
+    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
         # type: (float, float, float, ..., Iterable[float]) -> None
+        """
+        ### 旋转
+        `dx`: x 方向旋转弧度 \ 
+        `dy`: y 方向旋转弧度 \ 
+        `dz`: z 方向旋转弧度 \ 
+        `center`: 旋转中心，默认为原点
+        """
         for side in self.sides:
             side.rotate(dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
-        if center is None:  # BUG: 公式对凹面几何体不成立
-            center = [statistics.mean(axis) for axis in zip(
-                *set(tuple(coord) for side in self.sides for coord in side.coords))]
+        """
+        ### 缩放
+        `kx`: x 方向缩放比例 \ 
+        `ky`: y 方向缩放比例 \ 
+        `kz`: z 方向缩放比例 \ 
+        `center`: 缩放中心，默认为几何中心
+        """
+        if center is None:
+            center = self.center()
         for side in self.sides:
             side.scale(kx, ky, kz, center=center)
 
+    def center(self):  # type: () -> tuple[float, float, float]
+        """ 几何中心 """
+        # BUG: 公式对凹面几何体不成立
+        return tuple(statistics.mean(axis) for axis in zip(*set(tuple(coord) for side in self.sides for coord in side.coords)))
+
     def update(self):  # type: () -> None
         """ 更新几何体 """
         for side in self.sides:
             side.update()
 
     def append(self, *sides):  # type: (Side) -> None
         """
-        添加面\n
-        `sides`: `Side`类\n
+        ### 添加面
+        `sides`: `Side` 类
         """
         for side in sides:
             self.sides.append(side)
 
 
 class Cuboid(Geometry):
     """ 长方体 """
@@ -531,27 +572,27 @@
         color_down='',  # type: str
         color_left='',  # type: str
         color_right='',  # type: str
         color_front='',  # type: str
         color_back='',  # type: str
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布\n
-        `x`: 左上角x坐标\n
-        `y`: 左上角y坐标\n
-        `z`: 左上角z坐标\n
-        `length`: 长度\n
-        `width`: 宽度\n
-        `height`: 高度\n
-        `color_up`: 上表面颜色\n
-        `color_down`: 下表面颜色\n
-        `color_left`: 左侧面颜色\n
-        `color_right`: 右侧面颜色\n
-        `color_front`: 正面颜色\n
-        `color_back`: 后面颜色\n
+        `canvas`: 父画布 \ 
+        `x`: 左上角 x 坐标 \ 
+        `y`: 左上角 y 坐标 \ 
+        `z`: 左上角 z 坐标 \ 
+        `length`: 长度 \ 
+        `width`: 宽度 \ 
+        `height`: 高度 \ 
+        `color_up`: 上表面颜色 \ 
+        `color_down`: 下表面颜色 \ 
+        `color_left`: 左侧面颜色 \ 
+        `color_right`: 右侧面颜色 \ 
+        `color_front`: 正面颜色 \ 
+        `color_back`: 后面颜色
         """
         canvas._geos.append(self)
         self.canvas = canvas
         coords = [[x+l, y+w, z+h]
                   for l in (0, length)
                   for w in (0, width)
                   for h in (0, height)]
@@ -581,20 +622,20 @@
         point_2,  # type: Iterable[float]
         point_3,  # type: Iterable[float]
         point_4,  # type: Iterable[float]
         *,
         colors=('',)*4  # type: Iterable[str]
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布\n
-        `point_1`: 第一个顶点\n
-        `point_2`: 第二个顶点\n
-        `point_3`: 第三个顶点\n
-        `point_4`: 第四个顶点\n
-        `colors`: 颜色序列\n
+        `canvas`: 父画布 \ 
+        `point_1`: 第一个顶点 \ 
+        `point_2`: 第二个顶点 \ 
+        `point_3`: 第三个顶点 \ 
+        `point_4`: 第四个顶点 \ 
+        `colors`: 颜色序列
         """
         canvas._geos.append(self)
         self.canvas = canvas
         self.sides = [
             Side(canvas, point_1, point_2, point_3, fill=colors[0]),
             Side(canvas, point_1, point_2, point_4, fill=colors[1]),
             Side(canvas, point_1, point_3, point_4, fill=colors[2]),
```

### Comparing `tkintertools-2.6.6.dev0/tkintertools.egg-info/PKG-INFO` & `tkintertools-2.6.7.dev0/tkintertools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.6.dev0
+Version: 2.6.7.dev0
 Summary: An auxiliary module of the tkinter module.
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 Maintainer: Xiaokang2022
 Maintainer-email: 2951256653@qq.com
 License: MulanPSL-2.0
@@ -23,66 +23,66 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/06/29-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/03-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
-[![Wiki](https://img.shields.io/badge/Wiki-15-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
+[![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
 [![Insights](https://repobeats.axiom.co/api/embed/ab8fae686a5a96f91fa71c40c53c189310924f5e.svg)](https://github.com/Xiaokang2022/tkintertools/pulse)
 
 </div>
 
 Install/模块安装👇
 -----------------
 
 ### Stable Version/稳定版本
 
-* Version/最新版本 : `2.6.5`
-* Release/发布日期 : 2023/06/17 (UTC+08)
+* Version/最新版本 : `2.6.6`
+* Release/发布日期 : 2023/07/01 (UTC+08)
 
 这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。  
 稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.5
+pip install tkintertools==2.6.6
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.6.dev`
-* Release/发布日期 : 2023/06/29 (UTC+08)
+* Version/最新版本 : `2.6.7.dev0`
+* Release/发布日期 : 2023/07/03 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
 开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
 大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.6.dev
+pip install tkintertools==2.6.7.dev0
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
 
-目前稳定版在以下操作系统中已经测试通过:
+目前 **稳定版** 在以下操作系统中已经测试通过:
 
 ![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows)
 ![Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11)
 ![Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
 
 可能还有其他的操作系统也是可以运行 tkintertools 的，我没有进行更多的验证。  
 没有任何额外的依赖包（除了一般 Python 内置的 tkinter），但只支持以下 Python 版本:
@@ -92,66 +92,97 @@
 ![Python3.10.*](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
 ![Python3.11.*](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
-**最新版本: tkintertools-2.6.6.dev 开发版**
+### Release Notes/版本说明
+
+**最新版本: `tkintertools-v2.6.7.dev0`**
 
 > **Note**  
-> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！
+> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！  
+> tkintertools 的介绍和使用教程均在 Wiki 中，[点我传送](https://github.com/Xiaokang2022/tkintertools/wiki)
 
 下面是本次版本更新内容条目：
 
-- [X] 新增抽象类 `_3D_Object` 来作为类 `_Point`、`_Line` 和 `_Side` 的元基类；
-- [X] 优化了 3D 子模块中的参数传递，使用者不需要时刻保证 `list` 的传递性，且原来只能使用 `list` 类型的参数现在为 `Iterable` 类型；
-- [X] 3D 子模块中 3D 对象居中方式改变，相比原来性能提升了不少，代码量也减少了；
-- [X] 改正了部分错误的类型提示，完善了部分缺少的方法注释；
-- [X] 3D 子模块中原来用函数 `hypot` 计算两点间距离，现在直接用函数 `dist` 计算两点间欧几里得距离，提高性能；
-- [X] 3D 子模块中优化了类 `Point` 的控件位置显示，让其始终保持在最前；
-- [X] 3D 子模块的类 `Point` 及其父类 `_Point` 的参数 `point1` 和 `point2` 分别被重命名为 `point_start` 和 `point_end`；
-- [X] 3D 子模块的类 `Space` 的参数 `origin_color` 被更改为四个新的参数，分别是 `origin_size`、`origin_width`、`origin_fill` 和 `origin_outline`；
-- [X] 3D 子模块的类 `Canvas_3D` 和 `Space` 移除参数 `dx` 和 `dy`，画布默认视野保持居中，也就是说，现在它们的中心位置才是原来的左上角顶点；
+- [X] 新增常量 `ROTATE_CENTER`、`ORIGIN_COORDINATE`、`ORIGIN_SIZE`、`ORIGIN_WIDTH`、`ORIGIN_FILL` 和 `ORIGIN_OUTLINE`；
+- [X] 类 `Tk` 和 `Toplevel` 新增关键字参数 `alpha`、`toolwindow`、`topmost` 和 `transparentcolor`；
+- [X] 修复了类 `Text` 在使用鼠标滚轮滚动时会报错的 bug；
+- [X] 优化函数 `translate`、`rotate` 和 `scale` 内部的实现，提高了性能；
+- [X] 修改和完善了大量的不完整的文档注释；
+- [X] 将部分类的部分方法更改为保护方法；
+
+### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 滚动鼠标中键可以放大和缩小画面；
+* 这多个几何体会自动地旋转以及上下浮动；
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
-![news](news.png)
+![news](news.gif)
 
 <details><summary><b>点击查看源代码</b></summary>
 
 ```python
 import math  # 数学支持
 
 import tkintertools as tkt  # 引入基础模块
 from tkintertools import tools_3d as t3d  # 引入 3d 子模块
 
 root = tkt.Tk('3D', 1280, 720)  # 创建窗口
 space = t3d.Space(root, 1280, 720, 0, 0)  # 创建空间
-last_point = [0, 100*math.cos(-math.pi/3), 100*math.sin(-math.pi/3)]
-color_lst = ['red', 'orange', 'yellow', 'green', 'blue', 'purple']
-color_lst += color_lst
-
-for i in range(6):
-    rad = i*math.pi/3
-    next_point = [0, 100*math.cos(rad), 100*math.sin(rad)]
-    point_h2 = [0, 150*math.cos(rad), 150*math.sin(rad)]
-    t3d.Line(space, last_point, next_point, width=3, fill=color_lst[i])
-    t3d.Line(space, next_point, point_h2, width=3, fill=color_lst[i+1])
-    t3d.Point(space, last_point, size=20, fill=color_lst[i+2])
-    t3d.Point(space, point_h2, size=10, fill=color_lst[i+3])
-    last_point = next_point
 
-space.space_sort()  # 给它们的空间位置排序以正确显示
+for a in -100, 0, 100:
+    for b in -100, 0, 100:
+        for c in -100, 0, 100:
+            t3d.Cuboid(space, a-50, b-50, c-50, 100, 100, 100,  # 创建正方体
+                       color_up='white', color_down='yellow', color_left='red',
+                       color_right='orange', color_front='blue', color_back='green')
+
+
+def spin():
+    """ 自动旋转 """
+    for geo in space.geos():
+        geo.rotate(dz=0.01)
+
+
+def floating(value):
+    """ 上下浮动 """
+    for geo in space.geos():
+        geo.translate(dz=math.sin(value))
+
+
+def animation(value=0):
+    """ 形成动画 """
+    spin()
+    floating(value)
+    space.space_sort()  # 给它们的空间位置排序以正确显示
+    for geo in space.geos():
+        geo.update()
+    space.after(10, animation, value+math.pi/60)
+
+
+def scale(event):
+    """ 缩放事件 """
+    k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1  # 缩放比率
+    for geo in space.geos():  # 遍历所有的几何体（不包括基本 3D 对象）
+        geo.scale(k, k, k)  # 缩放
+        geo.update()  # 更新改对象的实际画面
+    space.space_sort()  # 空间前后位置排序
+
+
+animation()
+root.bind('<Key-equal>', scale)  # 绑定等号按键
+root.bind('<Key-minus>', scale)  # 绑定减号按键
 root.mainloop()  # 消息事件循环
 ```
 
 </details>
 
 More/更多👇
 -----------
```

