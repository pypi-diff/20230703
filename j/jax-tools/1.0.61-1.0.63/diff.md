# Comparing `tmp/jax-tools-1.0.61.tar.gz` & `tmp/jax-tools-1.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-tools-1.0.61.tar", last modified: Tue Jun 27 07:13:39 2023, max compression
+gzip compressed data, was "jax-tools-1.0.63.tar", last modified: Mon Jul  3 01:29:30 2023, max compression
```

## Comparing `jax-tools-1.0.61.tar` & `jax-tools-1.0.63.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.747789 jax-tools-1.0.61/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-27 07:13:39.747499 jax-tools-1.0.61/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      580 2023-06-02 08:47:19.000000 jax-tools-1.0.61/README.md
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.711933 jax-tools-1.0.61/jax_tools/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.61/jax_tools/__init__.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.725444 jax-tools-1.0.61/jax_tools/cmd/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 10:01:41.000000 jax-tools-1.0.61/jax_tools/cmd/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      245 2023-06-02 10:08:59.000000 jax-tools-1.0.61/jax_tools/cmd/jax.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1609 2023-06-06 02:34:28.000000 jax-tools-1.0.61/jax_tools/cmd/jax_encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      643 2023-06-06 03:32:23.000000 jax-tools-1.0.61/jax_tools/cmd/jax_fix.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.61/jax_tools/cmd/jax_nd.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1737 2023-06-21 02:57:30.000000 jax-tools-1.0.61/jax_tools/cmd/jax_pam.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.61/jax_tools/cmd/nd.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.727907 jax-tools-1.0.61/jax_tools/cmd_tools/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 02:29:37.000000 jax-tools-1.0.61/jax_tools/cmd_tools/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     8063 2023-06-25 00:48:51.000000 jax-tools-1.0.61/jax_tools/cmd_tools/pam.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     6271 2023-06-27 02:06:15.000000 jax-tools-1.0.61/jax_tools/colorful_font.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     4444 2023-06-06 02:37:59.000000 jax-tools-1.0.61/jax_tools/encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 08:32:18.000000 jax-tools-1.0.61/jax_tools/logger.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     3301 2023-06-02 11:00:20.000000 jax-tools-1.0.61/jax_tools/network_test.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      651 2023-06-02 07:00:58.000000 jax-tools-1.0.61/jax_tools/proxies.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     2772 2023-06-06 03:34:47.000000 jax-tools-1.0.61/jax_tools/ssh.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.746594 jax-tools-1.0.61/jax_tools/utils/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.61/jax_tools/utils/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      254 2023-06-01 08:29:19.000000 jax-tools-1.0.61/jax_tools/utils/settings.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.716149 jax-tools-1.0.61/jax_tools.egg-info/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      657 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      224 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/entry_points.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       83 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/requires.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/top_level.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-27 07:13:39.747896 jax-tools-1.0.61/setup.cfg
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1963 2023-06-27 07:13:39.000000 jax-tools-1.0.61/setup.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-07-03 01:29:30.530545 jax-tools-1.0.63/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-07-03 01:29:30.530121 jax-tools-1.0.63/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      580 2023-06-02 08:47:19.000000 jax-tools-1.0.63/README.md
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-07-03 01:29:30.520825 jax-tools-1.0.63/jax_tools/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.63/jax_tools/__init__.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-07-03 01:29:30.527238 jax-tools-1.0.63/jax_tools/cmd/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 10:01:41.000000 jax-tools-1.0.63/jax_tools/cmd/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      245 2023-06-02 10:08:59.000000 jax-tools-1.0.63/jax_tools/cmd/jax.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1609 2023-06-06 02:34:28.000000 jax-tools-1.0.63/jax_tools/cmd/jax_encrypt.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      643 2023-06-06 03:32:23.000000 jax-tools-1.0.63/jax_tools/cmd/jax_fix.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.63/jax_tools/cmd/jax_nd.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1737 2023-06-21 02:57:30.000000 jax-tools-1.0.63/jax_tools/cmd/jax_pam.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.63/jax_tools/cmd/nd.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-07-03 01:29:30.528221 jax-tools-1.0.63/jax_tools/cmd_tools/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 02:29:37.000000 jax-tools-1.0.63/jax_tools/cmd_tools/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     8063 2023-06-25 00:48:51.000000 jax-tools-1.0.63/jax_tools/cmd_tools/pam.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     6271 2023-06-27 02:06:15.000000 jax-tools-1.0.63/jax_tools/colorful_font.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     4444 2023-06-06 02:37:59.000000 jax-tools-1.0.63/jax_tools/encrypt.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 08:32:18.000000 jax-tools-1.0.63/jax_tools/logger.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     3301 2023-06-02 11:00:20.000000 jax-tools-1.0.63/jax_tools/network_test.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      651 2023-06-02 07:00:58.000000 jax-tools-1.0.63/jax_tools/proxies.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     4060 2023-07-03 01:29:09.000000 jax-tools-1.0.63/jax_tools/ssh.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-07-03 01:29:30.529448 jax-tools-1.0.63/jax_tools/utils/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.63/jax_tools/utils/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      254 2023-06-01 08:29:19.000000 jax-tools-1.0.63/jax_tools/utils/settings.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-07-03 01:29:30.523720 jax-tools-1.0.63/jax_tools.egg-info/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-07-03 01:29:30.000000 jax-tools-1.0.63/jax_tools.egg-info/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      657 2023-07-03 01:29:30.000000 jax-tools-1.0.63/jax_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-07-03 01:29:30.000000 jax-tools-1.0.63/jax_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      224 2023-07-03 01:29:30.000000 jax-tools-1.0.63/jax_tools.egg-info/entry_points.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       83 2023-07-03 01:29:30.000000 jax-tools-1.0.63/jax_tools.egg-info/requires.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-07-03 01:29:30.000000 jax-tools-1.0.63/jax_tools.egg-info/top_level.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-07-03 01:29:30.530707 jax-tools-1.0.63/setup.cfg
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1963 2023-07-03 01:29:30.000000 jax-tools-1.0.63/setup.py
```

### Comparing `jax-tools-1.0.61/PKG-INFO` & `jax-tools-1.0.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-tools
-Version: 1.0.61
+Version: 1.0.63
 Summary: Jax common tools library
 Home-page: https://jax-arsenals.com
 Download-URL: https://jax-arsenals.com
 Author: Jax
 Author-email: alvin.wan.cn@hotmail.com
 License: MIT Licence
 Keywords: jax
```

### Comparing `jax-tools-1.0.61/README.md` & `jax-tools-1.0.63/README.md`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/jax_tools/cmd/jax_encrypt.py` & `jax-tools-1.0.63/jax_tools/cmd/jax_encrypt.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/jax_tools/cmd/jax_fix.py` & `jax-tools-1.0.63/jax_tools/cmd/jax_fix.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/jax_tools/cmd/jax_pam.py` & `jax-tools-1.0.63/jax_tools/cmd/jax_pam.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/jax_tools/cmd_tools/pam.py` & `jax-tools-1.0.63/jax_tools/cmd_tools/pam.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/jax_tools/colorful_font.py` & `jax-tools-1.0.63/jax_tools/colorful_font.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/jax_tools/encrypt.py` & `jax-tools-1.0.63/jax_tools/encrypt.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/jax_tools/logger.py` & `jax-tools-1.0.63/jax_tools/logger.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/jax_tools/network_test.py` & `jax-tools-1.0.63/jax_tools/network_test.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/jax_tools/proxies.py` & `jax-tools-1.0.63/jax_tools/proxies.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/jax_tools/ssh.py` & `jax-tools-1.0.63/jax_tools/ssh.py`

 * *Files 23% similar despite different names*

```diff
@@ -82,14 +82,54 @@
             else:
                 result = std_out.read().decode('utf-8').rstrip()
         except Exception as e:
             logger.error('Connection exception, User login info may be wrong, or connection has been closed, '
                          ' msg: %s' % e)
         return result
 
+    def put_file(self, local_file, remote_file):
+        """
+        Put file to remote host
+        Args:
+            local_file (str): local file path
+            remote_file (str): remote file path
+
+        Returns:
+
+        """
+        if self.ssh_client is None:
+            logger.warning('SSH connection failed')
+            return
+        try:
+            sftp_client = self.ssh_client.open_sftp()
+            sftp_client.put(local_file, remote_file)
+        except Exception as e:
+            logger.error('Connection exception, User login info may be wrong, or connection has been closed, '
+                         ' msg: %s' % e)
+
+    def get_file(self, remote_file, local_file):
+        """
+        Get file from remote host
+        Args:
+            remote_file (str): remote file path
+            local_file (str): local file path
+
+        Returns:
+
+        """
+        if self.ssh_client is None:
+            logger.warning('SSH connection failed')
+            return
+        try:
+            sftp_client = self.ssh_client.open_sftp()
+            sftp_client.get(remote_file, local_file)
+        except Exception as e:
+            logger.error('Connection exception, User login info may be wrong, or connection has been closed, '
+                         ' msg: %s' % e)
+
     def close(self) -> None:
         """
         Close ssh connection
         Returns:
 
         """
         self.ssh_client.close()
```

### Comparing `jax-tools-1.0.61/jax_tools.egg-info/PKG-INFO` & `jax-tools-1.0.63/jax_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-tools
-Version: 1.0.61
+Version: 1.0.63
 Summary: Jax common tools library
 Home-page: https://jax-arsenals.com
 Download-URL: https://jax-arsenals.com
 Author: Jax
 Author-email: alvin.wan.cn@hotmail.com
 License: MIT Licence
 Keywords: jax
```

### Comparing `jax-tools-1.0.61/jax_tools.egg-info/SOURCES.txt` & `jax-tools-1.0.63/jax_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.61/setup.py` & `jax-tools-1.0.63/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
     with open(file_path, 'r') as f:
         return f.read()
 
 
 setuptools.setup(
     name="jax-tools",
-    version="1.0.61",
+    version="1.0.63",
     author=u"Jax",
     author_email='alvin.wan.cn@hotmail.com',
     description=u"Jax common tools library",
     platforms=['CentOS', 'Redhat', 'MacOS', 'Windows'],
     long_description=read_file('README.md'),
     long_description_content_type="text/markdown",
     url="https://jax-arsenals.com",
```

