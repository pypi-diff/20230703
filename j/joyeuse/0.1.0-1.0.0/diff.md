# Comparing `tmp/joyeuse-0.1.0.tar.gz` & `tmp/joyeuse-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyeuse-0.1.0.tar", last modified: Sun Jul  2 20:28:56 2023, max compression
+gzip compressed data, was "joyeuse-1.0.0.tar", last modified: Mon Jul  3 20:31:36 2023, max compression
```

## Comparing `joyeuse-0.1.0.tar` & `joyeuse-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:28:56.884421 joyeuse-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 20:28:51.000000 joyeuse-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-02 20:28:56.884421 joyeuse-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-02 20:28:51.000000 joyeuse-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:28:56.876422 joyeuse-0.1.0/joyeuse/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:28:56.880421 joyeuse-0.1.0/joyeuse/cube/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/cube/cube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:28:56.880421 joyeuse-0.1.0/joyeuse/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/misc/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/misc/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:28:56.880421 joyeuse-0.1.0/joyeuse/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/settings/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/settings/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/settings/section.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/settings/sub_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:28:56.880421 joyeuse-0.1.0/joyeuse/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/ui/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-02 20:28:52.000000 joyeuse-0.1.0/joyeuse/ui/main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:28:56.880421 joyeuse-0.1.0/joyeuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-02 20:28:56.000000 joyeuse-0.1.0/joyeuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-02 20:28:56.000000 joyeuse-0.1.0/joyeuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:28:56.000000 joyeuse-0.1.0/joyeuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 20:28:56.000000 joyeuse-0.1.0/joyeuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-02 20:28:56.000000 joyeuse-0.1.0/joyeuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 20:28:56.000000 joyeuse-0.1.0/joyeuse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 20:28:56.884421 joyeuse-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-02 20:28:52.000000 joyeuse-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:36.254527 joyeuse-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 20:31:26.000000 joyeuse-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-03 20:31:36.254527 joyeuse-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-03 20:31:26.000000 joyeuse-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:36.250527 joyeuse-1.0.0/joyeuse/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:36.250527 joyeuse-1.0.0/joyeuse/cube/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/cube/cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:36.250527 joyeuse-1.0.0/joyeuse/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/misc/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/misc/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:36.254527 joyeuse-1.0.0/joyeuse/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/settings/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/settings/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/settings/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/settings/sub_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:36.254527 joyeuse-1.0.0/joyeuse/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/ui/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-03 20:31:26.000000 joyeuse-1.0.0/joyeuse/ui/main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:36.250527 joyeuse-1.0.0/joyeuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-03 20:31:36.000000 joyeuse-1.0.0/joyeuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-03 20:31:36.000000 joyeuse-1.0.0/joyeuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:31:36.000000 joyeuse-1.0.0/joyeuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 20:31:36.000000 joyeuse-1.0.0/joyeuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-03 20:31:36.000000 joyeuse-1.0.0/joyeuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 20:31:36.000000 joyeuse-1.0.0/joyeuse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 20:31:36.254527 joyeuse-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 20:31:26.000000 joyeuse-1.0.0/setup.py
```

### Comparing `joyeuse-0.1.0/LICENSE.txt` & `joyeuse-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joyeuse-0.1.0/PKG-INFO` & `joyeuse-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,149 +1,190 @@
-Metadata-Version: 2.1
-Name: joyeuse
-Version: 0.1.0
-Summary: Configuration tool for the joyeuse storyteller
-Home-page: https://github.com/ncarrier/joyeuse
-Author: Nicolas Carrier
-Author-email: carrier.nicolas0@gmail.com
-License: GPLv3+
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: X11 Applications
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Topic :: Other/Nonlisted Topic
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-![windows executable generation](https://github.com/ncarrier/joyeuse/actions/workflows/windows_build.yml/badge.svg?branch=master)
+![continuous integration](https://github.com/ncarrier/joyeuse/actions/workflows/continuous_integration.yml/badge.svg?branch=master)
 
 # fr - Outil de configuration de la conteuse Joyeuse
 
 Cet outil permet de modifier les paramètres de la conteuse Joyeuse
 (fichier **Secrets/SETTINGS.txt**).
 
-Son état actuel est très basique et il manque encore cruellement de
-fonctionnalités.
+## Installation
 
-## Utilisation
+### Windows
+
+Télécharger la [dernière version pour Windows][windows].
+
+### Linux
+
+### Ubuntu
 
-Brancher la conteuse, puis :
+Télécharger la dernière version pour Ubuntu 22.04 :
 
 ```sh
-python3 -m joyeuse /chemin/vers/la/conteuse
+wget https://github.com/ncarrier/joyeuse/releases/latest/download/joyeuse-ubuntu-22.04.tar.gz
 ```
 
-Il est possible de tester son fonctionnement en utilisant le dossier
-**example/copie** au lieu du chemin vers la conteuse.
+L'extraire :
 
-## Générer un package pip
+```sh
+tar xf joyeuse-ubuntu-22.04.tar.gz
+```
+
+L'installer :
 
 ```sh
-make pip
+sudo apt install ./joyeuse_*.deb
 ```
 
-Le package généré se trouve dans **dist/**.
+Une version pour Ubuntu 20.04 est également disponible, remplacer dans les
+instructions précédentes, 22 par 20.
+
+## Tous systèmes Windows ou Linux
 
-## Générer un package debian
+Pour les utilisateurs ayant python installé, avec pip :
 
 ```sh
-make debian
+pip install joyeuse
 ```
 
-Le package généré se trouve dans le répertoire parent.
+## Utilisation
+
+Lancer l'application en double-cliquant sur le fichier .exe sous Windows, ou en
+entrant la commande :
+
+```sh
+joyeuse
+```
+
+sous Linux.
+
+Puis brancher la conteuse, qui affichera les paramètres de configuration de la
+conteuse.
 
 ## Compatibilité
 
-Pour l'instant, le logiciel n'a été testé que sous Linux (Debian 10).
+Pour l'instant, le logiciel a été testé sous :
+
+ * Windows
+     * version 10
+ * Linux
+     * Debian 10 et 11 (via pip)
+     * Ubuntu 20.04 et 22.04
 
 ## License
 
 Ce logiciel est sous GPLv3, ou (en fonction de votre choix), n'importe quelle
 version future.
 
 Les personnes qui envoient des contributions, sous quelque forme que ce soit,
 patch, pull request, conseil... Acceptent en le faisant, que leur propriété me
 soit transférée à moi, **Nicolas Carrier**.
+Ceci au moyen de l'ajout d'un sign-off aux commits.
 
 ## Autres
 
 **Note** : Je n'ai aucun lien avec la société JOYEUSE qui fabrique cette
 conteuse.
 
 Pour plus d'information sur Joyeuse, rendez vous sur son
-[site web](https://www.joyeuse.io/).
+[site web][joyeuse].
 
 # en - Joyeuse configuration tool
 
 This tool is meant to configure the parameters of the Joyeuse
 (**Secrets/SETTINGS.txt**).
 
-Its current state is very basic and it's still severely lacking features.
+## Installation
+
+### Windows
+
+Download [the latest Windows version][windows].
+
+### Linux
+
+### Ubuntu
+
+Download the latest Ubuntu 22.04 version:
+
+```sh
+wget https://github.com/ncarrier/joyeuse/releases/latest/download/joyeuse-ubuntu-22.04.tar.gz
+```
+
+Extract it:
 
-## Usage
+```sh
+tar xf joyeuse-ubuntu-22.04.tar.gz
+```
 
-Plug the Joyeuse, then:
+Install it:
 
 ```sh
-python3 -m joyeuse /path/to/the/joyeuse
+sudo apt install ./joyeuse_*.deb
 ```
 
-It is possible to test how it works by using the **example/copie** instead of
-the path to the joyeuse.
+An Ubuntu 20.04 version is availe too, remplace 22 with 20 in the instructions
+above.
 
-## Generate a pip package
+## All Windows or Linux systems
+
+For the users having python installed, with pip :
 
 ```sh
-make pip
+pip install joyeuse
 ```
 
-The resulting package will be in **dist/**.
+## Utilisation
 
-## Generate a debian package
+Launch the application with a double-click on the .exe, for Windows, or by
+running:
 
 ```sh
-make debian
+joyeuse
 ```
 
-The generated packages is in the parent folder.
+under Linux.
+
+Then plug the Joyeuse in, which will make its configuration parameters appear.
 
 ## Compatibility
 
-For now, this software was only tested on Linux (Debian 10).
+For now, the software has been tested for:
+
+ * Windows
+     * version 10
+ * Linux
+     * Debian 10 and 11 (via pip)
+     * Ubuntu 20.04 and 22.04
 
 ## License
 
 This software is placed under the GPLv3, or (at your option) any later version.
 
 People sending contributions under any form, patch, pull request, advice...
 Accept by doing so, that their ownership gets transferred to me,
 **Nicolas Carrier**.
 
 ## Others
 
 **Note**: I am not related with the JOYEUSE company which builds the Joyeuse
 storyteller.
 
-For more information on Joyeuse, go to its [web site](https://www.joyeuse.io/).
+For more information on Joyeuse, go to its [web site][joyeuse].
 
-## TODO
+## What's next
 
-Here is my tentative TODO list, sorted by order of priorities (most priority
-first):
+Here is my tentative roadmap:
 
- * Windows packaging
- * Input parameters validation
- * Auto-detect of the device
- * Publication of 1.0.0
- * Implement a Tutorial tab, allowing to play the videos inside the
+ * Version 1.0.0
+     * Support of parameters control
+ * Version 1.1.0
+     * Implement a Tutorial tab, allowing to play the videos inside the
    'Tutos vidéo' folder
- * Implement the Sound library, allowing to manage the sounds which can be
-   uploaded to the Joyeuse
- * Implement the Music / Stories tab, allowing to add / remove sounds to the
-   cube faces
- * Internationalization
- * Implement a studio tab, allowing to record sound files
+     * Internationalization
+ * Version 1.2.0
+     * Implement the Sound library, allowing to manage the sounds which can be
+     uploaded to the Joyeuse
+     * Implement the Music / Stories tab, allowing to add / remove sounds to the
+     cube faces
+ * Version 1.3.0
+     * Implement a studio tab, allowing to record sound files
 
- * man page? cli? completion?
+[joyeuse]: https://www.joyeuse.io/
+[windows]: https://github.com/ncarrier/joyeuse/releases/latest/download/joyeuse.exe
```

### Comparing `joyeuse-0.1.0/joyeuse/__init__.py` & `joyeuse-1.0.0/joyeuse/__init__.py`

 * *Files identical despite different names*

### Comparing `joyeuse-0.1.0/joyeuse/__main__.py` & `joyeuse-1.0.0/joyeuse/__main__.py`

 * *Files identical despite different names*

### Comparing `joyeuse-0.1.0/joyeuse/__version__.py` & `joyeuse-1.0.0/joyeuse/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 #
 # You should have received a copy of the GNU General Public License along with
 # Joyeuse. If not, see <https://www.gnu.org/licenses/>.
 
 __title__ = "joyeuse"
 __description__ = "Configuration tool for the joyeuse storyteller"
 __url__ = "https://github.com/ncarrier/joyeuse"
-__version__ = "0.1.0"
+__version__ = "1.0.0"
 __author__ = "Nicolas Carrier"
 __author_email__ = "carrier.nicolas0@gmail.com"
 __license__ = "GPLv3+"
```

### Comparing `joyeuse-0.1.0/joyeuse/cube/cube.py` & `joyeuse-1.0.0/joyeuse/cube/cube.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,41 +8,34 @@
 # Joyeuse is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # Joyeuse. If not, see <https://www.gnu.org/licenses/>.
 import os
-import string
 from PIL import ImageTk
 
 from joyeuse.settings.settings import Settings
 from joyeuse.misc.log import Log
+from joyeuse.misc.compat import Compat
 
 
 class Cube(object):
     '''
     classdocs
     '''
     EXTRA_LOCATIONS = []
 
     @staticmethod
-    def __get_subdirs(a_dir):
-        full_paths = [os.path.join(a_dir, name) for name in os.listdir(a_dir)]
-        return [path for path in full_paths if os.path.isdir(path)]
-
-    @staticmethod
     def __get_search_locations():
         return (
             # passed by parameter
             Cube.EXTRA_LOCATIONS +
-            # linux
-            Cube.__get_subdirs(f"/media/{os.getlogin()}") +
-            # windows
-            [f"{d}" for d in string.ascii_uppercase if os.path.exists(f"{d}:")]
+            # os specific
+            Compat.get_os_mount_search_path()
         )
 
     @staticmethod
     def get_cube():
         cube = None
         for loc in Cube.__get_search_locations():
             try:
```

### Comparing `joyeuse-0.1.0/joyeuse/misc/compat.py` & `joyeuse-1.0.0/joyeuse/ui/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,19 +7,7 @@
 #
 # Joyeuse is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # Joyeuse. If not, see <https://www.gnu.org/licenses/>.
-import os
-from enum import Enum, auto
-
-
-class Os(Enum):
-    LINUX = auto()
-    WINDOWS = auto()
-
-
-class Compat(object):
-    OS = Os.WINDOWS if os.name == "nt" else Os.LINUX
-    newline = '\r\n' if OS == Os.LINUX else '\n'
```

### Comparing `joyeuse-0.1.0/joyeuse/misc/log.py` & `joyeuse-1.0.0/joyeuse/misc/log.py`

 * *Files identical despite different names*

### Comparing `joyeuse-0.1.0/joyeuse/settings/item.py` & `joyeuse-1.0.0/joyeuse/settings/item.py`

 * *Files identical despite different names*

### Comparing `joyeuse-0.1.0/joyeuse/settings/parameter.py` & `joyeuse-1.0.0/joyeuse/settings/parameter.py`

 * *Files identical despite different names*

### Comparing `joyeuse-0.1.0/joyeuse/settings/section.py` & `joyeuse-1.0.0/joyeuse/settings/section.py`

 * *Files identical despite different names*

### Comparing `joyeuse-0.1.0/joyeuse/settings/settings.py` & `joyeuse-1.0.0/joyeuse/settings/settings.py`

 * *Files identical despite different names*

### Comparing `joyeuse-0.1.0/joyeuse/settings/sub_section.py` & `joyeuse-1.0.0/joyeuse/settings/sub_section.py`

 * *Files identical despite different names*

### Comparing `joyeuse-0.1.0/joyeuse/ui/input_validation.py` & `joyeuse-1.0.0/joyeuse/ui/input_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Joyeuse is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # Joyeuse. If not, see <https://www.gnu.org/licenses/>.
-from tkinter import IntVar, StringVar, BooleanVar, ttk, Frame
+from tkinter import IntVar, StringVar, BooleanVar, ttk, Frame, TclError
 
 
 class Setting(object):
     def get_var(self, **kw):
         return self.VAR_KLASS(**kw)
 
 
@@ -29,25 +29,39 @@
         '''
         Constructor
         '''
         self.__lower = lower
         self.__upper = upper
 
     def get_value(self, var):
-        return str(var.get())
+        try:
+            return str(var.get())
+        except TclError:
+            return self.__lower
 
     def get_input_widget(self, parent, var, edit_action):
         var.trace("w", edit_action)
-        return ttk.Spinbox(
+        sb = ttk.Spinbox(
             parent,
             from_=self.lower,
             to=self.upper,
             textvariable=var,
             width=3
         )
+        vcmd = (parent.register(self.validate_spinbox), '%P')
+        sb.configure(validate="key", validatecommand=vcmd)
+
+        return sb
+
+    def validate_spinbox(self, new_value):
+        try:
+            v = int(new_value)
+            return v >= self.__lower and v <= self.__upper
+        except ValueError:
+            return False
 
     @property
     def lower(self):
         return self.__lower
 
     @property
     def upper(self):
@@ -59,26 +73,29 @@
     classdocs
     '''
     VAR_KLASS = StringVar
 
     class __SpinboxWithCheckButton(Frame):
         def __init__(self, parent, setting, var, edit_action):
             Frame.__init__(self, parent)
+            self.__lower = setting.lower
             checked = var.get() != "N"
             int_value = int(var.get()) if checked else setting.lower
 
             self.__int_var = IntVar(value=int_value)
             self.__int_var.trace("w", edit_action)
             self.__spin_box = ttk.Spinbox(
                 self,
                 from_=setting.lower,
                 to=setting.upper,
                 textvariable=self.__int_var,
                 width=3
             )
+            vcmd = (parent.register(setting.validate_spinbox), '%P')
+            self.__spin_box.configure(validate="key", validatecommand=vcmd)
             self.__spin_box.pack(side="right", fill="both")
 
             self.__boolean_var = BooleanVar(value=checked)
             self.__boolean_var.trace("w", edit_action)
             cb = ttk.Checkbutton(self, var=self.__boolean_var,
                                  command=lambda: self.__check())
             cb.pack(side="left")
@@ -91,15 +108,18 @@
 
         @property
         def checked(self):
             return not self.__boolean_var.get()
 
         @property
         def value(self):
-            return self.__int_var.get()
+            try:
+                return self.__int_var.get()
+            except TclError:
+                return self.__lower
 
     def get_value(self, _):
         return "N" if self.__widget.checked else str(self.__widget.value)
 
     def get_input_widget(self, parent, var, edit_action):
         self.__widget = FalseOrIntInRangeSetting.__SpinboxWithCheckButton(
             parent,
```

### Comparing `joyeuse-0.1.0/joyeuse/ui/main_window.py` & `joyeuse-1.0.0/joyeuse/ui/main_window.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 
 
 class MainWindow(object):
     '''
     classdocs
     '''
     WELCOME_MESSAGE = "Branchez votre joyeuse :)"
-    __period = 1  # in seconds
+    __period = 1  # in seconds, used by joyeuse detector and save debouncer
 
     def __init__(self):
         '''
         Constructor
         '''
         self.__cube = None
+        self.__after_identifier = None
         self.__root = Tk(className='joyeuse')
         self.__setup_window()
 
     def __unload_cube(self):
         self.__notebook.destroy()
         self.__cube = None
 
@@ -106,27 +107,38 @@
 
     def __get_input_widget(self, frame, parameter, edit_action):
         validation_obj = InputValidation.get(parameter.name)
 
         return validation_obj.get_input_widget(frame, parameter.var,
                                                edit_action)
 
+    def __do_save(self):
+        self.__cube.settings.save()
+        self.__after_identifier = None
+
+    def __save_scheduler(self):
+        if self.__after_identifier is not None:
+            self.__root.after_cancel(self.__after_identifier)
+
+        self.__after_identifier = self.__root.after(1000 * self.__period,
+                                                    self.__do_save)
+
     def __load_parameter(self, frame, parameter, index):
         label = tkinter.Label(frame, text=parameter.name)
         label.grid(
             column=0,
             row=index,
             sticky=tkinter.W,
             padx=(3, 3),
             pady=(3, 3)
         )
         widget = self.__get_input_widget(
             frame,
             parameter,
-            lambda a, b, c: self.__cube.settings.save()
+            lambda a, b, c: self.__save_scheduler()
         )
         widget.grid(column=1, row=index, sticky=tkinter.E, pady=3, padx=3)
         if len(parameter.comments) > 0:
             Hovertip(label, parameter.comments)
             Hovertip(widget, parameter.comments)
 
     def __load_cube_section(self, section, index):
```

### Comparing `joyeuse-0.1.0/joyeuse.egg-info/SOURCES.txt` & `joyeuse-1.0.0/joyeuse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joyeuse-0.1.0/setup.py` & `joyeuse-1.0.0/setup.py`

 * *Files identical despite different names*

