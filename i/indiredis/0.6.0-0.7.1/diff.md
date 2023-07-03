# Comparing `tmp/indiredis-0.6.0.tar.gz` & `tmp/indiredis-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indiredis-0.6.0.tar", last modified: Sat Apr  8 16:38:38 2023, max compression
+gzip compressed data, was "indiredis-0.7.1.tar", last modified: Mon Jul  3 09:02:39 2023, max compression
```

## Comparing `indiredis-0.6.0.tar` & `indiredis-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1056 2023-01-08 14:22:55.619352 indiredis-0.6.0/LICENSE
--rw-r--r--   0        0        0     3029 2023-04-07 21:50:40.093339 indiredis-0.6.0/README.md
--rw-r--r--   0        0        0    27523 2023-04-07 21:39:09.514020 indiredis-0.6.0/indiredis/__init__.py
--rw-r--r--   0        0        0     3310 2023-04-07 20:33:19.729769 indiredis-0.6.0/indiredis/__main__.py
--rw-r--r--   0        0        0    13939 2023-03-17 15:56:20.966801 indiredis-0.6.0/indiredis/indiredis/data/defaults.json
--rw-r--r--   0        0        0    64481 2023-04-07 20:34:39.214839 indiredis-0.6.0/indiredis/indiredis/data/project.json
--rw-r--r--   0        0        0     3008 2023-03-17 15:56:20.970802 indiredis-0.6.0/indiredis/indiredis/data/textblocks_json/en.json
--rw-r--r--   0        0        0     1524 2023-01-08 14:22:55.631352 indiredis-0.6.0/indiredis/indiredis/static/css/w3-theme-ski.css
--rw-r--r--   0        0        0      712 2023-01-08 14:22:55.631352 indiredis-0.6.0/indiredis/indiredis/static/images/logo.svg
--rw-r--r--   0        0        0      513 2023-01-08 14:22:55.631352 indiredis-0.6.0/indiredis/indiredis/static/images/logo_icon16.svg
--rw-r--r--   0        0        0        0 2023-01-08 14:22:55.631352 indiredis-0.6.0/indiredis/webcode/__init__.py
--rw-r--r--   0        0        0     1505 2023-03-17 15:56:20.970802 indiredis-0.6.0/indiredis/webcode/authenticate.py
--rw-r--r--   0        0        0     1846 2023-03-17 15:56:20.970802 indiredis-0.6.0/indiredis/webcode/blobs.py
--rw-r--r--   0        0        0    52352 2023-03-17 15:56:20.970802 indiredis-0.6.0/indiredis/webcode/devices.py
--rw-r--r--   0        0        0    20618 2023-01-08 14:44:11.760425 indiredis-0.6.0/indiredis/webcode/setvalues.py
--rw-r--r--   0        0        0     1000 2023-04-07 20:51:10.300544 indiredis-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3973 1970-01-01 00:00:00.000000 indiredis-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-03-09 20:41:53.000000 indiredis-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3152 2023-04-09 16:31:47.000000 indiredis-0.7.1/README.md
+-rw-r--r--   0        0        0    27975 2023-07-03 08:44:38.000000 indiredis-0.7.1/indiredis/__init__.py
+-rw-r--r--   0        0        0     4281 2023-07-02 21:58:36.000000 indiredis-0.7.1/indiredis/__main__.py
+-rw-r--r--   0        0        0    13939 2023-03-10 12:21:24.000000 indiredis-0.7.1/indiredis/indiredis/data/defaults.json
+-rw-r--r--   0        0        0    64481 2023-07-02 21:57:31.000000 indiredis-0.7.1/indiredis/indiredis/data/project.json
+-rw-r--r--   0        0        0     3008 2023-03-10 22:48:31.000000 indiredis-0.7.1/indiredis/indiredis/data/textblocks_json/en.json
+-rw-r--r--   0        0        0     1524 2023-03-09 20:41:53.000000 indiredis-0.7.1/indiredis/indiredis/static/css/w3-theme-ski.css
+-rw-r--r--   0        0        0      712 2023-03-09 20:41:53.000000 indiredis-0.7.1/indiredis/indiredis/static/images/logo.svg
+-rw-r--r--   0        0        0      513 2023-03-09 20:41:53.000000 indiredis-0.7.1/indiredis/indiredis/static/images/logo_icon16.svg
+-rw-r--r--   0        0        0        0 2023-03-09 20:41:53.000000 indiredis-0.7.1/indiredis/webcode/__init__.py
+-rw-r--r--   0        0        0     1505 2023-03-11 17:09:55.000000 indiredis-0.7.1/indiredis/webcode/authenticate.py
+-rw-r--r--   0        0        0     1846 2023-03-10 15:01:26.000000 indiredis-0.7.1/indiredis/webcode/blobs.py
+-rw-r--r--   0        0        0    52167 2023-07-03 08:41:14.000000 indiredis-0.7.1/indiredis/webcode/devices.py
+-rw-r--r--   0        0        0    20832 2023-07-03 08:49:15.000000 indiredis-0.7.1/indiredis/webcode/setvalues.py
+-rw-r--r--   0        0        0     1000 2023-07-02 21:57:39.000000 indiredis-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4096 1970-01-01 00:00:00.000000 indiredis-0.7.1/PKG-INFO
```

### Comparing `indiredis-0.6.0/LICENSE` & `indiredis-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `indiredis-0.6.0/README.md` & `indiredis-0.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This Python3 package provides an INDI web client for general Instrument control.
 
 INDI - Instrument Neutral Distributed Interface.
 
 See https://en.wikipedia.org/wiki/Instrument_Neutral_Distributed_Interface
 
-The package does not include indiserver or drivers, but is compatable with them, indiserver is an application (debian package indi-bin) which runs instrument drivers, and listens on port 7624. This client (or other INDI clients), can connect to this port and using an XML based protocol, control the connected instruments.
+The package does not include indiserver or drivers, but is compatable with them, indiserver is an application (debian package indi-bin) which runs instrument drivers, and listens on port 7624. This client can connect to this port, and then serves web pages allowing the user to control the connected instruments.
 
 Though the INDI protocol is generally used for astronomical instruments, it can work with any instrument if appropriate INDI drivers are available.
 
 If this indiredis package is imported it provides functions for running a web client connected to either: an INDI server port; an MQTT server; or directly to INDI instrument drivers.
 
 If indiredis is run with the python -m option, then the web client is started and connects to an INDI server port.
 
@@ -29,14 +29,16 @@
 
 The directory /path/to/blobfolder should be a path to a directory of your choice, where BLOB's (Binary Large Objects), such as images will be stored, it will be created if it does not exist. Then connecting with a browser to http://localhost:8000 should enable you to view and control the connected instruments.
 
 For further usage information, including setting ports and hosts, try:
 
 > python3 -m indiredis --help
 
+If the package is imported into your own scripts, it provides a runclient function which accepts a configuration file. This file specifies the INDI drivers to run, or the MQTT or indiserver connections to use. The function then runs the web client.
+
 
 ## Installation
 
 Server dependencies: A redis server (For debian systems; apt-get install redis-server), and indiserver with drivers (apt-get install indi-bin).
 
 For debian systems you may need apt-get install python3-pip, and then use whichever variation of the pip command required by your environment, one example being:
 
@@ -61,10 +63,10 @@
 redis - Python redis client.
 
 paho-mqtt - Python mqtt client.
 
 
 ## Documentation
 
-If the package is imported into your own scripts, it provides functions which can be adapted to your own web server. Detailed information is available at:
+Detailed information is available at:
 
 https://indiredis.readthedocs.io
```

### Comparing `indiredis-0.6.0/indiredis/__init__.py` & `indiredis-0.7.1/indiredis/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -200,14 +200,16 @@
 #  hashedpassword = hash-of-password
 #  # web service host and port
 #  host = localhost
 #  port = 8000
 #
 #  # only one of the following [INDI], [MQTT] or [DRIVERS] should
 #  # be given. They are mutually exclusive.
+#  # If none are given the web client runs but the redis server must be
+#  # connected to drivers by some other process
 #
 #  [INDI]
 #  # indi server host and port
 #  ihost = localhost
 #  iport = 7624
 #
 #  [MQTT]
@@ -299,18 +301,19 @@
             print("Invalid web host:port")
             continue
         print("Value set at : " + newhp + "\n")
         q = input("OK (y/n)?")
         if q == "y" or q == "Y":
             break
 
-    print("\nYou can specify one of the following three:")
+    print("\nYou can specify one, or none, of the following three:")
     print("The host:port of an INDI server (which itself connects to instruments and drivers).")
     print("Or\nThe host:port of an MQTT server (which connect to instruments using the indi-mr package).")
-    print("Or\nA list of indi drivers, which in turn connect to instruments.\n")
+    print("Or\nA list of indi drivers, which in turn connect to instruments.")
+    print("Or\nNone of these, in which case the redis database should be connected\nto drivers by some other process.\n")
     q = input("Do you wish to connect to an INDI server (y/n)?")
     if q == "y" or q == "Y":
         while True:
             print("\nType in the host and port of the indi service to connect to,\nas colon separated host:number")
             newihp = input("Currently : " + ihp + "\nEnter to accept, or input new value>")
             if not newihp:
                 newihp = ihp
@@ -404,30 +407,29 @@
                 while True:
                     idstring = input("mqtt_id : ")
                     idstring = idstring.strip(" \"\'")
                     if not idstring:
                         break
                     remote_ids.add(dstring)
         else:
-            # neither indi nor mqtt servers, therfore should be drivers
-            q = input("\nDo you wish to define one or more drivers (y/n)?")
-            if q != "y" and q != "Y":
-                print("No other options are available. Exiting without creating config file")
-                sys.exit(0)
-            print("\nType a driver string and Enter, you will then be prompted for the next driver.")
-            print("Continue adding drivers, and then just press Enter without input to finish.")
-            while True:
-                dstring = input("Driver : ")
-                dstring = dstring.strip(" \"\'")
-                if not dstring:
-                    break
-                drivers.add(dstring)
-            if not drivers:
-                print("No drivers specified, no other options are available. Exiting without creating config file")
-                sys.exit(0)
+            # neither indi nor mqtt servers, therfore should be drivers or nothing
+            q = input("\nDo you wish to specify one or more drivers (y/n)?")
+            if q == "y" or q == "Y":
+                print("\nType a driver string and Enter, you will then be prompted for the next driver.")
+                print("Continue adding drivers, and then just press Enter without input to finish.")
+                while True:
+                    dstring = input("Driver : ")
+                    dstring = dstring.strip(" \"\'")
+                    if not dstring:
+                        break
+                    drivers.add(dstring)
+                if not drivers:
+                    print("No drivers specified, the config file will not contain these sections.")
+            else:
+                print("\nNo connectivity to drivers has been specified.")
 
     while True:
         print("\nType in the host and port of the redis service to connect to,\nas colon separated host:number")
         newrhp = input("Currently : " + rhp + "\nEnter to accept, or input new value>")
         if not newrhp:
             newrhp = rhp
         if ":" not in newrhp:
@@ -601,17 +603,14 @@
             configdict['subscribe_list'] = []
     elif 'DRIVERS' in config:
         drivers = config['DRIVERS']
         configdict['drivers'] = list(drivers.keys())
         if not configdict['drivers']:
             print("ERROR: No drivers given under DRIVERS.")
             sys.exit(1)
-    else:
-        print("ERROR: No INDI, MQTT or DRIVERS section in the config file.")
-        sys.exit(1)
     if 'REDIS' not in config:
         print("ERROR: The config file does not include a REDIS section.")
         sys.exit(1)
     redisparams = config['REDIS']
     configdict['rhost'] = redisparams.get('rhost', 'localhost')
     configdict['rport'] = redisparams.getint('rport', 6379)
     configdict['prefix'] = redisparams.get('prefix', 'indi_')
@@ -640,26 +639,30 @@
                               keyprefix=configdict['prefix'],
                               to_indi_channel=configdict['toindipub'],
                               from_indi_channel=configdict['fromindipub'])
 
     # create a wsgi application
     application = make_wsgi_app(redis_host, configdict['blob_folder'], url='/', hashedpassword=configdict['hashedpassword'])
 
-    # serve the application with the python waitress web server in another thread
-    webapp = threading.Thread(target=serve, args=(application,), kwargs={'host':configdict['host'], 'port':configdict['port']})
-    webapp.start()
-
-    if "ihost" in configdict:
-        indi_host = indi_server(host=configdict["ihost"], port=configdict["iport"])
-        # start the blocking function inditoredis
-        inditoredis(indi_host, redis_host, log_lengths={}, blob_folder=configdict['blob_folder'])
-    elif "mhost" in configdict:
-        mqtt_host = mqtt_server(host=configdict["mhost"], port=configdict["mport"],
-                                to_indi_topic = configdict['to_indi_topic'],
-                                from_indi_topic = configdict['from_indi_topic'],
-                                snoop_control_topic = configdict['snoop_control_topic'],
-                                snoop_data_topic = configdict['snoop_data_topic'] )
-        # start the blocking function mqtttoredis
-        mqtttoredis(configdict['mqtt_id'], mqtt_host, redis_host, subscribe_list=configdict['subscribe_list'], blob_folder=configdict['blob_folder'])
-    elif "drivers" in configdict:
-        # start the blocking function driverstoredis
-        driverstoredis(configdict['drivers'], redis_host, blob_folder=configdict['blob_folder'])
+    if ("ihost" in configdict) or ("mhost" in configdict) or ("drivers" in configdict):
+        # serve the application with the python waitress web server in another thread
+        webapp = threading.Thread(target=serve, args=(application,), kwargs={'host':configdict['host'], 'port':configdict['port']})
+        webapp.start()
+
+        if "ihost" in configdict:
+            indi_host = indi_server(host=configdict["ihost"], port=configdict["iport"])
+            # start the blocking function inditoredis
+            inditoredis(indi_host, redis_host, log_lengths={}, blob_folder=configdict['blob_folder'])
+        elif "mhost" in configdict:
+            mqtt_host = mqtt_server(host=configdict["mhost"], port=configdict["mport"],
+                                    to_indi_topic = configdict['to_indi_topic'],
+                                    from_indi_topic = configdict['from_indi_topic'],
+                                    snoop_control_topic = configdict['snoop_control_topic'],
+                                    snoop_data_topic = configdict['snoop_data_topic'] )
+            # start the blocking function mqtttoredis
+            mqtttoredis(configdict['mqtt_id'], mqtt_host, redis_host, subscribe_list=configdict['subscribe_list'], blob_folder=configdict['blob_folder'])
+        elif "drivers" in configdict:
+            # start the blocking function driverstoredis
+            driverstoredis(configdict['drivers'], redis_host, blob_folder=configdict['blob_folder'])
+    else:
+        # blocking call which serves the application with the python waitress web server
+        serve(application, host=configdict['host'], port=configdict['port'])
```

### Comparing `indiredis-0.6.0/indiredis/__main__.py` & `indiredis-0.7.1/indiredis/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 indiserver should already be running in a separate process, for example,
 prior to running this script, in another terminal, run:
 indiserver -v indi_simulator_telescope indi_simulator_dome
 
 This script then creates the directory /path/to/blobfolder if it does not
 exist, and then communicates with the indiserver on localhost port 7624 and
 a redis server on localhost port 6379. It runs a web server on port 8000,
-so connecting with a browser to http://localhost:8000 
+so connecting with a browser to http://localhost:8000
 should enable you to view and control the connected instruments.
 """
 
 
 import threading, argparse
 
 from indi_mr import inditoredis, indi_server, redis_server
@@ -22,25 +22,26 @@
 # any wsgi web server can serve the wsgi application produced by make_wsgi_app,
 # in this example the web server 'waitress' is used
 
 from waitress import serve
 
 from . import make_wsgi_app
 
-
-version = "0.6.0"
+version = "0.7.1"
 
 if __name__ == "__main__":
 
 
     parser = argparse.ArgumentParser(usage="python3 -m indiredis [options] blobdirectorypath",
-        description="INDI web client communicating to indiserver and saving data to redis and to a BLOB directory.")
+        description="INDI web client communicating to indiserver and saving data to redis and to a BLOB directory.",
+        epilog="The --clientonly option disables the connection to indiserver, iport and ihost will be ignored. This requires the redis database to be connected to drivers by some other process, typically using functions from package indi-mr.")
     parser.add_argument("blobdirectorypath", help="Path of the directory where BLOB's will be set")
     parser.add_argument("-p", "--port", type=int, default=8000, help="Port of the web service (default 8000).")
     parser.add_argument("--host", default="localhost", help="Listenning IP address of the web service (default localhost).")
+    parser.add_argument("--clientonly", action="store_true", help="Do not connect to indiserver port.")
     parser.add_argument("--iport", type=int, default=7624, help="Port of the indiserver (default 7624).")
     parser.add_argument("--ihost", default="localhost", help="Hostname of the indiserver (default localhost).")
     parser.add_argument("--rport", type=int, default=6379, help="Port of the redis server (default 6379).")
     parser.add_argument("--rhost", default="localhost", help="Hostname of the redis server (default localhost).")
     parser.add_argument("--prefix", default="indi_", help="Prefix applied to redis keys (default indi_).")
     parser.add_argument("--toindipub", default="to_indi", help="Redis channel used to publish data to indiserver (default to_indi).")
     parser.add_argument("--fromindipub", default="from_indi", help="Redis channel on which data is published from indiserver (default from_indi).")
@@ -53,15 +54,27 @@
     indi_host = indi_server(host=args.ihost, port=args.iport)
     redis_host = redis_server(host=args.rhost, port=args.rport, db=0, password='', keyprefix=args.prefix,
                               to_indi_channel=args.toindipub, from_indi_channel=args.fromindipub)
 
     # create a wsgi application
     application = make_wsgi_app(redis_host, args.blobdirectorypath, url='/')
 
+<<<<<<< HEAD
 
     # serve the application with the python waitress web server in another thread
     webapp = threading.Thread(target=serve, args=(application,), kwargs={'host':args.host, 'port':args.port})
     webapp.start()
 
     # and start the blocking function inditoredis
     inditoredis(indi_host, redis_host, log_lengths={}, blob_folder=args.blobdirectorypath)
+=======
+    if args.clientonly:
+        # blocking call which serves the application with the python waitress web server
+        serve(application, host=args.host, port=args.port)
+    else:
+        # serve the application with the python waitress web server in another thread
+        webapp = threading.Thread(target=serve, args=(application,), kwargs={'host':args.host, 'port':args.port})
+        webapp.start()
+        # and start the blocking function inditoredis
+        inditoredis(indi_host, redis_host, log_lengths={}, blob_folder=args.blobdirectorypath)
 
+>>>>>>> 6f1160a9d49c1389e503389f35351870101dd24e
```

### Comparing `indiredis-0.6.0/indiredis/indiredis/data/defaults.json` & `indiredis-0.7.1/indiredis/indiredis/data/defaults.json`

 * *Files identical despite different names*

### Comparing `indiredis-0.6.0/indiredis/indiredis/data/project.json` & `indiredis-0.7.1/indiredis/indiredis/data/project.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'0.7.1'"}*

```diff
@@ -4317,9 +4317,9 @@
         "skipolelogo": 3001,
         "url_not_found": 2080,
         "validate_error": 2010,
         "w3_css": "skis,w3_css",
         "w3_theme_ski_css": 1008
     },
     "url": "/",
-    "version": "0.6.0"
+    "version": "0.7.1"
 }
```

### Comparing `indiredis-0.6.0/indiredis/indiredis/data/textblocks_json/en.json` & `indiredis-0.7.1/indiredis/indiredis/data/textblocks_json/en.json`

 * *Files identical despite different names*

### Comparing `indiredis-0.6.0/indiredis/indiredis/static/css/w3-theme-ski.css` & `indiredis-0.7.1/indiredis/indiredis/static/css/w3-theme-ski.css`

 * *Files identical despite different names*

### Comparing `indiredis-0.6.0/indiredis/indiredis/static/images/logo.svg` & `indiredis-0.7.1/indiredis/indiredis/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `indiredis-0.6.0/indiredis/indiredis/static/images/logo_icon16.svg` & `indiredis-0.7.1/indiredis/indiredis/static/images/logo_icon16.svg`

 * *Files identical despite different names*

### Comparing `indiredis-0.6.0/indiredis/webcode/authenticate.py` & `indiredis-0.7.1/indiredis/webcode/authenticate.py`

 * *Files identical despite different names*

### Comparing `indiredis-0.6.0/indiredis/webcode/blobs.py` & `indiredis-0.7.1/indiredis/webcode/blobs.py`

 * *Files identical despite different names*

### Comparing `indiredis-0.6.0/indiredis/webcode/devices.py` & `indiredis-0.7.1/indiredis/webcode/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     skicall.call_data.clear()
     if authenticate:
         skicall.call_data['authenticate'] = authenticate
     # If a password has been set, a logout button is displayed
     # since the user must have logged in to see this page
     # if no password, the logout button is not shown
     if not skicall.proj_data["hashedpassword"]:
-        skicall.page_data['logout', 'show'] = False 
+        skicall.page_data['logout', 'show'] = False
     rconn = skicall.proj_data["rconn"]
     redisserver = skicall.proj_data["redisserver"]
     checksum1 = ''
     # get last message
     message = tools.last_message(rconn, redisserver)
     if message:
         skicall.page_data['message', 'para_text'] = message
@@ -155,15 +155,15 @@
     redisserver = skicall.proj_data["redisserver"]
     # publish getProperties
     textsent = tools.getProperties(rconn, redisserver)
 
 
 def getDeviceProperties(skicall):
     "Sends getProperties request for a given device, and refresh properties page"
-    # gets device from page_data, which is set into skicall.call_data["device"] 
+    # gets device from page_data, which is set into skicall.call_data["device"]
     devicename = skicall.call_data.get("device","")
     if not devicename:
         raise FailPage("Device not recognised")
     rconn = skicall.proj_data["rconn"]
     redisserver = skicall.proj_data["redisserver"]
     # publish getProperties
     textsent = tools.getProperties(rconn, redisserver, device=devicename)
@@ -598,16 +598,16 @@
     redisserver = skicall.proj_data["redisserver"]
     element_list = ad["elements"]
     if not element_list:
         return
     # permission is one of ro, wo, rw
     if ad['perm'] == "wo":
         # permission is wo
-        if (ad['rule'] == "OneOfMany") and (len(element_list) == 1):
-            # only one element, but rule is OneOfMany, so must give an off/on choice, with button names name_on and name_off
+        if len(element_list) == 1:
+            # only one element, must give an off/on choice regardless of rule
             skicall.page_data['property_'+str(index),'setswitch', 'show'] = True
             skicall.page_data['property_'+str(index),'svradio', 'show'] = True
             eld = element_list[0]
             skicall.page_data['property_'+str(index),'svradio', 'col1'] = [eld['label'] + ":"]
             skicall.page_data['property_'+str(index),'svradio', 'col2'] = ["On", "Off"]
             skicall.page_data['property_'+str(index),'svradio', 'radiocol'] = [eld['name'] + "_on", eld['name'] + "_off"]
             skicall.page_data['property_'+str(index),'svradio', 'row_classes'] = ['', '']
@@ -658,16 +658,16 @@
             skicall.page_data['property_'+str(index),'svradio', 'row_classes'] = row_classes
 
         # set hidden fields on the form
         skicall.page_data['property_'+str(index),'setswitch', 'propertyname'] = ad['name']
         skicall.page_data['property_'+str(index),'setswitch', 'sectionindex'] = index
 
     elif ad['perm'] == "rw":
-        if (ad['rule'] == "OneOfMany") and (len(element_list) == 1):
-            # only one element, but rule is OneOfMany, so must give an off/on choice, with button names name_on and name_off
+        if len(element_list) == 1:
+            # only one element, must give an off/on choice regardless of rule
             skicall.page_data['property_'+str(index),'setswitch', 'show'] = True
             skicall.page_data['property_'+str(index),'svradio', 'show'] = True
             eld = element_list[0]
             skicall.page_data['property_'+str(index),'svradio', 'col1'] = [eld['label'] + ":"]
             skicall.page_data['property_'+str(index),'svradio', 'col2'] = ["On", "Off"]
             skicall.page_data['property_'+str(index),'svradio', 'radiocol'] = [eld['name'] + "_on", eld['name'] + "_off"]
             if eld['value'] == "On":
@@ -801,15 +801,15 @@
     for eld in element_list:
         contents.append([eld['label'] + ":", "black", ""]) # pale yellow is "#ffffcc"
         if eld['value'] == "Idle":
             contents.append([eld['value'], "white", "grey"])
         if eld['value'] == "Ok":
             contents.append([eld['value'], "white", "green"])
         if eld['value'] == "Busy":
-            contents.append([eld['value'], "white", "yellow"])
+            contents.append([eld['value'], "black", "yellow"])
         if eld['value'] == "Alert":
             contents.append([eld['value'], "white", "red"])
     skicall.page_data['property_'+str(index),'lvelements', 'contents'] = contents
 
 
 
 
@@ -989,16 +989,16 @@
 
 
 def check_for_device_change(skicall):
     """Called to update the properties page, which should occur every ten seconds"""
     # The page which has called for this update shows all the properties in
     # a particular group, and the device, group and checksums should all be present
     # in call_data
-    if (('device' not in skicall.call_data) or 
-        ('group' not in skicall.call_data) or 
+    if (('device' not in skicall.call_data) or
+        ('group' not in skicall.call_data) or
         ('checksum1' not in skicall.call_data) or
         ('checksum2' not in skicall.call_data)):
         # something wrong, divert to the home page
         skicall.page_data['JSONtoHTML'] = 'home'
         return
     rconn = skicall.proj_data["rconn"]
     redisserver = skicall.proj_data["redisserver"]
@@ -1018,15 +1018,15 @@
     # if checksum2 is unchanged, this means those items requiring a whole page refresh (groups, propertynames)
     # are unchanged, and therefore only a json refresh is needed
 
     if checksum2 != skicall.call_data['checksum2']:
         # the whole page needs refreshing, request the browser to make an html call
         skicall.page_data['JSONtoHTML'] = 'refreshproperties'
         return
-        
+
     #############################################################################################################
     # To reach this point, only those items which can be updated by json have changed, therefore do a json update
 
     if 'message' in pdict:
         skicall.page_data['message', 'para_text'] = pdict['message']
     if 'devicemessage' in pdict:
         skicall.page_data['devicemessage','para_text'] = pdict['devicemessage']
@@ -1040,16 +1040,16 @@
     # refresh numbervectors in this group only
 
     for index, ad in enumerate(att_list):
         # loops through each property, where ad is the attribute directory of the property
         # and index is the section index on the web page
         propertyname = ad['name']
         if propertyname not in numbervectors:
-            continue 
-        
+            continue
+
         # set the change into page data
         # items which may have changed:
         #            state
         #            timeout
         #            timestamp
         #            message
         #            elements:{name:number,...}
@@ -1079,9 +1079,7 @@
                 col2.append(eld['formatted_number'])
             skicall.page_data['property_'+str(index),'nvelements', 'col2'] = col2
 
     # as this new data is inserted into the page, the page data should now have the same
     # checksums as the generated checksums
 
     skicall.call_data['checksum1'] = checksum1
-
-
```

### Comparing `indiredis-0.6.0/indiredis/webcode/setvalues.py` & `indiredis-0.7.1/indiredis/webcode/setvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,88 +80,87 @@
         raise FailPage("Invalid data")
 
     if p != "property":
         raise FailPage("Invalid data")
 
     if (propertyindex, setstring, 'sectionindex') not in received_data:
         raise FailPage("Invalid data")
-    
+
     # sectionindex should be equal to the provided sectionindex
     if received_data[(propertyindex, setstring, 'sectionindex')] != sectionindex:
         raise FailPage("Invalid data")
 
     propertyname = received_data[propertyindex, setstring, 'propertyname']
 
     return devicename, propertyindex, sectionindex, propertyname
 
 
-
 def set_switch(skicall):
     "Responds to a submission to set a switch vector"
     rconn = skicall.proj_data["rconn"]
     redisserver = skicall.proj_data["redisserver"]
     devicename, propertyindex, sectionindex, propertyname = _check_received_data(skicall, 'setswitch')
     # get list of element names for this property
     names = tools.elements(rconn, redisserver, propertyname, devicename)
     if not names:
-        raise FailPage("Error parsing data")
+        raise FailPage(f"Error parsing data for device {devicename}, property {propertyname}")
     # initially set all element switch values to be Off
     valuedict = {nm:'Off' for nm in names}
     received_data = skicall.submit_dict['received_data']
     if (propertyindex, 'svradio', 'radio_checked') in received_data:
         # a value has been received from a radio control
         value = received_data[propertyindex, 'svradio', 'radio_checked']
         if len(names) == 1:
-            # only one element, can be either on or off
-            # this value is a string of the format name or name_on or name_off
+            onename = names[0]
+            # only one element
+            # this value could be a string of the format name_on or name_off
             if value.endswith("_on"):
                 ename = value[0:-3]
-                if ename in names:
+                if ename == onename:
                     valuedict = {ename : "On"}
                 else:
-                    raise FailPage("Error parsing data")
+                    raise FailPage(f"Error parsing data, received value {value} not recognised")
             elif value.endswith("_off"):
                 ename = value[0:-4]
-                if ename in names:
+                if ename == onename:
                     valuedict = {ename : "Off"}
                 else:
-                    raise FailPage("Error parsing data")
+                    raise FailPage(f"Error parsing data, received value {value} not recognised")
             else:
-                # only one value, but does not end in _on or _off
-                raise FailPage("Error parsing data")
+                raise FailPage(f"Error parsing data, received value {value} not recognised")
         else:
             # multiple names, but only one received, and to be set to On
             # however if value is noneoftheabove, then all should be Off
             if value != "noneoftheabove":
                 if value in names:
                     valuedict[value] = "On"
                 else:
-                    raise FailPage("Error parsing data")
+                    raise FailPage(f"Error parsing data, received value {value} not a recognised switch name.")
         data_sent = tools.newswitchvector(rconn, redisserver, propertyname, devicename, valuedict)
         # print(data_sent)
         if not data_sent:
             raise FailPage("Error sending data")
     elif (propertyindex, 'svcheckbox', 'checked') in received_data:
         # a dictionary of keys values has been received from a checkbox control
         value = received_data[propertyindex, 'svcheckbox', 'checked']
         # Only need keys, as all values of checked items are 'On'
         for ename in value.keys():
             if ename in names:
                 valuedict[ename] = "On"
             else:
-                raise FailPage("Error sending data")
+                raise FailPage(f"Error parsing data, received value {value} not recognised")
         data_sent = tools.newswitchvector(rconn, redisserver, propertyname, devicename, valuedict)
         # print(data_sent)
         if not data_sent:
-            raise FailPage("Error sending data")
+            raise FailPage("Error parsing data, received value not recognised")
     else:
         skicall.call_data["status"] = "Unable to parse received data"
         return
     set_state(skicall, sectionindex, "Busy")
-    skicall.call_data["status"] = f"Change to property {propertyname} has been submitted" 
+    skicall.call_data["status"] = f"Change to property {propertyname} has been submitted"
 
 
 # The Client must send all members of Number and Text vectors,
 # or may send just the members that change for other types.
 
 def set_text(skicall):
     "Responds to a submission to set a text vector"
@@ -329,20 +328,20 @@
             # This element is unchanged
             up_hide.append(None)
             down_hide.append(None)
             getfield3values.append(None)
             # elements[index] gives a dictionary of the element at this index position, sorted by label
             # and ['name'] gives it by name. Setting the inputdict value to None means no change
             inputdict[_safekey(elements[index]['name'])] = None
- 
+
     skicall.page_data[propertyindex,'nvinputtable', 'inputdict'] = inputdict
     skicall.page_data[propertyindex,'nvinputtable', 'up_hide'] = up_hide
     skicall.page_data[propertyindex,'nvinputtable', 'down_hide'] = down_hide
     skicall.page_data[propertyindex,'nvinputtable', 'getfield3'] = getfield3values
-    
+
 
 
 
 def down_number(skicall):
     "An arrow down has been pressed to decrement a numeric value on the page only - but not yet to be submitted"
     if skicall.ident_data:
         devicename = skicall.call_data["device"]
@@ -435,17 +434,17 @@
     else:
         down_hide[elementindex] = False
     getfield3values[elementindex] = formatted_value
 
     skicall.page_data[propertyindex,'nvinputtable', 'up_hide'] = up_hide
     skicall.page_data[propertyindex,'nvinputtable', 'down_hide'] = down_hide
     skicall.page_data[propertyindex,'nvinputtable', 'getfield3'] = getfield3values
-    
 
-    
+
+
 def toggle_blob(skicall):
     "toggles a blob vector between enabled, disabled"
     rconn = skicall.proj_data["rconn"]
     redisserver = skicall.proj_data["redisserver"]
     if skicall.ident_data:
         devicename = skicall.call_data["device"]
     else:
@@ -524,12 +523,7 @@
     set_state(skicall, sectionindex, "Busy")
     skicall.call_data["status"] = f"""The file has been submitted:
     Device name   : {devicename}
     Property name : {propertyname}
     Element name  : {elementname}
     Size          : {lenrxfile}
     Format        : {fext}"""
-
-
-
-
-
```

### Comparing `indiredis-0.6.0/pyproject.toml` & `indiredis-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indiredis"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License","Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.6.0"
+version = "0.7.1"
 description="An INDI web client for general Instrument control. If the package is run, it provides a web service for controlling instruments. If imported, it provides functions which can be adapted to your own web server."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords=['indi', 'client', 'astronomy', 'instrument']
-dependencies = ["skipole>=5.5.2", "indi-mr>=0.2.3", "paho-mqtt>=1.5.1", "redis>=3.5.3", "waitress>=1.4.4"]
+dependencies = ["skipole>=5.5.2", "indi-mr>=0.4.0", "paho-mqtt>=1.5.1", "redis>=3.5.3", "waitress>=1.4.4"]
 
 [project.urls]
 Documentation = "https://indiredis.readthedocs.io"
 Source = "https://github.com/bernie-skipole/indi"
```

### Comparing `indiredis-0.6.0/PKG-INFO` & `indiredis-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: indiredis
-Version: 0.6.0
+Version: 0.7.1
 Summary: An INDI web client for general Instrument control. If the package is run, it provides a web service for controlling instruments. If imported, it provides functions which can be adapted to your own web server.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Requires-Dist: skipole>=5.5.2
-Requires-Dist: indi-mr>=0.2.3
+Requires-Dist: indi-mr>=0.4.0
 Requires-Dist: paho-mqtt>=1.5.1
 Requires-Dist: redis>=3.5.3
 Requires-Dist: waitress>=1.4.4
 Project-URL: Documentation, https://indiredis.readthedocs.io
 Project-URL: Source, https://github.com/bernie-skipole/indi
 
 # indiredis
@@ -23,15 +23,15 @@
 
 This Python3 package provides an INDI web client for general Instrument control.
 
 INDI - Instrument Neutral Distributed Interface.
 
 See https://en.wikipedia.org/wiki/Instrument_Neutral_Distributed_Interface
 
-The package does not include indiserver or drivers, but is compatable with them, indiserver is an application (debian package indi-bin) which runs instrument drivers, and listens on port 7624. This client (or other INDI clients), can connect to this port and using an XML based protocol, control the connected instruments.
+The package does not include indiserver or drivers, but is compatable with them, indiserver is an application (debian package indi-bin) which runs instrument drivers, and listens on port 7624. This client can connect to this port, and then serves web pages allowing the user to control the connected instruments.
 
 Though the INDI protocol is generally used for astronomical instruments, it can work with any instrument if appropriate INDI drivers are available.
 
 If this indiredis package is imported it provides functions for running a web client connected to either: an INDI server port; an MQTT server; or directly to INDI instrument drivers.
 
 If indiredis is run with the python -m option, then the web client is started and connects to an INDI server port.
 
@@ -49,14 +49,16 @@
 
 The directory /path/to/blobfolder should be a path to a directory of your choice, where BLOB's (Binary Large Objects), such as images will be stored, it will be created if it does not exist. Then connecting with a browser to http://localhost:8000 should enable you to view and control the connected instruments.
 
 For further usage information, including setting ports and hosts, try:
 
 > python3 -m indiredis --help
 
+If the package is imported into your own scripts, it provides a runclient function which accepts a configuration file. This file specifies the INDI drivers to run, or the MQTT or indiserver connections to use. The function then runs the web client.
+
 
 ## Installation
 
 Server dependencies: A redis server (For debian systems; apt-get install redis-server), and indiserver with drivers (apt-get install indi-bin).
 
 For debian systems you may need apt-get install python3-pip, and then use whichever variation of the pip command required by your environment, one example being:
 
@@ -81,11 +83,11 @@
 redis - Python redis client.
 
 paho-mqtt - Python mqtt client.
 
 
 ## Documentation
 
-If the package is imported into your own scripts, it provides functions which can be adapted to your own web server. Detailed information is available at:
+Detailed information is available at:
 
 https://indiredis.readthedocs.io
```

