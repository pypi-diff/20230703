# Comparing `tmp/pioreactor_basic_auth_for_ui-0.0.1-py3-none-any.whl.zip` & `tmp/pioreactor_basic_auth_for_ui-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4145 bytes, number of entries: 9
+Zip file size: 4232 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      921 b- defN 23-Jul-03 00:54 pioreactor_basic_auth_for_ui/__init__.py
--rw-r--r--  2.0 unx      615 b- defN 23-Jul-03 00:54 pioreactor_basic_auth_for_ui/post_install.sh
+-rw-r--r--  2.0 unx      494 b- defN 23-Jul-03 01:03 pioreactor_basic_auth_for_ui/post_install.sh
 -rw-r--r--  2.0 unx      116 b- defN 23-Jul-02 21:00 pioreactor_basic_auth_for_ui/pre_uninstall.sh
--rw-r--r--  2.0 unx     1079 b- defN 23-Jul-03 00:54 pioreactor_basic_auth_for_ui-0.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      518 b- defN 23-Jul-03 00:54 pioreactor_basic_auth_for_ui-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 00:54 pioreactor_basic_auth_for_ui-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       81 b- defN 23-Jul-03 00:54 pioreactor_basic_auth_for_ui-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-03 00:54 pioreactor_basic_auth_for_ui-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      907 b- defN 23-Jul-03 00:54 pioreactor_basic_auth_for_ui-0.0.1.dist-info/RECORD
-9 files, 4358 bytes uncompressed, 2523 bytes compressed:  42.1%
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jul-03 12:39 pioreactor_basic_auth_for_ui-0.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      835 b- defN 23-Jul-03 12:39 pioreactor_basic_auth_for_ui-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 12:39 pioreactor_basic_auth_for_ui-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       81 b- defN 23-Jul-03 12:39 pioreactor_basic_auth_for_ui-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-03 12:39 pioreactor_basic_auth_for_ui-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      907 b- defN 23-Jul-03 12:39 pioreactor_basic_auth_for_ui-0.0.2.dist-info/RECORD
+9 files, 4554 bytes uncompressed, 2610 bytes compressed:  42.7%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: pioreactor_basic_auth_for_ui/post_install.sh
 Comment: 
 
 Filename: pioreactor_basic_auth_for_ui/pre_uninstall.sh
 Comment: 
 
-Filename: pioreactor_basic_auth_for_ui-0.0.1.dist-info/LICENSE.txt
+Filename: pioreactor_basic_auth_for_ui-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pioreactor_basic_auth_for_ui-0.0.1.dist-info/METADATA
+Filename: pioreactor_basic_auth_for_ui-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pioreactor_basic_auth_for_ui-0.0.1.dist-info/WHEEL
+Filename: pioreactor_basic_auth_for_ui-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pioreactor_basic_auth_for_ui-0.0.1.dist-info/entry_points.txt
+Filename: pioreactor_basic_auth_for_ui-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioreactor_basic_auth_for_ui-0.0.1.dist-info/top_level.txt
+Filename: pioreactor_basic_auth_for_ui-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pioreactor_basic_auth_for_ui-0.0.1.dist-info/RECORD
+Filename: pioreactor_basic_auth_for_ui-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioreactor_basic_auth_for_ui/post_install.sh

```diff
@@ -14,11 +14,7 @@
 auth.backend = "htpasswd"
 auth.backend.htpasswd.userfile = "/etc/lighttpd.user.htpasswd"
 auth.require = ( "" => ("method" => "basic", "realm" => "example", "require" => "valid-user") )
 EOL
 
 # enable mod
 sudo lighttpd-enable-mod basic-auth
-
-# user next needs to run a pio command
-echo "Next, execute:"
-echo "pio run change_ui_credentials <username> <password>"
```

## Comparing `pioreactor_basic_auth_for_ui-0.0.1.dist-info/LICENSE.txt` & `pioreactor_basic_auth_for_ui-0.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pioreactor_basic_auth_for_ui-0.0.1.dist-info/METADATA` & `pioreactor_basic_auth_for_ui-0.0.2.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 Metadata-Version: 2.1
 Name: pioreactor-basic-auth-for-ui
-Version: 0.0.1
+Version: 0.0.2
 Summary: Adding basic auth to the Pioreactor UI
 Home-page: 
 Author: Cameron Davidson-Pilon
 Author-email: hello@pioreactor.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pioreactor-basic-auth-for-ui
 
 
-This adds basic auth to your Pioreactor UI. 
+This adds basic auth to access your Pioreactor UI.
 
 > **Warning**
-> The web server is still HTTP. Malicious users _on your network_ can read any data going back and forth, including a hashed version of the user/name password.
+> The web server is still HTTP. Malicious users _on your network_ can read any data going back and forth, including an encoded version of the user/name password.
+
+
+## Installation
+
+1. On your leader Pioreactor, run
+```
+pio install-plugin pioreactor-basic-auth-for-ui
+```
+2. Next, execute:
+```
+pio run change_ui_credentials <ui_username> <ui_password>
+```
+3. Refresh the UI and you should be greeted with a pop up.
+4. Finally, you should restart the leader now, or later.
```

## Comparing `pioreactor_basic_auth_for_ui-0.0.1.dist-info/RECORD` & `pioreactor_basic_auth_for_ui-0.0.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 pioreactor_basic_auth_for_ui/__init__.py,sha256=hWcXYvRsx7aCTvN9unElwcOPN2CPdZ1LvXfIqg9zCkk,921
-pioreactor_basic_auth_for_ui/post_install.sh,sha256=j0hVLdOwfyZiflNhnQcMVSmXEYfuofEoh5rLosMfhxk,615
+pioreactor_basic_auth_for_ui/post_install.sh,sha256=ZiH0w1gAlNMmP7lITeR0PUw-ZdkS1iVnX4uobO4UJEA,494
 pioreactor_basic_auth_for_ui/pre_uninstall.sh,sha256=2WKXdkDT12X_g5wThfey9xc6ynWcnYYh_rpUe3Biamo,116
-pioreactor_basic_auth_for_ui-0.0.1.dist-info/LICENSE.txt,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
-pioreactor_basic_auth_for_ui-0.0.1.dist-info/METADATA,sha256=pBkXfnyi1qg7DNF6CNNSSGt0lBaJXzq1mp8zkwvn4XI,518
-pioreactor_basic_auth_for_ui-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pioreactor_basic_auth_for_ui-0.0.1.dist-info/entry_points.txt,sha256=zRMF8Q3XmiqG4iS1HFX2jeYP9spwssC4cUnf4bCoeIM,81
-pioreactor_basic_auth_for_ui-0.0.1.dist-info/top_level.txt,sha256=P8Y7wsgMRz6C9u3bPNoXTZcR5lK18DPwG13YcNQ5veM,29
-pioreactor_basic_auth_for_ui-0.0.1.dist-info/RECORD,,
+pioreactor_basic_auth_for_ui-0.0.2.dist-info/LICENSE.txt,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
+pioreactor_basic_auth_for_ui-0.0.2.dist-info/METADATA,sha256=mQu1DyUs6e99XXN56PnEgmR4wW9MRpQIiDXnCGdJmvI,835
+pioreactor_basic_auth_for_ui-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pioreactor_basic_auth_for_ui-0.0.2.dist-info/entry_points.txt,sha256=zRMF8Q3XmiqG4iS1HFX2jeYP9spwssC4cUnf4bCoeIM,81
+pioreactor_basic_auth_for_ui-0.0.2.dist-info/top_level.txt,sha256=P8Y7wsgMRz6C9u3bPNoXTZcR5lK18DPwG13YcNQ5veM,29
+pioreactor_basic_auth_for_ui-0.0.2.dist-info/RECORD,,
```

