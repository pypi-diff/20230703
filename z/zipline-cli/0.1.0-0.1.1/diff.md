# Comparing `tmp/zipline-cli-0.1.0.tar.gz` & `tmp/zipline-cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipline-cli-0.1.0.tar", last modified: Mon Jul  3 04:07:56 2023, max compression
+gzip compressed data, was "zipline-cli-0.1.1.tar", last modified: Mon Jul  3 09:33:10 2023, max compression
```

## Comparing `zipline-cli-0.1.0.tar` & `zipline-cli-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 04:07:56.241380 zipline-cli-0.1.0/
--rw-rw-rw-   0        0        0     3656 2023-07-03 04:07:56.240879 zipline-cli-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2976 2023-07-03 03:46:20.000000 zipline-cli-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 04:07:56.241880 zipline-cli-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1153 2023-07-02 06:31:47.000000 zipline-cli-0.1.0/setup.py
--rw-rw-rw-   0        0        0     5835 2023-07-03 03:54:25.000000 zipline-cli-0.1.0/zipline.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:07:56.239878 zipline-cli-0.1.0/zipline_cli.egg-info/
--rw-rw-rw-   0        0        0     3656 2023-07-03 04:07:56.000000 zipline-cli-0.1.0/zipline_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-03 04:07:56.000000 zipline-cli-0.1.0/zipline_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 04:07:56.000000 zipline-cli-0.1.0/zipline_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-03 04:07:56.000000 zipline-cli-0.1.0/zipline_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-03 04:07:55.000000 zipline-cli-0.1.0/zipline_cli.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2023-07-03 04:07:56.000000 zipline-cli-0.1.0/zipline_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 04:07:56.000000 zipline-cli-0.1.0/zipline_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 09:33:10.574757 zipline-cli-0.1.1/
+-rw-rw-rw-   0        0        0     3660 2023-07-03 09:33:10.575257 zipline-cli-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2980 2023-07-03 05:02:33.000000 zipline-cli-0.1.1/README.md
+-rw-rw-rw-   0        0        0      161 2023-07-03 09:33:10.576257 zipline-cli-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2023-07-03 09:11:55.000000 zipline-cli-0.1.1/setup.py
+-rw-rw-rw-   0        0        0     6977 2023-07-03 09:05:01.000000 zipline-cli-0.1.1/zipline.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:33:10.574255 zipline-cli-0.1.1/zipline_cli.egg-info/
+-rw-rw-rw-   0        0        0     3660 2023-07-03 09:33:10.000000 zipline-cli-0.1.1/zipline_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-07-03 09:33:10.000000 zipline-cli-0.1.1/zipline_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 09:33:10.000000 zipline-cli-0.1.1/zipline_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-03 09:33:10.000000 zipline-cli-0.1.1/zipline_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-03 09:33:10.000000 zipline-cli-0.1.1/zipline_cli.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-07-03 09:33:10.000000 zipline-cli-0.1.1/zipline_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 09:33:10.000000 zipline-cli-0.1.1/zipline_cli.egg-info/top_level.txt
```

### Comparing `zipline-cli-0.1.0/PKG-INFO` & `zipline-cli-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python 3 CLI for Zipline
 Home-page: https://github.com/cssnr/zipline-cli
 Author: Shane
 Author-email: shane@sapps.me
 Project-URL: Source, https://github.com/cssnr/zipline-cli
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -27,32 +27,32 @@
 
 This is currently a **WIP** and not complete, but has some useful functions.
 
 ## Install
 
 From PyPi using pip:
 ```text
-python -m pip install zipline-cli
+python3 -m pip install zipline-cli
 ```
 
 From GitHub using pip:
 ```text
-python -m pip install git+https://github.com/cssnr/zipline-cli.git
+python3 -m pip install git+https://github.com/cssnr/zipline-cli.git
 ```
 
 From Source using setuptools:
 ```text
 git clone https://github.com/cssnr/zipline-cli.git
 cd zipline-cli
-python setup.py install
+python3 setup.py install
 ```
 
 Uninstall:
 ```text
-python -m pip uninstall zipline-cli
+python3 -m pip uninstall zipline-cli
 ```
 
 ## CLI Usage
 
 You will need a Zipline URL and Token to use the utility.
 
 Setup Zipline URL and Token:
```

### Comparing `zipline-cli-0.1.0/README.md` & `zipline-cli-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 
 This is currently a **WIP** and not complete, but has some useful functions.
 
 ## Install
 
 From PyPi using pip:
 ```text
-python -m pip install zipline-cli
+python3 -m pip install zipline-cli
 ```
 
 From GitHub using pip:
 ```text
-python -m pip install git+https://github.com/cssnr/zipline-cli.git
+python3 -m pip install git+https://github.com/cssnr/zipline-cli.git
 ```
 
 From Source using setuptools:
 ```text
 git clone https://github.com/cssnr/zipline-cli.git
 cd zipline-cli
-python setup.py install
+python3 setup.py install
 ```
 
 Uninstall:
 ```text
-python -m pip uninstall zipline-cli
+python3 -m pip uninstall zipline-cli
 ```
 
 ## CLI Usage
 
 You will need a Zipline URL and Token to use the utility.
 
 Setup Zipline URL and Token:
```

### Comparing `zipline-cli-0.1.0/setup.py` & `zipline-cli-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setup(
     name='zipline-cli',
-    version='0.1.0',
+    version='0.1.1',
     description='Python 3 CLI for Zipline',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/cssnr/zipline-cli',
     author='Shane',
     author_email='shane@sapps.me',
     py_modules=['zipline'],
```

### Comparing `zipline-cli-0.1.0/zipline.py` & `zipline-cli-0.1.1/zipline.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 import random
 import re
 import requests
 import string
 import sys
 from decouple import config
-from dotenv import load_dotenv, find_dotenv
+from dotenv import find_dotenv, load_dotenv
 from pathlib import Path
-from typing import Optional, List, Any, TextIO
+from typing import Any, Dict, List, Optional, TextIO
 
 
 class Zipline(object):
     """
     Zipline Python API
     :param url: str: Zipline URL
     :param kwargs: Zipline Headers
@@ -21,19 +21,18 @@
     allowed_headers = ['format', 'image_compression_percent', 'expires_at',
                        'password', 'zws', 'embed', 'max_views', 'uploadtext',
                        'authorization', 'no_json', 'x_zipline_filename',
                        'original_name', 'override_domain']
 
     def __init__(self, zipline_url: str, **kwargs):
         self.zipline_url: str = zipline_url.rstrip('/')
-        self.headers: dict = {}
+        self.headers: Dict[str, str] = {}
         for header, value in kwargs.items():
             if header.lower() not in self.allowed_headers:
-                error = f'{header.lower()} not in {self.allowed_headers}'
-                raise ValueError(error)
+                continue
             if value is None:
                 continue
             key = header.replace('_', '-').title()
             self.headers[key] = str(value)
 
     def send_file(self, file_name: str, file_object: TextIO,
                   overrides: Optional[dict] = None) -> str:
@@ -50,104 +49,134 @@
         r = requests.post(url, headers=headers, files=files)
         r.raise_for_status()
         return r.json()['files'][0]
         # return f'https://example.com/dummy/{file_name}'
 
 
 def gen_rand(length: Optional[int] = 4) -> str:
+    """
+    Generate Random Streng at Given length
+    :param length: int: Length of Random String
+    :return: str: Random String
+    """
     length: int = length if not length < 0 else 4
     return ''.join(random.choice(string.ascii_letters) for _ in range(length))
 
 
-def get_default(values: List[str], default: Any = None,
-                cast: Optional[type] = str, pre: str = 'ZIPLINE_',
-                suf: str = '') -> Optional[str]:
+def get_default(values: List[str], default: Optional[Any] = None,
+                cast: Optional[type] = str, pre: Optional[str] = 'ZIPLINE_',
+                suf: Optional[str] = '') -> Optional[str]:
+    """
+    Get Default Environment Variable from List of values
+    :param values: list: List of Values to Check
+    :param default: any: Default Value if None
+    :param cast: type: Type to Cast Value
+    :param pre: str: Environment Variable Prefix
+    :param suf: str: Environment Variable Suffix
+    :return: str: Environment Variable or None
+    """
     for value in values:
         result = config(f'{pre}{value.upper()}{suf}', '', cast)
-        # print('value', value)
-        # print('result', result)
         if result:
             return result
     return default
 
 
-def main():
-    env_file = Path(os.path.expanduser('~')) / '.zipline'
-    # print(env_file)
-    dotenv_path = env_file if os.path.exists(env_file) else find_dotenv(filename='.zipline')
-    load_dotenv(dotenv_path=dotenv_path)
+def setup(env_file: Path) -> None:
+    print('Setting up Environment File...')
+    url = input('Zipline URL: ').strip()
+    token = input('Zipline Authorization Token: ').strip()
+    if not url or not token:
+        raise ValueError('Missing URL or Token.')
+    output = f'ZIPLINE_URL={url}\nZIPLINE_TOKEN={token}\n'
+    embed = input('Enabled Embed? [Yes]/No: ').strip()
+    if not embed or embed.lower() not in ['n', 'o', 'no', 'noo']:
+        output += 'ZIPLINE_EMBED=true\n'
+    expire = input('Default Expire? [Blank for None]: ').strip().lower()
+    match = re.search(r'^(\d+)(?:ms|s|m|h|d|w|y)$', expire)
+    if not match:
+        print(f'Warning: invalid expire format: {expire} skipping. See --help')
+    else:
+        output += f'ZIPLINE_EXPIRE={expire}\n'
+    with open(env_file, 'w') as f:
+        f.write(output)
+    print(f'Setup Complete. Variables Saved to: {env_file}')
+    sys.exit(0)
+
+
+def main() -> None:
+    zipline_file = '.zipline'
+    env_file = Path(os.path.expanduser('~')) / zipline_file
+    dotenv_path = env_file if os.path.isfile(env_file) else find_dotenv(filename=zipline_file)
+    env = load_dotenv(dotenv_path=dotenv_path)
+
     parser = argparse.ArgumentParser(description='Zipline CLI.')
-    parser.add_argument('files', metavar='Files', type=str, nargs='*',
-                        help='Files to Upload')
-    parser.add_argument('-u', '--url', type=str, default=get_default(['url']),
-                        help='Zipline URL.')
+    parser.add_argument('files', metavar='Files', type=str, nargs='*', help='Files to Upload.')
+    parser.add_argument('-u', '--url', type=str, default=get_default(['url']), help='Zipline URL.')
     parser.add_argument('-a', '-t', '--authorization', '--token', type=str,
                         default=get_default(['token', 'authorization']),
-                        help='Zipline Access Token for Authorization or ZIPLINE_TOKEN')
+                        help='Zipline Access Token for Authorization or ZIPLINE_TOKEN.')
     parser.add_argument('-e', '-x', '--expires_at', '--expire', type=str, default=get_default(['expire', 'expire_at']),
-                        help='Example: 1d. See: https://zipline.diced.tech/docs/guides/upload-options#image-expiration')
+                        help='Ex: 1d, 2w. See: https://zipline.diced.tech/docs/guides/upload-options#image-expiration')
     parser.add_argument('--embed', action=argparse.BooleanOptionalAction, default=get_default(['embed'], False, bool),
-                        help='Enable Embeds on Uploads')
-    parser.add_argument('--setup', action='store_true', default=False,
-                        help='Set Required Variables: URL and AUTHORIZATION')
+                        help='Enable Embeds on Uploads.')
+    parser.add_argument('-s', '--setup', action='store_true', default=False,
+                        help='Automatic Setup of Environment Variables.')
     args = parser.parse_args()
-    # print(args)
+
     if args.setup:
-        url = input('Zipline URL: ')
-        token = input('Zipline Authorization Token: ')
-        if not url or not token:
-            raise ValueError('Missing URL or Token.')
-        env_file = Path(os.path.expanduser('~')) / '.zipline'
-        with open(env_file, 'w') as f:
-            f.write(f'ZIPLINE_URL={url}\nZIPLINE_TOKEN={token}')
-        print('Setup Success. You can run again to change or update details.')
-        sys.exit(0)
+        setup(env_file)
+
+    if not env and not args.url and not args.authorization and not os.path.isfile(env_file):
+        env_file.touch()
+        print('First Run Detected, Entering Setup.')
+        setup(env_file)
 
     if not args.url:
         parser.print_help()
-        error = 'Missing Zipline URL. Use use --setup or specify --url'
-        raise ValueError(error)
+        raise ValueError('Missing URL. Use --setup or specify --url')
 
     if not args.authorization:
         parser.print_help()
-        error = 'Missing Zipline Token. Use use --setup or specify --token'
-        raise ValueError(error)
+        raise ValueError('Missing Token. Use --setup or specify --token')
 
     if args.expires_at:
-        args.expires_at = args.expires_at.lower()
-        match = re.search(r'(\d+(?:ms|s|m|h|d|w|y))', args.expires_at)
+        args.expires_at = args.expires_at.strip().lower()
+        match = re.search(r'^(\d+)(?:ms|s|m|h|d|w|y)$', args.expires_at)
         if not match:
             parser.print_help()
-            error = f'Invalid Expiration Format: {args.expires_at}. See --help'
-            raise ValueError(error)
+            raise ValueError(f'Invalid Expire Format: {args.expires_at}.')
 
-    url = args.url
-    files = args.files
-    vars(args).pop('url')
-    vars(args).pop('files')
-    vars(args).pop('setup')
-    # print(vars(args))
-    zipline = Zipline(url, **vars(args))
+    zipline = Zipline(args.url, **vars(args))
 
-    if not files:
+    if not args.files:
         content: str = sys.stdin.read().rstrip('\n') + '\n'
         text_f: TextIO = io.StringIO(content)
         name = f'{gen_rand(8)}.txt'
         url: str = zipline.send_file(name, text_f)
         print(f'{name} -> {url}')
         sys.exit(0)
 
     exit_code = 1
-    for name in files:
-        if not os.path.isfile(name):
-            print(f'File Not Found: {name}')
+    for filename in args.files:
+        if not os.path.isfile(filename):
+            print(f'Warning: File Not Found: {filename}')
             continue
-        with open(name) as f:
-            new_name = f'{gen_rand()}-{os.path.basename(name)}'
-            url: str = zipline.send_file(new_name, f)
-            print(f'{new_name} -> {url}')
+        with open(filename) as f:
+            # name, ext = os.path.splitext(os.path.basename(filename))
+            # ext = f'.{ext}' if ext else ''
+            # name = f'{name}-{gen_rand(8)}{ext}'
+            # url: str = zipline.send_file(name, f)
+            url: str = zipline.send_file(filename, f)
+            print(f'{filename} -> {url}')
             exit_code = 0
     sys.exit(exit_code)
 
 
 if __name__ == '__main__':
-    main()
+    try:
+        main()
+    except KeyboardInterrupt:
+        sys.exit(1)
+    except Exception as error:
+        print('\nError: {}'.format(str(error)))
+        sys.exit(1)
```

### Comparing `zipline-cli-0.1.0/zipline_cli.egg-info/PKG-INFO` & `zipline-cli-0.1.1/zipline_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python 3 CLI for Zipline
 Home-page: https://github.com/cssnr/zipline-cli
 Author: Shane
 Author-email: shane@sapps.me
 Project-URL: Source, https://github.com/cssnr/zipline-cli
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -27,32 +27,32 @@
 
 This is currently a **WIP** and not complete, but has some useful functions.
 
 ## Install
 
 From PyPi using pip:
 ```text
-python -m pip install zipline-cli
+python3 -m pip install zipline-cli
 ```
 
 From GitHub using pip:
 ```text
-python -m pip install git+https://github.com/cssnr/zipline-cli.git
+python3 -m pip install git+https://github.com/cssnr/zipline-cli.git
 ```
 
 From Source using setuptools:
 ```text
 git clone https://github.com/cssnr/zipline-cli.git
 cd zipline-cli
-python setup.py install
+python3 setup.py install
 ```
 
 Uninstall:
 ```text
-python -m pip uninstall zipline-cli
+python3 -m pip uninstall zipline-cli
 ```
 
 ## CLI Usage
 
 You will need a Zipline URL and Token to use the utility.
 
 Setup Zipline URL and Token:
```

