# Comparing `tmp/openioe-0.1.3.tar.gz` & `tmp/openioe-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openioe-0.1.3.tar", last modified: Sun Sep  4 13:46:05 2022, max compression
+gzip compressed data, was "openioe-1.0.0.tar", last modified: Mon Jul  3 10:51:17 2023, max compression
```

## Comparing `openioe-0.1.3.tar` & `openioe-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-09-04 13:46:05.154947 openioe-0.1.3/
--rw-rw-rw-   0        0        0     6898 2022-09-04 13:46:05.154947 openioe-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5984 2022-09-04 13:42:29.000000 openioe-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2022-09-04 13:46:05.142908 openioe-0.1.3/openioe/
--rw-rw-rw-   0        0        0      100 2022-09-04 08:32:51.000000 openioe-0.1.3/openioe/__init__.py
--rw-rw-rw-   0        0        0     1719 2022-09-04 10:51:04.000000 openioe-0.1.3/openioe/openioe_apis.py
-drwxrwxrwx   0        0        0        0 2022-09-04 13:46:05.153026 openioe-0.1.3/openioe.egg-info/
--rw-rw-rw-   0        0        0     6898 2022-09-04 13:46:04.000000 openioe-0.1.3/openioe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2022-09-04 13:46:05.000000 openioe-0.1.3/openioe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-04 13:46:04.000000 openioe-0.1.3/openioe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-09-04 13:46:04.000000 openioe-0.1.3/openioe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-04 13:46:05.155910 openioe-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      702 2022-09-04 13:45:14.000000 openioe-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:51:17.344422 openioe-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2020-04-05 22:23:47.000000 openioe-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     9082 2023-07-03 10:51:17.344422 openioe-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8664 2023-07-03 10:43:13.000000 openioe-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 10:51:17.324428 openioe-1.0.0/openioe/
+-rw-rw-rw-   0        0        0      100 2022-09-04 08:32:51.000000 openioe-1.0.0/openioe/__init__.py
+-rw-rw-rw-   0        0        0     4747 2023-07-03 09:27:22.000000 openioe-1.0.0/openioe/openioe_apis.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:51:17.344422 openioe-1.0.0/openioe.egg-info/
+-rw-rw-rw-   0        0        0     9082 2023-07-03 10:51:17.000000 openioe-1.0.0/openioe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-03 10:51:17.000000 openioe-1.0.0/openioe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 10:51:17.000000 openioe-1.0.0/openioe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 10:51:17.000000 openioe-1.0.0/openioe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 10:51:17.344422 openioe-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-07-03 10:51:01.000000 openioe-1.0.0/setup.py
```

### Comparing `openioe-0.1.3/PKG-INFO` & `openioe-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,126 @@
-Metadata-Version: 2.1
-Name: openioe
-Version: 0.1.3
-Summary: Open IoE
-Home-page: https://openioe.in/
-Author: Venkataswamy R
-Author-email: opensourceioe@gmail.com
-License: UNKNOWN
-Description: ## Open IoE
-        
-        Open IoE is a simple IoT platform to operate IoT devices.
-        
-        There are two options available,
-        
-        1.  API creation and Consumption (REST APIs)
-        2.  Python Library (Client)
-        
-        ---
-        
-        ### 1\. API Creation for IoT Device and Its Consumption
-        
-        Users are expected to take these steps,
-        
-        1.  Add device using [Link \<Add Device>](http://gnanodaya.org:8080/openioe/device.jsp)
-        2.  (Optional) Verify device data or API using [Link \<Verify Device>](http://gnanodaya.org:8080/openioe/console.jsp)
-        3.  Embed the API in your application using [Client Code/API](http://gnanodaya.org:8080/openioe/embed.jsp)
-        
-        #### Visit the OpenIoE 1.0 web portal at [https://v3.openioe.in](https://v3.openioe.in)
-        
-        #### API List:
-        
-        <table><tbody><tr><td><strong>No</strong></td><td><strong>API</strong></td><td><strong>Description</strong></td><td><strong>Type</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>showvalue</td><td>To get hardware value from web service.</td><td>http get</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/showvalue/2/433</code></pre></td></tr><tr><td>2</td><td>updatevalue</td><td>Update the hardware value passed as a parameter</td><td>http get</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/updatevalue/2/433/2</code></pre></td></tr><tr><td>3</td><td>showjson</td><td>To get hardware JSON from web service.</td><td>http get</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/showjson/2/433</code></pre></td></tr><tr><td>4</td><td>updatejson</td><td>Update the hardware JSON passed as parameter</td><td>http post</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/updatejson/2/433 &lt;Data&gt;</code></pre></td></tr><tr><td>5</td><td>showxml</td><td>To get hardware XML file from web service.</td><td>http get</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/showxml/2/433</code></pre></td></tr><tr><td>6</td><td>updatexml</td><td>Update the hardware XML passed as parameter</td><td>http post</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/updatexml/2/433 &lt;Data&gt;</code></pre></td></tr></tbody></table>
-        
-        ---
-        
-        ### 2\. Python Library
-        
-        Users are expected to take these steps,
-        
-        1.  Install Python Library  
-            `pip install openioe`
-        2.  Write the client code using the following methods
-        
-        #### Method List:
-        
-        <table><tbody><tr><td><strong>No</strong></td><td><strong>Method</strong></td><td><strong>Description</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>ReadAPI</td><td>To read the sensor data from multiple nodes</td><td><pre><code class="language-python">from openioe.openioe_apis import *
-        oi=openioe_apis()
-        oi.UserIDPinAPIKeys=[[2, 433], [3, 986]]
-        SensorData,ResposeCode=oi.ReadAPI()
-        print(SensorData)
-        print(ResposeCode)</code></pre></td></tr><tr><td>2</td><td>WriteAPI</td><td>To modify the control signal at multiple nodes</td><td><pre><code class="language-python">from openioe.openioe_apis import *
-        oi=openioe_apis()
-        oi.UserIDPinAPIKeys=[[2, 433], [3, 986]]
-        
-        oi.Data=[1,2]
-        Confirmation,ResposeCode=oi.ReadAPI()
-        print(Confirmation)
-        print(ResposeCode)</code></pre></td></tr><tr><td>3</td><td>Developer</td><td>To display the developer information</td><td><pre><code class="language-python">from openioe.openioe_apis import *
-        oi=openioe_apis()
-        oi.Developer()</code></pre></td></tr></tbody></table>
-        
-        ---
-        
-        ### Developers
-        <p>
-         <img src="https://venkataswamy.in/images/img1.jpg" alt="Dr. Venkataswamy R" width="100"> 
-        </p>
-        
-        <div><div dir="ltr"><div style="font-size:small"><i><font face="times new roman, serif">Thanks and Regards</font><font face="arial">,</font></i></div><div style="font-family:arial"><b><font size="2" color="#0000ff"><span></span>Venkataswamy R</font><font size="2"><span></span></font></b></div><div style="font-size:small"><span style="color:rgb(0,0,0)"><font face="trebuchet ms, sans-serif"><b>Assistant Professor,</b></font></span></div><div style="font-size:small"><span style="color:rgb(0,0,0)"><font face="trebuchet ms, sans-serif"><b>Department of Electrical and Electronics Engineering,</b></font></span></div><div style="font-size:small"><span style="color:rgb(0,0,0)"><font face="trebuchet ms, sans-serif"><b>School of Engineering and Technology,<br></b></font></span></div><div style="font-size:small"><span style="color:rgb(0,0,0)"><font face="trebuchet ms, sans-serif"><b>Christ (Deemed to be University),</b></font></span></div><div style="font-size:small"><span style="color:rgb(56,118,29)"><font face="trebuchet ms, sans-serif"><b><span style="color:rgb(0,0,0)">Bengaluru-560074, India</span><br><br></b></font></span></div><div style="font-family:arial;font-size:small"><b style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img src="https://ci4.googleusercontent.com/proxy/JGrPNyQPabY_rra4ygFQhpV3cMA7ITqb5WxBKVcm5J7nUXsWZgk4oUuqR-1Dso97mGx5TF4OvAWyEvAm6fA0h9EhgVZcO6VnO77JetkXhoxX6-7YrakgsA=s0-d-e1-ft#https://openclipart.org/image/2400px/svg_to_png/262221/phone25.png" alt="Image result for phone icon" style="margin-top:0px" width="17" height="14"> 080-4012-9961 (O)</i></b><font face="trebuchet ms, sans-serif" color="#073763"><b><i>&nbsp;&nbsp; </i></b></font><b style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img src="https://ci4.googleusercontent.com/proxy/xDyzoCUBYbAyKgjwt27Jl4lkN_6MrkWuk-4BQ2IgMCZEuCMwJLtZjRYqLSrgS6SGWQcpQOVuNmBzqrKJpes9riut82x8hJ1GJVKL=s0-d-e1-ft#http://simpleicon.com/wp-content/uploads/mobile-1.png" style="margin-top:0px" alt="Image result for mobile icon" width="21" height="21">+91-7829222446</i></b><i><b>&nbsp; </b></i><img src="https://lh4.googleusercontent.com/-FqpLVHU8eMw/AAAAAAAAAAI/AAAAAAAAABM/ivbX55TtoV4/photo.jpg" alt="Related image" style="margin-top:0px" width="21" height="21"><span><b style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i> <a href="http://venkataswamy.in" target="_blank">venkatswamy.in</a><br><br><br></i></b></span></div></div></div>
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+
+## Open IoE
+
+
+Open IoE is a simple IoT platform to operate IoT devices.
+
+There are two options available,
+
+1. Python Library (Client) 
+2. Web services (REST APIs)
+---
+
+### 1\. Python Library
+
+Users are expected to take these steps,
+1. Install Python Library
+
+    `pip install openioe`
+
+2. Write the client code using the following methods
+
+#### Method List:
+<table><tbody><tr><td><strong>No</strong></td><td><strong>Method</strong></td><td><strong>Description</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>ReadValue</td><td>To read the sensor data from single nodes. Type of data is "Numeric/String"</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xxx
+SensorData,ResposeCode=oi.ReadValue()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>2</td><td>WriteValue</td><td>To modify the control signal at single nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xx
+oi.Data=10
+SensorData,ResposeCode=oi.WriteValue()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>3</td><td>ReadJSON</td><td>To read the sensor data from single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xxx
+SensorData,ResposeCode=oi.ReadJSON()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>4</td><td>WriteJSON</td><td>To modify the control signal at single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xxx
+oi.DataJSON={'Value': '10'}
+SensorData,ResposeCode=oi.WriteJSON()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>5</td><td>ReadXML</td><td>To read the sensor data from single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xxx
+SensorData,ResposeCode=oi.ReadXML()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>6</td><td>WriteXML</td><td>To modify the control signal at single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xxx
+oi.DataXML='<Name>OpenIoE</Name>'
+SensorData,ResposeCode=oi.WriteXML()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>7</td><td>Read</td><td>To read the sensor data from multiple nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.UserIDPinAPIKeys=[[xx, xxx], [x, xxx]]
+SensorData,ResposeCode=oi.Read()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>8</td><td>Write</td><td>To modify the control signal at multiple nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.UserIDPinAPIKeys=[[xx, xxx], [xx, xxx]]
+oi.Data=[xx,xx]
+Confirmation,ResposeCode=oi.ReadAPI()
+print(Confirmation)
+print(ResposeCode)</code></pre></td></tr><tr><td>3</td><td>Developer</td><td>To display the developer information</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
+oi=openioe_apis()
+oi.Developer()</code></pre></td></tr></tbody></table>
+
+  
+
+---
+
+### 2\. Web Services
+
+Users are expected to take these steps,
+
+1. Register and login to OpenIoE- [Register/Login](https://openioe.gnanodaya.org/)
+
+2. Create API Key/ Get API Key from OpenIoE.
+
+3. Embed the API Key, Device ID and Pin into the client code.
+
+ 
+#### Visit the OpenIoE 3.0 web portal at [https://openioe.gnanodaya.org](https://openioe.gnanodaya.org)
+
+#### Visit the OpenIoE 3.0 Help Portal at [https://openioedoc.gnanodaya.org](https://openioedoc.gnanodaya.org)
+  
+
+#### API List:
+
+<table><tbody><tr><td><strong>No</strong></td><td><strong>API</strong></td><td><strong>Description</strong></td><td><strong>Type</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>showdevicevalue</td><td>To get hardware value from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicevalue/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>2</td><td>updatedevicevalue</td><td>Update the hardware value passed as a parameter</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevievalue/&lt;apikey&gt;/2/433/2</code></pre></td></tr><tr><td>3</td><td>showdevicejson</td><td>To get hardware JSON from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicejson/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>4</td><td>updatedevicejson</td><td>Update the hardware JSON passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicejson/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr><tr><td>5</td><td>showdevicexml</td><td>To get hardware XML file from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicexml/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>6</td><td>updatedevicexml</td><td>Update the hardware XML passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicexml/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr></tbody></table>
+
+  
+
+---
+
+ 
+### Developers
+
+<p>
+<img  src="https://venkataswamy.in/images/img1.jpg"  alt="Dr. Venkataswamy R"  width="100"/>
+</p>
+<div><div  dir="ltr"><div  style="font-size:small"><i><font  face="times new roman, serif">Thanks and Regards</font><font  face="arial">,</font></i></div><div  style="font-family:arial"><b><font  size="2"  color="#0000ff"><span></span>Venkataswamy R</font><font  size="2"><span></span></font></b></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Assistant Professor,</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Department of Electrical and Electronics Engineering,</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>School of Engineering and Technology,<br></b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Christ (Deemed to be University),</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(56,118,29)"><font  face="trebuchet ms, sans-serif"><b><span  style="color:rgb(0,0,0)">Bengaluru-560074, India</span><br><br></b></font></span></div><div  style="font-family:arial;font-size:small"><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img  src="https://ci4.googleusercontent.com/proxy/JGrPNyQPabY_rra4ygFQhpV3cMA7ITqb5WxBKVcm5J7nUXsWZgk4oUuqR-1Dso97mGx5TF4OvAWyEvAm6fA0h9EhgVZcO6VnO77JetkXhoxX6-7YrakgsA=s0-d-e1-ft#https://openclipart.org/image/2400px/svg_to_png/262221/phone25.png"  alt="Image result for phone icon"  style="margin-top:0px"  width="17"  height="14"> 080-4012-9961 (O)</i></b><font  face="trebuchet ms, sans-serif"  color="#073763"><b><i>&nbsp;&nbsp;  </i></b></font><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img  src="https://ci4.googleusercontent.com/proxy/xDyzoCUBYbAyKgjwt27Jl4lkN_6MrkWuk-4BQ2IgMCZEuCMwJLtZjRYqLSrgS6SGWQcpQOVuNmBzqrKJpes9riut82x8hJ1GJVKL=s0-d-e1-ft#http://simpleicon.com/wp-content/uploads/mobile-1.png"  style="margin-top:0px"  alt="Image result for mobile icon"  width="21"  height="21">+91-7829222446</i></b><i><b>&nbsp;  </b></i><img  src="https://lh4.googleusercontent.com/-FqpLVHU8eMw/AAAAAAAAAAI/AAAAAAAAABM/ivbX55TtoV4/photo.jpg"  alt="Related image"  style="margin-top:0px"  width="21"  height="21"><span><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i>  <a  href="http://venkataswamy.in"  target="_blank">venkatswamy.in</a><br><br><br></i></b></span></div></div></div>
```

#### html2text {}

```diff
@@ -1,68 +1,121 @@
-Metadata-Version: 2.1 Name: openioe Version: 0.1.3 Summary: Open IoE Home-page:
-https://openioe.in/ Author: Venkataswamy R Author-email:
-opensourceioe@gmail.com License: UNKNOWN Description: ## Open IoE Open IoE is a
-simple IoT platform to operate IoT devices. There are two options available, 1.
-API creation and Consumption (REST APIs) 2. Python Library (Client) --- ### 1\.
-API Creation for IoT Device and Its Consumption Users are expected to take
-these steps, 1. Add device using [Link \](http://gnanodaya.org:8080/openioe/
-device.jsp) 2. (Optional) Verify device data or API using [Link \](http://
-gnanodaya.org:8080/openioe/console.jsp) 3. Embed the API in your application
-using [Client Code/API](http://gnanodaya.org:8080/openioe/embed.jsp) #### Visit
-the OpenIoE 1.0 web portal at [https://v3.openioe.in](https://v3.openioe.in)
-#### API List:
-No API         Description                Type      Example
-1  showvalue   To get hardware value from http get  <endpoint>/showvalue/2/433
-               web service.
-2  updatevalue Update the hardware value  http get  <endpoint>/updatevalue/2/
-               passed as a parameter                433/2
-3  showjson    To get hardware JSON from  http get  <endpoint>/showjson/2/433
-               web service.
-4  updatejson  Update the hardware JSON   http post <endpoint>/updatejson/2/433
-               passed as parameter                  <Data>
-5  showxml     To get hardware XML file   http get  <endpoint>/showxml/2/433
-               from web service.
-6  updatexml   Update the hardware XML    http post <endpoint>/updatexml/2/433
-               passed as parameter                  <Data>
---- ### 2\. Python Library Users are expected to take these steps, 1. Install
-Python Library `pip install openioe` 2. Write the client code using the
+ ## Open IoE Open IoE is a simple IoT platform to operate IoT devices. There
+are two options available, 1. Python Library (Client) 2. Web services (REST
+APIs) --- ### 1\. Python Library Users are expected to take these steps, 1.
+Install Python Library `pip install openioe` 2. Write the client code using the
 following methods #### Method List:
-No Method    Description                  Example
-                                          from openioe.openioe_apis import *
-                                                  oi=openioe_apis()
-                                                  oi.UserIDPinAPIKeys=[[2,
-1  ReadAPI   To read the sensor data from 433], [3, 986]]
-             multiple nodes
-                                          SensorData,ResposeCode=oi.ReadAPI()
-                                                  print(SensorData)
-                                                  print(ResposeCode)
-                                          from openioe.openioe_apis import *
-                                                  oi=openioe_apis()
-                                                  oi.UserIDPinAPIKeys=[[2,
-                                          433], [3, 986]]
-             To modify the control signal
-2  WriteAPI  at multiple nodes                    oi.Data=[1,2]
-
-                                          Confirmation,ResposeCode=oi.ReadAPI
-                                          ()
-                                                  print(Confirmation)
-                                                  print(ResposeCode)
-             To display the developer     from openioe.openioe_apis import *
-3  Developer information                          oi=openioe_apis()
-                                                  oi.Developer()
+No Method     Description                  Example
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+              To read the sensor data from oi.DeviceID=xx
+1  ReadValue  single nodes. Type of data   oi.DevicePin=xxx
+              is "Numeric/String"          SensorData,ResposeCode=oi.ReadValue
+                                           ()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+              To modify the control signal oi.DeviceID=xx
+2  WriteValue at single nodes. Type of     oi.DevicePin=xx
+              data is "Numeric/String".    oi.Data=10
+                                           SensorData,ResposeCode=oi.WriteValue
+                                           ()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+3  ReadJSON   single nodes. Type of data   oi.DeviceID=xx
+              is "JSON".                   oi.DevicePin=xxx
+                                           SensorData,ResposeCode=oi.ReadJSON()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+              To modify the control signal oi.DeviceID=xx
+4  WriteJSON  at single nodes. Type of     oi.DevicePin=xxx
+              data is "JSON".              oi.DataJSON={'Value': '10'}
+                                           SensorData,ResposeCode=oi.WriteJSON
+                                           ()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+5  ReadXML    single nodes. Type of data   oi.DeviceID=xx
+              is "XML".                    oi.DevicePin=xxx
+                                           SensorData,ResposeCode=oi.ReadXML()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+              To modify the control signal oi.DeviceID=xx
+6  WriteXML   at single nodes. Type of     oi.DevicePin=xxx
+              data is "XML".               oi.DataXML='OpenIoE'
+                                           SensorData,ResposeCode=oi.WriteXML()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+7  Read       multiple nodes. Type of data oi.UserIDPinAPIKeys=[[xx, xxx], [x,
+              is "Numeric/String".         xxx]]
+                                           SensorData,ResposeCode=oi.Read()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from openioe.openioe_apis import *
+                                           oi=openioe_apis()
+                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+              To modify the control signal oi.UserIDPinAPIKeys=[[xx, xxx], [xx,
+8  Write      at multiple nodes. Type of   xxx]]
+              data is "Numeric/String".    oi.Data=[xx,xx]
+                                           Confirmation,ResposeCode=oi.ReadAPI
+                                           ()
+                                           print(Confirmation)
+                                           print(ResposeCode)
+              To display the developer     from openioe.openioe_apis import *
+3  Developer  information                  oi=openioe_apis()
+                                           oi.Developer()
+--- ### 2\. Web Services Users are expected to take these steps, 1. Register
+and login to OpenIoE- [Register/Login](https://openioe.gnanodaya.org/) 2.
+Create API Key/ Get API Key from OpenIoE. 3. Embed the API Key, Device ID and
+Pin into the client code. #### Visit the OpenIoE 3.0 web portal at [https://
+openioe.gnanodaya.org](https://openioe.gnanodaya.org) #### Visit the OpenIoE
+3.0 Help Portal at [https://openioedoc.gnanodaya.org](https://
+openioedoc.gnanodaya.org) #### API List:
+No API               Description             Type      Example
+                     To get hardware value             <endpoint>/
+1  showdevicevalue   from web service.       http get  showdevicevalue/
+                                                       <apikey>/2/433
+                     Update the hardware               <endpoint>/
+2  updatedevicevalue value passed as a       http get  updatedevievalue/
+                     parameter                         <apikey>/2/433/2
+                     To get hardware JSON              <endpoint>/
+3  showdevicejson    from web service.       http get  showdevicejson/<apikey>/
+                                                       2/433
+                     Update the hardware               <endpoint>/
+4  updatedevicejson  JSON passed as          http post updatedevicejson/
+                     parameter                         <apikey>/2/433 <Data>
+                     To get hardware XML               <endpoint>/
+5  showdevicexml     file from web service.  http get  showdevicexml/<apikey>/
+                                                       2/433
+                     Update the hardware XML           <endpoint>/
+6  updatedevicexml   passed as parameter     http post updatedevicexml/
+                                                       <apikey>/2/433 <Data>
 --- ### Developers
 [Dr. Venkataswamy R]
 Thanks and Regards,
 Venkataswamy R
 Assistant Professor,
 Department of Electrical and Electronics Engineering,
 School of Engineering and Technology,
 Christ (Deemed to be University),
 Bengaluru-560074, India
 
 [Image result for phone icon] 080-4012-9961 (O)  [Image result for mobile
 icon]+91-7829222446 [Related image]venkatswamy.in
 
 
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `openioe-0.1.3/openioe.egg-info/PKG-INFO` & `openioe-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,140 @@
 Metadata-Version: 2.1
 Name: openioe
-Version: 0.1.3
+Version: 1.0.0
 Summary: Open IoE
-Home-page: https://openioe.in/
+Home-page: https://openioe.gnanodaya.org/
 Author: Venkataswamy R
 Author-email: opensourceioe@gmail.com
-License: UNKNOWN
-Description: ## Open IoE
-        
-        Open IoE is a simple IoT platform to operate IoT devices.
-        
-        There are two options available,
-        
-        1.  API creation and Consumption (REST APIs)
-        2.  Python Library (Client)
-        
-        ---
-        
-        ### 1\. API Creation for IoT Device and Its Consumption
-        
-        Users are expected to take these steps,
-        
-        1.  Add device using [Link \<Add Device>](http://gnanodaya.org:8080/openioe/device.jsp)
-        2.  (Optional) Verify device data or API using [Link \<Verify Device>](http://gnanodaya.org:8080/openioe/console.jsp)
-        3.  Embed the API in your application using [Client Code/API](http://gnanodaya.org:8080/openioe/embed.jsp)
-        
-        #### Visit the OpenIoE 1.0 web portal at [https://v3.openioe.in](https://v3.openioe.in)
-        
-        #### API List:
-        
-        <table><tbody><tr><td><strong>No</strong></td><td><strong>API</strong></td><td><strong>Description</strong></td><td><strong>Type</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>showvalue</td><td>To get hardware value from web service.</td><td>http get</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/showvalue/2/433</code></pre></td></tr><tr><td>2</td><td>updatevalue</td><td>Update the hardware value passed as a parameter</td><td>http get</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/updatevalue/2/433/2</code></pre></td></tr><tr><td>3</td><td>showjson</td><td>To get hardware JSON from web service.</td><td>http get</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/showjson/2/433</code></pre></td></tr><tr><td>4</td><td>updatejson</td><td>Update the hardware JSON passed as parameter</td><td>http post</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/updatejson/2/433 &lt;Data&gt;</code></pre></td></tr><tr><td>5</td><td>showxml</td><td>To get hardware XML file from web service.</td><td>http get</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/showxml/2/433</code></pre></td></tr><tr><td>6</td><td>updatexml</td><td>Update the hardware XML passed as parameter</td><td>http post</td><td><pre><code class="language-plaintext">&lt;endpoint&gt;/updatexml/2/433 &lt;Data&gt;</code></pre></td></tr></tbody></table>
-        
-        ---
-        
-        ### 2\. Python Library
-        
-        Users are expected to take these steps,
-        
-        1.  Install Python Library  
-            `pip install openioe`
-        2.  Write the client code using the following methods
-        
-        #### Method List:
-        
-        <table><tbody><tr><td><strong>No</strong></td><td><strong>Method</strong></td><td><strong>Description</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>ReadAPI</td><td>To read the sensor data from multiple nodes</td><td><pre><code class="language-python">from openioe.openioe_apis import *
-        oi=openioe_apis()
-        oi.UserIDPinAPIKeys=[[2, 433], [3, 986]]
-        SensorData,ResposeCode=oi.ReadAPI()
-        print(SensorData)
-        print(ResposeCode)</code></pre></td></tr><tr><td>2</td><td>WriteAPI</td><td>To modify the control signal at multiple nodes</td><td><pre><code class="language-python">from openioe.openioe_apis import *
-        oi=openioe_apis()
-        oi.UserIDPinAPIKeys=[[2, 433], [3, 986]]
-        
-        oi.Data=[1,2]
-        Confirmation,ResposeCode=oi.ReadAPI()
-        print(Confirmation)
-        print(ResposeCode)</code></pre></td></tr><tr><td>3</td><td>Developer</td><td>To display the developer information</td><td><pre><code class="language-python">from openioe.openioe_apis import *
-        oi=openioe_apis()
-        oi.Developer()</code></pre></td></tr></tbody></table>
-        
-        ---
-        
-        ### Developers
-        <p>
-         <img src="https://venkataswamy.in/images/img1.jpg" alt="Dr. Venkataswamy R" width="100"> 
-        </p>
-        
-        <div><div dir="ltr"><div style="font-size:small"><i><font face="times new roman, serif">Thanks and Regards</font><font face="arial">,</font></i></div><div style="font-family:arial"><b><font size="2" color="#0000ff"><span></span>Venkataswamy R</font><font size="2"><span></span></font></b></div><div style="font-size:small"><span style="color:rgb(0,0,0)"><font face="trebuchet ms, sans-serif"><b>Assistant Professor,</b></font></span></div><div style="font-size:small"><span style="color:rgb(0,0,0)"><font face="trebuchet ms, sans-serif"><b>Department of Electrical and Electronics Engineering,</b></font></span></div><div style="font-size:small"><span style="color:rgb(0,0,0)"><font face="trebuchet ms, sans-serif"><b>School of Engineering and Technology,<br></b></font></span></div><div style="font-size:small"><span style="color:rgb(0,0,0)"><font face="trebuchet ms, sans-serif"><b>Christ (Deemed to be University),</b></font></span></div><div style="font-size:small"><span style="color:rgb(56,118,29)"><font face="trebuchet ms, sans-serif"><b><span style="color:rgb(0,0,0)">Bengaluru-560074, India</span><br><br></b></font></span></div><div style="font-family:arial;font-size:small"><b style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img src="https://ci4.googleusercontent.com/proxy/JGrPNyQPabY_rra4ygFQhpV3cMA7ITqb5WxBKVcm5J7nUXsWZgk4oUuqR-1Dso97mGx5TF4OvAWyEvAm6fA0h9EhgVZcO6VnO77JetkXhoxX6-7YrakgsA=s0-d-e1-ft#https://openclipart.org/image/2400px/svg_to_png/262221/phone25.png" alt="Image result for phone icon" style="margin-top:0px" width="17" height="14"> 080-4012-9961 (O)</i></b><font face="trebuchet ms, sans-serif" color="#073763"><b><i>&nbsp;&nbsp; </i></b></font><b style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img src="https://ci4.googleusercontent.com/proxy/xDyzoCUBYbAyKgjwt27Jl4lkN_6MrkWuk-4BQ2IgMCZEuCMwJLtZjRYqLSrgS6SGWQcpQOVuNmBzqrKJpes9riut82x8hJ1GJVKL=s0-d-e1-ft#http://simpleicon.com/wp-content/uploads/mobile-1.png" style="margin-top:0px" alt="Image result for mobile icon" width="21" height="21">+91-7829222446</i></b><i><b>&nbsp; </b></i><img src="https://lh4.googleusercontent.com/-FqpLVHU8eMw/AAAAAAAAAAI/AAAAAAAAABM/ivbX55TtoV4/photo.jpg" alt="Related image" style="margin-top:0px" width="21" height="21"><span><b style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i> <a href="http://venkataswamy.in" target="_blank">venkatswamy.in</a><br><br><br></i></b></span></div></div></div>
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+## Open IoE
+
+
+Open IoE is a simple IoT platform to operate IoT devices.
+
+There are two options available,
+
+1. Python Library (Client) 
+2. Web services (REST APIs)
+---
+
+### 1\. Python Library
+
+Users are expected to take these steps,
+1. Install Python Library
+
+    `pip install openioe`
+
+2. Write the client code using the following methods
+
+#### Method List:
+<table><tbody><tr><td><strong>No</strong></td><td><strong>Method</strong></td><td><strong>Description</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>ReadValue</td><td>To read the sensor data from single nodes. Type of data is "Numeric/String"</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xxx
+SensorData,ResposeCode=oi.ReadValue()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>2</td><td>WriteValue</td><td>To modify the control signal at single nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xx
+oi.Data=10
+SensorData,ResposeCode=oi.WriteValue()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>3</td><td>ReadJSON</td><td>To read the sensor data from single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xxx
+SensorData,ResposeCode=oi.ReadJSON()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>4</td><td>WriteJSON</td><td>To modify the control signal at single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xxx
+oi.DataJSON={'Value': '10'}
+SensorData,ResposeCode=oi.WriteJSON()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>5</td><td>ReadXML</td><td>To read the sensor data from single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xxx
+SensorData,ResposeCode=oi.ReadXML()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>6</td><td>WriteXML</td><td>To modify the control signal at single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.DeviceID=xx
+oi.DevicePin=xxx
+oi.DataXML='<Name>OpenIoE</Name>'
+SensorData,ResposeCode=oi.WriteXML()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>7</td><td>Read</td><td>To read the sensor data from multiple nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.UserIDPinAPIKeys=[[xx, xxx], [x, xxx]]
+SensorData,ResposeCode=oi.Read()
+print(SensorData)
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>8</td><td>Write</td><td>To modify the control signal at multiple nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
+oi=openioe_apis()
+oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+oi.UserIDPinAPIKeys=[[xx, xxx], [xx, xxx]]
+oi.Data=[xx,xx]
+Confirmation,ResposeCode=oi.ReadAPI()
+print(Confirmation)
+print(ResposeCode)</code></pre></td></tr><tr><td>3</td><td>Developer</td><td>To display the developer information</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
+oi=openioe_apis()
+oi.Developer()</code></pre></td></tr></tbody></table>
+
+  
+
+---
+
+### 2\. Web Services
+
+Users are expected to take these steps,
+
+1. Register and login to OpenIoE- [Register/Login](https://openioe.gnanodaya.org/)
+
+2. Create API Key/ Get API Key from OpenIoE.
+
+3. Embed the API Key, Device ID and Pin into the client code.
+
+ 
+#### Visit the OpenIoE 3.0 web portal at [https://openioe.gnanodaya.org](https://openioe.gnanodaya.org)
+
+#### Visit the OpenIoE 3.0 Help Portal at [https://openioedoc.gnanodaya.org](https://openioedoc.gnanodaya.org)
+  
+
+#### API List:
+
+<table><tbody><tr><td><strong>No</strong></td><td><strong>API</strong></td><td><strong>Description</strong></td><td><strong>Type</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>showdevicevalue</td><td>To get hardware value from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicevalue/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>2</td><td>updatedevicevalue</td><td>Update the hardware value passed as a parameter</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevievalue/&lt;apikey&gt;/2/433/2</code></pre></td></tr><tr><td>3</td><td>showdevicejson</td><td>To get hardware JSON from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicejson/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>4</td><td>updatedevicejson</td><td>Update the hardware JSON passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicejson/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr><tr><td>5</td><td>showdevicexml</td><td>To get hardware XML file from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicexml/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>6</td><td>updatedevicexml</td><td>Update the hardware XML passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicexml/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr></tbody></table>
+
+  
+
+---
+
+ 
+### Developers
+
+<p>
+<img  src="https://venkataswamy.in/images/img1.jpg"  alt="Dr. Venkataswamy R"  width="100"/>
+</p>
+<div><div  dir="ltr"><div  style="font-size:small"><i><font  face="times new roman, serif">Thanks and Regards</font><font  face="arial">,</font></i></div><div  style="font-family:arial"><b><font  size="2"  color="#0000ff"><span></span>Venkataswamy R</font><font  size="2"><span></span></font></b></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Assistant Professor,</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Department of Electrical and Electronics Engineering,</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>School of Engineering and Technology,<br></b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Christ (Deemed to be University),</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(56,118,29)"><font  face="trebuchet ms, sans-serif"><b><span  style="color:rgb(0,0,0)">Bengaluru-560074, India</span><br><br></b></font></span></div><div  style="font-family:arial;font-size:small"><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img  src="https://ci4.googleusercontent.com/proxy/JGrPNyQPabY_rra4ygFQhpV3cMA7ITqb5WxBKVcm5J7nUXsWZgk4oUuqR-1Dso97mGx5TF4OvAWyEvAm6fA0h9EhgVZcO6VnO77JetkXhoxX6-7YrakgsA=s0-d-e1-ft#https://openclipart.org/image/2400px/svg_to_png/262221/phone25.png"  alt="Image result for phone icon"  style="margin-top:0px"  width="17"  height="14"> 080-4012-9961 (O)</i></b><font  face="trebuchet ms, sans-serif"  color="#073763"><b><i>&nbsp;&nbsp;  </i></b></font><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img  src="https://ci4.googleusercontent.com/proxy/xDyzoCUBYbAyKgjwt27Jl4lkN_6MrkWuk-4BQ2IgMCZEuCMwJLtZjRYqLSrgS6SGWQcpQOVuNmBzqrKJpes9riut82x8hJ1GJVKL=s0-d-e1-ft#http://simpleicon.com/wp-content/uploads/mobile-1.png"  style="margin-top:0px"  alt="Image result for mobile icon"  width="21"  height="21">+91-7829222446</i></b><i><b>&nbsp;  </b></i><img  src="https://lh4.googleusercontent.com/-FqpLVHU8eMw/AAAAAAAAAAI/AAAAAAAAABM/ivbX55TtoV4/photo.jpg"  alt="Related image"  style="margin-top:0px"  width="21"  height="21"><span><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i>  <a  href="http://venkataswamy.in"  target="_blank">venkatswamy.in</a><br><br><br></i></b></span></div></div></div>
```

#### html2text {}

```diff
@@ -1,68 +1,126 @@
-Metadata-Version: 2.1 Name: openioe Version: 0.1.3 Summary: Open IoE Home-page:
-https://openioe.in/ Author: Venkataswamy R Author-email:
-opensourceioe@gmail.com License: UNKNOWN Description: ## Open IoE Open IoE is a
-simple IoT platform to operate IoT devices. There are two options available, 1.
-API creation and Consumption (REST APIs) 2. Python Library (Client) --- ### 1\.
-API Creation for IoT Device and Its Consumption Users are expected to take
-these steps, 1. Add device using [Link \](http://gnanodaya.org:8080/openioe/
-device.jsp) 2. (Optional) Verify device data or API using [Link \](http://
-gnanodaya.org:8080/openioe/console.jsp) 3. Embed the API in your application
-using [Client Code/API](http://gnanodaya.org:8080/openioe/embed.jsp) #### Visit
-the OpenIoE 1.0 web portal at [https://v3.openioe.in](https://v3.openioe.in)
-#### API List:
-No API         Description                Type      Example
-1  showvalue   To get hardware value from http get  <endpoint>/showvalue/2/433
-               web service.
-2  updatevalue Update the hardware value  http get  <endpoint>/updatevalue/2/
-               passed as a parameter                433/2
-3  showjson    To get hardware JSON from  http get  <endpoint>/showjson/2/433
-               web service.
-4  updatejson  Update the hardware JSON   http post <endpoint>/updatejson/2/433
-               passed as parameter                  <Data>
-5  showxml     To get hardware XML file   http get  <endpoint>/showxml/2/433
-               from web service.
-6  updatexml   Update the hardware XML    http post <endpoint>/updatexml/2/433
-               passed as parameter                  <Data>
---- ### 2\. Python Library Users are expected to take these steps, 1. Install
-Python Library `pip install openioe` 2. Write the client code using the
-following methods #### Method List:
-No Method    Description                  Example
-                                          from openioe.openioe_apis import *
-                                                  oi=openioe_apis()
-                                                  oi.UserIDPinAPIKeys=[[2,
-1  ReadAPI   To read the sensor data from 433], [3, 986]]
-             multiple nodes
-                                          SensorData,ResposeCode=oi.ReadAPI()
-                                                  print(SensorData)
-                                                  print(ResposeCode)
-                                          from openioe.openioe_apis import *
-                                                  oi=openioe_apis()
-                                                  oi.UserIDPinAPIKeys=[[2,
-                                          433], [3, 986]]
-             To modify the control signal
-2  WriteAPI  at multiple nodes                    oi.Data=[1,2]
-
-                                          Confirmation,ResposeCode=oi.ReadAPI
-                                          ()
-                                                  print(Confirmation)
-                                                  print(ResposeCode)
-             To display the developer     from openioe.openioe_apis import *
-3  Developer information                          oi=openioe_apis()
-                                                  oi.Developer()
+Metadata-Version: 2.1 Name: openioe Version: 1.0.0 Summary: Open IoE Home-page:
+https://openioe.gnanodaya.org/ Author: Venkataswamy R Author-email:
+opensourceioe@gmail.com Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE ## Open IoE Open IoE is a simple IoT platform to
+operate IoT devices. There are two options available, 1. Python Library
+(Client) 2. Web services (REST APIs) --- ### 1\. Python Library Users are
+expected to take these steps, 1. Install Python Library `pip install openioe`
+2. Write the client code using the following methods #### Method List:
+No Method     Description                  Example
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+              To read the sensor data from oi.DeviceID=xx
+1  ReadValue  single nodes. Type of data   oi.DevicePin=xxx
+              is "Numeric/String"          SensorData,ResposeCode=oi.ReadValue
+                                           ()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+              To modify the control signal oi.DeviceID=xx
+2  WriteValue at single nodes. Type of     oi.DevicePin=xx
+              data is "Numeric/String".    oi.Data=10
+                                           SensorData,ResposeCode=oi.WriteValue
+                                           ()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+3  ReadJSON   single nodes. Type of data   oi.DeviceID=xx
+              is "JSON".                   oi.DevicePin=xxx
+                                           SensorData,ResposeCode=oi.ReadJSON()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+              To modify the control signal oi.DeviceID=xx
+4  WriteJSON  at single nodes. Type of     oi.DevicePin=xxx
+              data is "JSON".              oi.DataJSON={'Value': '10'}
+                                           SensorData,ResposeCode=oi.WriteJSON
+                                           ()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+5  ReadXML    single nodes. Type of data   oi.DeviceID=xx
+              is "XML".                    oi.DevicePin=xxx
+                                           SensorData,ResposeCode=oi.ReadXML()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+              To modify the control signal oi.DeviceID=xx
+6  WriteXML   at single nodes. Type of     oi.DevicePin=xxx
+              data is "XML".               oi.DataXML='OpenIoE'
+                                           SensorData,ResposeCode=oi.WriteXML()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from  openioe.openioe_apis  import *
+                                           oi=openioe_apis()
+              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+7  Read       multiple nodes. Type of data oi.UserIDPinAPIKeys=[[xx, xxx], [x,
+              is "Numeric/String".         xxx]]
+                                           SensorData,ResposeCode=oi.Read()
+                                           print(SensorData)
+                                           print(ResposeCode)
+                                           from openioe.openioe_apis import *
+                                           oi=openioe_apis()
+                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+              To modify the control signal oi.UserIDPinAPIKeys=[[xx, xxx], [xx,
+8  Write      at multiple nodes. Type of   xxx]]
+              data is "Numeric/String".    oi.Data=[xx,xx]
+                                           Confirmation,ResposeCode=oi.ReadAPI
+                                           ()
+                                           print(Confirmation)
+                                           print(ResposeCode)
+              To display the developer     from openioe.openioe_apis import *
+3  Developer  information                  oi=openioe_apis()
+                                           oi.Developer()
+--- ### 2\. Web Services Users are expected to take these steps, 1. Register
+and login to OpenIoE- [Register/Login](https://openioe.gnanodaya.org/) 2.
+Create API Key/ Get API Key from OpenIoE. 3. Embed the API Key, Device ID and
+Pin into the client code. #### Visit the OpenIoE 3.0 web portal at [https://
+openioe.gnanodaya.org](https://openioe.gnanodaya.org) #### Visit the OpenIoE
+3.0 Help Portal at [https://openioedoc.gnanodaya.org](https://
+openioedoc.gnanodaya.org) #### API List:
+No API               Description             Type      Example
+                     To get hardware value             <endpoint>/
+1  showdevicevalue   from web service.       http get  showdevicevalue/
+                                                       <apikey>/2/433
+                     Update the hardware               <endpoint>/
+2  updatedevicevalue value passed as a       http get  updatedevievalue/
+                     parameter                         <apikey>/2/433/2
+                     To get hardware JSON              <endpoint>/
+3  showdevicejson    from web service.       http get  showdevicejson/<apikey>/
+                                                       2/433
+                     Update the hardware               <endpoint>/
+4  updatedevicejson  JSON passed as          http post updatedevicejson/
+                     parameter                         <apikey>/2/433 <Data>
+                     To get hardware XML               <endpoint>/
+5  showdevicexml     file from web service.  http get  showdevicexml/<apikey>/
+                                                       2/433
+                     Update the hardware XML           <endpoint>/
+6  updatedevicexml   passed as parameter     http post updatedevicexml/
+                                                       <apikey>/2/433 <Data>
 --- ### Developers
 [Dr. Venkataswamy R]
 Thanks and Regards,
 Venkataswamy R
 Assistant Professor,
 Department of Electrical and Electronics Engineering,
 School of Engineering and Technology,
 Christ (Deemed to be University),
 Bengaluru-560074, India
 
 [Image result for phone icon] 080-4012-9961 (O)  [Image result for mobile
 icon]+91-7829222446 [Related image]venkatswamy.in
 
 
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `openioe-0.1.3/setup.py` & `openioe-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="openioe", # Replace with your own username
-    version="0.1.3",
+    version="1.0.0",
     author="Venkataswamy R",
 	scripts=['openioe\openioe_apis.py'] ,
     author_email="opensourceioe@gmail.com",
     description="Open IoE",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://openioe.in/",
+    url="https://openioe.gnanodaya.org/",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

