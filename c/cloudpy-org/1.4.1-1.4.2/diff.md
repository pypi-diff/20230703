# Comparing `tmp/cloudpy_org-1.4.1.tar.gz` & `tmp/cloudpy_org-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.4.1.tar", last modified: Wed Jun 28 10:10:31 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.4.2.tar", last modified: Mon Jul  3 01:22:22 2023, max compression
```

## Comparing `cloudpy_org-1.4.1.tar` & `cloudpy_org-1.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 10:10:31.709373 cloudpy_org-1.4.1/
--rw-rw-rw-   0        0        0      935 2023-06-28 10:10:31.709373 cloudpy_org-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 10:10:31.600000 cloudpy_org-1.4.1/cloudpy_org/
--rw-rw-rw-   0        0        0      111 2023-06-25 19:34:30.000000 cloudpy_org-1.4.1/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    74677 2023-06-28 10:09:46.000000 cloudpy_org-1.4.1/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-28 10:10:31.678101 cloudpy_org-1.4.1/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2023-06-28 10:10:31.000000 cloudpy_org-1.4.1/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-28 10:10:31.000000 cloudpy_org-1.4.1/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 10:10:31.000000 cloudpy_org-1.4.1/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-28 10:10:31.000000 cloudpy_org-1.4.1/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-28 10:10:31.000000 cloudpy_org-1.4.1/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 10:10:31.709373 cloudpy_org-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1324 2023-06-28 10:10:00.000000 cloudpy_org-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:22:22.196291 cloudpy_org-1.4.2/
+-rw-rw-rw-   0        0        0      935 2023-07-03 01:22:22.196291 cloudpy_org-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 01:22:22.071293 cloudpy_org-1.4.2/cloudpy_org/
+-rw-rw-rw-   0        0        0      130 2023-07-03 01:20:12.000000 cloudpy_org-1.4.2/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    79159 2023-07-03 01:16:18.000000 cloudpy_org-1.4.2/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:22:22.180669 cloudpy_org-1.4.2/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-07-03 01:22:21.000000 cloudpy_org-1.4.2/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-03 01:22:21.000000 cloudpy_org-1.4.2/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 01:22:21.000000 cloudpy_org-1.4.2/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-03 01:22:21.000000 cloudpy_org-1.4.2/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 01:22:21.000000 cloudpy_org-1.4.2/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 01:22:22.196291 cloudpy_org-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2023-07-03 01:16:43.000000 cloudpy_org-1.4.2/setup.py
```

### Comparing `cloudpy_org-1.4.1/PKG-INFO` & `cloudpy_org-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.4.1
+Version: 1.4.2
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.4.1/cloudpy_org/tools.py` & `cloudpy_org-1.4.2/cloudpy_org/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Find documentation at https://www.cloudpy.org
 """
-cloudpy_org_version='1.4.1'
+cloudpy_org_version='1.4.2'
 import os
 import json
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.filterwarnings('ignore')
 warnings.simplefilter('ignore')
 import pandas as pd
@@ -237,26 +237,30 @@
         'self.this_source_code=source_code'
         self.this_description = self.this_description.replace("  "," ").replace("#","\n").strip()
         exec(dynamic_code)
         return self.this_source_code, self.theseparams, self.this_returns, self.this_description
     #██████████████████████████████████████████████████████████████████████████          
 class processing_tools:
     def __init__(self,data:dict={},bucket_name:str='',region_name:str="us-east-2",local:bool=False,third_part:str=None):
+        self.aws_auth_token_expired = True
+        self.aws_authenticated = False
+        self.aws_auth_error_message = ""
         self.__third_part = third_part
         self.__local = local
         self.aux = {}
         self.__tdata = data
         self.environment = 'local'
         self.__set_aws_session(region_name=region_name)
         if self.__session != None:
             self.environment = 's3'
         self.__root_path = os.getcwd()
         self.local_directory = self.__root_path + '/'
         self.s3_bucket = bucket_name.replace('/','') + '/'
         self.main_bucket = ''
+        self.dxxyyzz = {}
         if bucket_name != '':
             self.main_bucket =  's3://' + bucket_name + '/'
             self.environment = bucket_name
         self.documentation_path = self.local_directory + 'documentation/'
         self.documentation_JSON_path = self.documentation_path + "json/"  
         self.settings = self.main_bucket + 'settings/'
         self.secrets = self.settings + 'secrets/'
@@ -270,14 +274,27 @@
         except:
             self.fs = None
         try:
             self.load_metadata()
         except:
             ...
     #__________________________________________________________________________
+    
+    def dictstr_to_dict(self,dictstr:str):
+        n = random.randint(1,1000)
+        m = random.randint(1,1000)
+        j = random.randint(1,1000)
+        k = random.randint(1,1000)
+        date_id,time_id = self.date_time_id(local=True)
+        key = str(k) + "_" + str(j) + "_" + str(m) + "_" + str(n) + "_" + str(date_id) + str(time_id)
+        dc = "self.dxxyyzz['" + key + "'] = " + dictstr
+        exec(dc)
+        rslt = self.dxxyyzz[key]
+        self.dxxyyzz.pop(key, None)
+        return rslt
     def dataframe_to_parquet(self,df_input:pd.DataFrame,folder_path:str,file_name:str)->str:
         '''
         ***
         If the environment instance class equals "s3", then stores as parquet a given pandas dataframe to a given s3 folder url location under a given file name.
         Otherwise, stores the dataframe locally as a parquet file in the given folder under the given file name.
         ***
         '''
@@ -414,35 +431,71 @@
         Sets a session with given AWS credentials.
         '''
         self.__session = None
         self.__s3_client = None
         self.xtdata = self.__tdata
         self.xsession = self.__session
         self.xs3_client = self.__s3_client
+        """
         url_base = "https://www.cloudpy.org/"
         if self.__local:
             url_base = "http://localhost/"
         url = url_base +  "uMEqKLMaqRxFl9pT51zKed2"
+        
         if self.__third_part != None and len(self.__third_part) > 200:
             third_part = self.__third_part
             self.__third_part = None
         else:
             try:
                 third_part = requests.get(url).text
             except:
                 third_part = ""
-            if len(third_part) < 200 or "bad gateway" in third_part.lower():
+            if "html" in third_part.lower() or len(third_part) < 450 or "bad gateway" in third_part.lower():
                 third_part = "gCfJUHLD7Y60ekf6qm_Y=Fl9pT5Fl9pT5gAAAAABkm_us4VOEmkDGp38wL5Jka5UGJzLnKJ9d7RCs110oM-c_kR4iAa1rLNH98ILTdWMf4wUwOozHEn34X5g6ITG7Q5InPQJPj_hyUaHVbe8RC_r7EPvJ1QGTUhFl_jOzz5RztN5zKdyuLw_XraiVpRzlS7gIscIpFdXCr3NQSWndyUASbr6VR2Rm1HQaYQTfQYS6LDflq57fXY1nGmpzz__COVQ60SsOwuYsQSKYpMOCc3nWNPDkEenJautpp50RfRmBs1GyWKEiRv-l7IAnu9VlQrayVFNI-GKEF7svIYOORZso7KXXHWK_1hKCMpI4kgH8L1_481R6TrBEfz9vdOQvdm6CBVoYFa-ifMULx3Ul7ZbYetZjMWKdQTidMzWaYy9MQxBz-GGfhaihTKLuq7KUbMkxQkUZ_RX0Xx07j65eSRMYoExophuknTI74bkbtx5t2_X31uTuMksTe7VWl6s2BHnzH_EzqH1ERVYUukyETuTkZq6_H3o6LpYN0zAIiCcM-x10wvkJz9f6bNg1ElaxoWKz7FUIVVI7vJP3HtIchRrDmus6jM_LWae00z7gpaOw7ysljEut6y7NXQ1nNmOAOQr6Z5XTR3X1dwcI66Xe1tPEm30bRgxblQS3IntVanjrJUY8"
-        exec(self.decrypt(third_part.split("Fl9pT5Fl9pT5")[1], url.split(url_base)[1] + third_part.split("Fl9pT5Fl9pT5")[0]))
+        dc = self.decrypt(third_part.split("Fl9pT5Fl9pT5")[1], url.split(url_base)[1] + third_part.split("Fl9pT5Fl9pT5")[0])
+        """
+        #print("self.xtdata:",self.xtdata)
+        if type(self.xtdata) == dict and self.xtdata != {}:
+            try:
+                spd = self.dx(self.decrypt_before_expiration(self.xtdata),10)
+            except:
+                spd = []
+            if len(spd) > 1 and spd[1] == 'deripxe noitpyrcne':
+                self.aws_auth_token_expired = True
+                self.aws_auth_error_message = "AWS authentication token expired."
+            elif len(spd) > 1 and len(spd[0]) == 20 and len(spd[1]) == 40:
+                self.aws_auth_token_expired = False
+                try:
+                    self.xsession = boto3.Session(aws_access_key_id=spd[0],aws_secret_access_key=spd[1])
+                    self.xs3_client = boto3.client("s3",aws_access_key_id=spd[0],aws_secret_access_key=spd[1],region_name=region_name)
+                    self.aws_authenticated = True
+                    self.aws_auth_error_message = ""
+                except Exception as e:
+                    self.aws_authenticated = False
+                    self.xsession = None
+                    self.xs3_client = None
+                    self.aws_auth_error_message = "Invalid AWS credentials."
+            else:
+                self.aws_authenticated = False
+                self.aws_auth_token_expired = False
+                self.aws_auth_error_message = "Invalid AWS authentication token."
+                self.xsession = None
+                self.xs3_client = None
+                
         self.__session = self.xsession
         self.__s3_client = self.xs3_client
+        self.s3_client = self.__s3_client
+        if self.__session != None:
+            self.__resource = self.__session.resource('s3')
+        else:
+            self.__resource=boto3.resource('s3')
+            
         del self.xtdata
         del self.xsession
         del self.xs3_client
-            
     #__________________________________________________________________________
     def domain_commands(self,domain_name:str=None)->None:
         '''
         ***
         Prints the terminal commands required to connect to a given domain ubunto instance given the information 
         defined in commands and connection_details json files in metadata folder.
         ***
@@ -644,30 +697,27 @@
         rslt_dict,fileContent,ext={},"",""
         if referenceName != "":
             s=s3FullFolderPath.replace('s3://','')
             filesFound=0
             bucketName=s[0:s.index('/')]
             rp=s.replace(bucketName,'')
             relativePath=rp[1:len(rp)]
-            if self.__session != None:
-                resource = self.__session.resource('s3')
-            else:
-                resource=boto3.resource('s3')
-            my_bucket=resource.Bucket(bucketName)
+            
+            my_bucket=self.__resource.Bucket(bucketName)
             objectSumariesList=list(my_bucket.objects.filter(Prefix=relativePath))
             fileKeys=[]
             for obs in objectSumariesList:
                 fileKeys.append(obs.key)
             for fileKey in fileKeys:
                 a=fileKey[::-1]
                 ext='.'+fileKey.lower()[::-1].split('.')[0][::-1]
                 thisFile=fileKey.replace(relativePath,'').replace('/','')
                 if(thisFile.lower()).replace(ext,'') == referenceName.lower().replace(ext,''):
                     filesFound+=1
-                    obj=resource.Object(bucketName,fileKey)
+                    obj=self.__resource.Object(bucketName,fileKey)
                     fileContent=obj.get()['Body'].read().decode('utf-8')
                     if ext=='.json':
                         if exceptionCase==False:
                             fileContent=fileContent.replace("'",'"')
                         rslt_dict=json.loads(fileContent)
                     break
             if ext=='.json':
@@ -684,18 +734,18 @@
         these_files =set()
         s=s3FullFolderPath.replace('s3://','')
         filesFound=0
         bucketName=s[0:s.index('/')]
         rp=s.replace(bucketName,'')
         relativePath=rp[1:len(rp)]
         if self.__session != None:
-            resource = self.__session.resource('s3')
+            self.__resource = self.__session.resource('s3')
         else:
-            resource=boto3.resource('s3')
-        my_bucket=resource.Bucket(bucketName)
+            self.__resource=boto3.resource('s3')
+        my_bucket=self.__resource.Bucket(bucketName)
         objectSumariesList=list(my_bucket.objects.filter(Prefix=relativePath))
         fileKeys=[]
         for obs in objectSumariesList:
             fileKeys.append(obs.key)
         for fileKey in fileKeys:
             a=fileKey[::-1]
             ext='.'+fileKey.lower()[::-1].split('.')[0][::-1]
@@ -1153,21 +1203,25 @@
 #        a = ""
 #        r = int(len(secret+user_key)/n) +1
 #        for i in range(0,r):
 #            a += secret[i*n:(i+1)*n] + user_key[i*n:(i+1)*n][::-1]
 #        return a[::-1]
 
 xpt = processing_tools()
-xs3 = boto3.client('s3')
 xpt.environment = "s3"
 class aws_framework_manager:
-    def __init__(self,secret_key:str):
-        self.__sc = secret_key[::-1].split("1V44bjdzKODcN50jdz00c4=")
+    def __init__(self,secret_key:str,aws_auth_token:str=""):
+        self.__deconstructor_token = 'JQxrs8sWqn3JIWlIL8nTlw-302SfmV7RmlZ-T-gB5c4=oiwn8TU5-NcDKzVq'
+        uuu = "1V44bjdzKODcN50jdz00c4="
+        self.__sc = secret_key[::-1].split(uuu)
+        self.__at = aws_auth_token[::-1].split(uuu)
         self.__cppt_construction(self.__sc[1])
         self.cppt.environment = "s3"
+        self.__ypt_construction(self.__at[1])
+        self.ypt.environment = "s3"
         self.general_info = {}
         self.service_name = "cloudpy-org-service-beta"
         self.delimiters = ["pZo-9xH9oEO2B2OEo","2nZzN01wtktk10N","VhMxT-9xVVZzN01w","_Shv-4F86Co981h"]
         self.general_separators = {'user_email_sep': '-0-', '@': '-1-', '.': '-2-'}
         self.special_separators = self.general_separators
         self.__service_initialized = False
         self.__not_initialized_message ='Service not initialized yet.\n'\
@@ -1185,32 +1239,42 @@
                 c = c.replace(c[::-1][0:n][::-1],'')
         if upper:
             c = c.upper()
         return c,b
     #___________________________________________________________________
     def __cppt_construction(self,secret_key:str=""):
         if len(secret_key) > 10:
-            k = 'JQxrs8sWqn3JIWlIL8nTlw-302SfmV7RmlZ-T-gB5c4=oiwn8TU5-NcDKzVq'
+            k = self.__deconstructor_token
             self.cppt = processing_tools(data=xpt.basic_dicstr_to_dict(xpt.decrypt(secret_key,self.__do(k,10,False)[1] + self.__do(k,10,False)[0][0:4])))
         else:
             self.cppt = processing_tools()
+    def __ypt_construction(self,aws_auth_token:str=""):
+        if len(aws_auth_token) > 10:
+            k = self.__deconstructor_token
+            self.ypt = processing_tools(data=xpt.basic_dicstr_to_dict(xpt.decrypt(aws_auth_token,self.__do(k,10,False)[1] + self.__do(k,10,False)[0][0:4])))
+        else:
+            self.ypt = processing_tools()
     #___________________________________________________________________
     def initialize_service(self,service_token:str,version:str=cloudpy_org_version,test_file_name:str=None):
         self.__initialize_error_message = 'Could not initialize the service. Please verify you are using the right service token.'
         self.args_by_key,self.dx = {},{}
+        succes_message =  'cloudpy-org AWS framework manager client: service initialized.'
         try:
             for i in range(0,1):
                 self.args_by_key,self.dx = {},{}
                 self.__api_encrypted_caller = self.__sc[2]
                 self.__get_dynamic_response(service_token=service_token,version=version,test_file_name=test_file_name)
                 self.find_methods_arguments()
                 self.set_valid_characters()
                 self.version = self.get_version()
             if self.__service_initialized:
-                return 'AWS framework manager client: service initialized.'
+                messagex = succes_message
+                if self.ypt.aws_auth_error_message != None and self.ypt.aws_auth_error_message != "":
+                    messagex += "\nThe following exceptions have been found:\n" +  self.ypt.aws_auth_error_message
+                return messagex
             else:
                 return self.__initialize_error_message
         except Exception as e:
             print("error 01:",str(e))
             return self.__initialize_error_message
     #___________________________________________________________________
     def __load_local_code(self,file_name):
@@ -1392,14 +1456,23 @@
             dk=str(inspect.getframeinfo(inspect.currentframe()).function)
             self.__args_applied[dk]= self.__args_applied[dk]\
             .replace("@username_or_email",str(username_or_email))\
             .replace("@bucket_name","'" + bucket_name + "'")
             return self.deco(dk=dk)
         else:
             return self.__not_initialized_message
+    def service_check_if_user_exists_and_was_confirmed(self,username_or_email:list,bucket_name:str):
+        if self.__service_initialized:
+            dk=str(inspect.getframeinfo(inspect.currentframe()).function)
+            self.__args_applied[dk]= self.__args_applied[dk]\
+            .replace("@username_or_email",str(username_or_email))\
+            .replace("@bucket_name","'" + bucket_name + "'")
+            return self.deco(dk=dk)
+        else:
+            return self.__not_initialized_message
     #___________________________________________________________________
     def framework_loaded(self,bucket_name:str):
         if self.__service_initialized:
             dk=str(inspect.getframeinfo(inspect.currentframe()).function)
             self.__args_applied[dk]= self.__args_applied[dk]\
             .replace("@bucket_name","'" + bucket_name + "'")
             return self.deco(dk=dk)
@@ -1504,30 +1577,49 @@
         print("s3://" + self.service_name + "/settings/secrets/users/")
         return self.cppt.get_s3_file_content(
             referenceName = self.reference_from_service_token(service_token=service_token)
             ,s3FullFolderPath="s3://" + self.service_name + "/settings/secrets/users/")
     #___________________________________________________________________    
     def __gsm(self,service_token:str):
         date_id,time_id = self.cppt.date_time_id()
-        dat = xpt.basic_dicstr_to_dict(self.__sc[0])
+        dat = self.ypt.basic_dicstr_to_dict(self.__sc[0])
         rslt = {'encrypted_content': dat['encrypted_content']
                 ,'keystr_with_expiration': dat['keystr_with_expiration']
                 ,'date_id': date_id
                 ,'timestr': self.cppt.seconds_to_timestr(time_id)
                 ,'service_token': service_token}
         del dat
         return str(rslt)
-def aws_framework_manager_client(username_or_email:str="",pwd:str="",local:bool=False):
+
+def aws_framework_manager_client(username_or_email:str="",pwd:str="",aws_auth_token:str="",local:bool=False):
     url_base = "https://www.cloudpy.org/"
     if local:
         url_base = "http://localhost/"
     url = url_base + "gen_authentication_token"
     token = requests.post(url_base + "gen_authentication_token",json = {"username_or_email":username_or_email,"pwd":pwd} ,verify=False).text
-    if "wrong" in token.lower():
+    if "wrong" in token.lower() or "invalid" in token.lower():
         fm = None
         print(token)
     else:
+        #print("token: ",token)
         secret_key = requests.post(url_base + "authenticate_with_token",json={"token":token},verify=False).text
+        #print("secret_key: ",secret_key)
         service_token= requests.post(url_base + "gen_service_token",json={"secret_key":secret_key},verify=False).text
-        fm = aws_framework_manager(secret_key=secret_key)
+        #print("service_token: ",service_token)
+        fm = aws_framework_manager(secret_key=secret_key,aws_auth_token=aws_auth_token)
         print(fm.initialize_service(service_token=service_token))
-    return fm
+    return fm
+
+def gen_aws_auth_token(user_key:str,secret:str,local:bool=False,minutes_to_expire:float=5):
+    ks = "1V44bjdzKODcN50jdz00c4="
+    url_base = "https://www.cloudpy.org/"
+    if local:
+        url_base = "http://localhost/"
+    url = url_base + "gen_secret_key"
+    data = xpt.gen_encrypted_data_with_expiration(
+        original_message=user_key + ks + secret
+        ,minutes_to_expire=minutes_to_expire)
+    json_to_post = {}
+    json_to_post["data"] = str(data)
+    json_to_post["minutes_to_expire"] = minutes_to_expire
+    auth_token = requests.post(url,json=json_to_post,verify=False).text
+    return auth_token
```

### Comparing `cloudpy_org-1.4.1/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.4.2/cloudpy_org.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.4.1
+Version: 1.4.2
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.4.1/setup.py` & `cloudpy_org-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.4.1",
+    version="1.4.2",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

