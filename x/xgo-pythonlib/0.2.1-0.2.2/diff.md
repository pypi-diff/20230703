# Comparing `tmp/xgo-pythonlib-0.2.1.tar.gz` & `tmp/xgo-pythonlib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.2.1.tar", last modified: Sun Jul  2 10:40:47 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.2.2.tar", last modified: Mon Jul  3 08:00:16 2023, max compression
```

## Comparing `xgo-pythonlib-0.2.1.tar` & `xgo-pythonlib-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 10:40:47.061341 xgo-pythonlib-0.2.1/
--rw-rw-rw-   0        0        0     2337 2023-07-02 10:40:47.059836 xgo-pythonlib-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1710 2023-07-02 10:39:24.000000 xgo-pythonlib-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-02 10:40:47.061341 xgo-pythonlib-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     3744 2023-07-02 10:40:40.000000 xgo-pythonlib-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 10:40:47.051523 xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     2337 2023-07-02 10:40:46.000000 xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-02 10:40:46.000000 xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 10:40:46.000000 xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-02 10:40:46.000000 xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 10:40:47.052829 xgo-pythonlib-0.2.1/xgoedu/
--rw-rw-rw-   0        0        0    46584 2023-07-02 10:39:06.000000 xgo-pythonlib-0.2.1/xgoedu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 10:40:47.053836 xgo-pythonlib-0.2.1/xgolib/
--rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.2.1/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 10:40:47.058835 xgo-pythonlib-0.2.1/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.2.1/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.2.1/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.2.1/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:00:16.830679 xgo-pythonlib-0.2.2/
+-rw-rw-rw-   0        0        0     2337 2023-07-03 08:00:16.829679 xgo-pythonlib-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1710 2023-07-02 10:39:24.000000 xgo-pythonlib-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 08:00:16.830679 xgo-pythonlib-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     3744 2023-07-03 07:59:45.000000 xgo-pythonlib-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:00:16.819880 xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     2337 2023-07-03 08:00:16.000000 xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-03 08:00:16.000000 xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 08:00:16.000000 xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-03 08:00:16.000000 xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 08:00:16.820893 xgo-pythonlib-0.2.2/xgoedu/
+-rw-rw-rw-   0        0        0    47784 2023-07-03 07:59:25.000000 xgo-pythonlib-0.2.2/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:00:16.822894 xgo-pythonlib-0.2.2/xgolib/
+-rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.2.2/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:00:16.828678 xgo-pythonlib-0.2.2/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.2.2/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.2.2/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.2.2/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.2.1/PKG-INFO` & `xgo-pythonlib-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.2.1
+Version: 0.2.2
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xgo-pythonlib-0.2.1/README.md` & `xgo-pythonlib-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.1/setup.py` & `xgo-pythonlib-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.2.1
+Version: 0.2.2
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xgo-pythonlib-0.2.1/xgoedu/__init__.py` & `xgo-pythonlib-0.2.2/xgoedu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import json
 import threading
 # from xgolib import XGO
 # from keras.preprocessing import image
 # import _thread  使用_thread会报错，坑！
 
 
-__versinon__ = '1.2.7'
-__last_modified__ = '2023/7/2'
+__versinon__ = '1.2.8'
+__last_modified__ = '2023/7/3'
 
 GPIO.setwarnings(False)
 GPIO.setmode(GPIO.BCM)
 
 camera_still=False
 
 
@@ -759,37 +759,52 @@
             if (IS_PY3):
                 result_str = str(result_str, 'utf-8')
             print("tts api  error:" + result_str)
 
         print("result saved as :" + save_file)
 
         self.xgoSpeaker("result.wav")
+
+    def cv2AddChineseText(self,img, text, position, textColor=(0, 255, 0), textSize=30):
+        if (isinstance(img, np.ndarray)):  
+            img = Image.fromarray(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
+        draw = ImageDraw.Draw(img)
+        fontStyle = ImageFont.truetype(
+            "/home/pi/model/msyh.ttc", textSize, encoding="utf-8")
+        draw.text(position, text, textColor, font=fontStyle)
+        return cv2.cvtColor(np.asarray(img), cv2.COLOR_RGB2BGR)
     
     def QRRecognition(self,target="camera"):
         import pyzbar.pyzbar as pyzbar
         if target=="camera":
-            self.xgoTakePhoto(filename="photo")
-            path="/home/pi/xgoPictures/photo.jpg"
-            img=cv2.imread(path)
+            self.open_camera()
+            success,img = self.cap.read()
         else:
-            img=cv2.imread("/home/pi/xgoPictures/"+target)
+            path="/home/pi/xgoPictures/"
+            img=np.array(Image.open(path+target))
+     
         barcodes = pyzbar.decode(img) 
         result=[]
         for barcode in barcodes:
             barcodeData = barcode.data.decode("utf-8")
             barcodeType = barcode.type
             result.append(barcodeData)
+            text = "{} ({})".format(barcodeData, barcodeType)
+            img=self.cv2AddChineseText(img,text, (10, 30),(0, 255, 0), 30)
         try:
             re=result[0]
         except:
             result=[]
-        self.xgoCamera(False)
+        b,g,r = cv2.split(img)
+        img = cv2.merge((r,g,b))
+        imgok = Image.fromarray(img)
+        self.display.ShowImage(imgok)
         return result
 
-    def ColorRecognitio(self,target="camera",mode='R'):
+    def ColorRecognition(self,target="camera",mode='R'):
         color_x = 0
         color_y = 0
         color_radius = 0
 
         if mode=='R':  #red
             color_lower = np.array([0, 43, 46])
             color_upper = np.array([10, 255, 255])
@@ -799,53 +814,64 @@
         elif mode=='B':   #blue
             color_lower = np.array([100, 43, 46])
             color_upper = np.array([124, 255, 255])
         elif mode=='Y':   #yellow
             color_lower = np.array([26, 43, 46])
             color_upper = np.array([34, 255, 255])
         if target=="camera":
-            self.xgoTakePhoto(filename="photo")
-            path="/home/pi/xgoPictures/photo.jpg"
-            img=cv2.imread(path)
-        else:
-            img=cv2.imread("/home/pi/xgoPictures/"+target)
-        frame_ = cv2.GaussianBlur(img,(5,5),0)                    
-        hsv = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
+            self.open_camera()
+            success,frame = self.cap.read()
+        else:
+            path="/home/pi/xgoPictures/"
+            frame=np.array(Image.open(path+target))
+        frame_ = cv2.GaussianBlur(frame,(5,5),0)                    
+        hsv = cv2.cvtColor(frame,cv2.COLOR_BGR2HSV)
         mask = cv2.inRange(hsv,color_lower,color_upper)  
         mask = cv2.erode(mask,None,iterations=2)
         mask = cv2.dilate(mask,None,iterations=2)
         mask = cv2.GaussianBlur(mask,(3,3),0)     
         cnts = cv2.findContours(mask.copy(),cv2.RETR_EXTERNAL,cv2.CHAIN_APPROX_SIMPLE)[-2] 
 
         if len(cnts) > 0:
             cnt = max (cnts, key = cv2.contourArea)
             (color_x,color_y),color_radius = cv2.minEnclosingCircle(cnt)
+            cv2.circle(frame,(int(color_x),int(color_y)),int(color_radius),(255,0,255),2)  
+        cv2.putText(frame, "X:%d, Y%d" % (int(color_x), int(color_y)), (40,40), cv2.FONT_HERSHEY_SIMPLEX, 0.8, (255,255,0), 3)
 
-        self.xgoCamera(False)
+        b,g,r = cv2.split(frame)
+        img = cv2.merge((r,g,b))
+        imgok = Image.fromarray(img)
+        self.display.ShowImage(imgok)
 
         return ((color_x,color_y),color_radius)
 
     def CircleRecognition(self,target="camera"):
         if target=="camera":
-            self.xgoTakePhoto(filename="photo")
-            path="/home/pi/xgoPictures/photo.jpg"
-            img = cv2.imread(path, cv2.IMREAD_GRAYSCALE)     # 0 转为灰度图像
-            #img2 = cv2.imread(path, cv2.IMREAD_COLOR)     # 1 为彩色图像
+            self.open_camera()
+            success,image = self.cap.read()
         else:
-            img=cv2.imread("/home/pi/xgoPictures/"+target,cv2.IMREAD_GRAYSCALE)
+            path="/home/pi/xgoPictures/"
+            image=np.array(Image.open(path+target))
+        img = cv2.cvtColor(image,cv2.COLOR_BGR2GRAY)
+        
         numpy_img = cv2.adaptiveThreshold(img, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY, 11, 15)   # 自动阈值二值化
         #                                                      圆心距 canny阈值    投票数      最小半径       最大半径
         circles = cv2.HoughCircles(img, cv2.HOUGH_GRADIENT, 1, 18,   param1=100, param2=80,  minRadius=40, maxRadius=150)
         arr1 = np.zeros([0, 2], dtype=int)                      # 创建一个0行, 2列的空数组
         re=[]
         if circles is not None:
             circles = np.uint16(np.around(circles))   
             for i in circles[0, :]:
                 re.append(((i[0], i[1]), i[2]))
-        self.xgoCamera(False)
+                cv2.circle(image, (i[0], i[1]), i[2], (0, 0, 255), 3)  # 轮廓
+                cv2.circle(image, (i[0], i[1]), 2, (0, 0, 0), 6)     # 圆心
+        b,g,r = cv2.split(image)
+        image = cv2.merge((r,g,b))
+        imgok = Image.fromarray(image)
+        self.display.ShowImage(imgok)
         return re
 
 
 
 
 
 class DemoError(Exception):
```

### Comparing `xgo-pythonlib-0.2.1/xgolib/__init__.py` & `xgo-pythonlib-0.2.2/xgolib/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.1/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.2.2/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.1/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.2.2/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

