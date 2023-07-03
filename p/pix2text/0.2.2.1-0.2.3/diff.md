# Comparing `tmp/pix2text-0.2.2.1.tar.gz` & `tmp/pix2text-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pix2text-0.2.2.1.tar", last modified: Sun Feb 19 12:08:05 2023, max compression
+gzip compressed data, was "pix2text-0.2.3.tar", last modified: Mon Jul  3 10:12:44 2023, max compression
```

## Comparing `pix2text-0.2.2.1.tar` & `pix2text-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,42 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 12:08:05.079082 pix2text-0.2.2.1/
--rw-r--r--   0 king       (501) staff       (20)    24597 2023-02-19 12:08:05.078524 pix2text-0.2.2.1/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    19309 2023-02-19 07:35:57.000000 pix2text-0.2.2.1/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 12:08:05.061148 pix2text-0.2.2.1/pix2text/
--rw-r--r--   0 king       (501) staff       (20)      190 2022-09-09 10:39:02.000000 pix2text-0.2.2.1/pix2text/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      108 2023-02-19 11:57:05.000000 pix2text-0.2.2.1/pix2text/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-0.2.2.1/pix2text/app.py
--rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-0.2.2.1/pix2text/category_mapping.py
--rw-r--r--   0 king       (501) staff       (20)     4150 2023-02-19 07:12:47.000000 pix2text-0.2.2.1/pix2text/cli.py
--rw-r--r--   0 king       (501) staff       (20)      800 2022-09-09 09:47:09.000000 pix2text-0.2.2.1/pix2text/consts.py
--rw-r--r--   0 king       (501) staff       (20)      862 2022-07-13 13:10:07.000000 pix2text-0.2.2.1/pix2text/latex_config.yaml
--rw-r--r--   0 king       (501) staff       (20)    12392 2023-02-19 12:06:20.000000 pix2text-0.2.2.1/pix2text/latex_ocr.py
--rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-0.2.2.1/pix2text/object_detector.py
--rw-r--r--   0 king       (501) staff       (20)    19919 2023-02-19 10:53:03.000000 pix2text-0.2.2.1/pix2text/pix_to_text.py
--rw-r--r--   0 king       (501) staff       (20)     5300 2023-02-03 11:26:24.000000 pix2text-0.2.2.1/pix2text/render.py
--rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-0.2.2.1/pix2text/screenshot_daemon_with_server2.py
--rw-r--r--   0 king       (501) staff       (20)     1943 2023-02-03 11:08:30.000000 pix2text-0.2.2.1/pix2text/serve.py
--rw-r--r--   0 king       (501) staff       (20)     9963 2023-02-19 10:32:43.000000 pix2text-0.2.2.1/pix2text/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 12:08:05.070778 pix2text-0.2.2.1/pix2text.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    24597 2023-02-19 12:08:04.000000 pix2text-0.2.2.1/pix2text.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)      690 2023-02-19 12:08:04.000000 pix2text-0.2.2.1/pix2text.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2023-02-19 12:08:04.000000 pix2text-0.2.2.1/pix2text.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       42 2023-02-19 12:08:04.000000 pix2text-0.2.2.1/pix2text.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-0.2.2.1/pix2text.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      175 2023-02-19 12:08:04.000000 pix2text-0.2.2.1/pix2text.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)       17 2023-02-19 12:08:04.000000 pix2text-0.2.2.1/pix2text.egg-info/top_level.txt
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 12:08:05.077020 pix2text-0.2.2.1/scripts/
--rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-0.2.2.1/scripts/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-0.2.2.1/scripts/object_detection3.py
--rw-r--r--   0 king       (501) staff       (20)     2393 2023-02-03 07:13:43.000000 pix2text-0.2.2.1/scripts/screenshot_daemon.py
--rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-0.2.2.1/scripts/try_layout.py
--rw-r--r--   0 king       (501) staff       (20)      554 2023-02-03 09:49:06.000000 pix2text-0.2.2.1/scripts/try_service.py
--rw-r--r--   0 king       (501) staff       (20)       38 2023-02-19 12:08:05.079290 pix2text-0.2.2.1/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     2120 2023-02-19 03:36:43.000000 pix2text-0.2.2.1/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-03 10:12:44.363506 pix2text-0.2.3/
+-rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-0.2.3/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    24094 2023-07-03 10:12:44.362534 pix2text-0.2.3/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    23013 2023-07-03 10:03:16.000000 pix2text-0.2.3/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-03 10:12:44.339966 pix2text-0.2.3/pix2text/
+-rw-r--r--   0 king       (501) staff       (20)      210 2023-07-03 02:18:23.000000 pix2text-0.2.3/pix2text/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      108 2023-06-30 06:16:40.000000 pix2text-0.2.3/pix2text/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-0.2.3/pix2text/app.py
+-rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-0.2.3/pix2text/category_mapping.py
+-rw-r--r--   0 king       (501) staff       (20)     4947 2023-07-03 06:25:56.000000 pix2text-0.2.3/pix2text/cli.py
+-rw-r--r--   0 king       (501) staff       (20)      929 2023-07-01 16:05:56.000000 pix2text-0.2.3/pix2text/consts.py
+-rw-r--r--   0 king       (501) staff       (20)      862 2022-07-13 13:10:07.000000 pix2text-0.2.3/pix2text/latex_config.yaml
+-rw-r--r--   0 king       (501) staff       (20)    12842 2023-07-03 09:34:16.000000 pix2text-0.2.3/pix2text/latex_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-0.2.3/pix2text/object_detector.py
+-rw-r--r--   0 king       (501) staff       (20)    20490 2023-07-03 09:30:59.000000 pix2text-0.2.3/pix2text/pix_to_text.py
+-rw-r--r--   0 king       (501) staff       (20)     5300 2023-02-03 11:26:24.000000 pix2text-0.2.3/pix2text/render.py
+-rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-0.2.3/pix2text/screenshot_daemon_with_server2.py
+-rw-r--r--   0 king       (501) staff       (20)     2026 2023-07-02 13:12:54.000000 pix2text-0.2.3/pix2text/serve.py
+-rw-r--r--   0 king       (501) staff       (20)    14209 2023-07-03 03:07:25.000000 pix2text-0.2.3/pix2text/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-03 10:12:44.345337 pix2text-0.2.3/pix2text.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    24094 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)      904 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       41 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-0.2.3/pix2text.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      172 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)       17 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/top_level.txt
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-03 10:12:44.358879 pix2text-0.2.3/scripts/
+-rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-0.2.3/scripts/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-0.2.3/scripts/convert_label_studio_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-0.2.3/scripts/gen_label_studio_json.py
+-rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-0.2.3/scripts/gen_pure_formula_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-0.2.3/scripts/merge_label_studio_anno_pred_json.py
+-rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-0.2.3/scripts/object_detection3.py
+-rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-0.2.3/scripts/screenshot_daemon.py
+-rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-0.2.3/scripts/try_layout.py
+-rw-r--r--   0 king       (501) staff       (20)      554 2023-02-03 09:49:06.000000 pix2text-0.2.3/scripts/try_service.py
+-rw-r--r--   0 king       (501) staff       (20)       38 2023-07-03 10:12:44.363697 pix2text-0.2.3/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     2185 2023-07-02 12:56:12.000000 pix2text-0.2.3/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-03 10:12:44.361000 pix2text-0.2.3/tests/
+-rw-r--r--   0 king       (501) staff       (20)     1372 2023-02-14 10:16:51.000000 pix2text-0.2.3/tests/test_pix2text.py
+-rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-0.2.3/tests/test_sort_boxes.py
```

### Comparing `pix2text-0.2.2.1/PKG-INFO` & `pix2text-0.2.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,570 +1,618 @@
-Metadata-Version: 2.1
-Name: pix2text
-Version: 0.2.2.1
-Summary: Python3 package to extract text information from images
-Home-page: https://github.com/breezedeus/pix2text
-Author: breezedeus
-Author-email: breezedeus@163.com
-License: MIT
-Description: <div align="center">
-          <img src="./docs/figs/p2t.jpg" width="250px"/>
-          <div>&nbsp;</div>
-        
-        [![Downloads](https://static.pepy.tech/personalized-badge/pix2text?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pix2text)
-        [![license](https://img.shields.io/github/license/breezedeus/pix2text)](./LICENSE)
-        [![PyPI version](https://badge.fury.io/py/pix2text.svg)](https://badge.fury.io/py/pix2text)
-        [![forks](https://img.shields.io/github/forks/breezedeus/pix2text)](https://github.com/breezedeus/pix2text)
-        [![stars](https://img.shields.io/github/stars/breezedeus/pix2text)](https://github.com/breezedeus/pix2text)
-        ![last-release](https://img.shields.io/github/release-date/breezedeus/pix2text)
-        ![last-commit](https://img.shields.io/github/last-commit/breezedeus/pix2text)
-        [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
-        
-        [👩🏻‍💻网页版](https://p2t.behye.com) |
-        [💬 交流群](https://cnocr.readthedocs.io/zh/latest/contact/)
-        
-        </div>
-        
-        <div align="center">
-        
-        [English](./README_en.md) | 中文
-        </div>
-        
-        # Pix2Text (P2T)
-        
-        
-        【Update 2023.02.10： **[P2T网页版](https://p2t.behye.com)** 开放免费使用】
-        
-        * P2T作为Python包，对于不熟悉Python的朋友还是太不友好，所以我们也开发了 [P2T网页版](https://p2t.behye.com)，可直接免费使用，欢迎帮忙推荐分享。
-        * 视频介绍：[Pix2Text 新版和网页版发布，离Mathpix又近了一大步_bilibili](https://www.bilibili.com/video/BV1U24y1q7n3) 。
-        * 文字版介绍：[Pix2Text (P2T) 新版发布，离Mathpix又近了一大步 - 知乎](https://zhuanlan.zhihu.com/p/604999678) 。
-        
-        【Update 2023.02.03：**V0.2** 发布】
-        
-        * 利用 **[CnSTD](https://github.com/breezedeus/cnstd)** 新版的**数学公式检测**（**Mathematical Formula Detection**，简称 **MFD**）能力，**P2T V0.2** 支持**识别既包含文字又包含公式的混合图片**。
-        
-        了解更多：[RELEASE.md](./RELEASE.md) 。
-        
-        ---
-        
-        
-        
-        **Pix2Text** 期望成为 **[Mathpix](https://mathpix.com/)** 的**免费开源 Python **替代工具，目前已经可以完成 **Mathpix** 的核心功能。**Pix2Text (P2T)** 自 **V0.2** 开始，支持识别**既包含文字又包含公式的混合图片**，返回效果类似于 **Mathpix**。P2T 的核心原理见下图（文字识别支持**中文**和**英文**）：
-        
-        <div align="center">
-          <img src="./docs/figs/arch-flow2.jpg" alt="Pix2Text流程" width="600px"/>
-        </div>
-        
-        
-        
-        **P2T** 使用开源工具  **[CnSTD](https://github.com/breezedeus/cnstd)** 检测出图片中**数学公式**所在位置，再交由 **[LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)** 识别出各对应位置数学公式的Latex表示。图片的剩余部分再交由 **[CnOCR](https://github.com/breezedeus/cnocr)** 进行文字检测和文字识别。最后 P2T 合并所有识别结果，获得最终的图片识别结果。感谢这些开源工具。
-        
-        
-        
-        P2T 作为Python3工具包，对于不熟悉Python的朋友不太友好，我们近期也会发布 **P2T网页版**，直接把图片丢进网页就能输出P2T的解析结果。
-        
-        网页版会提供一些**免费名额**供有需要的朋友使用，优先在校学生（**[MathPix](https://link.zhihu.com/?target=https%3A//mathpix.com/)** 每月要5美元，对在校生来说还是蛮贵的）。
-        
-        
-        
-        感兴趣的朋友欢迎扫码加小助手为好友，备注 `p2t`，小助手会定期统一邀请大家入群。群内会发布P2T相关工具的最新进展：
-        
-        <div align="center">
-          <img src="./docs/figs/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
-        </div>
-        
-        
-        
-        作者也维护 **知识星球** [**P2T/CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) ，这里面的提问会较快得到作者的回复，欢迎加入。**知识星球私享群**也会陆续发布一些P2T/CnOCR/CnSTD相关的私有资料，包括[**更详细的训练教程**](https://articles.zsxq.com/id_u6b4u0wrf46e.html)，**未公开的模型**，**不同应用场景的调用代码**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。
-        
-        
-        
-        ## 使用说明
-        
-        
-        调用很简单，以下是示例：
-        
-        ```python
-        from pix2text import Pix2Text
-        
-        img_fp = './docs/examples/formula.jpg'
-        p2t = Pix2Text(analyzer_config=dict(model_name='mfd'))
-        outs = p2t(img_fp, resized_shape=600)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
-        print(outs)
-        # 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
-        only_text = '\n'.join([out['text'] for out in outs])
-        ```
-        
-        
-        
-        返回结果 `out_text` 是个 `dict`，其中 key `position` 表示位置信息，`type` 表示类别信息，而 `text` 表示识别的结果。具体见下面的[接口说明](#接口说明)。
-        
-        
-        
-        ## 示例
-        
-        <table>
-        <tr>
-        <th> 图片 </th> 
-        <th> Pix2Text识别结果 </th>
-        </tr>
-        <tr>
-        <td>
-        <img src="./docs/examples/mixed.jpg" alt="mixed"> 
-        
-        </td>
-        <td>
-        
-        ```python
-        [{"position": array([[         22,          29],
-               [       1055,          29],
-               [       1055,          56],
-               [         22,          56]], dtype=float32),
-          "text": "JVAE的训练loss和VQ-VAE类似，只是使用了KL距离来让分布尽量分散",
-          "type": "text"},
-         {"position": array([[        629,         124],
-               [       1389,         124],
-               [       1389,         183],
-               [        629,         183]]),
-          "text": "$$\n"
-                  "-{\\cal E}_{z\\sim q(z|x)}[\\log(p(x\\mid z))]"
-                  "+{\\cal K}{\\cal L}(q(z\\mid x)||p(z))\n"
-                  "$$",
-          "type": "isolated"},
-         {"position": array([[         20,         248],
-               [       1297,         248],
-               [       1297,         275],
-               [         20,         275]], dtype=float32),
-          "text": "其中之利用 Gumbel-Softmax从 $z\\sim q(z|x)$ 中抽样得到，"
-          " $p(z)$ 是个等概率的多项式分布。",
-          "type": "text-embed"}]
-        ```
-        
-        </td>
-        </tr>
-        <tr>
-        <td>
-        
-        <img src="./docs/examples/formula.jpg" alt="formula"> 
-        </td>
-        <td>
-        
-        ```python
-        [{"position": array([[         12,          19],
-               [        749,          19],
-               [        749,         150],
-               [         12,         150]]),
-          "text": "$$\n"
-                  "\\mathcal{L}_{\\mathrm{eyelid}}~\\equiv~"
-                  "\\sum_{t=1}^{T}\\sum_{v=1}^{V}"
-                  "\\mathcal{N}_{U}^{\\mathrm{(eyelid)}}"
-                  "\\left(\\left|\\left|\\hat{h}_{t,v}\\,-\\,"
-                  "\\mathcal{x}_{t,v}\\right|\\right|^{2}\\right)\n"
-                  "$$",
-          "type": "isolated"}]
-        ```
-        </div>
-        </td>
-        </tr>
-        <tr>
-        <td>
-        
-         <img src="./docs/examples/english.jpg" alt="english"> 
-        </td>
-        <td>
-        
-        ```python
-        [{"position": array([[          0,           0],
-               [        710,           0],
-               [        710,         116],
-               [          0,         116]]),
-          "text": "python scripts/screenshot_daemon_with_server\n"
-                  "2-get_model:178usemodel:/Users/king/.cr\n"
-                  "enet_lite_136-fc-epoch=039-complete_match_er",
-          "type": "english"}]
-        ```
-        </td>
-        </tr>
-        <tr>
-        <td>
-        
-         <img src="./docs/examples/general.jpg" alt="general"  width="300px"> 
-        </td>
-        <td>
-        
-        ```python
-        [{"position": array([[          0,           0],
-               [        800,           0],
-               [        800,         800],
-               [          0,         800]]),
-          "text": "618\n开门红提前购\n很贵\n买贵返差"
-          "\n终于降价了\n100%桑蚕丝\n要买趁早\n今日下单188元\n仅限一天",
-          "type": "general"}]
-        ```
-        </td>
-        </tr>
-        </table>
-        
-        
-        
-        ## 模型下载
-        
-        安装好 Pix2Text 后，首次使用时系统会**自动下载** 模型文件，并存于 `~/.pix2text`目录（Windows下默认路径为 `C:\Users\<username>\AppData\Roaming\pix2text`）。
-        
-        
-        
-        > **Note**
-        >
-        > 如果已成功运行上面的示例，说明模型已完成自动下载，可忽略本节后续内容。
-        
-        
-        
-        对于**分类模型**，系统会自动下载模型`mobilenet_v2.zip`文件并对其解压，然后把解压后的模型相关目录放于`~/.pix2text`目录中。如果系统无法自动成功下载`mobilenet_v2.zip`文件，则需要手动从 **[cnstd-cnocr-models/pix2text](https://huggingface.co/breezedeus/cnstd-cnocr-models/tree/main/models/pix2text/0.2)** 下载此zip文件并把它放于 `~/.pix2text`目录。如果下载太慢，也可以从 [百度云盘](https://pan.baidu.com/s/1kubZF4JGE19d98NDoPHJzQ?pwd=p2t0) 下载， 提取码为 ` p2t0`。
-        
-        对于  **[LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)** ，系统同样会自动下载模型文件并把它们存放于`~/.pix2text/formula`目录中。如果系统无法自动成功下载这些模型文件，则需从  [百度云盘](https://pan.baidu.com/s/1kubZF4JGE19d98NDoPHJzQ?pwd=p2t0) 下载文件 `weights.pth` 和 `image_resizer.pth`， 并把它们存放于`~/.pix2text/formula`目录中；提取码为 ` p2t0`。
-        
-        
-        
-        ## 安装
-        
-        嗯，顺利的话一行命令即可。
-        
-        ```bash
-        pip install pix2text
-        ```
-        
-        安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
-        
-        ```bash
-        pip install pix2text -i https://pypi.doubanio.com/simple
-        ```
-        
-        
-        
-        如果是初次使用**OpenCV**，那估计安装都不会很顺利，bless。
-        
-        **Pix2Text** 主要依赖 [**CnSTD>=1.2.1**](https://github.com/breezedeus/cnstd)、[**CnOCR>=2.2.2.1**](https://github.com/breezedeus/cnocr) ，以及 [**LaTeX-OCR**](https://github.com/lukas-blecher/LaTeX-OCR) 。如果安装过程遇到问题，也可参考它们的安装说明文档。
-        
-        
-        
-        > **Warning** 
-        >
-        > 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到不少问题，但一般都是常见问题，可以自行百度/Google解决。
-        
-        
-        
-        ## 接口说明
-        
-        ### 类初始化
-        
-        主类为 [**Pix2Text**](pix2text/pix_to_text.py) ，其初始化函数如下：
-        
-        ```python
-        class Pix2Text(object):
-        
-            def __init__(
-                self,
-                *,
-                analyzer_config: Dict[str, Any] = None,
-                clf_config: Dict[str, Any] = None,
-                general_config: Dict[str, Any] = None,
-                english_config: Dict[str, Any] = None,
-                formula_config: Dict[str, Any] = None,
-                thresholds: Dict[str, Any] = None,
-                device: str = 'cpu',  # ['cpu', 'cuda', 'gpu']
-                **kwargs,
-            ):
-        ```
-        
-        其中的各参数说明如下：
-        * `analyzer_config` (dict): 分类模型对应的配置信息；默认为 `None`，表示使用默认配置（使用**MFD** Analyzer）：
-        	
-          ```python
-          {
-                'model_name': 'mfd'  # 可以取值为 'mfd'（MFD），或者 'layout'（版面分析）
-        	}
-        	```
-        	
-        * `clf_config` (dict): 分类模型对应的配置信息；默认为 `None`，表示使用默认配置：
-        	```python
-          {
-                'base_model_name': 'mobilenet_v2',
-                'categories': IMAGE_TYPES,
-                'transform_configs': {
-                    'crop_size': [150, 450],
-                    'resize_size': 160,
-                    'resize_max_size': 1000,
-                },
-                'model_dir': Path(data_dir()) / 'clf',
-                'model_fp': None  # 如果指定，直接使用此模型文件
-          }
-        	```
-        	
-        * `general_config` (dict): 通用模型对应的配置信息；默认为 `None`，表示使用默认配置：
-        
-          ```python
-          {}
-          ```
-        
-        * `english_config` (dict): 英文模型对应的配置信息；默认为 `None`，表示使用默认配置：
-        
-          ```py
-          {'det_model_name': 'en_PP-OCRv3_det', 'rec_model_name': 'en_PP-OCRv3'}
-          ```
-        
-        * `formula_config` (dict): 公式识别模型对应的配置信息；默认为 `None`，表示使用默认配置：
-        
-          ```python
-          {
-              'config': LATEX_CONFIG_FP,
-              'checkpoint': Path(data_dir()) / 'formular' / 'weights.pth',
-              'no_resize': False
-          }
-          ```
-        
-        * `thresholds` (dict): 识别阈值对应的配置信息；默认为 `None`，表示使用默认配置：
-        
-          ```py
-          {
-              'formula2general': 0.65,  # 如果识别为 `formula` 类型，但得分小于此阈值，则改为 `general` 类型
-              'english2general': 0.75,  # 如果识别为 `english` 类型，但得分小于此阈值，则改为 `general` 类型
-          }
-          ```
-        
-        * `device` (str): 使用什么资源进行计算，支持 `['cpu', 'cuda', 'gpu']`；默认为 `cpu`
-        
-        * `**kwargs` (): 预留的其他参数；目前未被使用
-        
-        
-        
-        ### 识别类函数
-        
-        通过调用类 **`Pix2Text`** 的类函数 `.recognize()` 完成对指定图片进行识别。类函数 `.recognize()` 说明如下：
-        
-        ```python
-            def recognize(
-                self, img: Union[str, Path, Image.Image], use_analyzer: bool = True, **kwargs
-            ) -> List[Dict[str, Any]]:
-        ```
-        
-        
-        
-        其中的输入参数说明如下：
-        
-        * `img` (`str` or `Image.Image`)：待识别图片的路径，或者利用 `Image.open()` 已读入的图片 `Image` 。
-        * `use_analyzer` (`bool`)：是否使用 Analyzer (**MFD** or **Layout**); `False` 表示把图片看成纯文本或者纯图片处理，相当于 **P2T V0.1.*** 的效果。Default: `True`。
-        * `kwargs`: 保留字段，可以包含以下值，
-          * `resized_shape` (`int`): 把图片宽度resize到此大小再进行处理；默认值为 `700`；
-          * `save_analysis_res` (`str`): 把解析结果图片存在此文件中；默认值为 `None`，表示不存储；
-          * `embed_sep` (`tuple`): embedding latex的前后缀；只针对使用 `MFD` 时才有效；默认值为 `(' $', '$ ')`；
-          * `isolated_sep` (`tuple`): isolated latex的前后缀；只针对使用 `MFD` 时才有效；默认值为 `('$$\n', '\n$$')`。
-        
-        
-        
-        返回结果为列表（`list`），列表中的每个元素为`dict`，包含如下 `key`：
-        
-        * `type`：识别出的图像类别；
-          * 当开启Analyzer时（`use_analyzer==True`），取值为 `text`（纯文本）、`isolated`（独立行的数学公式） 或者 `text-embed`（文本行中包含了嵌入式的数学公式）；
-          * 当未开启Analyzer时（`use_analyzer==False`），取值为`formula`（纯数学公式）、`english`（纯英文文字）、`general`（纯文字，可能包含中英文）；
-        
-        * `text`：识别出的文字或Latex表达式；
-        * `position`：所在块的位置信息，`np.ndarray`, with shape of `[4, 2]`。
-        
-        
-        
-        `Pix2Text` 类也实现了 `__call__()` 函数，其功能与 `.recognize()` 函数完全相同。所以才会有以下的调用方式：
-        
-        ```python
-        from pix2text import Pix2Text
-        
-        img_fp = './docs/examples/formula.jpg'
-        p2t = Pix2Text(analyzer_config=dict(model_name='mfd'))
-        outs = p2t(img_fp, resized_shape=600)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
-        print(outs)
-        # 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
-        only_text = '\n'.join([out['text'] for out in outs])
-        ```
-        
-        
-        
-        ## 脚本使用
-        
-        **P2T** 包含了以下命令行工具。
-        
-        
-        
-        ### 对单张图片或单个文件夹中的图片进行识别
-        
-        使用命令 **`p2t predict`** 预测单个文件或文件夹中所有图片，以下是使用说明：
-        
-        ```bash
-        $ p2t predict -h
-        Usage: p2t predict [OPTIONS]
-        
-          模型预测
-        
-        Options:
-          --use-analyzer / --no-use-analyzer
-                                          是否使用 MFD 或者版面分析 Analyzer  [default: use-
-                                          analyzer]
-          -a, --analyzer-name [mfd|layout]
-                                          使用哪个Analyzer，MFD还是版面分析  [default: mfd]
-          -t, --analyzer-type TEXT        Analyzer使用哪个模型，'yolov7_tiny' or 'yolov7'
-                                          [default: yolov7_tiny]
-          -d, --device TEXT               使用 `cpu` 还是 `gpu` 运行代码，也可指定为特定gpu，如`cuda:0`
-                                          [default: cpu]
-          --resized-shape INTEGER         把图片宽度resize到此大小再进行处理  [default: 600]
-          -i, --img-file-or-dir TEXT      输入图片的文件路径或者指定的文件夹  [required]
-          --save-analysis-res TEXT        把解析结果存储到此文件或目录中（如果'--img-file-or-
-                                          dir'为文件/文件夹，则'--save-analysis-
-                                          res'也应该是文件/文件夹）。取值为 `None` 表示不存储
-          -l, --log-level TEXT            Log Level, such as `INFO`, `DEBUG`
-                                          [default: INFO]
-          -h, --help                      Show this message and exit.
-        ```
-        
-        
-        
-        ## HTTP服务
-        
-         **Pix2Text** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
-        
-        ```bash
-        $ pip install pix2text[serve]
-        ```
-        
-        
-        
-        安装完成后，可以通过以下命令启动HTTP服务（**`-p`** 后面的数字是**端口**，可以根据需要自行调整）：
-        
-        ```bash
-        $ p2t serve -p 8503
-        ```
-        
-        
-        
-        `p2t serve` 命令使用说明：
-        
-        ```bash
-        $ p2t serve -h
-        Usage: p2t serve [OPTIONS]
-        
-          开启HTTP服务。
-        
-        Options:
-          -H, --host TEXT     server host  [default: 0.0.0.0]
-          -p, --port INTEGER  server port  [default: 8503]
-          --reload            whether to reload the server when the codes have been
-                              changed
-          -h, --help          Show this message and exit.
-        ```
-        
-        
-        
-        服务开启后，可以使用以下方式调用服务。
-        
-        
-        
-        ### 命令行
-        
-        比如待识别文件为 `docs/examples/mixed.jpg`，如下使用 `curl` 调用服务：
-        
-        ```bash
-        $ curl -F image=@docs/examples/mixed.jpg --form 'use_analyzer=true' --form 'resized_shape=600' http://0.0.0.0:8503/pix2text
-        ```
-        
-        
-        
-        ### Python
-        
-        使用如下方式调用服务，参考文件 [scripts/try_service.py](scripts/try_service.py)：
-        
-        ```python
-        import requests
-        
-        url = 'http://0.0.0.0:8503/pix2text'
-        
-        image_fp = 'docs/examples/mixed.jpg'
-        data = {
-            "use_analyzer": True,
-            "resized_shape": 600,
-            "embed_sep": " $,$ ",
-            "isolated_sep": "$$\n, \n$$"
-        }
-        files = {
-            "image": (image_fp, open(image_fp, 'rb'))
-        }
-        
-        r = requests.post(url, data=data, files=files)
-        
-        outs = r.json()['results']
-        only_text = '\n'.join([out['text'] for out in outs])
-        print(f'{only_text=}')
-        ```
-        
-        
-        
-        ### 其他语言
-        
-        请参照 `curl` 的调用方式自行实现。
-        
-        
-        
-        ## 脚本运行
-        
-        脚本 [scripts/screenshot_daemon.py](scripts/screenshot_daemon.py) 实现了自动对截屏图片调用 Pixe2Text 进行公式或者文字识别。这个功能是如何实现的呢？
-        
-        
-        
-        **以下是具体的运行流程（请先安装好 Pix2Text）：**
-        
-        1. 找一个喜欢的截屏软件，这个软件只要**支持把截屏图片存储在指定文件夹**即可。比如Mac下免费的 **Xnip** 就很好用。
-        
-        2. 除了安装Pix2Text外，还需要额外安装一个Python包 **pyperclip**，利用它把识别结果复制进系统的剪切板：
-        
-           ```bash
-           $ pip install pyperclip
-           ```
-        
-        3. 下载脚本文件 [scripts/screenshot_daemon.py](scripts/screenshot_daemon.py) 到本地，编辑此文件 `"SCREENSHOT_DIR"` 所在行（第 `17` 行），把路径改为你的截屏图片所存储的目录。
-        
-        4. 运行此脚本：
-        
-           ```bash
-           $ python scripts/screenshot_daemon.py
-           ```
-        
-        好了，现在就用你的截屏软件试试效果吧。截屏后的识别结果会写入电脑剪切板，直接 **Ctrl-V** / **Cmd-V** 即可粘贴使用。
-        
-        
-        
-        更详细使用介绍可参考视频：《[Pix2Text: 替代 Mathpix 的免费 Python 开源工具](https://www.bilibili.com/video/BV12e4y1871U)》。
-        
-        
-        
-        
-        ## 给作者来杯咖啡
-        
-        开源不易，如果此项目对您有帮助，可以考虑 [给作者加点油🥤，鼓鼓气💪🏻](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
-        
-        ---
-        
-        官方代码库：[https://github.com/breezedeus/pix2text](https://github.com/breezedeus/pix2text)。
-        
-        
-Platform: Mac
-Platform: Linux
-Platform: Windows
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-Provides-Extra: serve
-Provides-Extra: dev
+<div align="center">
+  <img src="./docs/figs/p2t.jpg" width="250px"/>
+  <div>&nbsp;</div>
+
+[![Downloads](https://static.pepy.tech/personalized-badge/pix2text?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pix2text)
+[![license](https://img.shields.io/github/license/breezedeus/pix2text)](./LICENSE)
+[![PyPI version](https://badge.fury.io/py/pix2text.svg)](https://badge.fury.io/py/pix2text)
+[![forks](https://img.shields.io/github/forks/breezedeus/pix2text)](https://github.com/breezedeus/pix2text)
+[![stars](https://img.shields.io/github/stars/breezedeus/pix2text)](https://github.com/breezedeus/pix2text)
+![last-release](https://img.shields.io/github/release-date/breezedeus/pix2text)
+![last-commit](https://img.shields.io/github/last-commit/breezedeus/pix2text)
+[![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
+
+[👩🏻‍💻网页版](https://p2t.behye.com) |
+[💬 交流群](https://cnocr.readthedocs.io/zh/latest/contact/)
+
+</div>
+
+<div align="center">
+
+[English](./README_en.md) | 中文
+</div>
+
+# Pix2Text (P2T)
+## Update 2023.07.03：发布 V0.2.3
+
+主要变更：
+* 训练了新的**公式识别模型**，供 **[P2T网页版](https://p2t.behye.com)** 使用。新模型精度更高，尤其对**手写公式**和**多行公式**类图片。具体参考：[Pix2Text 新版公式识别模型 | Breezedeus.com](https://www.breezedeus.com/article/p2t-mfd-20230702) 。
+* 优化了对检测出的boxes的排序逻辑，以及对混合图片的处理逻辑，使得最终识别效果更符合直觉。
+* 优化了识别结果的合并逻辑，自动判断是否该换行，是否分段。
+* 修复了模型文件自动下载的功能。HuggingFace似乎对下载文件的逻辑做了调整，导致之前版本的自动下载失败，当前版本已修复。但由于HuggingFace国内被墙，国内下载仍需 **梯子（VPN）**。
+* 更新了各个依赖包的版本号。
+
+## Update 2023.06.20：发布新版 MFD 模型
+
+主要变更：
+* 基于新标注的数据，重新训练了 **MFD YoloV7** 模型，目前新模型已部署到 [P2T网页版](https://p2t.behye.com) 。具体说明见：[Pix2Text (P2T) 新版公式检测模型 | Breezedeus.com](https://www.breezedeus.com/article/p2t-mfd-20230613) 。
+* 之前的 MFD YoloV7 模型已开放给星球会员下载，具体说明见：[P2T YoloV7 数学公式检测模型开放给星球会员下载 | Breezedeus.com](https://www.breezedeus.com/article/p2t-yolov7-for-zsxq-20230619) 。
+
+## Update 2023.02.10： **[P2T网页版](https://p2t.behye.com)** 开放免费使用
+
+* P2T作为Python包，对于不熟悉Python的朋友还是太不友好，所以我们也开发了 [P2T网页版](https://p2t.behye.com)，可直接免费使用，欢迎帮忙推荐分享。
+* 视频介绍：[Pix2Text 新版和网页版发布，离Mathpix又近了一大步_bilibili](https://www.bilibili.com/video/BV1U24y1q7n3) 。
+* 文字版介绍：[Pix2Text (P2T) 新版发布，离Mathpix又近了一大步 - 知乎](https://zhuanlan.zhihu.com/p/604999678) 。
+
+
+了解更多：[RELEASE.md](./RELEASE.md) 。
+
+---
+
+
+
+**Pix2Text** 期望成为 **[Mathpix](https://mathpix.com/)** 的**免费开源 Python **替代工具，目前已经可以完成 **Mathpix** 的核心功能。**Pix2Text (P2T)** 自 **V0.2** 开始，支持识别**既包含文字又包含公式的混合图片**，返回效果类似于 **Mathpix**。P2T 的核心原理见下图（文字识别支持**中文**和**英文**）：
+
+<div align="center">
+  <img src="./docs/figs/arch-flow2.jpg" alt="Pix2Text流程" width="600px"/>
+</div>
+
+
+
+**P2T** 使用开源工具  **[CnSTD](https://github.com/breezedeus/cnstd)** 检测出图片中**数学公式**所在位置，再交由 **[LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)** 识别出各对应位置数学公式的Latex表示。图片的剩余部分再交由 **[CnOCR](https://github.com/breezedeus/cnocr)** 进行文字检测和文字识别。最后 P2T 合并所有识别结果，获得最终的图片识别结果。感谢这些开源工具。
+
+
+
+P2T 作为Python3工具包，对于不熟悉Python的朋友不太友好，所以我们也发布了**可免费使用**的 **[P2T网页版](https://p2t.behye.com)**，直接把图片丢进网页就能输出P2T的解析结果。**网页版会使用最新的模型，效果会比开源模型更好。**
+
+
+
+感兴趣的朋友欢迎扫码加小助手为好友，备注 `p2t`，小助手会定期统一邀请大家入群。群内会发布P2T相关工具的最新进展：
+
+<div align="center">
+  <img src="./docs/figs/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
+</div>
+
+
+
+作者也维护 **知识星球** [**P2T/CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) ，这里面的提问会较快得到作者的回复，欢迎加入。**知识星球私享群**也会陆续发布一些P2T/CnOCR/CnSTD相关的私有资料，包括[**更详细的训练教程**](https://articles.zsxq.com/id_u6b4u0wrf46e.html)，**部分未公开的模型**，**购买付费模型享优惠**，**不同应用场景的调用代码**，使用过程中遇到的难题解答等。星球也会发布P2T/OCR/STD相关的最新研究资料。
+
+
+
+## 使用说明
+
+
+调用很简单，以下是示例：
+
+```python
+from pix2text import Pix2Text, merge_line_texts
+
+img_fp = './docs/examples/formula.jpg'
+p2t = Pix2Text(analyzer_config=dict(model_name='mfd'))
+outs = p2t(img_fp, resized_shape=600)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
+print(outs)
+# 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
+only_text = merge_line_texts(outs, auto_line_break=True)
+print(only_text)
+```
+
+
+
+返回结果 `outs` 是个 `dict`，其中 key `position` 表示Box位置信息，`type` 表示类别信息，而 `text` 表示识别的结果。具体见下面的[接口说明](#接口说明)。
+
+
+
+## 示例
+
+<table>
+<tr>
+<th> 图片 </th> 
+<th> Pix2Text识别结果 </th>
+</tr>
+<tr>
+<td>
+<img src="./docs/examples/mixed.jpg" alt="mixed"> 
+
+</td>
+<td>
+
+```python
+[{'line_number': 0,
+  'position': array([[         22,          31],
+       [       1057,          31],
+       [       1057,          58],
+       [         22,          58]]),
+  'text': 'JVAE的训练loss和VQ-VAE类似，只是使用了KL距离来让分布尽量分散',
+  'type': 'text'},
+ {'line_number': 1,
+  'position': array([[        625,         121],
+       [       1388,         121],
+       [       1388,         182],
+       [        625,         182]]),
+  'text': '$$\n'
+          '-E_{z\\sim q(z\\mid x)}[\\log(p(x\\mid z))]+K L(q(z\\mid x))|p(z))\n'
+          '$$',
+  'type': 'isolated'},
+ {'line_number': 2,
+  'position': array([[         18,         242],
+       [        470,         242],
+       [        470,         275],
+       [         18,         275]]),
+  'text': '其中之利用 Gumbel-Softmax 人',
+  'type': 'text'},
+ {'line_number': 2,
+  'position': array([[        481,         238],
+       [        664,         238],
+       [        664,         287],
+       [        481,         287]]),
+  'text': ' $z\\sim q(z|x)$ ',
+  'type': 'embedding'},
+ {'line_number': 2,
+  'position': array([[        667,         244],
+       [        840,         244],
+       [        840,         277],
+       [        667,         277]]),
+  'text': '中抽样得到,',
+  'type': 'text'},
+ {'line_number': 2,
+  'position': array([[        852,         239],
+       [        932,         239],
+       [        932,         288],
+       [        852,         288]]),
+  'text': ' $\\scriptstyle{p(z)}$ ',
+  'type': 'embedding'},
+ {'line_number': 2,
+  'position': array([[        937,         244],
+       [       1299,         244],
+       [       1299,         277],
+       [        937,         277]]),
+  'text': '是个等概率的多项式分布',
+  'type': 'text'}]
+```
+
+</td>
+</tr>
+<tr>
+<td>
+
+<img src="./docs/examples/formula.jpg" alt="formula"> 
+</td>
+<td>
+
+```python
+[{"line_number": 0,
+  "position": array([[         12,          19],
+       [        749,          19],
+       [        749,         150],
+       [         12,         150]]),
+  "text": "$$\n"
+          "\\mathcal{L}_{\\mathrm{eyelid}}~\\equiv~"
+          "\\sum_{t=1}^{T}\\sum_{v=1}^{V}"
+          "\\mathcal{N}_{U}^{\\mathrm{(eyelid)}}"
+          "\\left(\\left|\\left|\\hat{h}_{t,v}\\,-\\,"
+          "\\mathcal{x}_{t,v}\\right|\\right|^{2}\\right)\n"
+          "$$",
+  "type": "isolated"}]
+```
+</div>
+</td>
+</tr>
+<tr>
+<td>
+
+ <img src="./docs/examples/english.jpg" alt="english"> 
+</td>
+<td>
+
+```python
+[{"position": array([[          0,           0],
+       [        710,           0],
+       [        710,         116],
+       [          0,         116]]),
+  "text": "python scripts/screenshot_daemon_with_server\n"
+          "2-get_model:178usemodel:/Users/king/.cr\n"
+          "enet_lite_136-fc-epoch=039-complete_match_er",
+  "type": "english"}]
+```
+</td>
+</tr>
+<tr>
+<td>
+
+ <img src="./docs/examples/general.jpg" alt="general"  width="300px"> 
+</td>
+<td>
+
+```python
+[{"position": array([[          0,           0],
+       [        800,           0],
+       [        800,         800],
+       [          0,         800]]),
+  "text": "618\n开门红提前购\n很贵\n买贵返差"
+  "\n终于降价了\n100%桑蚕丝\n要买趁早\n今日下单188元\n仅限一天",
+  "type": "general"}]
+```
+</td>
+</tr>
+</table>
+
+
+
+## 模型下载
+
+### 开源免费模型
+
+安装好 Pix2Text 后，首次使用时系统会**自动下载** 免费模型文件，并存于 `~/.pix2text`目录（Windows下默认路径为 `C:\Users\<username>\AppData\Roaming\pix2text`）。
+
+
+
+> **Note**
+>
+> 如果已成功运行上面的示例，说明模型已完成自动下载，可忽略本节后续内容。
+
+
+
+对于**分类模型**，系统会自动下载模型`mobilenet_v2.zip`文件并对其解压，然后把解压后的模型相关目录放于`~/.pix2text`目录中。如果系统无法自动成功下载`mobilenet_v2.zip`文件，则需要手动从 **[cnstd-cnocr-models/pix2text](https://huggingface.co/breezedeus/cnstd-cnocr-models/tree/main/models/pix2text/0.2)** 下载此zip文件并把它放于 `~/.pix2text`目录。如果下载太慢，也可以从 [百度云盘](https://pan.baidu.com/s/1kubZF4JGE19d98NDoPHJzQ?pwd=p2t0) 下载， 提取码为 ` p2t0`。
+
+对于  **[LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)** ，系统同样会自动下载模型文件并把它们存放于`~/.pix2text/formula`目录中。如果系统无法自动成功下载这些模型文件，则需从  [百度云盘](https://pan.baidu.com/s/1kubZF4JGE19d98NDoPHJzQ?pwd=p2t0) 下载文件 `weights.pth` 和 `image_resizer.pth`， 并把它们存放于`~/.pix2text/formula`目录中；提取码为 ` p2t0`。
+
+
+
+### 付费模型
+
+除了上面免费的开源模型，P2T 也训练了精度更高的数学公式检测和识别模型，这些模型供 **[P2T网页版](https://p2t.behye.com)** 使用，它们的效果也可以在网页版体验。这些模型不是免费的（抱歉开源作者也是要喝咖啡的），具体可参考 [Pix2Text (P2T) | Breezedeus.com](https://www.breezedeus.com/pix2text#259b04346dd94f45a65c10ff3db48540) 。
+
+
+
+## 安装
+
+嗯，顺利的话一行命令即可。
+
+```bash
+pip install pix2text
+```
+
+安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
+
+```bash
+pip install pix2text -i https://pypi.doubanio.com/simple
+```
+
+
+
+如果是初次使用**OpenCV**，那估计安装都不会很顺利，bless。
+
+**Pix2Text** 主要依赖 [**CnSTD>=1.2.1**](https://github.com/breezedeus/cnstd)、[**CnOCR>=2.2.2.1**](https://github.com/breezedeus/cnocr) ，以及 [**LaTeX-OCR**](https://github.com/lukas-blecher/LaTeX-OCR) 。如果安装过程遇到问题，也可参考它们的安装说明文档。
+
+
+
+> **Warning** 
+>
+> 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到不少问题，但一般都是常见问题，可以自行百度/Google解决。
+
+
+
+## 接口说明
+
+### 类初始化
+
+主类为 [**Pix2Text**](pix2text/pix_to_text.py) ，其初始化函数如下：
+
+```python
+class Pix2Text(object):
+
+    def __init__(
+        self,
+        *,
+        analyzer_config: Dict[str, Any] = None,
+        clf_config: Dict[str, Any] = None,
+        general_config: Dict[str, Any] = None,
+        english_config: Dict[str, Any] = None,
+        formula_config: Dict[str, Any] = None,
+        thresholds: Dict[str, Any] = None,
+        device: str = 'cpu',  # ['cpu', 'cuda', 'gpu']
+        **kwargs,
+    ):
+```
+
+其中的各参数说明如下：
+* `analyzer_config` (dict): 分类模型对应的配置信息；默认为 `None`，表示使用默认配置（使用**MFD** Analyzer）：
+	
+  ```python
+  {
+        'model_name': 'mfd'  # 可以取值为 'mfd'（MFD），或者 'layout'（版面分析）
+	}
+	```
+	
+* `clf_config` (dict): 分类模型对应的配置信息；默认为 `None`，表示使用默认配置：
+	```python
+  {
+        'base_model_name': 'mobilenet_v2',
+        'categories': IMAGE_TYPES,
+        'transform_configs': {
+            'crop_size': [150, 450],
+            'resize_size': 160,
+            'resize_max_size': 1000,
+        },
+        'model_dir': Path(data_dir()) / 'clf',
+        'model_fp': None  # 如果指定，直接使用此模型文件
+  }
+	```
+	
+* `general_config` (dict): 通用模型对应的配置信息；默认为 `None`，表示使用默认配置：
+
+  ```python
+  {}
+  ```
+
+* `english_config` (dict): 英文模型对应的配置信息；默认为 `None`，表示使用默认配置：
+
+  ```py
+  {'det_model_name': 'en_PP-OCRv3_det', 'rec_model_name': 'en_PP-OCRv3'}
+  ```
+
+* `formula_config` (dict): 公式识别模型对应的配置信息；默认为 `None`，表示使用默认配置：
+
+  ```python
+  {
+      'config': LATEX_CONFIG_FP,
+      'checkpoint': Path(data_dir()) / 'formula' / 'weights.pth',
+      'no_resize': False
+  }
+  ```
+
+* `thresholds` (dict): 识别阈值对应的配置信息；默认为 `None`，表示使用默认配置：
+
+  ```py
+  {
+      'formula2general': 0.65,  # 如果识别为 `formula` 类型，但得分小于此阈值，则改为 `general` 类型
+      'english2general': 0.75,  # 如果识别为 `english` 类型，但得分小于此阈值，则改为 `general` 类型
+  }
+  ```
+
+* `device` (str): 使用什么资源进行计算，支持 `['cpu', 'cuda', 'gpu']`；默认为 `cpu`
+
+* `**kwargs` (): 预留的其他参数；目前未被使用
+
+
+
+### 识别类函数
+
+通过调用类 **`Pix2Text`** 的类函数 `.recognize()` 完成对指定图片进行识别。类函数 `.recognize()` 说明如下：
+
+```python
+    def recognize(
+        self, img: Union[str, Path, Image.Image], use_analyzer: bool = True, **kwargs
+    ) -> List[Dict[str, Any]]:
+```
+
+
+
+其中的输入参数说明如下：
+
+* `img` (`str` or `Image.Image`)：待识别图片的路径，或者利用 `Image.open()` 已读入的图片 `Image` 。
+* `use_analyzer` (`bool`)：是否使用 Analyzer (**MFD** or **Layout**); `False` 表示把图片看成纯文本或者纯图片处理，相当于 **P2T V0.1.*** 的效果。Default: `True`。
+* `kwargs`: 保留字段，可以包含以下值，
+  * `resized_shape` (`int`): 把图片宽度resize到此大小再进行处理；默认值为 `700`；
+  * `save_analysis_res` (`str`): 把解析结果图片存在此文件中；默认值为 `None`，表示不存储；
+  * `embed_sep` (`tuple`): embedding latex的前后缀；只针对使用 `MFD` 时才有效；默认值为 `(' $', '$ ')`；
+  * `isolated_sep` (`tuple`): isolated latex的前后缀；只针对使用 `MFD` 时才有效；默认值为 `('$$\n', '\n$$')`。
+
+
+
+返回结果为列表（`list`），列表中的每个元素为`dict`，包含如下 `key`：
+
+* `type`：识别出的图像类别；
+  * 当开启Analyzer时（`use_analyzer==True`），取值为 `text`（纯文本）、`isolated`（独立行的数学公式） 或者 `embedding`（行内的数学公式）；
+  
+    >  Warning
+    > 对于 **MFD Analyzer** ，此取值从 P2T **v0.2.3** 开始与之前不同。
+  * 当未开启Analyzer时（`use_analyzer==False`），取值为`formula`（纯数学公式）、`english`（纯英文文字）、`general`（纯文字，可能包含中英文）；
+  
+* `text`：识别出的文字或Latex表达式；
+* `position`：所在块的位置信息，`np.ndarray`, with shape of `[4, 2]`；
+* `line_number`：仅在使用 **MFD Analyzer** 时，才会包含此字段。此字段为 Box 所在的行号（第一行 **`line_number=0`**），值相同的 Box 表示它们在同一行。
+
+  > Warning
+  > 此取值从 P2T **v0.2.3** 开始才有，之前版本没有此 `key`。
+
+
+
+`Pix2Text` 类也实现了 `__call__()` 函数，其功能与 `.recognize()` 函数完全相同。所以才会有以下的调用方式：
+
+```python
+from pix2text import Pix2Text, merge_line_texts
+
+img_fp = './docs/examples/formula.jpg'
+p2t = Pix2Text(analyzer_config=dict(model_name='mfd'))
+outs = p2t(img_fp, resized_shape=608)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
+print(outs)
+# 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
+only_text = merge_line_texts(outs, auto_line_break=True)
+print(only_text)
+```
+
+
+
+## 脚本使用
+
+**P2T** 包含了以下命令行工具。
+
+
+
+### 对单张图片或单个文件夹中的图片进行识别
+
+使用命令 **`p2t predict`** 预测单张图片或文件夹中所有图片，以下是使用说明：
+
+```bash
+$ p2t predict -h
+Usage: p2t predict [OPTIONS]
+
+  模型预测
+
+Options:
+  --use-analyzer / --no-use-analyzer
+                                  是否使用 MFD 或者版面分析 Analyzer  [default: use-
+                                  analyzer]
+  -a, --analyzer-name [mfd|layout]
+                                  使用哪个Analyzer，MFD还是版面分析  [default: mfd]
+  -t, --analyzer-type TEXT        Analyzer使用哪个模型，'yolov7_tiny' or 'yolov7'
+                                  [default: yolov7_tiny]
+  --analyzer-model-fp TEXT        Analyzer检测模型的文件路径。Default：`None`，表示使用默认模型
+  --latex-ocr-model-fp TEXT       Latex-OCR
+                                  数学公式识别模型的文件路径。Default：`None`，表示使用默认模型
+  -d, --device TEXT               使用 `cpu` 还是 `gpu` 运行代码，也可指定为特定gpu，如`cuda:0`
+                                  [default: cpu]
+  --resized-shape INTEGER         把图片宽度resize到此大小再进行处理  [default: 608]
+  -i, --img-file-or-dir TEXT      输入图片的文件路径或者指定的文件夹  [required]
+  --save-analysis-res TEXT        把解析结果存储到此文件或目录中（如果'--img-file-or-
+                                  dir'为文件/文件夹，则'--save-analysis-
+                                  res'也应该是文件/文件夹）。取值为 `None` 表示不存储
+  -l, --log-level TEXT            Log Level, such as `INFO`, `DEBUG`
+                                  [default: INFO]
+  -h, --help                      Show this message and exit.
+```
+
+
+
+此命令可用于**打印对指定图片的检测和识别结果**，如运行：
+
+```bash
+$ p2t predict --use-analyzer -a mfd --resized-shape 608 -i docs/examples/en1.jpg --save-analysis-res output-en1.jpg
+```
+
+上面命令打印出识别结果，同时会把检测结果存储在 `output-en1.jpg` 文件中，类似以下效果：
+
+
+<div align="center">
+  <img src="./docs/figs/output-en1.jpg" alt="P2T 数学公式检测效果图" width="600px"/>
+</div>
+
+
+## HTTP服务
+
+ **Pix2Text** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
+
+```bash
+$ pip install pix2text[serve]
+```
+
+
+
+安装完成后，可以通过以下命令启动HTTP服务（**`-p`** 后面的数字是**端口**，可以根据需要自行调整）：
+
+```bash
+$ p2t serve -p 8503
+```
+
+
+
+`p2t serve` 命令使用说明：
+
+```bash
+$ p2t serve -h
+Usage: p2t serve [OPTIONS]
+
+  开启HTTP服务。
+
+Options:
+  -H, --host TEXT     server host  [default: 0.0.0.0]
+  -p, --port INTEGER  server port  [default: 8503]
+  --reload            whether to reload the server when the codes have been
+                      changed
+  -h, --help          Show this message and exit.
+```
+
+
+
+服务开启后，可以使用以下方式调用服务。
+
+
+
+### 命令行
+
+比如待识别文件为 `docs/examples/mixed.jpg`，如下使用 `curl` 调用服务：
+
+```bash
+$ curl -F image=@docs/examples/mixed.jpg --form 'use_analyzer=true' --form 'resized_shape=600' http://0.0.0.0:8503/pix2text
+```
+
+
+
+### Python
+
+使用如下方式调用服务，参考文件 [scripts/try_service.py](scripts/try_service.py)：
+
+```python
+import requests
+
+url = 'http://0.0.0.0:8503/pix2text'
+
+image_fp = 'docs/examples/mixed.jpg'
+data = {
+    "use_analyzer": True,
+    "resized_shape": 608,
+    "embed_sep": " $,$ ",
+    "isolated_sep": "$$\n, \n$$"
+}
+files = {
+    "image": (image_fp, open(image_fp, 'rb'))
+}
+
+r = requests.post(url, data=data, files=files)
+
+outs = r.json()['results']
+only_text = '\n'.join([out['text'] for out in outs])
+print(f'{only_text=}')
+```
+
+
+
+### 其他语言
+
+请参照 `curl` 的调用方式自行实现。
+
+
+
+## 脚本运行
+
+脚本 [scripts/screenshot_daemon.py](scripts/screenshot_daemon.py) 实现了自动对截屏图片调用 Pixe2Text 进行公式或者文字识别。这个功能是如何实现的呢？
+
+
+
+**以下是具体的运行流程（请先安装好 Pix2Text）：**
+
+1. 找一个喜欢的截屏软件，这个软件只要**支持把截屏图片存储在指定文件夹**即可。比如Mac下免费的 **Xnip** 就很好用。
+
+2. 除了安装Pix2Text外，还需要额外安装一个Python包 **pyperclip**，利用它把识别结果复制进系统的剪切板：
+
+   ```bash
+   $ pip install pyperclip
+   ```
+
+3. 下载脚本文件 [scripts/screenshot_daemon.py](scripts/screenshot_daemon.py) 到本地，编辑此文件 `"SCREENSHOT_DIR"` 所在行（第 `17` 行），把路径改为你的截屏图片所存储的目录。
+
+4. 运行此脚本：
+
+   ```bash
+   $ python scripts/screenshot_daemon.py
+   ```
+
+好了，现在就用你的截屏软件试试效果吧。截屏后的识别结果会写入电脑剪切板，直接 **Ctrl-V** / **Cmd-V** 即可粘贴使用。
+
+
+
+更详细使用介绍可参考视频：《[Pix2Text: 替代 Mathpix 的免费 Python 开源工具](https://www.bilibili.com/video/BV12e4y1871U)》。
+
+
+
+
+## 给作者来杯咖啡
+
+开源不易，如果此项目对您有帮助，可以考虑 [给作者加点油🥤，鼓鼓气💪🏻](https://www.breezedeus.com/buy-me-coffee) 。
+
+---
+
+官方代码库：[https://github.com/breezedeus/pix2text](https://github.com/breezedeus/pix2text) 。
+
+Pix2Text (P2T) 更多信息：[https://www.breezedeus.com/pix2text](https://www.breezedeus.com/pix2text) 。
+
```

### Comparing `pix2text-0.2.2.1/README.md` & `pix2text-0.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: pix2text
+Version: 0.2.3
+Summary: An open-source Python3 tool for Optical Character Recognition (OCR) and LaTeX expression extraction from images, a Free Alternative to Mathpix
+Home-page: https://github.com/breezedeus/pix2text
+Author: breezedeus
+Author-email: breezedeus@163.com
+License: MIT
+Platform: Mac
+Platform: Linux
+Platform: Windows
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: serve
+License-File: LICENSE
+
 <div align="center">
   <img src="./docs/figs/p2t.jpg" width="250px"/>
   <div>&nbsp;</div>
 
 [![Downloads](https://static.pepy.tech/personalized-badge/pix2text?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pix2text)
 [![license](https://img.shields.io/github/license/breezedeus/pix2text)](./LICENSE)
 [![PyPI version](https://badge.fury.io/py/pix2text.svg)](https://badge.fury.io/py/pix2text)
@@ -18,25 +46,35 @@
 
 <div align="center">
 
 [English](./README_en.md) | 中文
 </div>
 
 # Pix2Text (P2T)
+## Update 2023.07.03：发布 V0.2.3
 
+主要变更：
+* 训练了新的**公式识别模型**，供 **[P2T网页版](https://p2t.behye.com)** 使用。新模型精度更高，尤其对**手写公式**和**多行公式**类图片。具体参考：[Pix2Text 新版公式识别模型 | Breezedeus.com](https://www.breezedeus.com/article/p2t-mfd-20230702) 。
+* 优化了对检测出的boxes的排序逻辑，以及对混合图片的处理逻辑，使得最终识别效果更符合直觉。
+* 优化了识别结果的合并逻辑，自动判断是否该换行，是否分段。
+* 修复了模型文件自动下载的功能。HuggingFace似乎对下载文件的逻辑做了调整，导致之前版本的自动下载失败，当前版本已修复。但由于HuggingFace国内被墙，国内下载仍需 **梯子（VPN）**。
+* 更新了各个依赖包的版本号。
+
+## Update 2023.06.20：发布新版 MFD 模型
+
+主要变更：
+* 基于新标注的数据，重新训练了 **MFD YoloV7** 模型，目前新模型已部署到 [P2T网页版](https://p2t.behye.com) 。具体说明见：[Pix2Text (P2T) 新版公式检测模型 | Breezedeus.com](https://www.breezedeus.com/article/p2t-mfd-20230613) 。
+* 之前的 MFD YoloV7 模型已开放给星球会员下载，具体说明见：[P2T YoloV7 数学公式检测模型开放给星球会员下载 | Breezedeus.com](https://www.breezedeus.com/article/p2t-yolov7-for-zsxq-20230619) 。
 
-【Update 2023.02.10： **[P2T网页版](https://p2t.behye.com)** 开放免费使用】
+## Update 2023.02.10： **[P2T网页版](https://p2t.behye.com)** 开放免费使用
 
 * P2T作为Python包，对于不熟悉Python的朋友还是太不友好，所以我们也开发了 [P2T网页版](https://p2t.behye.com)，可直接免费使用，欢迎帮忙推荐分享。
 * 视频介绍：[Pix2Text 新版和网页版发布，离Mathpix又近了一大步_bilibili](https://www.bilibili.com/video/BV1U24y1q7n3) 。
 * 文字版介绍：[Pix2Text (P2T) 新版发布，离Mathpix又近了一大步 - 知乎](https://zhuanlan.zhihu.com/p/604999678) 。
 
-【Update 2023.02.03：**V0.2** 发布】
-
-* 利用 **[CnSTD](https://github.com/breezedeus/cnstd)** 新版的**数学公式检测**（**Mathematical Formula Detection**，简称 **MFD**）能力，**P2T V0.2** 支持**识别既包含文字又包含公式的混合图片**。
 
 了解更多：[RELEASE.md](./RELEASE.md) 。
 
 ---
 
 
 
@@ -48,51 +86,50 @@
 
 
 
 **P2T** 使用开源工具  **[CnSTD](https://github.com/breezedeus/cnstd)** 检测出图片中**数学公式**所在位置，再交由 **[LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)** 识别出各对应位置数学公式的Latex表示。图片的剩余部分再交由 **[CnOCR](https://github.com/breezedeus/cnocr)** 进行文字检测和文字识别。最后 P2T 合并所有识别结果，获得最终的图片识别结果。感谢这些开源工具。
 
 
 
-P2T 作为Python3工具包，对于不熟悉Python的朋友不太友好，我们近期也会发布 **P2T网页版**，直接把图片丢进网页就能输出P2T的解析结果。
-
-网页版会提供一些**免费名额**供有需要的朋友使用，优先在校学生（**[MathPix](https://link.zhihu.com/?target=https%3A//mathpix.com/)** 每月要5美元，对在校生来说还是蛮贵的）。
+P2T 作为Python3工具包，对于不熟悉Python的朋友不太友好，所以我们也发布了**可免费使用**的 **[P2T网页版](https://p2t.behye.com)**，直接把图片丢进网页就能输出P2T的解析结果。**网页版会使用最新的模型，效果会比开源模型更好。**
 
 
 
 感兴趣的朋友欢迎扫码加小助手为好友，备注 `p2t`，小助手会定期统一邀请大家入群。群内会发布P2T相关工具的最新进展：
 
 <div align="center">
   <img src="./docs/figs/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
 </div>
 
 
 
-作者也维护 **知识星球** [**P2T/CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) ，这里面的提问会较快得到作者的回复，欢迎加入。**知识星球私享群**也会陆续发布一些P2T/CnOCR/CnSTD相关的私有资料，包括[**更详细的训练教程**](https://articles.zsxq.com/id_u6b4u0wrf46e.html)，**未公开的模型**，**不同应用场景的调用代码**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。
+作者也维护 **知识星球** [**P2T/CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) ，这里面的提问会较快得到作者的回复，欢迎加入。**知识星球私享群**也会陆续发布一些P2T/CnOCR/CnSTD相关的私有资料，包括[**更详细的训练教程**](https://articles.zsxq.com/id_u6b4u0wrf46e.html)，**部分未公开的模型**，**购买付费模型享优惠**，**不同应用场景的调用代码**，使用过程中遇到的难题解答等。星球也会发布P2T/OCR/STD相关的最新研究资料。
 
 
 
 ## 使用说明
 
 
 调用很简单，以下是示例：
 
 ```python
-from pix2text import Pix2Text
+from pix2text import Pix2Text, merge_line_texts
 
 img_fp = './docs/examples/formula.jpg'
 p2t = Pix2Text(analyzer_config=dict(model_name='mfd'))
 outs = p2t(img_fp, resized_shape=600)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
 print(outs)
 # 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
-only_text = '\n'.join([out['text'] for out in outs])
+only_text = merge_line_texts(outs, auto_line_break=True)
+print(only_text)
 ```
 
 
 
-返回结果 `out_text` 是个 `dict`，其中 key `position` 表示位置信息，`type` 表示类别信息，而 `text` 表示识别的结果。具体见下面的[接口说明](#接口说明)。
+返回结果 `outs` 是个 `dict`，其中 key `position` 表示Box位置信息，`type` 表示类别信息，而 `text` 表示识别的结果。具体见下面的[接口说明](#接口说明)。
 
 
 
 ## 示例
 
 <table>
 <tr>
@@ -103,49 +140,79 @@
 <td>
 <img src="./docs/examples/mixed.jpg" alt="mixed"> 
 
 </td>
 <td>
 
 ```python
-[{"position": array([[         22,          29],
-       [       1055,          29],
-       [       1055,          56],
-       [         22,          56]], dtype=float32),
-  "text": "JVAE的训练loss和VQ-VAE类似，只是使用了KL距离来让分布尽量分散",
-  "type": "text"},
- {"position": array([[        629,         124],
-       [       1389,         124],
-       [       1389,         183],
-       [        629,         183]]),
-  "text": "$$\n"
-          "-{\\cal E}_{z\\sim q(z|x)}[\\log(p(x\\mid z))]"
-          "+{\\cal K}{\\cal L}(q(z\\mid x)||p(z))\n"
-          "$$",
-  "type": "isolated"},
- {"position": array([[         20,         248],
-       [       1297,         248],
-       [       1297,         275],
-       [         20,         275]], dtype=float32),
-  "text": "其中之利用 Gumbel-Softmax从 $z\\sim q(z|x)$ 中抽样得到，"
-  " $p(z)$ 是个等概率的多项式分布。",
-  "type": "text-embed"}]
+[{'line_number': 0,
+  'position': array([[         22,          31],
+       [       1057,          31],
+       [       1057,          58],
+       [         22,          58]]),
+  'text': 'JVAE的训练loss和VQ-VAE类似，只是使用了KL距离来让分布尽量分散',
+  'type': 'text'},
+ {'line_number': 1,
+  'position': array([[        625,         121],
+       [       1388,         121],
+       [       1388,         182],
+       [        625,         182]]),
+  'text': '$$\n'
+          '-E_{z\\sim q(z\\mid x)}[\\log(p(x\\mid z))]+K L(q(z\\mid x))|p(z))\n'
+          '$$',
+  'type': 'isolated'},
+ {'line_number': 2,
+  'position': array([[         18,         242],
+       [        470,         242],
+       [        470,         275],
+       [         18,         275]]),
+  'text': '其中之利用 Gumbel-Softmax 人',
+  'type': 'text'},
+ {'line_number': 2,
+  'position': array([[        481,         238],
+       [        664,         238],
+       [        664,         287],
+       [        481,         287]]),
+  'text': ' $z\\sim q(z|x)$ ',
+  'type': 'embedding'},
+ {'line_number': 2,
+  'position': array([[        667,         244],
+       [        840,         244],
+       [        840,         277],
+       [        667,         277]]),
+  'text': '中抽样得到,',
+  'type': 'text'},
+ {'line_number': 2,
+  'position': array([[        852,         239],
+       [        932,         239],
+       [        932,         288],
+       [        852,         288]]),
+  'text': ' $\\scriptstyle{p(z)}$ ',
+  'type': 'embedding'},
+ {'line_number': 2,
+  'position': array([[        937,         244],
+       [       1299,         244],
+       [       1299,         277],
+       [        937,         277]]),
+  'text': '是个等概率的多项式分布',
+  'type': 'text'}]
 ```
 
 </td>
 </tr>
 <tr>
 <td>
 
 <img src="./docs/examples/formula.jpg" alt="formula"> 
 </td>
 <td>
 
 ```python
-[{"position": array([[         12,          19],
+[{"line_number": 0,
+  "position": array([[         12,          19],
        [        749,          19],
        [        749,         150],
        [         12,         150]]),
   "text": "$$\n"
           "\\mathcal{L}_{\\mathrm{eyelid}}~\\equiv~"
           "\\sum_{t=1}^{T}\\sum_{v=1}^{V}"
           "\\mathcal{N}_{U}^{\\mathrm{(eyelid)}}"
@@ -196,15 +263,17 @@
 </tr>
 </table>
 
 
 
 ## 模型下载
 
-安装好 Pix2Text 后，首次使用时系统会**自动下载** 模型文件，并存于 `~/.pix2text`目录（Windows下默认路径为 `C:\Users\<username>\AppData\Roaming\pix2text`）。
+### 开源免费模型
+
+安装好 Pix2Text 后，首次使用时系统会**自动下载** 免费模型文件，并存于 `~/.pix2text`目录（Windows下默认路径为 `C:\Users\<username>\AppData\Roaming\pix2text`）。
 
 
 
 > **Note**
 >
 > 如果已成功运行上面的示例，说明模型已完成自动下载，可忽略本节后续内容。
 
@@ -212,14 +281,20 @@
 
 对于**分类模型**，系统会自动下载模型`mobilenet_v2.zip`文件并对其解压，然后把解压后的模型相关目录放于`~/.pix2text`目录中。如果系统无法自动成功下载`mobilenet_v2.zip`文件，则需要手动从 **[cnstd-cnocr-models/pix2text](https://huggingface.co/breezedeus/cnstd-cnocr-models/tree/main/models/pix2text/0.2)** 下载此zip文件并把它放于 `~/.pix2text`目录。如果下载太慢，也可以从 [百度云盘](https://pan.baidu.com/s/1kubZF4JGE19d98NDoPHJzQ?pwd=p2t0) 下载， 提取码为 ` p2t0`。
 
 对于  **[LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)** ，系统同样会自动下载模型文件并把它们存放于`~/.pix2text/formula`目录中。如果系统无法自动成功下载这些模型文件，则需从  [百度云盘](https://pan.baidu.com/s/1kubZF4JGE19d98NDoPHJzQ?pwd=p2t0) 下载文件 `weights.pth` 和 `image_resizer.pth`， 并把它们存放于`~/.pix2text/formula`目录中；提取码为 ` p2t0`。
 
 
 
+### 付费模型
+
+除了上面免费的开源模型，P2T 也训练了精度更高的数学公式检测和识别模型，这些模型供 **[P2T网页版](https://p2t.behye.com)** 使用，它们的效果也可以在网页版体验。这些模型不是免费的（抱歉开源作者也是要喝咖啡的），具体可参考 [Pix2Text (P2T) | Breezedeus.com](https://www.breezedeus.com/pix2text#259b04346dd94f45a65c10ff3db48540) 。
+
+
+
 ## 安装
 
 嗯，顺利的话一行命令即可。
 
 ```bash
 pip install pix2text
 ```
@@ -304,15 +379,15 @@
   ```
 
 * `formula_config` (dict): 公式识别模型对应的配置信息；默认为 `None`，表示使用默认配置：
 
   ```python
   {
       'config': LATEX_CONFIG_FP,
-      'checkpoint': Path(data_dir()) / 'formular' / 'weights.pth',
+      'checkpoint': Path(data_dir()) / 'formula' / 'weights.pth',
       'no_resize': False
   }
   ```
 
 * `thresholds` (dict): 识别阈值对应的配置信息；默认为 `None`，表示使用默认配置：
 
   ```py
@@ -351,46 +426,54 @@
   * `isolated_sep` (`tuple`): isolated latex的前后缀；只针对使用 `MFD` 时才有效；默认值为 `('$$\n', '\n$$')`。
 
 
 
 返回结果为列表（`list`），列表中的每个元素为`dict`，包含如下 `key`：
 
 * `type`：识别出的图像类别；
-  * 当开启Analyzer时（`use_analyzer==True`），取值为 `text`（纯文本）、`isolated`（独立行的数学公式） 或者 `text-embed`（文本行中包含了嵌入式的数学公式）；
+  * 当开启Analyzer时（`use_analyzer==True`），取值为 `text`（纯文本）、`isolated`（独立行的数学公式） 或者 `embedding`（行内的数学公式）；
+  
+    >  Warning
+    > 对于 **MFD Analyzer** ，此取值从 P2T **v0.2.3** 开始与之前不同。
   * 当未开启Analyzer时（`use_analyzer==False`），取值为`formula`（纯数学公式）、`english`（纯英文文字）、`general`（纯文字，可能包含中英文）；
-
+  
 * `text`：识别出的文字或Latex表达式；
-* `position`：所在块的位置信息，`np.ndarray`, with shape of `[4, 2]`。
+* `position`：所在块的位置信息，`np.ndarray`, with shape of `[4, 2]`；
+* `line_number`：仅在使用 **MFD Analyzer** 时，才会包含此字段。此字段为 Box 所在的行号（第一行 **`line_number=0`**），值相同的 Box 表示它们在同一行。
+
+  > Warning
+  > 此取值从 P2T **v0.2.3** 开始才有，之前版本没有此 `key`。
 
 
 
 `Pix2Text` 类也实现了 `__call__()` 函数，其功能与 `.recognize()` 函数完全相同。所以才会有以下的调用方式：
 
 ```python
-from pix2text import Pix2Text
+from pix2text import Pix2Text, merge_line_texts
 
 img_fp = './docs/examples/formula.jpg'
 p2t = Pix2Text(analyzer_config=dict(model_name='mfd'))
-outs = p2t(img_fp, resized_shape=600)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
+outs = p2t(img_fp, resized_shape=608)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
 print(outs)
 # 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
-only_text = '\n'.join([out['text'] for out in outs])
+only_text = merge_line_texts(outs, auto_line_break=True)
+print(only_text)
 ```
 
 
 
 ## 脚本使用
 
 **P2T** 包含了以下命令行工具。
 
 
 
 ### 对单张图片或单个文件夹中的图片进行识别
 
-使用命令 **`p2t predict`** 预测单个文件或文件夹中所有图片，以下是使用说明：
+使用命令 **`p2t predict`** 预测单张图片或文件夹中所有图片，以下是使用说明：
 
 ```bash
 $ p2t predict -h
 Usage: p2t predict [OPTIONS]
 
   模型预测
 
@@ -398,28 +481,45 @@
   --use-analyzer / --no-use-analyzer
                                   是否使用 MFD 或者版面分析 Analyzer  [default: use-
                                   analyzer]
   -a, --analyzer-name [mfd|layout]
                                   使用哪个Analyzer，MFD还是版面分析  [default: mfd]
   -t, --analyzer-type TEXT        Analyzer使用哪个模型，'yolov7_tiny' or 'yolov7'
                                   [default: yolov7_tiny]
+  --analyzer-model-fp TEXT        Analyzer检测模型的文件路径。Default：`None`，表示使用默认模型
+  --latex-ocr-model-fp TEXT       Latex-OCR
+                                  数学公式识别模型的文件路径。Default：`None`，表示使用默认模型
   -d, --device TEXT               使用 `cpu` 还是 `gpu` 运行代码，也可指定为特定gpu，如`cuda:0`
                                   [default: cpu]
-  --resized-shape INTEGER         把图片宽度resize到此大小再进行处理  [default: 600]
+  --resized-shape INTEGER         把图片宽度resize到此大小再进行处理  [default: 608]
   -i, --img-file-or-dir TEXT      输入图片的文件路径或者指定的文件夹  [required]
   --save-analysis-res TEXT        把解析结果存储到此文件或目录中（如果'--img-file-or-
                                   dir'为文件/文件夹，则'--save-analysis-
                                   res'也应该是文件/文件夹）。取值为 `None` 表示不存储
   -l, --log-level TEXT            Log Level, such as `INFO`, `DEBUG`
                                   [default: INFO]
   -h, --help                      Show this message and exit.
 ```
 
 
 
+此命令可用于**打印对指定图片的检测和识别结果**，如运行：
+
+```bash
+$ p2t predict --use-analyzer -a mfd --resized-shape 608 -i docs/examples/en1.jpg --save-analysis-res output-en1.jpg
+```
+
+上面命令打印出识别结果，同时会把检测结果存储在 `output-en1.jpg` 文件中，类似以下效果：
+
+
+<div align="center">
+  <img src="./docs/figs/output-en1.jpg" alt="P2T 数学公式检测效果图" width="600px"/>
+</div>
+
+
 ## HTTP服务
 
  **Pix2Text** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
 
 ```bash
 $ pip install pix2text[serve]
 ```
@@ -474,15 +574,15 @@
 import requests
 
 url = 'http://0.0.0.0:8503/pix2text'
 
 image_fp = 'docs/examples/mixed.jpg'
 data = {
     "use_analyzer": True,
-    "resized_shape": 600,
+    "resized_shape": 608,
     "embed_sep": " $,$ ",
     "isolated_sep": "$$\n, \n$$"
 }
 files = {
     "image": (image_fp, open(image_fp, 'rb'))
 }
 
@@ -532,13 +632,15 @@
 更详细使用介绍可参考视频：《[Pix2Text: 替代 Mathpix 的免费 Python 开源工具](https://www.bilibili.com/video/BV12e4y1871U)》。
 
 
 
 
 ## 给作者来杯咖啡
 
-开源不易，如果此项目对您有帮助，可以考虑 [给作者加点油🥤，鼓鼓气💪🏻](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
+开源不易，如果此项目对您有帮助，可以考虑 [给作者加点油🥤，鼓鼓气💪🏻](https://www.breezedeus.com/buy-me-coffee) 。
 
 ---
 
-官方代码库：[https://github.com/breezedeus/pix2text](https://github.com/breezedeus/pix2text)。
+官方代码库：[https://github.com/breezedeus/pix2text](https://github.com/breezedeus/pix2text) 。
+
+Pix2Text (P2T) 更多信息：[https://www.breezedeus.com/pix2text](https://www.breezedeus.com/pix2text) 。
```

### Comparing `pix2text-0.2.2.1/pix2text/app.py` & `pix2text-0.2.3/pix2text/app.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.2.1/pix2text/category_mapping.py` & `pix2text-0.2.3/pix2text/category_mapping.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.2.1/pix2text/cli.py` & `pix2text-0.2.3/pix2text/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # coding: utf-8
-# Copyright (C) 2022, [Breezedeus](https://github.com/breezedeus).
+# Copyright (C) 2022-2023, [Breezedeus](https://www.breezedeus.com).
 
 import os
 import logging
 import glob
 from multiprocessing import Process
 import subprocess
 from pprint import pformat
 
 import click
 
-from pix2text import set_logger, Pix2Text
+from pix2text import set_logger, Pix2Text, merge_line_texts
+from pix2text.consts import LATEX_CONFIG_FP
 
 _CONTEXT_SETTINGS = {"help_option_names": ['-h', '--help']}
 logger = set_logger(log_level=logging.INFO)
 
 
 @click.group(context_settings=_CONTEXT_SETTINGS)
 def cli():
@@ -41,26 +42,40 @@
     "--analyzer-type",
     type=str,
     default='yolov7_tiny',
     help="Analyzer使用哪个模型，'yolov7_tiny' or 'yolov7'",
     show_default=True,
 )
 @click.option(
+    "--analyzer-model-fp",
+    type=str,
+    default=None,
+    help="Analyzer检测模型的文件路径。Default：`None`，表示使用默认模型",
+    show_default=True,
+)
+@click.option(
+    "--latex-ocr-model-fp",
+    type=str,
+    default=None,
+    help="Latex-OCR 数学公式识别模型的文件路径。Default：`None`，表示使用默认模型",
+    show_default=True,
+)
+@click.option(
     "-d",
     "--device",
     help="使用 `cpu` 还是 `gpu` 运行代码，也可指定为特定gpu，如`cuda:0`",
     type=str,
     default='cpu',
     show_default=True,
 )
 @click.option(
     "--resized-shape",
     help="把图片宽度resize到此大小再进行处理",
     type=int,
-    default=600,
+    default=608,
     show_default=True,
 )
 @click.option("-i", "--img-file-or-dir", required=True, help="输入图片的文件路径或者指定的文件夹")
 @click.option(
     "--save-analysis-res",
     default=None,
     help="把解析结果存储到此文件或目录中"
@@ -75,26 +90,34 @@
     help="Log Level, such as `INFO`, `DEBUG`",
     show_default=True,
 )
 def predict(
     use_analyzer,
     analyzer_name,
     analyzer_type,
+    analyzer_model_fp,
+    latex_ocr_model_fp,
     device,
     resized_shape,
     img_file_or_dir,
     save_analysis_res,
     log_level,
 ):
     """模型预测"""
     logger = set_logger(log_level=log_level)
 
+    analyzer_config = dict(model_name=analyzer_name, model_type=analyzer_type)
+    if analyzer_model_fp is not None:
+        analyzer_config['model_fp'] = analyzer_model_fp
+
+    formula_config = None
+    if latex_ocr_model_fp is not None:
+        formula_config = {'model_fp': latex_ocr_model_fp}
     p2t = Pix2Text(
-        analyzer_config=dict(model_name=analyzer_name, model_type=analyzer_type),
-        device=device,
+        analyzer_config=analyzer_config, formula_config=formula_config, device=device,
     )
 
     fp_list = []
     if os.path.isfile(img_file_or_dir):
         fp_list.append(img_file_or_dir)
         if save_analysis_res:
             save_analysis_res = [save_analysis_res]
@@ -111,16 +134,16 @@
         analysis_res = save_analysis_res[idx] if save_analysis_res is not None else None
         out = p2t.recognize(
             fp,
             use_analyzer=use_analyzer,
             resized_shape=resized_shape,
             save_analysis_res=analysis_res,
         )
-        res = '\n'.join([o['text'] for o in out])
-        logger.info(f'In image: {fp}\nOuts: \n\t{pformat(out)}\nOnly texts: \n\t{res}')
+        res = merge_line_texts(out, auto_line_break=True)
+        logger.info(f'In image: {fp}\nOuts: \n\t{pformat(out)}\nOnly texts: \n{res}')
 
 
 @cli.command('serve')
 @click.option(
     '-H', '--host', type=str, default='0.0.0.0', help='server host', show_default=True,
 )
 @click.option(
```

### Comparing `pix2text-0.2.2.1/pix2text/latex_config.yaml` & `pix2text-0.2.3/pix2text/latex_config.yaml`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.2.1/pix2text/latex_ocr.py` & `pix2text-0.2.3/pix2text/latex_ocr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding: utf-8
 # Copyright (C) 2022, [Breezedeus](https://github.com/breezedeus).
 #
 # credit to: pix2tex, lukas-blecher/LaTeX-OCR
 # Adapted from https://github.com/lukas-blecher/LaTeX-OCR/blob/main/pix2tex/cli.py
-
 from typing import Tuple, Optional, Dict, Any
 import logging
 import yaml
 from pathlib import Path
 
 from PIL import Image
 from transformers import PreTrainedTokenizerFast
@@ -24,34 +23,41 @@
 from .consts import LATEX_CONFIG_FP
 from .utils import data_dir
 
 
 logger = logging.getLogger(__name__)
 
 
-def download_checkpoints(out_dl_dir):
+def download_checkpoints(args):
     # adapted from pix2tex.model.checkpoints.get_latest_checkpoint
+    ckpt_list = [args.mfr_checkpoint, args.resizer_checkpoint]
     tag = 'v0.0.1'  # get_latest_tag()
-    os.makedirs(out_dl_dir, exist_ok=True)
     weights = (
         'https://github.com/lukas-blecher/LaTeX-OCR/releases/download/%s/weights.pth'
         % tag
     )
     resizer = (
         'https://github.com/lukas-blecher/LaTeX-OCR/releases/download/%s/image_resizer.pth'
         % tag
     )
-    for url, name in zip([weights, resizer], ['weights.pth', 'image_resizer.pth']):
-        if not os.path.exists(os.path.join(out_dl_dir, name)):
+    for idx, (url, fp) in enumerate(zip([weights, resizer], ckpt_list)):
+        name = os.path.basename(url)
+        if not os.path.exists(fp):
+            if os.path.basename(fp) != name:
+                logger.warning(f'can not find file {fp}, download {name} from {url} instead')
+                fp = os.path.join(os.path.dirname(fp), name)
+                if idx == 0:
+                    args.mfr_checkpoint = fp
+                else:
+                    args.resizer_checkpoint = fp
+            os.makedirs(os.path.dirname(fp), exist_ok=True)
             file = download_as_bytes_with_progress(url, name)
-            logger.info('downloading file %s to path %s', name, out_dl_dir)
-            open(os.path.join(out_dl_dir, name), "wb").write(file)
-            logger.info(f'save {name} to path {out_dl_dir}')
-        else:
-            logger.info(f'use model {name} from path {out_dl_dir}')
+            logger.info('downloading file %s to path %s', name, fp)
+            open(fp, "wb").write(file)
+            logger.info(f'save {name} to path {fp}')
 
 
 def minmax_size(
     img: Image,
     max_dimensions: Tuple[int, int] = None,
     min_dimensions: Tuple[int, int] = None,
 ) -> Image:
@@ -202,63 +208,65 @@
     @in_model_path()
     def __init__(self, arguments: Optional[Dict[str, Any]] = None):
         """Initialize a LatexOCR model
 
         Args:
             arguments (Union[Namespace, Munch], optional): Special model parameters. Defaults to None.
         """
-        if arguments is None:
-            arguments = {
-                'config': LATEX_CONFIG_FP,
-                'checkpoint': Path(data_dir()) / 'formula' / 'weights.pth',
-                # 'no_cuda': True,
-                'no_resize': False,
-                'device': 'cpu',
-            }
+        def_arguments = {
+            'config': LATEX_CONFIG_FP,
+            'mfr_checkpoint': Path(data_dir()) / 'formula' / 'weights.pth',
+            'resizer_checkpoint': Path(data_dir()) / 'formula' / 'image_resizer.pth',
+            # 'no_cuda': True,
+            'no_resize': False,
+            'device': 'cpu',
+        }
+        if arguments is not None:
+            if 'model_fp' in arguments:
+                arguments['mfr_checkpoint'] = arguments.pop('model_fp')
+            def_arguments.update(arguments)
+        arguments = def_arguments
 
         arguments = Munch(arguments)
         os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
         with open(arguments.config, 'r') as f:
             params = yaml.load(f, Loader=yaml.FullLoader)
         self.args = parse_args(Munch(params))
         self.args.update(**vars(arguments))
         self.args.wandb = False
         # self.args.device = (
         #     'cuda' if torch.cuda.is_available() and not self.args.no_cuda else 'cpu'
         # )
-        # if not os.path.exists(self.args.checkpoint):
-        download_checkpoints(os.path.dirname(arguments.checkpoint))
+        download_checkpoints(self.args)
+
         self.model = get_model(self.args)
         self.model.load_state_dict(
-            torch.load(self.args.checkpoint, map_location=self.args.device)
+            torch.load(self.args.mfr_checkpoint, map_location=self.args.device)
         )
+        logger.info(f'use model: {self.args.mfr_checkpoint}')
         self.model.eval()
 
-        if (
-            'image_resizer.pth' in os.listdir(os.path.dirname(self.args.checkpoint))
-            and not arguments.no_resize
-        ):
+        if not self.args.no_resize and os.path.isfile(self.args.resizer_checkpoint):
             self.image_resizer = ResNetV2(
                 layers=[2, 3, 3],
                 num_classes=max(self.args.max_dimensions) // 32,
                 global_pool='avg',
                 in_chans=1,
                 drop_rate=0.05,
                 preact=True,
                 stem_type='same',
                 conv_layer=StdConv2dSame,
             ).to(self.args.device)
             self.image_resizer.load_state_dict(
                 torch.load(
-                    os.path.join(
-                        os.path.dirname(self.args.checkpoint), 'image_resizer.pth'
-                    ),
+                    self.args.resizer_checkpoint,
                     map_location=self.args.device,
                 )
             )
+            logger.info(f'use model: {self.args.resizer_checkpoint}')
             self.image_resizer.eval()
         self.tokenizer = PreTrainedTokenizerFast(tokenizer_file=self.args.tokenizer)
 
     @in_model_path()
     def __call__(self, img=None, resize=True) -> str:
         """Get a prediction from an image
```

### Comparing `pix2text-0.2.2.1/pix2text/object_detector.py` & `pix2text-0.2.3/pix2text/object_detector.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.2.1/pix2text/pix_to_text.py` & `pix2text-0.2.3/pix2text/pix_to_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 # coding: utf-8
-# Copyright (C) 2022, [Breezedeus](https://github.com/breezedeus).
+# Copyright (C) 2022-2023, [Breezedeus](https://www.breezedeus.com).
 
 import os
 from glob import glob
 import logging
+from itertools import chain
 from pathlib import Path
 from typing import Dict, Any, Optional, Union, List
-from copy import deepcopy
+from copy import deepcopy, copy
 
 from PIL import Image
 import numpy as np
 import torch
 from cnocr import CnOcr, ImageClassifier
+from cnstd.utils import get_model_file
 from cnstd import LayoutAnalyzer
 from cnstd.yolov7.consts import CATEGORY_DICT
-from cnstd.utils.utils import sort_boxes
+
+from .utils import sort_boxes, rotated_box_to_horizontal, is_valid_box, list2box
 from cnstd.yolov7.general import xyxy24p, box_partial_overlap
 
-from .consts import IMAGE_TYPES, LATEX_CONFIG_FP, MODEL_VERSION, CLF_MODEL_URL_FMT
+from .consts import (
+    IMAGE_TYPES,
+    LATEX_CONFIG_FP,
+    MODEL_VERSION,
+    CLF_MODEL_URL_FMT,
+    format_hf_hub_url,
+)
 from .latex_ocr import LatexOCR
 from .utils import (
     data_dir,
     read_img,
-    get_model_file,
     save_layout_img,
-    is_valid_box,
-    rotated_box_to_horizontal,
 )
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_CONFIGS = {
     'analyzer': {'model_name': 'mfd'},
@@ -44,15 +50,15 @@
         'model_dir': Path(data_dir()) / 'clf',
         'model_fp': None,  # 如果指定，直接使用此模型文件
     },
     'general': {},
     'english': {'det_model_name': 'en_PP-OCRv3_det', 'rec_model_name': 'en_PP-OCRv3'},
     'formula': {
         'config': LATEX_CONFIG_FP,
-        'checkpoint': Path(data_dir()) / 'formular' / 'weights.pth',
+        'checkpoint': Path(data_dir()) / 'formula' / 'weights.pth',
         'no_resize': False,
     },
     'thresholds': {  # 用于clf场景
         'formula2general': 0.65,  # 如果识别为 `formula` 类型，但阈值小于此值，则改为 `general` 类型
         'english2general': 0.75,  # 如果识别为 `english` 类型，但阈值小于此值，则改为 `general` 类型
     },
 }
@@ -164,15 +170,15 @@
         if len(fps) > 1:
             raise ValueError(
                 'multiple .ckpt files are found in %s, not sure which one should be used'
                 % model_dir
             )
         elif len(fps) < 1:
             logger.warning('no .ckpt file is found in %s' % model_dir)
-            url = CLF_MODEL_URL_FMT % clf_config['base_model_name']
+            url = format_hf_hub_url(CLF_MODEL_URL_FMT % clf_config['base_model_name'])
             get_model_file(url, model_dir)  # download the .zip file and unzip
             fps = glob(os.path.join(model_dir, model_file_prefix) + '*.ckpt')
 
         model_fp = fps[0]
         self.image_clf.load(model_fp, self.device)
 
     @classmethod
@@ -271,28 +277,30 @@
     ) -> List[Dict[str, Any]]:
         """
         对图片先做MFD 或 版面分析，然后再识别每块中包含的信息。
 
         Args:
             img (str or Image.Image): an image path, or `Image.Image` loaded by `Image.open()`
             kwargs ():
-                * resized_shape (int): 把图片宽度resize到此大小再进行处理；默认值为 `700`
+                * resized_shape (int): 把图片宽度resize到此大小再进行处理；默认值为 `608`
                 * save_analysis_res (str): 把解析结果图片存在此文件中；默认值为 `None`，表示不存储
                 * embed_sep (tuple): embedding latex的前后缀；默认值为 `(' $', '$ ')`
                 * isolated_sep (tuple): isolated latex的前后缀；默认值为 `('$$\n', '\n$$')`
 
-        Returns: a list of dicts, with keys:
-           `type`: 图像类别；
+        Returns: a list of ordered (top to bottom, left to right) dicts,
+            with each dict representing one detected box, containing keys:
+           `type`: 图像类别；Optional: 'text', 'isolated', 'embedding'
            `text`: 识别出的文字或Latex公式
            `position`: 所在块的位置信息，`np.ndarray`, with shape of [4, 2]
+           `line_number`: box 所在行号（第一行 `line_number==0`），值相同的box表示它们在同一行
 
         """
         # 对于大图片，把图片宽度resize到此大小；宽度比此小的图片，其实不会放大到此大小，
         # 具体参考：cnstd.yolov7.layout_analyzer.LayoutAnalyzer._preprocess_images 中的 `letterbox` 行
-        resized_shape = kwargs.get('resized_shape', 700)
+        resized_shape = kwargs.get('resized_shape', 608)
         if isinstance(img, Image.Image):
             img0 = img.convert('RGB')
         else:
             img0 = read_img(img, return_type='Image')
         w, h = img0.size
         ratio = resized_shape / w
         resized_shape = (int(h * ratio), resized_shape)  # (H, W)
@@ -315,15 +323,15 @@
             sep = isolated_sep if box_info['type'] == 'isolated' else embed_sep
             text = sep[0] + patch_out + sep[1]
             mf_out.append({'type': box_info['type'], 'text': text, 'position': box})
 
         img = np.array(img0.copy())
         # 把公式部分mask掉，然后对其他部分进行OCR
         for box_info in analyzer_outs:
-            if box_info['type'] == 'isolated':
+            if box_info['type'] in ('isolated', 'embedding'):
                 box = box_info['box']
                 xmin, ymin = max(0, int(box[0][0]) - 1), max(0, int(box[0][1]) - 1)
                 xmax, ymax = (
                     min(img0.size[0], int(box[2][0]) + 1),
                     min(img0.size[1], int(box[2][1]) + 1),
                 )
                 img[ymin:ymax, xmin:xmax, :] = 255
@@ -331,83 +339,88 @@
         box_infos = self.general_ocr.det_model.detect(img)
 
         def _to_iou_box(ori):
             return torch.tensor([ori[0][0], ori[0][1], ori[2][0], ori[2][1]]).unsqueeze(
                 0
             )
 
-        outs = [box_info for box_info in mf_out if box_info['type'] == 'isolated']
+        total_text_boxes = []
         for crop_img_info in box_infos['detected_texts']:
             # crop_img_info['box'] 可能是一个带角度的矩形框，需要转换成水平的矩形框
             hor_box = rotated_box_to_horizontal(crop_img_info['box'])
             if not is_valid_box(hor_box, min_height=8, min_width=2):
                 continue
             line_box = _to_iou_box(hor_box)
             embed_mfs = []
             for box_info in mf_out:
                 if box_info['type'] == 'embedding':
                     box2 = _to_iou_box(box_info['position'])
-                    if float(box_partial_overlap(line_box, box2).squeeze()) > 0.3:
+                    if float(box_partial_overlap(line_box, box2).squeeze()) > 0.7:
                         embed_mfs.append(
                             {
                                 'position': box2[0].int().tolist(),
                                 'text': box_info['text'],
                                 'type': box_info['type'],
                             }
                         )
 
             ocr_boxes = self._split_line_image(line_box, embed_mfs)
+            total_text_boxes.extend(ocr_boxes)
 
-            text = []
-            for box in ocr_boxes:
-                if box['type'] == 'text':
-                    crop_patch = torch.tensor(np.asarray(img0.crop(box['position'])))
-                    part_text = self._ocr_for_single_line(crop_patch, 'general')
-                else:
-                    part_text = box['text']
-                text.append(part_text)
-            text = ''.join(text)
-
-            outs.append(
-                {
-                    'type': 'text-embed' if embed_mfs else 'text',
-                    'text': text,
-                    'position': hor_box,
-                }
-            )
+        outs = copy(mf_out)
+        for box in total_text_boxes:
+            crop_patch = torch.tensor(np.asarray(img0.crop(box['position'])))
+            part_res = self._ocr_for_single_line(crop_patch, 'general')
+            if part_res['text']:
+                box['position'] = list2box(*box['position'])
+                box['text'] = part_res['text']
+                outs.append(box)
 
         outs = sort_boxes(outs, key='position')
         logger.debug(outs)
+        outs = self._post_process(outs)
 
+        outs = list(chain(*outs))
         if kwargs.get('save_analysis_res'):
             save_layout_img(
                 img0,
-                ('isolated', 'text', 'text-embed'),
+                ('text', 'isolated', 'embedding'),
                 outs,
                 kwargs.get('save_analysis_res'),
             )
 
         return outs
 
     @classmethod
+    def _post_process(cls, outs):
+        for line_boxes in outs:
+            if (
+                len(line_boxes) > 1
+                and line_boxes[-1]['type'] == 'text'
+                and line_boxes[-2]['type'] != 'text'
+            ):
+                if line_boxes[-1]['text'].lower() == 'o':
+                    line_boxes[-1]['text'] = '。'
+        return outs
+
+    @classmethod
     def _split_line_image(cls, line_box, embed_mfs):
         # 利用embedding formula所在位置，把单行文字图片切割成多个小段，之后这些小段会分别扔进OCR进行文字识别
         line_box = line_box[0]
         if not embed_mfs:
             return [{'position': line_box.int().tolist(), 'type': 'text'}]
         embed_mfs.sort(key=lambda x: x['position'][0])
 
         outs = []
         start = int(line_box[0])
         xmax, ymin, ymax = int(line_box[2]), int(line_box[1]), int(line_box[-1])
         for mf in embed_mfs:
             _xmax = min(xmax, int(mf['position'][0]) + 1)
             if start + 8 < _xmax:
                 outs.append({'position': [start, ymin, _xmax, ymax], 'type': 'text'})
-            outs.append(mf)
             start = int(mf['position'][2])
         if start < xmax:
             outs.append({'position': [start, ymin, xmax, ymax], 'type': 'text'})
         return outs
 
     def recognize_by_layout(
         self, img: Union[str, Path, Image.Image], **kwargs
@@ -471,18 +484,17 @@
             )
 
         return out
 
     def _ocr_for_single_line(self, image, image_type):
         ocr_model = self.english_ocr if image_type == 'english' else self.general_ocr
         try:
-            result = ocr_model.ocr_for_single_line(image)
+            return ocr_model.ocr_for_single_line(image)
         except:
-            return ''
-        return result['text']
+            return {'text': '', 'score': 0.0}
 
     def _ocr(self, image, image_type):
         ocr_model = self.english_ocr if image_type == 'english' else self.general_ocr
         result = ocr_model.ocr(image)
         texts = [_one['text'] for _one in result]
         result = '\n'.join(texts)
         return result
```

### Comparing `pix2text-0.2.2.1/pix2text/render.py` & `pix2text-0.2.3/pix2text/render.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.2.1/pix2text/screenshot_daemon_with_server2.py` & `pix2text-0.2.3/pix2text/screenshot_daemon_with_server2.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.2.1/pix2text/serve.py` & `pix2text-0.2.3/pix2text/serve.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,28 +37,29 @@
     return {"message": "Welcome to Pix2Text Server!"}
 
 
 @app.post("/pix2text")
 async def ocr(
     image: UploadFile,
     use_analyzer: str = Form(default=True),
-    resized_shape: str = Form(default=600),
+    resized_shape: str = Form(default=608),
     embed_sep: str = Form(default=' $,$ '),
     isolated_sep: str = Form(default='$$\n, \n$$'),
 ) -> Dict[str, Any]:
     # curl 调用方式：
     # $ curl -F image=@docs/examples/english.jpg --form 'use_analyzer=false' --form 'resized_shape=700' \
     #       http://0.0.0.0:8503/pix2text
     image = image.file
     image = read_img(image, return_type='Image')
     embed_sep = embed_sep.split(',')
     isolated_sep = isolated_sep.split(',')
+    use_analyzer = use_analyzer.lower() != 'false' if isinstance(use_analyzer, str) else use_analyzer
 
     params = dict(
-        use_analyzer=use_analyzer.lower() != 'false', resized_shape=int(resized_shape),
+        use_analyzer=use_analyzer, resized_shape=int(resized_shape),
     )
     if len(embed_sep) == 2:
         params['embed_sep'] = embed_sep
     if len(isolated_sep) == 2:
         params['isolated_sep'] = isolated_sep
 
     logger.info(f'input {params=}')
```

### Comparing `pix2text-0.2.2.1/pix2text.egg-info/PKG-INFO` & `pix2text-0.2.3/pix2text.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,570 +1,646 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 0.2.2.1
-Summary: Python3 package to extract text information from images
+Version: 0.2.3
+Summary: An open-source Python3 tool for Optical Character Recognition (OCR) and LaTeX expression extraction from images, a Free Alternative to Mathpix
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
-Description: <div align="center">
-          <img src="./docs/figs/p2t.jpg" width="250px"/>
-          <div>&nbsp;</div>
-        
-        [![Downloads](https://static.pepy.tech/personalized-badge/pix2text?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pix2text)
-        [![license](https://img.shields.io/github/license/breezedeus/pix2text)](./LICENSE)
-        [![PyPI version](https://badge.fury.io/py/pix2text.svg)](https://badge.fury.io/py/pix2text)
-        [![forks](https://img.shields.io/github/forks/breezedeus/pix2text)](https://github.com/breezedeus/pix2text)
-        [![stars](https://img.shields.io/github/stars/breezedeus/pix2text)](https://github.com/breezedeus/pix2text)
-        ![last-release](https://img.shields.io/github/release-date/breezedeus/pix2text)
-        ![last-commit](https://img.shields.io/github/last-commit/breezedeus/pix2text)
-        [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
-        
-        [👩🏻‍💻网页版](https://p2t.behye.com) |
-        [💬 交流群](https://cnocr.readthedocs.io/zh/latest/contact/)
-        
-        </div>
-        
-        <div align="center">
-        
-        [English](./README_en.md) | 中文
-        </div>
-        
-        # Pix2Text (P2T)
-        
-        
-        【Update 2023.02.10： **[P2T网页版](https://p2t.behye.com)** 开放免费使用】
-        
-        * P2T作为Python包，对于不熟悉Python的朋友还是太不友好，所以我们也开发了 [P2T网页版](https://p2t.behye.com)，可直接免费使用，欢迎帮忙推荐分享。
-        * 视频介绍：[Pix2Text 新版和网页版发布，离Mathpix又近了一大步_bilibili](https://www.bilibili.com/video/BV1U24y1q7n3) 。
-        * 文字版介绍：[Pix2Text (P2T) 新版发布，离Mathpix又近了一大步 - 知乎](https://zhuanlan.zhihu.com/p/604999678) 。
-        
-        【Update 2023.02.03：**V0.2** 发布】
-        
-        * 利用 **[CnSTD](https://github.com/breezedeus/cnstd)** 新版的**数学公式检测**（**Mathematical Formula Detection**，简称 **MFD**）能力，**P2T V0.2** 支持**识别既包含文字又包含公式的混合图片**。
-        
-        了解更多：[RELEASE.md](./RELEASE.md) 。
-        
-        ---
-        
-        
-        
-        **Pix2Text** 期望成为 **[Mathpix](https://mathpix.com/)** 的**免费开源 Python **替代工具，目前已经可以完成 **Mathpix** 的核心功能。**Pix2Text (P2T)** 自 **V0.2** 开始，支持识别**既包含文字又包含公式的混合图片**，返回效果类似于 **Mathpix**。P2T 的核心原理见下图（文字识别支持**中文**和**英文**）：
-        
-        <div align="center">
-          <img src="./docs/figs/arch-flow2.jpg" alt="Pix2Text流程" width="600px"/>
-        </div>
-        
-        
-        
-        **P2T** 使用开源工具  **[CnSTD](https://github.com/breezedeus/cnstd)** 检测出图片中**数学公式**所在位置，再交由 **[LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)** 识别出各对应位置数学公式的Latex表示。图片的剩余部分再交由 **[CnOCR](https://github.com/breezedeus/cnocr)** 进行文字检测和文字识别。最后 P2T 合并所有识别结果，获得最终的图片识别结果。感谢这些开源工具。
-        
-        
-        
-        P2T 作为Python3工具包，对于不熟悉Python的朋友不太友好，我们近期也会发布 **P2T网页版**，直接把图片丢进网页就能输出P2T的解析结果。
-        
-        网页版会提供一些**免费名额**供有需要的朋友使用，优先在校学生（**[MathPix](https://link.zhihu.com/?target=https%3A//mathpix.com/)** 每月要5美元，对在校生来说还是蛮贵的）。
-        
-        
-        
-        感兴趣的朋友欢迎扫码加小助手为好友，备注 `p2t`，小助手会定期统一邀请大家入群。群内会发布P2T相关工具的最新进展：
-        
-        <div align="center">
-          <img src="./docs/figs/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
-        </div>
-        
-        
-        
-        作者也维护 **知识星球** [**P2T/CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) ，这里面的提问会较快得到作者的回复，欢迎加入。**知识星球私享群**也会陆续发布一些P2T/CnOCR/CnSTD相关的私有资料，包括[**更详细的训练教程**](https://articles.zsxq.com/id_u6b4u0wrf46e.html)，**未公开的模型**，**不同应用场景的调用代码**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。
-        
-        
-        
-        ## 使用说明
-        
-        
-        调用很简单，以下是示例：
-        
-        ```python
-        from pix2text import Pix2Text
-        
-        img_fp = './docs/examples/formula.jpg'
-        p2t = Pix2Text(analyzer_config=dict(model_name='mfd'))
-        outs = p2t(img_fp, resized_shape=600)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
-        print(outs)
-        # 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
-        only_text = '\n'.join([out['text'] for out in outs])
-        ```
-        
-        
-        
-        返回结果 `out_text` 是个 `dict`，其中 key `position` 表示位置信息，`type` 表示类别信息，而 `text` 表示识别的结果。具体见下面的[接口说明](#接口说明)。
-        
-        
-        
-        ## 示例
-        
-        <table>
-        <tr>
-        <th> 图片 </th> 
-        <th> Pix2Text识别结果 </th>
-        </tr>
-        <tr>
-        <td>
-        <img src="./docs/examples/mixed.jpg" alt="mixed"> 
-        
-        </td>
-        <td>
-        
-        ```python
-        [{"position": array([[         22,          29],
-               [       1055,          29],
-               [       1055,          56],
-               [         22,          56]], dtype=float32),
-          "text": "JVAE的训练loss和VQ-VAE类似，只是使用了KL距离来让分布尽量分散",
-          "type": "text"},
-         {"position": array([[        629,         124],
-               [       1389,         124],
-               [       1389,         183],
-               [        629,         183]]),
-          "text": "$$\n"
-                  "-{\\cal E}_{z\\sim q(z|x)}[\\log(p(x\\mid z))]"
-                  "+{\\cal K}{\\cal L}(q(z\\mid x)||p(z))\n"
-                  "$$",
-          "type": "isolated"},
-         {"position": array([[         20,         248],
-               [       1297,         248],
-               [       1297,         275],
-               [         20,         275]], dtype=float32),
-          "text": "其中之利用 Gumbel-Softmax从 $z\\sim q(z|x)$ 中抽样得到，"
-          " $p(z)$ 是个等概率的多项式分布。",
-          "type": "text-embed"}]
-        ```
-        
-        </td>
-        </tr>
-        <tr>
-        <td>
-        
-        <img src="./docs/examples/formula.jpg" alt="formula"> 
-        </td>
-        <td>
-        
-        ```python
-        [{"position": array([[         12,          19],
-               [        749,          19],
-               [        749,         150],
-               [         12,         150]]),
-          "text": "$$\n"
-                  "\\mathcal{L}_{\\mathrm{eyelid}}~\\equiv~"
-                  "\\sum_{t=1}^{T}\\sum_{v=1}^{V}"
-                  "\\mathcal{N}_{U}^{\\mathrm{(eyelid)}}"
-                  "\\left(\\left|\\left|\\hat{h}_{t,v}\\,-\\,"
-                  "\\mathcal{x}_{t,v}\\right|\\right|^{2}\\right)\n"
-                  "$$",
-          "type": "isolated"}]
-        ```
-        </div>
-        </td>
-        </tr>
-        <tr>
-        <td>
-        
-         <img src="./docs/examples/english.jpg" alt="english"> 
-        </td>
-        <td>
-        
-        ```python
-        [{"position": array([[          0,           0],
-               [        710,           0],
-               [        710,         116],
-               [          0,         116]]),
-          "text": "python scripts/screenshot_daemon_with_server\n"
-                  "2-get_model:178usemodel:/Users/king/.cr\n"
-                  "enet_lite_136-fc-epoch=039-complete_match_er",
-          "type": "english"}]
-        ```
-        </td>
-        </tr>
-        <tr>
-        <td>
-        
-         <img src="./docs/examples/general.jpg" alt="general"  width="300px"> 
-        </td>
-        <td>
-        
-        ```python
-        [{"position": array([[          0,           0],
-               [        800,           0],
-               [        800,         800],
-               [          0,         800]]),
-          "text": "618\n开门红提前购\n很贵\n买贵返差"
-          "\n终于降价了\n100%桑蚕丝\n要买趁早\n今日下单188元\n仅限一天",
-          "type": "general"}]
-        ```
-        </td>
-        </tr>
-        </table>
-        
-        
-        
-        ## 模型下载
-        
-        安装好 Pix2Text 后，首次使用时系统会**自动下载** 模型文件，并存于 `~/.pix2text`目录（Windows下默认路径为 `C:\Users\<username>\AppData\Roaming\pix2text`）。
-        
-        
-        
-        > **Note**
-        >
-        > 如果已成功运行上面的示例，说明模型已完成自动下载，可忽略本节后续内容。
-        
-        
-        
-        对于**分类模型**，系统会自动下载模型`mobilenet_v2.zip`文件并对其解压，然后把解压后的模型相关目录放于`~/.pix2text`目录中。如果系统无法自动成功下载`mobilenet_v2.zip`文件，则需要手动从 **[cnstd-cnocr-models/pix2text](https://huggingface.co/breezedeus/cnstd-cnocr-models/tree/main/models/pix2text/0.2)** 下载此zip文件并把它放于 `~/.pix2text`目录。如果下载太慢，也可以从 [百度云盘](https://pan.baidu.com/s/1kubZF4JGE19d98NDoPHJzQ?pwd=p2t0) 下载， 提取码为 ` p2t0`。
-        
-        对于  **[LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)** ，系统同样会自动下载模型文件并把它们存放于`~/.pix2text/formula`目录中。如果系统无法自动成功下载这些模型文件，则需从  [百度云盘](https://pan.baidu.com/s/1kubZF4JGE19d98NDoPHJzQ?pwd=p2t0) 下载文件 `weights.pth` 和 `image_resizer.pth`， 并把它们存放于`~/.pix2text/formula`目录中；提取码为 ` p2t0`。
-        
-        
-        
-        ## 安装
-        
-        嗯，顺利的话一行命令即可。
-        
-        ```bash
-        pip install pix2text
-        ```
-        
-        安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
-        
-        ```bash
-        pip install pix2text -i https://pypi.doubanio.com/simple
-        ```
-        
-        
-        
-        如果是初次使用**OpenCV**，那估计安装都不会很顺利，bless。
-        
-        **Pix2Text** 主要依赖 [**CnSTD>=1.2.1**](https://github.com/breezedeus/cnstd)、[**CnOCR>=2.2.2.1**](https://github.com/breezedeus/cnocr) ，以及 [**LaTeX-OCR**](https://github.com/lukas-blecher/LaTeX-OCR) 。如果安装过程遇到问题，也可参考它们的安装说明文档。
-        
-        
-        
-        > **Warning** 
-        >
-        > 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到不少问题，但一般都是常见问题，可以自行百度/Google解决。
-        
-        
-        
-        ## 接口说明
-        
-        ### 类初始化
-        
-        主类为 [**Pix2Text**](pix2text/pix_to_text.py) ，其初始化函数如下：
-        
-        ```python
-        class Pix2Text(object):
-        
-            def __init__(
-                self,
-                *,
-                analyzer_config: Dict[str, Any] = None,
-                clf_config: Dict[str, Any] = None,
-                general_config: Dict[str, Any] = None,
-                english_config: Dict[str, Any] = None,
-                formula_config: Dict[str, Any] = None,
-                thresholds: Dict[str, Any] = None,
-                device: str = 'cpu',  # ['cpu', 'cuda', 'gpu']
-                **kwargs,
-            ):
-        ```
-        
-        其中的各参数说明如下：
-        * `analyzer_config` (dict): 分类模型对应的配置信息；默认为 `None`，表示使用默认配置（使用**MFD** Analyzer）：
-        	
-          ```python
-          {
-                'model_name': 'mfd'  # 可以取值为 'mfd'（MFD），或者 'layout'（版面分析）
-        	}
-        	```
-        	
-        * `clf_config` (dict): 分类模型对应的配置信息；默认为 `None`，表示使用默认配置：
-        	```python
-          {
-                'base_model_name': 'mobilenet_v2',
-                'categories': IMAGE_TYPES,
-                'transform_configs': {
-                    'crop_size': [150, 450],
-                    'resize_size': 160,
-                    'resize_max_size': 1000,
-                },
-                'model_dir': Path(data_dir()) / 'clf',
-                'model_fp': None  # 如果指定，直接使用此模型文件
-          }
-        	```
-        	
-        * `general_config` (dict): 通用模型对应的配置信息；默认为 `None`，表示使用默认配置：
-        
-          ```python
-          {}
-          ```
-        
-        * `english_config` (dict): 英文模型对应的配置信息；默认为 `None`，表示使用默认配置：
-        
-          ```py
-          {'det_model_name': 'en_PP-OCRv3_det', 'rec_model_name': 'en_PP-OCRv3'}
-          ```
-        
-        * `formula_config` (dict): 公式识别模型对应的配置信息；默认为 `None`，表示使用默认配置：
-        
-          ```python
-          {
-              'config': LATEX_CONFIG_FP,
-              'checkpoint': Path(data_dir()) / 'formular' / 'weights.pth',
-              'no_resize': False
-          }
-          ```
-        
-        * `thresholds` (dict): 识别阈值对应的配置信息；默认为 `None`，表示使用默认配置：
-        
-          ```py
-          {
-              'formula2general': 0.65,  # 如果识别为 `formula` 类型，但得分小于此阈值，则改为 `general` 类型
-              'english2general': 0.75,  # 如果识别为 `english` 类型，但得分小于此阈值，则改为 `general` 类型
-          }
-          ```
-        
-        * `device` (str): 使用什么资源进行计算，支持 `['cpu', 'cuda', 'gpu']`；默认为 `cpu`
-        
-        * `**kwargs` (): 预留的其他参数；目前未被使用
-        
-        
-        
-        ### 识别类函数
-        
-        通过调用类 **`Pix2Text`** 的类函数 `.recognize()` 完成对指定图片进行识别。类函数 `.recognize()` 说明如下：
-        
-        ```python
-            def recognize(
-                self, img: Union[str, Path, Image.Image], use_analyzer: bool = True, **kwargs
-            ) -> List[Dict[str, Any]]:
-        ```
-        
-        
-        
-        其中的输入参数说明如下：
-        
-        * `img` (`str` or `Image.Image`)：待识别图片的路径，或者利用 `Image.open()` 已读入的图片 `Image` 。
-        * `use_analyzer` (`bool`)：是否使用 Analyzer (**MFD** or **Layout**); `False` 表示把图片看成纯文本或者纯图片处理，相当于 **P2T V0.1.*** 的效果。Default: `True`。
-        * `kwargs`: 保留字段，可以包含以下值，
-          * `resized_shape` (`int`): 把图片宽度resize到此大小再进行处理；默认值为 `700`；
-          * `save_analysis_res` (`str`): 把解析结果图片存在此文件中；默认值为 `None`，表示不存储；
-          * `embed_sep` (`tuple`): embedding latex的前后缀；只针对使用 `MFD` 时才有效；默认值为 `(' $', '$ ')`；
-          * `isolated_sep` (`tuple`): isolated latex的前后缀；只针对使用 `MFD` 时才有效；默认值为 `('$$\n', '\n$$')`。
-        
-        
-        
-        返回结果为列表（`list`），列表中的每个元素为`dict`，包含如下 `key`：
-        
-        * `type`：识别出的图像类别；
-          * 当开启Analyzer时（`use_analyzer==True`），取值为 `text`（纯文本）、`isolated`（独立行的数学公式） 或者 `text-embed`（文本行中包含了嵌入式的数学公式）；
-          * 当未开启Analyzer时（`use_analyzer==False`），取值为`formula`（纯数学公式）、`english`（纯英文文字）、`general`（纯文字，可能包含中英文）；
-        
-        * `text`：识别出的文字或Latex表达式；
-        * `position`：所在块的位置信息，`np.ndarray`, with shape of `[4, 2]`。
-        
-        
-        
-        `Pix2Text` 类也实现了 `__call__()` 函数，其功能与 `.recognize()` 函数完全相同。所以才会有以下的调用方式：
-        
-        ```python
-        from pix2text import Pix2Text
-        
-        img_fp = './docs/examples/formula.jpg'
-        p2t = Pix2Text(analyzer_config=dict(model_name='mfd'))
-        outs = p2t(img_fp, resized_shape=600)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
-        print(outs)
-        # 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
-        only_text = '\n'.join([out['text'] for out in outs])
-        ```
-        
-        
-        
-        ## 脚本使用
-        
-        **P2T** 包含了以下命令行工具。
-        
-        
-        
-        ### 对单张图片或单个文件夹中的图片进行识别
-        
-        使用命令 **`p2t predict`** 预测单个文件或文件夹中所有图片，以下是使用说明：
-        
-        ```bash
-        $ p2t predict -h
-        Usage: p2t predict [OPTIONS]
-        
-          模型预测
-        
-        Options:
-          --use-analyzer / --no-use-analyzer
-                                          是否使用 MFD 或者版面分析 Analyzer  [default: use-
-                                          analyzer]
-          -a, --analyzer-name [mfd|layout]
-                                          使用哪个Analyzer，MFD还是版面分析  [default: mfd]
-          -t, --analyzer-type TEXT        Analyzer使用哪个模型，'yolov7_tiny' or 'yolov7'
-                                          [default: yolov7_tiny]
-          -d, --device TEXT               使用 `cpu` 还是 `gpu` 运行代码，也可指定为特定gpu，如`cuda:0`
-                                          [default: cpu]
-          --resized-shape INTEGER         把图片宽度resize到此大小再进行处理  [default: 600]
-          -i, --img-file-or-dir TEXT      输入图片的文件路径或者指定的文件夹  [required]
-          --save-analysis-res TEXT        把解析结果存储到此文件或目录中（如果'--img-file-or-
-                                          dir'为文件/文件夹，则'--save-analysis-
-                                          res'也应该是文件/文件夹）。取值为 `None` 表示不存储
-          -l, --log-level TEXT            Log Level, such as `INFO`, `DEBUG`
-                                          [default: INFO]
-          -h, --help                      Show this message and exit.
-        ```
-        
-        
-        
-        ## HTTP服务
-        
-         **Pix2Text** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
-        
-        ```bash
-        $ pip install pix2text[serve]
-        ```
-        
-        
-        
-        安装完成后，可以通过以下命令启动HTTP服务（**`-p`** 后面的数字是**端口**，可以根据需要自行调整）：
-        
-        ```bash
-        $ p2t serve -p 8503
-        ```
-        
-        
-        
-        `p2t serve` 命令使用说明：
-        
-        ```bash
-        $ p2t serve -h
-        Usage: p2t serve [OPTIONS]
-        
-          开启HTTP服务。
-        
-        Options:
-          -H, --host TEXT     server host  [default: 0.0.0.0]
-          -p, --port INTEGER  server port  [default: 8503]
-          --reload            whether to reload the server when the codes have been
-                              changed
-          -h, --help          Show this message and exit.
-        ```
-        
-        
-        
-        服务开启后，可以使用以下方式调用服务。
-        
-        
-        
-        ### 命令行
-        
-        比如待识别文件为 `docs/examples/mixed.jpg`，如下使用 `curl` 调用服务：
-        
-        ```bash
-        $ curl -F image=@docs/examples/mixed.jpg --form 'use_analyzer=true' --form 'resized_shape=600' http://0.0.0.0:8503/pix2text
-        ```
-        
-        
-        
-        ### Python
-        
-        使用如下方式调用服务，参考文件 [scripts/try_service.py](scripts/try_service.py)：
-        
-        ```python
-        import requests
-        
-        url = 'http://0.0.0.0:8503/pix2text'
-        
-        image_fp = 'docs/examples/mixed.jpg'
-        data = {
-            "use_analyzer": True,
-            "resized_shape": 600,
-            "embed_sep": " $,$ ",
-            "isolated_sep": "$$\n, \n$$"
-        }
-        files = {
-            "image": (image_fp, open(image_fp, 'rb'))
-        }
-        
-        r = requests.post(url, data=data, files=files)
-        
-        outs = r.json()['results']
-        only_text = '\n'.join([out['text'] for out in outs])
-        print(f'{only_text=}')
-        ```
-        
-        
-        
-        ### 其他语言
-        
-        请参照 `curl` 的调用方式自行实现。
-        
-        
-        
-        ## 脚本运行
-        
-        脚本 [scripts/screenshot_daemon.py](scripts/screenshot_daemon.py) 实现了自动对截屏图片调用 Pixe2Text 进行公式或者文字识别。这个功能是如何实现的呢？
-        
-        
-        
-        **以下是具体的运行流程（请先安装好 Pix2Text）：**
-        
-        1. 找一个喜欢的截屏软件，这个软件只要**支持把截屏图片存储在指定文件夹**即可。比如Mac下免费的 **Xnip** 就很好用。
-        
-        2. 除了安装Pix2Text外，还需要额外安装一个Python包 **pyperclip**，利用它把识别结果复制进系统的剪切板：
-        
-           ```bash
-           $ pip install pyperclip
-           ```
-        
-        3. 下载脚本文件 [scripts/screenshot_daemon.py](scripts/screenshot_daemon.py) 到本地，编辑此文件 `"SCREENSHOT_DIR"` 所在行（第 `17` 行），把路径改为你的截屏图片所存储的目录。
-        
-        4. 运行此脚本：
-        
-           ```bash
-           $ python scripts/screenshot_daemon.py
-           ```
-        
-        好了，现在就用你的截屏软件试试效果吧。截屏后的识别结果会写入电脑剪切板，直接 **Ctrl-V** / **Cmd-V** 即可粘贴使用。
-        
-        
-        
-        更详细使用介绍可参考视频：《[Pix2Text: 替代 Mathpix 的免费 Python 开源工具](https://www.bilibili.com/video/BV12e4y1871U)》。
-        
-        
-        
-        
-        ## 给作者来杯咖啡
-        
-        开源不易，如果此项目对您有帮助，可以考虑 [给作者加点油🥤，鼓鼓气💪🏻](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
-        
-        ---
-        
-        官方代码库：[https://github.com/breezedeus/pix2text](https://github.com/breezedeus/pix2text)。
-        
-        
 Platform: Mac
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
-Provides-Extra: serve
 Provides-Extra: dev
+Provides-Extra: serve
+License-File: LICENSE
+
+<div align="center">
+  <img src="./docs/figs/p2t.jpg" width="250px"/>
+  <div>&nbsp;</div>
+
+[![Downloads](https://static.pepy.tech/personalized-badge/pix2text?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pix2text)
+[![license](https://img.shields.io/github/license/breezedeus/pix2text)](./LICENSE)
+[![PyPI version](https://badge.fury.io/py/pix2text.svg)](https://badge.fury.io/py/pix2text)
+[![forks](https://img.shields.io/github/forks/breezedeus/pix2text)](https://github.com/breezedeus/pix2text)
+[![stars](https://img.shields.io/github/stars/breezedeus/pix2text)](https://github.com/breezedeus/pix2text)
+![last-release](https://img.shields.io/github/release-date/breezedeus/pix2text)
+![last-commit](https://img.shields.io/github/last-commit/breezedeus/pix2text)
+[![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
+
+[👩🏻‍💻网页版](https://p2t.behye.com) |
+[💬 交流群](https://cnocr.readthedocs.io/zh/latest/contact/)
+
+</div>
+
+<div align="center">
+
+[English](./README_en.md) | 中文
+</div>
+
+# Pix2Text (P2T)
+## Update 2023.07.03：发布 V0.2.3
+
+主要变更：
+* 训练了新的**公式识别模型**，供 **[P2T网页版](https://p2t.behye.com)** 使用。新模型精度更高，尤其对**手写公式**和**多行公式**类图片。具体参考：[Pix2Text 新版公式识别模型 | Breezedeus.com](https://www.breezedeus.com/article/p2t-mfd-20230702) 。
+* 优化了对检测出的boxes的排序逻辑，以及对混合图片的处理逻辑，使得最终识别效果更符合直觉。
+* 优化了识别结果的合并逻辑，自动判断是否该换行，是否分段。
+* 修复了模型文件自动下载的功能。HuggingFace似乎对下载文件的逻辑做了调整，导致之前版本的自动下载失败，当前版本已修复。但由于HuggingFace国内被墙，国内下载仍需 **梯子（VPN）**。
+* 更新了各个依赖包的版本号。
+
+## Update 2023.06.20：发布新版 MFD 模型
+
+主要变更：
+* 基于新标注的数据，重新训练了 **MFD YoloV7** 模型，目前新模型已部署到 [P2T网页版](https://p2t.behye.com) 。具体说明见：[Pix2Text (P2T) 新版公式检测模型 | Breezedeus.com](https://www.breezedeus.com/article/p2t-mfd-20230613) 。
+* 之前的 MFD YoloV7 模型已开放给星球会员下载，具体说明见：[P2T YoloV7 数学公式检测模型开放给星球会员下载 | Breezedeus.com](https://www.breezedeus.com/article/p2t-yolov7-for-zsxq-20230619) 。
+
+## Update 2023.02.10： **[P2T网页版](https://p2t.behye.com)** 开放免费使用
+
+* P2T作为Python包，对于不熟悉Python的朋友还是太不友好，所以我们也开发了 [P2T网页版](https://p2t.behye.com)，可直接免费使用，欢迎帮忙推荐分享。
+* 视频介绍：[Pix2Text 新版和网页版发布，离Mathpix又近了一大步_bilibili](https://www.bilibili.com/video/BV1U24y1q7n3) 。
+* 文字版介绍：[Pix2Text (P2T) 新版发布，离Mathpix又近了一大步 - 知乎](https://zhuanlan.zhihu.com/p/604999678) 。
+
+
+了解更多：[RELEASE.md](./RELEASE.md) 。
+
+---
+
+
+
+**Pix2Text** 期望成为 **[Mathpix](https://mathpix.com/)** 的**免费开源 Python **替代工具，目前已经可以完成 **Mathpix** 的核心功能。**Pix2Text (P2T)** 自 **V0.2** 开始，支持识别**既包含文字又包含公式的混合图片**，返回效果类似于 **Mathpix**。P2T 的核心原理见下图（文字识别支持**中文**和**英文**）：
+
+<div align="center">
+  <img src="./docs/figs/arch-flow2.jpg" alt="Pix2Text流程" width="600px"/>
+</div>
+
+
+
+**P2T** 使用开源工具  **[CnSTD](https://github.com/breezedeus/cnstd)** 检测出图片中**数学公式**所在位置，再交由 **[LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)** 识别出各对应位置数学公式的Latex表示。图片的剩余部分再交由 **[CnOCR](https://github.com/breezedeus/cnocr)** 进行文字检测和文字识别。最后 P2T 合并所有识别结果，获得最终的图片识别结果。感谢这些开源工具。
+
+
+
+P2T 作为Python3工具包，对于不熟悉Python的朋友不太友好，所以我们也发布了**可免费使用**的 **[P2T网页版](https://p2t.behye.com)**，直接把图片丢进网页就能输出P2T的解析结果。**网页版会使用最新的模型，效果会比开源模型更好。**
+
+
+
+感兴趣的朋友欢迎扫码加小助手为好友，备注 `p2t`，小助手会定期统一邀请大家入群。群内会发布P2T相关工具的最新进展：
+
+<div align="center">
+  <img src="./docs/figs/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
+</div>
+
+
+
+作者也维护 **知识星球** [**P2T/CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) ，这里面的提问会较快得到作者的回复，欢迎加入。**知识星球私享群**也会陆续发布一些P2T/CnOCR/CnSTD相关的私有资料，包括[**更详细的训练教程**](https://articles.zsxq.com/id_u6b4u0wrf46e.html)，**部分未公开的模型**，**购买付费模型享优惠**，**不同应用场景的调用代码**，使用过程中遇到的难题解答等。星球也会发布P2T/OCR/STD相关的最新研究资料。
+
+
+
+## 使用说明
+
+
+调用很简单，以下是示例：
+
+```python
+from pix2text import Pix2Text, merge_line_texts
+
+img_fp = './docs/examples/formula.jpg'
+p2t = Pix2Text(analyzer_config=dict(model_name='mfd'))
+outs = p2t(img_fp, resized_shape=600)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
+print(outs)
+# 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
+only_text = merge_line_texts(outs, auto_line_break=True)
+print(only_text)
+```
+
+
+
+返回结果 `outs` 是个 `dict`，其中 key `position` 表示Box位置信息，`type` 表示类别信息，而 `text` 表示识别的结果。具体见下面的[接口说明](#接口说明)。
+
+
+
+## 示例
+
+<table>
+<tr>
+<th> 图片 </th> 
+<th> Pix2Text识别结果 </th>
+</tr>
+<tr>
+<td>
+<img src="./docs/examples/mixed.jpg" alt="mixed"> 
+
+</td>
+<td>
+
+```python
+[{'line_number': 0,
+  'position': array([[         22,          31],
+       [       1057,          31],
+       [       1057,          58],
+       [         22,          58]]),
+  'text': 'JVAE的训练loss和VQ-VAE类似，只是使用了KL距离来让分布尽量分散',
+  'type': 'text'},
+ {'line_number': 1,
+  'position': array([[        625,         121],
+       [       1388,         121],
+       [       1388,         182],
+       [        625,         182]]),
+  'text': '$$\n'
+          '-E_{z\\sim q(z\\mid x)}[\\log(p(x\\mid z))]+K L(q(z\\mid x))|p(z))\n'
+          '$$',
+  'type': 'isolated'},
+ {'line_number': 2,
+  'position': array([[         18,         242],
+       [        470,         242],
+       [        470,         275],
+       [         18,         275]]),
+  'text': '其中之利用 Gumbel-Softmax 人',
+  'type': 'text'},
+ {'line_number': 2,
+  'position': array([[        481,         238],
+       [        664,         238],
+       [        664,         287],
+       [        481,         287]]),
+  'text': ' $z\\sim q(z|x)$ ',
+  'type': 'embedding'},
+ {'line_number': 2,
+  'position': array([[        667,         244],
+       [        840,         244],
+       [        840,         277],
+       [        667,         277]]),
+  'text': '中抽样得到,',
+  'type': 'text'},
+ {'line_number': 2,
+  'position': array([[        852,         239],
+       [        932,         239],
+       [        932,         288],
+       [        852,         288]]),
+  'text': ' $\\scriptstyle{p(z)}$ ',
+  'type': 'embedding'},
+ {'line_number': 2,
+  'position': array([[        937,         244],
+       [       1299,         244],
+       [       1299,         277],
+       [        937,         277]]),
+  'text': '是个等概率的多项式分布',
+  'type': 'text'}]
+```
+
+</td>
+</tr>
+<tr>
+<td>
+
+<img src="./docs/examples/formula.jpg" alt="formula"> 
+</td>
+<td>
+
+```python
+[{"line_number": 0,
+  "position": array([[         12,          19],
+       [        749,          19],
+       [        749,         150],
+       [         12,         150]]),
+  "text": "$$\n"
+          "\\mathcal{L}_{\\mathrm{eyelid}}~\\equiv~"
+          "\\sum_{t=1}^{T}\\sum_{v=1}^{V}"
+          "\\mathcal{N}_{U}^{\\mathrm{(eyelid)}}"
+          "\\left(\\left|\\left|\\hat{h}_{t,v}\\,-\\,"
+          "\\mathcal{x}_{t,v}\\right|\\right|^{2}\\right)\n"
+          "$$",
+  "type": "isolated"}]
+```
+</div>
+</td>
+</tr>
+<tr>
+<td>
+
+ <img src="./docs/examples/english.jpg" alt="english"> 
+</td>
+<td>
+
+```python
+[{"position": array([[          0,           0],
+       [        710,           0],
+       [        710,         116],
+       [          0,         116]]),
+  "text": "python scripts/screenshot_daemon_with_server\n"
+          "2-get_model:178usemodel:/Users/king/.cr\n"
+          "enet_lite_136-fc-epoch=039-complete_match_er",
+  "type": "english"}]
+```
+</td>
+</tr>
+<tr>
+<td>
+
+ <img src="./docs/examples/general.jpg" alt="general"  width="300px"> 
+</td>
+<td>
+
+```python
+[{"position": array([[          0,           0],
+       [        800,           0],
+       [        800,         800],
+       [          0,         800]]),
+  "text": "618\n开门红提前购\n很贵\n买贵返差"
+  "\n终于降价了\n100%桑蚕丝\n要买趁早\n今日下单188元\n仅限一天",
+  "type": "general"}]
+```
+</td>
+</tr>
+</table>
+
+
+
+## 模型下载
+
+### 开源免费模型
+
+安装好 Pix2Text 后，首次使用时系统会**自动下载** 免费模型文件，并存于 `~/.pix2text`目录（Windows下默认路径为 `C:\Users\<username>\AppData\Roaming\pix2text`）。
+
+
+
+> **Note**
+>
+> 如果已成功运行上面的示例，说明模型已完成自动下载，可忽略本节后续内容。
+
+
+
+对于**分类模型**，系统会自动下载模型`mobilenet_v2.zip`文件并对其解压，然后把解压后的模型相关目录放于`~/.pix2text`目录中。如果系统无法自动成功下载`mobilenet_v2.zip`文件，则需要手动从 **[cnstd-cnocr-models/pix2text](https://huggingface.co/breezedeus/cnstd-cnocr-models/tree/main/models/pix2text/0.2)** 下载此zip文件并把它放于 `~/.pix2text`目录。如果下载太慢，也可以从 [百度云盘](https://pan.baidu.com/s/1kubZF4JGE19d98NDoPHJzQ?pwd=p2t0) 下载， 提取码为 ` p2t0`。
+
+对于  **[LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)** ，系统同样会自动下载模型文件并把它们存放于`~/.pix2text/formula`目录中。如果系统无法自动成功下载这些模型文件，则需从  [百度云盘](https://pan.baidu.com/s/1kubZF4JGE19d98NDoPHJzQ?pwd=p2t0) 下载文件 `weights.pth` 和 `image_resizer.pth`， 并把它们存放于`~/.pix2text/formula`目录中；提取码为 ` p2t0`。
+
+
+
+### 付费模型
+
+除了上面免费的开源模型，P2T 也训练了精度更高的数学公式检测和识别模型，这些模型供 **[P2T网页版](https://p2t.behye.com)** 使用，它们的效果也可以在网页版体验。这些模型不是免费的（抱歉开源作者也是要喝咖啡的），具体可参考 [Pix2Text (P2T) | Breezedeus.com](https://www.breezedeus.com/pix2text#259b04346dd94f45a65c10ff3db48540) 。
+
+
+
+## 安装
+
+嗯，顺利的话一行命令即可。
+
+```bash
+pip install pix2text
+```
+
+安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
+
+```bash
+pip install pix2text -i https://pypi.doubanio.com/simple
+```
+
+
+
+如果是初次使用**OpenCV**，那估计安装都不会很顺利，bless。
+
+**Pix2Text** 主要依赖 [**CnSTD>=1.2.1**](https://github.com/breezedeus/cnstd)、[**CnOCR>=2.2.2.1**](https://github.com/breezedeus/cnocr) ，以及 [**LaTeX-OCR**](https://github.com/lukas-blecher/LaTeX-OCR) 。如果安装过程遇到问题，也可参考它们的安装说明文档。
+
+
+
+> **Warning** 
+>
+> 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到不少问题，但一般都是常见问题，可以自行百度/Google解决。
+
+
+
+## 接口说明
+
+### 类初始化
+
+主类为 [**Pix2Text**](pix2text/pix_to_text.py) ，其初始化函数如下：
+
+```python
+class Pix2Text(object):
+
+    def __init__(
+        self,
+        *,
+        analyzer_config: Dict[str, Any] = None,
+        clf_config: Dict[str, Any] = None,
+        general_config: Dict[str, Any] = None,
+        english_config: Dict[str, Any] = None,
+        formula_config: Dict[str, Any] = None,
+        thresholds: Dict[str, Any] = None,
+        device: str = 'cpu',  # ['cpu', 'cuda', 'gpu']
+        **kwargs,
+    ):
+```
+
+其中的各参数说明如下：
+* `analyzer_config` (dict): 分类模型对应的配置信息；默认为 `None`，表示使用默认配置（使用**MFD** Analyzer）：
+	
+  ```python
+  {
+        'model_name': 'mfd'  # 可以取值为 'mfd'（MFD），或者 'layout'（版面分析）
+	}
+	```
+	
+* `clf_config` (dict): 分类模型对应的配置信息；默认为 `None`，表示使用默认配置：
+	```python
+  {
+        'base_model_name': 'mobilenet_v2',
+        'categories': IMAGE_TYPES,
+        'transform_configs': {
+            'crop_size': [150, 450],
+            'resize_size': 160,
+            'resize_max_size': 1000,
+        },
+        'model_dir': Path(data_dir()) / 'clf',
+        'model_fp': None  # 如果指定，直接使用此模型文件
+  }
+	```
+	
+* `general_config` (dict): 通用模型对应的配置信息；默认为 `None`，表示使用默认配置：
+
+  ```python
+  {}
+  ```
+
+* `english_config` (dict): 英文模型对应的配置信息；默认为 `None`，表示使用默认配置：
+
+  ```py
+  {'det_model_name': 'en_PP-OCRv3_det', 'rec_model_name': 'en_PP-OCRv3'}
+  ```
+
+* `formula_config` (dict): 公式识别模型对应的配置信息；默认为 `None`，表示使用默认配置：
+
+  ```python
+  {
+      'config': LATEX_CONFIG_FP,
+      'checkpoint': Path(data_dir()) / 'formula' / 'weights.pth',
+      'no_resize': False
+  }
+  ```
+
+* `thresholds` (dict): 识别阈值对应的配置信息；默认为 `None`，表示使用默认配置：
+
+  ```py
+  {
+      'formula2general': 0.65,  # 如果识别为 `formula` 类型，但得分小于此阈值，则改为 `general` 类型
+      'english2general': 0.75,  # 如果识别为 `english` 类型，但得分小于此阈值，则改为 `general` 类型
+  }
+  ```
+
+* `device` (str): 使用什么资源进行计算，支持 `['cpu', 'cuda', 'gpu']`；默认为 `cpu`
+
+* `**kwargs` (): 预留的其他参数；目前未被使用
+
+
+
+### 识别类函数
+
+通过调用类 **`Pix2Text`** 的类函数 `.recognize()` 完成对指定图片进行识别。类函数 `.recognize()` 说明如下：
+
+```python
+    def recognize(
+        self, img: Union[str, Path, Image.Image], use_analyzer: bool = True, **kwargs
+    ) -> List[Dict[str, Any]]:
+```
+
+
+
+其中的输入参数说明如下：
+
+* `img` (`str` or `Image.Image`)：待识别图片的路径，或者利用 `Image.open()` 已读入的图片 `Image` 。
+* `use_analyzer` (`bool`)：是否使用 Analyzer (**MFD** or **Layout**); `False` 表示把图片看成纯文本或者纯图片处理，相当于 **P2T V0.1.*** 的效果。Default: `True`。
+* `kwargs`: 保留字段，可以包含以下值，
+  * `resized_shape` (`int`): 把图片宽度resize到此大小再进行处理；默认值为 `700`；
+  * `save_analysis_res` (`str`): 把解析结果图片存在此文件中；默认值为 `None`，表示不存储；
+  * `embed_sep` (`tuple`): embedding latex的前后缀；只针对使用 `MFD` 时才有效；默认值为 `(' $', '$ ')`；
+  * `isolated_sep` (`tuple`): isolated latex的前后缀；只针对使用 `MFD` 时才有效；默认值为 `('$$\n', '\n$$')`。
+
+
+
+返回结果为列表（`list`），列表中的每个元素为`dict`，包含如下 `key`：
+
+* `type`：识别出的图像类别；
+  * 当开启Analyzer时（`use_analyzer==True`），取值为 `text`（纯文本）、`isolated`（独立行的数学公式） 或者 `embedding`（行内的数学公式）；
+  
+    >  Warning
+    > 对于 **MFD Analyzer** ，此取值从 P2T **v0.2.3** 开始与之前不同。
+  * 当未开启Analyzer时（`use_analyzer==False`），取值为`formula`（纯数学公式）、`english`（纯英文文字）、`general`（纯文字，可能包含中英文）；
+  
+* `text`：识别出的文字或Latex表达式；
+* `position`：所在块的位置信息，`np.ndarray`, with shape of `[4, 2]`；
+* `line_number`：仅在使用 **MFD Analyzer** 时，才会包含此字段。此字段为 Box 所在的行号（第一行 **`line_number=0`**），值相同的 Box 表示它们在同一行。
+
+  > Warning
+  > 此取值从 P2T **v0.2.3** 开始才有，之前版本没有此 `key`。
+
+
+
+`Pix2Text` 类也实现了 `__call__()` 函数，其功能与 `.recognize()` 函数完全相同。所以才会有以下的调用方式：
+
+```python
+from pix2text import Pix2Text, merge_line_texts
+
+img_fp = './docs/examples/formula.jpg'
+p2t = Pix2Text(analyzer_config=dict(model_name='mfd'))
+outs = p2t(img_fp, resized_shape=608)  # 也可以使用 `p2t.recognize(img_fp)` 获得相同的结果
+print(outs)
+# 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
+only_text = merge_line_texts(outs, auto_line_break=True)
+print(only_text)
+```
+
+
+
+## 脚本使用
+
+**P2T** 包含了以下命令行工具。
+
+
+
+### 对单张图片或单个文件夹中的图片进行识别
+
+使用命令 **`p2t predict`** 预测单张图片或文件夹中所有图片，以下是使用说明：
+
+```bash
+$ p2t predict -h
+Usage: p2t predict [OPTIONS]
+
+  模型预测
+
+Options:
+  --use-analyzer / --no-use-analyzer
+                                  是否使用 MFD 或者版面分析 Analyzer  [default: use-
+                                  analyzer]
+  -a, --analyzer-name [mfd|layout]
+                                  使用哪个Analyzer，MFD还是版面分析  [default: mfd]
+  -t, --analyzer-type TEXT        Analyzer使用哪个模型，'yolov7_tiny' or 'yolov7'
+                                  [default: yolov7_tiny]
+  --analyzer-model-fp TEXT        Analyzer检测模型的文件路径。Default：`None`，表示使用默认模型
+  --latex-ocr-model-fp TEXT       Latex-OCR
+                                  数学公式识别模型的文件路径。Default：`None`，表示使用默认模型
+  -d, --device TEXT               使用 `cpu` 还是 `gpu` 运行代码，也可指定为特定gpu，如`cuda:0`
+                                  [default: cpu]
+  --resized-shape INTEGER         把图片宽度resize到此大小再进行处理  [default: 608]
+  -i, --img-file-or-dir TEXT      输入图片的文件路径或者指定的文件夹  [required]
+  --save-analysis-res TEXT        把解析结果存储到此文件或目录中（如果'--img-file-or-
+                                  dir'为文件/文件夹，则'--save-analysis-
+                                  res'也应该是文件/文件夹）。取值为 `None` 表示不存储
+  -l, --log-level TEXT            Log Level, such as `INFO`, `DEBUG`
+                                  [default: INFO]
+  -h, --help                      Show this message and exit.
+```
+
+
+
+此命令可用于**打印对指定图片的检测和识别结果**，如运行：
+
+```bash
+$ p2t predict --use-analyzer -a mfd --resized-shape 608 -i docs/examples/en1.jpg --save-analysis-res output-en1.jpg
+```
+
+上面命令打印出识别结果，同时会把检测结果存储在 `output-en1.jpg` 文件中，类似以下效果：
+
+
+<div align="center">
+  <img src="./docs/figs/output-en1.jpg" alt="P2T 数学公式检测效果图" width="600px"/>
+</div>
+
+
+## HTTP服务
+
+ **Pix2Text** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
+
+```bash
+$ pip install pix2text[serve]
+```
+
+
+
+安装完成后，可以通过以下命令启动HTTP服务（**`-p`** 后面的数字是**端口**，可以根据需要自行调整）：
+
+```bash
+$ p2t serve -p 8503
+```
+
+
+
+`p2t serve` 命令使用说明：
+
+```bash
+$ p2t serve -h
+Usage: p2t serve [OPTIONS]
+
+  开启HTTP服务。
+
+Options:
+  -H, --host TEXT     server host  [default: 0.0.0.0]
+  -p, --port INTEGER  server port  [default: 8503]
+  --reload            whether to reload the server when the codes have been
+                      changed
+  -h, --help          Show this message and exit.
+```
+
+
+
+服务开启后，可以使用以下方式调用服务。
+
+
+
+### 命令行
+
+比如待识别文件为 `docs/examples/mixed.jpg`，如下使用 `curl` 调用服务：
+
+```bash
+$ curl -F image=@docs/examples/mixed.jpg --form 'use_analyzer=true' --form 'resized_shape=600' http://0.0.0.0:8503/pix2text
+```
+
+
+
+### Python
+
+使用如下方式调用服务，参考文件 [scripts/try_service.py](scripts/try_service.py)：
+
+```python
+import requests
+
+url = 'http://0.0.0.0:8503/pix2text'
+
+image_fp = 'docs/examples/mixed.jpg'
+data = {
+    "use_analyzer": True,
+    "resized_shape": 608,
+    "embed_sep": " $,$ ",
+    "isolated_sep": "$$\n, \n$$"
+}
+files = {
+    "image": (image_fp, open(image_fp, 'rb'))
+}
+
+r = requests.post(url, data=data, files=files)
+
+outs = r.json()['results']
+only_text = '\n'.join([out['text'] for out in outs])
+print(f'{only_text=}')
+```
+
+
+
+### 其他语言
+
+请参照 `curl` 的调用方式自行实现。
+
+
+
+## 脚本运行
+
+脚本 [scripts/screenshot_daemon.py](scripts/screenshot_daemon.py) 实现了自动对截屏图片调用 Pixe2Text 进行公式或者文字识别。这个功能是如何实现的呢？
+
+
+
+**以下是具体的运行流程（请先安装好 Pix2Text）：**
+
+1. 找一个喜欢的截屏软件，这个软件只要**支持把截屏图片存储在指定文件夹**即可。比如Mac下免费的 **Xnip** 就很好用。
+
+2. 除了安装Pix2Text外，还需要额外安装一个Python包 **pyperclip**，利用它把识别结果复制进系统的剪切板：
+
+   ```bash
+   $ pip install pyperclip
+   ```
+
+3. 下载脚本文件 [scripts/screenshot_daemon.py](scripts/screenshot_daemon.py) 到本地，编辑此文件 `"SCREENSHOT_DIR"` 所在行（第 `17` 行），把路径改为你的截屏图片所存储的目录。
+
+4. 运行此脚本：
+
+   ```bash
+   $ python scripts/screenshot_daemon.py
+   ```
+
+好了，现在就用你的截屏软件试试效果吧。截屏后的识别结果会写入电脑剪切板，直接 **Ctrl-V** / **Cmd-V** 即可粘贴使用。
+
+
+
+更详细使用介绍可参考视频：《[Pix2Text: 替代 Mathpix 的免费 Python 开源工具](https://www.bilibili.com/video/BV12e4y1871U)》。
+
+
+
+
+## 给作者来杯咖啡
+
+开源不易，如果此项目对您有帮助，可以考虑 [给作者加点油🥤，鼓鼓气💪🏻](https://www.breezedeus.com/buy-me-coffee) 。
+
+---
+
+官方代码库：[https://github.com/breezedeus/pix2text](https://github.com/breezedeus/pix2text) 。
+
+Pix2Text (P2T) 更多信息：[https://www.breezedeus.com/pix2text](https://www.breezedeus.com/pix2text) 。
+
```

### Comparing `pix2text-0.2.2.1/pix2text.egg-info/SOURCES.txt` & `pix2text-0.2.3/pix2text.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 pix2text/__init__.py
 pix2text/__version__.py
 pix2text/app.py
 pix2text/category_mapping.py
 pix2text/cli.py
@@ -18,11 +19,17 @@
 pix2text.egg-info/SOURCES.txt
 pix2text.egg-info/dependency_links.txt
 pix2text.egg-info/entry_points.txt
 pix2text.egg-info/not-zip-safe
 pix2text.egg-info/requires.txt
 pix2text.egg-info/top_level.txt
 scripts/__init__.py
+scripts/convert_label_studio_to_yolov7.py
+scripts/gen_label_studio_json.py
+scripts/gen_pure_formula_to_yolov7.py
+scripts/merge_label_studio_anno_pred_json.py
 scripts/object_detection3.py
 scripts/screenshot_daemon.py
 scripts/try_layout.py
-scripts/try_service.py
+scripts/try_service.py
+tests/test_pix2text.py
+tests/test_sort_boxes.py
```

### Comparing `pix2text-0.2.2.1/scripts/object_detection3.py` & `pix2text-0.2.3/scripts/object_detection3.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.2.1/scripts/screenshot_daemon.py` & `pix2text-0.2.3/scripts/screenshot_daemon.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import os
 import time
 import glob
 
 import pyperclip as pc
 
-from pix2text import set_logger, Pix2Text, render_html
+from pix2text import set_logger, Pix2Text, merge_line_texts, render_html
 
 logger = set_logger(log_level='DEBUG')
 
 SCREENSHOT_DIR = os.getenv(
     "SCREENSHOT_DIR", '/Users/king/Pictures/screenshot_from_xnip'
 )
 
@@ -63,15 +63,15 @@
         return res[0]['type'], res[0]['text']
     elif len(res) > 1:
         box_types = set([info['type'] for info in res])
         if len(box_types) > 1:
             image_type = 'hybrid'
         else:
             image_type = list(box_types)[0]
-        text = '\n'.join([info['text'] for info in res])
+        text = merge_line_texts(res, auto_line_break=True)
 
         return image_type, text
 
     return 'general', ''
 
 
 if __name__ == '__main__':
```

### Comparing `pix2text-0.2.2.1/scripts/try_layout.py` & `pix2text-0.2.3/scripts/try_layout.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.2.1/scripts/try_service.py` & `pix2text-0.2.3/scripts/try_service.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.2.1/setup.py` & `pix2text-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # coding: utf-8
-# Copyright (C) 2022, [Breezedeus](https://github.com/breezedeus).
+# Copyright (C) 2022-2023, [Breezedeus](https://www.breezedeus.com).
 
 import os
 from setuptools import find_packages, setup
 from pathlib import Path
 
 PACKAGE_NAME = "pix2text"
 
@@ -19,18 +19,18 @@
     ),
     about,
 )
 
 required = [
     "click",
     "tqdm",
-    "numpy<1.24",
+    "numpy",
     "opencv-python",
-    "cnocr>=2.2.2.2",
-    "cnstd>=1.2.2",
+    "cnocr>=2.2.3.1",
+    "cnstd>=1.2.3.2",
     "torch",
     "torchvision",
     "pix2tex",
 ]
 extras_require = {
     "dev": ["pip-tools", "pytest"],
     "serve": ["uvicorn[standard]", "fastapi", "python-multipart", "pydantic"],
@@ -40,43 +40,38 @@
 [console_scripts]
 p2t = pix2text.cli:cli
 """
 
 setup(
     name=PACKAGE_NAME,
     version=about['__version__'],
-    description="Python3 package to extract text information from images",
+    description="An open-source Python3 tool for Optical Character Recognition (OCR) "
+    "and LaTeX expression extraction from images, a Free Alternative to Mathpix",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='breezedeus',
     author_email='breezedeus@163.com',
     license='MIT',
     url='https://github.com/breezedeus/pix2text',
     platforms=["Mac", "Linux", "Windows"],
     packages=find_packages(),
     include_package_data=True,
-    data_files=[
-        (
-            '',
-            [
-                'pix2text/latex_config.yaml',
-            ],
-        )
-    ],
+    data_files=[('', ['pix2text/latex_config.yaml',],)],
     entry_points=entry_points,
     install_requires=required,
     extras_require=extras_require,
     zip_safe=False,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
 )
```

