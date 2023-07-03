# Comparing `tmp/fusion-engine-0.1.0.tar.gz` & `tmp/fusion-engine-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-0.1.0.tar", last modified: Mon Jul  3 05:07:47 2023, max compression
+gzip compressed data, was "fusion-engine-0.1.1.tar", last modified: Mon Jul  3 10:51:01 2023, max compression
```

## Comparing `fusion-engine-0.1.0.tar` & `fusion-engine-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-03 05:07:47.603092 fusion-engine-0.1.0/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/LICENCE.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4046 2023-07-03 05:07:47.602683 fusion-engine-0.1.0/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2803 2023-07-02 20:09:36.000000 fusion-engine-0.1.0/README.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1643 2023-07-02 14:45:04.000000 fusion-engine-0.1.0/pyproject.toml
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       34 2023-06-16 16:18:43.000000 fusion-engine-0.1.0/requirements.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-03 05:07:47.603228 fusion-engine-0.1.0/setup.cfg
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      819 2023-07-02 14:45:04.000000 fusion-engine-0.1.0/setup.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-03 05:07:47.584669 fusion-engine-0.1.0/src/
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-03 05:07:47.590737 fusion-engine-0.1.0/src/fusion_engine.egg-info/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4046 2023-07-03 05:07:47.000000 fusion-engine-0.1.0/src/fusion_engine.egg-info/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      790 2023-07-03 05:07:47.000000 fusion-engine-0.1.0/src/fusion_engine.egg-info/SOURCES.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-03 05:07:47.000000 fusion-engine-0.1.0/src/fusion_engine.egg-info/dependency_links.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       35 2023-07-03 05:07:47.000000 fusion-engine-0.1.0/src/fusion_engine.egg-info/requires.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       17 2023-07-03 05:07:47.000000 fusion-engine-0.1.0/src/fusion_engine.egg-info/top_level.txt
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-03 05:07:47.591072 fusion-engine-0.1.0/src/fusionengine/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      842 2023-07-02 14:46:24.000000 fusion-engine-0.1.0/src/fusionengine/__init__.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-03 05:07:47.591407 fusion-engine-0.1.0/src/fusionengine/debugfiles/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3326 2023-06-10 20:37:31.000000 fusion-engine-0.1.0/src/fusionengine/debugfiles/test.png
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-03 05:07:47.601824 fusion-engine-0.1.0/src/fusionengine/files/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2534 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/body.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      913 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/color.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      315 2023-07-01 19:18:56.000000 fusion-engine-0.1.0/src/fusionengine/files/data.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2156 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/draw.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      232 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/enums.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10606 2023-07-02 16:44:06.000000 fusion-engine-0.1.0/src/fusionengine/files/event.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       91 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/exceptions.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      734 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/image.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      461 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/imports.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.1.0/src/fusionengine/files/physics.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      497 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/shape.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5566 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/storage.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      767 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/systems.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1661 2023-07-02 09:01:28.000000 fusion-engine-0.1.0/src/fusionengine/files/window.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:51:01.044057 fusion-engine-0.1.1/
+-rw-rw-rw-   0        0        0     1092 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/LICENCE.md
+-rw-rw-rw-   0        0        0     4234 2023-07-03 10:51:01.035421 fusion-engine-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2964 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1688 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 10:51:01.045066 fusion-engine-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1055 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:51:00.801227 fusion-engine-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 10:51:00.956354 fusion-engine-0.1.1/src/fusion_engine.egg-info/
+-rw-rw-rw-   0        0        0     4234 2023-07-03 10:51:00.000000 fusion-engine-0.1.1/src/fusion_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2023-07-03 10:51:00.000000 fusion-engine-0.1.1/src/fusion_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 10:51:00.000000 fusion-engine-0.1.1/src/fusion_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-03 10:51:00.000000 fusion-engine-0.1.1/src/fusion_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 10:51:00.000000 fusion-engine-0.1.1/src/fusion_engine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 10:51:00.961844 fusion-engine-0.1.1/src/fusionengine/
+-rw-rw-rw-   0        0        0      871 2023-07-03 10:50:38.000000 fusion-engine-0.1.1/src/fusionengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:51:00.964840 fusion-engine-0.1.1/src/fusionengine/debugfiles/
+-rw-rw-rw-   0        0        0     3326 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/debugfiles/test.png
+drwxrwxrwx   0        0        0        0 2023-07-03 10:51:01.033424 fusion-engine-0.1.1/src/fusionengine/files/
+-rw-rw-rw-   0        0        0     2826 2023-07-03 09:35:35.000000 fusion-engine-0.1.1/src/fusionengine/files/body.py
+-rw-rw-rw-   0        0        0      939 2023-07-03 09:39:18.000000 fusion-engine-0.1.1/src/fusionengine/files/color.py
+-rw-rw-rw-   0        0        0      394 2023-07-03 09:40:19.000000 fusion-engine-0.1.1/src/fusionengine/files/data.py
+-rw-rw-rw-   0        0        0     2442 2023-07-03 09:41:16.000000 fusion-engine-0.1.1/src/fusionengine/files/draw.py
+-rw-rw-rw-   0        0        0      242 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/enums.py
+-rw-rw-rw-   0        0        0    10951 2023-07-03 09:42:09.000000 fusion-engine-0.1.1/src/fusionengine/files/event.py
+-rw-rw-rw-   0        0        0       96 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/exceptions.py
+-rw-rw-rw-   0        0        0      928 2023-07-03 09:44:32.000000 fusion-engine-0.1.1/src/fusionengine/files/image.py
+-rw-rw-rw-   0        0        0      481 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/imports.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/physics.py
+-rw-rw-rw-   0        0        0      552 2023-07-03 09:45:15.000000 fusion-engine-0.1.1/src/fusionengine/files/shape.py
+-rw-rw-rw-   0        0        0     5708 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/storage.py
+-rw-rw-rw-   0        0        0      788 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/systems.py
+-rw-rw-rw-   0        0        0     1759 2023-07-03 09:48:40.000000 fusion-engine-0.1.1/src/fusionengine/files/window.py
```

### Comparing `fusion-engine-0.1.0/PKG-INFO` & `fusion-engine-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,108 @@
-Metadata-Version: 2.1
-Name: fusion-engine
-Version: 0.1.0
-Summary: This a fully custom engine based on Python and PySDL2, it's written in pure python.
-Author-email: Dimkauzh <uzhdimka@gmail.com>
-License: LICENSE.md
-Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Multimedia :: Video
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE.md
-
-# Fusion Engine
-
-![logo](https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png)
-
-Fusion is a game engine for creating graphical applications using the PySDL2 library and the programming language Python. It provides a simple coding interface for creating windows,
-rendering graphics, and handling user input. It is and engine to create
-games fast and easy!
-
-## Development
-
-Keep in mind that this project is in work, so if you want to see code,
-then it is in dev branch but there is no 'full version' of this project!
-We working hard to make first alpha version of it!
-
-## Installation
-
-To install our package, run this:
-
-```bash
-  pip install fusion-engine
-```
-
-If you want to run the example, then just run this command:
-
-```bash
- git clone https://github.com/dimkauzh/fusion-engine
- cd fusion-engine
- python examples/example1.py
-```
-
-For different examples, you change the number to the number of the example file
-
-## Community
-
-Our community is just growing, so if you want to help us with the project,
-it will be very helpful!
-We have a discord server at this link (<https://discord.gg/Smg3CK4ZMc>)
-Need to contact us? Just DM the Owner or CEO in discord and we will try to react as fast as possible
-
-### Special thanks to these people❤️
-
-- Zenthm (Contributing)
-- XCarCedo (Contributing)
-- FBS_Gamer (Discord server)
-
-## Documentation
-
-See at [The wiki of the project](https://github.com/dimkauzh/fusion-engine/wiki) (Still in work!)
-
-## Coming features
-
-We are working hard to implement very basic and complex stuff so our engine becomes more rigid. These features are worked on or will be worked on:
-
-- Fysics system using PyMunk (Being worked on)
-- Delta-Time (Finished!)
-- Pip package and SetupTools (Being worked on)
-- Ui (Being worked on)
-- If you have more ideas, please tell us them in our discord group!
-
-## About
-
-Fusion Engine is currently (6/14/2023) build with Python and some Python libraries:
-
-- PySDL2 is used for rendering and windowing
-- PySDL2-DLL is used by PySDL2 for SDL2 binaries
-- PyMunk is used for fysics simulation
-- CX-Freeze is used for building executables (Temporary, it will change when SetupTools is setup)
-
-### Future of this engine
-
-This project began 1 may 2023. The original project began in C, but it's entirely rewritten in Python for it's big userbase and ease of use (productivity). This is actually also my EuroPython project.
-
-Our cool ideas:
-
-- Make a full GUI app (With something like Kyvi or TKinter) - Update: We are currenly working on it with tkinter
-
-## 🚀 About Me
-
-A 13 year old game developer with much passion about game development. So I made this project to grow my programming skills and just make a tool that I can use for myself or a tool for other people to help them develop games.
+Metadata-Version: 2.1
+Name: fusion-engine
+Version: 0.1.1
+Summary: This a fully custom engine based on Python and PySDL2, it's written in pure python.
+Author-email: Dimkauzh <uzhdimka@gmail.com>
+License: LICENSE.md
+Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Video
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENCE.md
+
+# Fusion Engine
+
+![logo](https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png)
+
+Fusion is a game engine for creating graphical applications using the PySDL2 library and the programming language Python. It provides a simple coding interface for creating windows,
+rendering graphics, and handling user input. It is and engine to create
+games fast and easy!
+
+## Development
+
+Keep in mind that this project is in work, so if you want to see code,
+then it is in dev branch but there is no 'full version' of this project!
+We working hard to make first alpha version of it!
+
+## Installation
+
+To install our package, run this:
+
+```bash
+  pip install fusion-engine
+```
+
+Our PyPI package is at this [link](<https://pypi.org/project/fusion-engine/>)
+
+If you want to run the example, then just run this command:
+
+```bash
+ git clone https://github.com/dimkauzh/fusion-engine
+ cd fusion-engine
+ python examples/example1.py
+```
+
+For different examples, you change the number to the number of the example file
+
+## Community
+
+Our community is just growing, so if you want to help us with the project,
+it will be very helpful!
+We have a discord server at this [link](https://discord.gg/Smg3CK4ZMc)
+Need to contact us? Just DM the Owner or CEO in discord and we will try to react as fast as possible
+
+### Special thanks to these people❤️
+
+- Zenthm (Contributing)
+- XCarCedo (Contributing)
+- FBS_Gamer (Discord server)
+
+## Documentation
+
+See at [The wiki of the project](https://github.com/dimkauzh/fusion-engine/wiki) (Still in work!)
+
+## Coming features
+
+We are working hard to implement very basic and complex stuff so our engine becomes more rigid. These features are worked on or will be worked on:
+
+- Physics system using PyMunk (Being worked on)
+- Delta-Time (Finished!)
+- Pip package and SetupTools (Being worked on)
+- UI (Being worked on)
+- If you have more ideas, please tell us them in our discord group!
+
+## About
+
+Fusion Engine is currently (6/14/2023) build with Python and some Python libraries:
+
+- PySDL2 is used for rendering and windowing
+- PySDL2-DLL is used by PySDL2 for SDL2 binaries
+- PyMunk is used for fysics simulation
+- CX-Freeze is used for building executables (Temporary, it will change when SetupTools is setup)
+
+### Future of this engine
+
+This project began May 1, 2023. The original project began in C, but it's entirely rewritten in Python for it's big userbase and ease of use (productivity). This is actually also my EuroPython project.
+
+Our cool ideas:
+
+- Make a full GUI app (With something like Kivy or Tkinter) - Update: We are currenly working on it with tkinter
+
+## 🚀 About Me
+
+A 13 year old game developer with much passion about game development. So I made this project to grow my programming skills and just make a tool that I can use for myself or a tool for other people to help them develop games.
```

### Comparing `fusion-engine-0.1.0/src/fusion_engine.egg-info/PKG-INFO` & `fusion-engine-0.1.1/src/fusion_engine.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,108 @@
-Metadata-Version: 2.1
-Name: fusion-engine
-Version: 0.1.0
-Summary: This a fully custom engine based on Python and PySDL2, it's written in pure python.
-Author-email: Dimkauzh <uzhdimka@gmail.com>
-License: LICENSE.md
-Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Multimedia :: Video
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE.md
-
-# Fusion Engine
-
-![logo](https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png)
-
-Fusion is a game engine for creating graphical applications using the PySDL2 library and the programming language Python. It provides a simple coding interface for creating windows,
-rendering graphics, and handling user input. It is and engine to create
-games fast and easy!
-
-## Development
-
-Keep in mind that this project is in work, so if you want to see code,
-then it is in dev branch but there is no 'full version' of this project!
-We working hard to make first alpha version of it!
-
-## Installation
-
-To install our package, run this:
-
-```bash
-  pip install fusion-engine
-```
-
-If you want to run the example, then just run this command:
-
-```bash
- git clone https://github.com/dimkauzh/fusion-engine
- cd fusion-engine
- python examples/example1.py
-```
-
-For different examples, you change the number to the number of the example file
-
-## Community
-
-Our community is just growing, so if you want to help us with the project,
-it will be very helpful!
-We have a discord server at this link (<https://discord.gg/Smg3CK4ZMc>)
-Need to contact us? Just DM the Owner or CEO in discord and we will try to react as fast as possible
-
-### Special thanks to these people❤️
-
-- Zenthm (Contributing)
-- XCarCedo (Contributing)
-- FBS_Gamer (Discord server)
-
-## Documentation
-
-See at [The wiki of the project](https://github.com/dimkauzh/fusion-engine/wiki) (Still in work!)
-
-## Coming features
-
-We are working hard to implement very basic and complex stuff so our engine becomes more rigid. These features are worked on or will be worked on:
-
-- Fysics system using PyMunk (Being worked on)
-- Delta-Time (Finished!)
-- Pip package and SetupTools (Being worked on)
-- Ui (Being worked on)
-- If you have more ideas, please tell us them in our discord group!
-
-## About
-
-Fusion Engine is currently (6/14/2023) build with Python and some Python libraries:
-
-- PySDL2 is used for rendering and windowing
-- PySDL2-DLL is used by PySDL2 for SDL2 binaries
-- PyMunk is used for fysics simulation
-- CX-Freeze is used for building executables (Temporary, it will change when SetupTools is setup)
-
-### Future of this engine
-
-This project began 1 may 2023. The original project began in C, but it's entirely rewritten in Python for it's big userbase and ease of use (productivity). This is actually also my EuroPython project.
-
-Our cool ideas:
-
-- Make a full GUI app (With something like Kyvi or TKinter) - Update: We are currenly working on it with tkinter
-
-## 🚀 About Me
-
-A 13 year old game developer with much passion about game development. So I made this project to grow my programming skills and just make a tool that I can use for myself or a tool for other people to help them develop games.
+Metadata-Version: 2.1
+Name: fusion-engine
+Version: 0.1.1
+Summary: This a fully custom engine based on Python and PySDL2, it's written in pure python.
+Author-email: Dimkauzh <uzhdimka@gmail.com>
+License: LICENSE.md
+Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Video
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENCE.md
+
+# Fusion Engine
+
+![logo](https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png)
+
+Fusion is a game engine for creating graphical applications using the PySDL2 library and the programming language Python. It provides a simple coding interface for creating windows,
+rendering graphics, and handling user input. It is and engine to create
+games fast and easy!
+
+## Development
+
+Keep in mind that this project is in work, so if you want to see code,
+then it is in dev branch but there is no 'full version' of this project!
+We working hard to make first alpha version of it!
+
+## Installation
+
+To install our package, run this:
+
+```bash
+  pip install fusion-engine
+```
+
+Our PyPI package is at this [link](<https://pypi.org/project/fusion-engine/>)
+
+If you want to run the example, then just run this command:
+
+```bash
+ git clone https://github.com/dimkauzh/fusion-engine
+ cd fusion-engine
+ python examples/example1.py
+```
+
+For different examples, you change the number to the number of the example file
+
+## Community
+
+Our community is just growing, so if you want to help us with the project,
+it will be very helpful!
+We have a discord server at this [link](https://discord.gg/Smg3CK4ZMc)
+Need to contact us? Just DM the Owner or CEO in discord and we will try to react as fast as possible
+
+### Special thanks to these people❤️
+
+- Zenthm (Contributing)
+- XCarCedo (Contributing)
+- FBS_Gamer (Discord server)
+
+## Documentation
+
+See at [The wiki of the project](https://github.com/dimkauzh/fusion-engine/wiki) (Still in work!)
+
+## Coming features
+
+We are working hard to implement very basic and complex stuff so our engine becomes more rigid. These features are worked on or will be worked on:
+
+- Physics system using PyMunk (Being worked on)
+- Delta-Time (Finished!)
+- Pip package and SetupTools (Being worked on)
+- UI (Being worked on)
+- If you have more ideas, please tell us them in our discord group!
+
+## About
+
+Fusion Engine is currently (6/14/2023) build with Python and some Python libraries:
+
+- PySDL2 is used for rendering and windowing
+- PySDL2-DLL is used by PySDL2 for SDL2 binaries
+- PyMunk is used for fysics simulation
+- CX-Freeze is used for building executables (Temporary, it will change when SetupTools is setup)
+
+### Future of this engine
+
+This project began May 1, 2023. The original project began in C, but it's entirely rewritten in Python for it's big userbase and ease of use (productivity). This is actually also my EuroPython project.
+
+Our cool ideas:
+
+- Make a full GUI app (With something like Kivy or Tkinter) - Update: We are currenly working on it with tkinter
+
+## 🚀 About Me
+
+A 13 year old game developer with much passion about game development. So I made this project to grow my programming skills and just make a tool that I can use for myself or a tool for other people to help them develop games.
```

### Comparing `fusion-engine-0.1.0/src/fusion_engine.egg-info/SOURCES.txt` & `fusion-engine-0.1.1/src/fusion_engine.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENCE.md
 README.md
 pyproject.toml
-requirements.txt
 setup.py
 src/fusion_engine.egg-info/PKG-INFO
 src/fusion_engine.egg-info/SOURCES.txt
 src/fusion_engine.egg-info/dependency_links.txt
 src/fusion_engine.egg-info/requires.txt
 src/fusion_engine.egg-info/top_level.txt
 src/fusionengine/__init__.py
```

### Comparing `fusion-engine-0.1.0/src/fusionengine/__init__.py` & `fusion-engine-0.1.1/src/fusionengine/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-__author__ = "Dimkauzh"
-__version__ = "0.1.0"
-
-import fusionengine.files.data as data
-import fusionengine.files.systems as sysconfig
-
-from fusionengine.files.imports import *
-
-class Main:
-    def __init__(self):
-        SDL_Init(SDL_INIT_VIDEO)
-        self.window = window.Window()
-        self.color = color.Colors()
-        self.event = event.Event()
-        self.keys = event.Keys()
-        self.draw = draw.Draw()
-        self.image = image.Image()
-        self.body = body
-        self.system = sysconfig.System()
-        self.rendereroptions = sysconfig.RendererOptions()
-        self.shape = shape.Shapes()
-        
-        self.DEBUGIMAGE = "src/fusionengine/debugfiles/test.png"
-
-    def quit(self, window):
-        SDL_DestroyRenderer(window.renderer)
-        SDL_DestroyWindow(window.window)
-        del window
-        SDL_Quit()
+__author__ = "Dimkauzh"
+__version__ = "0.1.1"
+
+import fusionengine.files.data as data
+import fusionengine.files.systems as sysconfig
+
+from fusionengine.files.imports import *
+
+class Main:
+    def __init__(self):
+        SDL_Init(SDL_INIT_VIDEO)
+        self.window = window.Window()
+        self.color = color.Colors()
+        self.event = event.Event()
+        self.keys = event.Keys()
+        self.draw = draw.Draw()
+        self.image = image.Image()
+        self.body = body
+        self.system = sysconfig.System()
+        self.rendereroptions = sysconfig.RendererOptions()
+        self.shape = shape.Shapes()
+        
+        self.DEBUGIMAGE = "src/fusionengine/debugfiles/test.png"
+
+    def quit(self, window):
+        SDL_DestroyRenderer(window.renderer)
+        SDL_DestroyWindow(window.window)
+        del window
+        SDL_Quit()
```

### Comparing `fusion-engine-0.1.0/src/fusionengine/debugfiles/test.png` & `fusion-engine-0.1.1/src/fusionengine/debugfiles/test.png`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.1.0/src/fusionengine/files/body.py` & `fusion-engine-0.1.1/src/fusionengine/files/body.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,74 @@
-import fusionengine.files.data as data
-
-from fusionengine.files.enums import BodyType
-from fusionengine.files.imports import *
-
-class _RigidBody:
-    def __init__(self, window, x: int, y: int, width: int, height: int) -> None:
-        self._body = data.DataBodies(window, x, y, width, height)
-        self.window = window
-        self.x = x
-        self.y = y
-        self.width = width
-        self.height = height
-        self.body = self._body.body
-        self.space = self._body.space
-        
-class _StaticBody:
-    def __init__(self, window, x: int, y: int, width: int, height: int) -> None:
-        self._body = data.DataBodies(window, x, y, width, height)
-        self.window = window
-        self.x = x
-        self.y = y
-        self.width = width
-        self.height = height
-        self.body = self._body.body
-        self.space = self._body.space
-    
-class Entity: 
-    def __init__(self, bodytype: BodyType, window, x: int, y: int, width: int, height: int) -> None:
-        self.image = None
-        self.x = x
-        self.y = y
-        self.width = width
-        self.height = height
-        self.window = window
-        self.gravity = 0
-        self._setBodyType(bodytype)
-    
-    def openImage(self, window, image, x: int, y: int, width: int, height: int) -> None:
-        image.openImage(window, image, x, y, width, height)
-        self.image = image
-        self.window = window
-        self.x = x
-        self.y = y
-        self.width = width
-        self.height = height
-
-    def newRect(self, window, color: tuple) -> None:
-        data.drawRect(self.window,
-                      self.x,
-                      self.y,
-                      self.width,
-                      self.height,
-                      color
-                      )
-    def setGravity(self, gravity: int) -> None:
-        self.gravity = gravity
-    
-    def _setBodyType(self, bodytype: BodyType) -> None:
-        if bodytype == BodyType.RIGID_BODY:
-            self.body = _RigidBody(self.window,
-                                   self.x,
-                                   self.y,
-                                   self.width,
-                                   self.height
-                                   )
-        elif bodytype == BodyType.STATIC_BODY:
-            self.body = _StaticBody(self.window,
-                                    self.x,
-                                    self.y,
-                                    self.width,
-                                    self.height
-                                    )
+import fusionengine.files.data as data
+import fusionengine.files.window as window
+from fusionengine.files.enums import BodyType
+from fusionengine.files.imports import *
+import fusionengine.files.image as image
+
+class _RigidBody:
+    def __init__(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int) -> None:
+        self._body = data.DataBodies(window, x, y, width, height)
+        self.window = window
+        self.x = x
+        self.y = y
+        self.width = width
+        self.height = height
+        self.body = self._body.body
+        self.space = self._body.space
+        
+class _StaticBody:
+    def __init__(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int) -> None:
+        self._body = data.DataBodies(window, x, y, width, height)
+        self.window = window
+        self.x = x
+        self.y = y
+        self.width = width
+        self.height = height
+        self.body = self._body.body
+        self.space = self._body.space
+    
+class Entity: 
+    def __init__(self, bodytype: BodyType, window: window._CustomRenderer, x: int, y: int, width: int, height: int) -> None:
+        self.image = None
+        self.x = x
+        self.y = y
+        self.width = width
+        self.height = height
+        self.window = window
+        self.gravity = 0
+        self._setBodyType(bodytype)
+    
+    def openImage(self, window: window._CustomRenderer, image: image._CustomImage, x: int, y: int, width: int, height: int) -> None:
+        image.openImage(window, image, x, y, width, height)
+        self.image = image
+        self.window = window
+        self.x = x
+        self.y = y
+        self.width = width
+        self.height = height
+
+    def newRect(self, window: window._CustomRenderer, color: tuple) -> None:
+        data.drawRect(window,
+                      self.x,
+                      self.y,
+                      self.width,
+                      self.height,
+                      color
+                      )
+    def setGravity(self, gravity: int) -> None:
+        self.gravity = gravity
+    
+    def _setBodyType(self, bodytype: BodyType) -> None:
+        if bodytype == BodyType.RIGID_BODY:
+            self.body = _RigidBody(self.window,
+                                   self.x,
+                                   self.y,
+                                   self.width,
+                                   self.height
+                                   )
+        elif bodytype == BodyType.STATIC_BODY:
+            self.body = _StaticBody(self.window,
+                                    self.x,
+                                    self.y,
+                                    self.width,
+                                    self.height
+                                    )
```

### Comparing `fusion-engine-0.1.0/src/fusionengine/files/color.py` & `fusion-engine-0.1.1/src/fusionengine/files/color.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-class Colors:
-    def __init__(self):
-        self.BLUE = (0, 0, 255, 255)
-        self.BLACK = (0, 0, 0, 255)
-        self.WHITE = (255, 255, 255, 255)
-        self.GREEN = (255, 255, 255, 255)
-        self.RED = (255, 0, 0, 255)
-        self.YELLOW = (255, 255, 0, 255)
-        self.PURPLE = (255, 0, 255, 255)
-        self.CYAN = (0, 255, 255, 255)
-        self.ORANGE = (255, 165, 0, 255)
-        self.GRAY = (128, 128, 128, 255)
-        self.BROWN = (165, 42, 42, 255)
-        self.PINK = (255, 192, 203, 255)
-        self.MAGENTA = (255, 0, 255, 255)
-        self.SILVER = (192, 192, 192, 255)
-        self.GOLD = (255, 215, 0, 255)
-        self.BRONZE = (205, 127, 50, 255)
-        self.LIME = (0, 255, 0, 255)
-        self.OLIVE = (128, 128, 0, 255)
-        self.TEAL = (0, 128, 128, 255)
-        self.NAVY = (0, 0, 128, 255)
-        self.MAROON = (128, 0, 0, 255)
-        self.INDIGO = (75, 0, 130, 255)
+
+class Colors:
+    def __init__(self):
+        self.BLUE = (0, 0, 255, 255)
+        self.BLACK = (0, 0, 0, 255)
+        self.WHITE = (255, 255, 255, 255)
+        self.GREEN = (255, 255, 255, 255)
+        self.RED = (255, 0, 0, 255)
+        self.YELLOW = (255, 255, 0, 255)
+        self.PURPLE = (255, 0, 255, 255)
+        self.CYAN = (0, 255, 255, 255)
+        self.ORANGE = (255, 165, 0, 255)
+        self.GRAY = (128, 128, 128, 255)
+        self.BROWN = (165, 42, 42, 255)
+        self.PINK = (255, 192, 203, 255)
+        self.MAGENTA = (255, 0, 255, 255)
+        self.SILVER = (192, 192, 192, 255)
+        self.GOLD = (255, 215, 0, 255)
+        self.BRONZE = (205, 127, 50, 255)
+        self.LIME = (0, 255, 0, 255)
+        self.OLIVE = (128, 128, 0, 255)
+        self.TEAL = (0, 128, 128, 255)
+        self.NAVY = (0, 0, 128, 255)
+        self.MAROON = (128, 0, 0, 255)
+        self.INDIGO = (75, 0, 130, 255)
```

### Comparing `fusion-engine-0.1.0/src/fusionengine/files/event.py` & `fusion-engine-0.1.1/src/fusionengine/files/event.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-from fusionengine.files.imports import *
-
-
-class Event:
-    def __init__(self) -> None:
-        pass
-
-    def keyDown(self, key: int, window) -> bool:
-        event = window.event
-        if event.type == sdl2.SDL_KEYDOWN:
-            if event.key.keysym.sym == key:
-                return True
-        return False
-    def keyDownOnce(self, key: int, window) -> None:
-        pass
-
-
-class Keys:
-    def __init__(self):
-        self.KEY_UNKNOWN = sdl2.SDLK_UNKNOWN
-        self.KEY_RETURN = sdl2.SDLK_RETURN
-        self.KEY_ESCAPE = sdl2.SDLK_ESCAPE
-        self.KEY_BACKSPACE = sdl2.SDLK_BACKSPACE
-        self.KEY_TAB = sdl2.SDLK_TAB
-        self.KEY_SPACE = sdl2.SDLK_SPACE
-        self.KEY_EXCLAIM = sdl2.SDLK_EXCLAIM
-        self.KEY_QUOTEDBL = sdl2.SDLK_QUOTEDBL
-        self.KEY_HASH = sdl2.SDLK_HASH
-        self.KEY_PERCENT = sdl2.SDLK_PERCENT
-        self.KEY_DOLLAR = sdl2.SDLK_DOLLAR
-        self.KEY_AMPERSAND = sdl2.SDLK_AMPERSAND
-        self.KEY_QUOTE = sdl2.SDLK_QUOTE
-        self.KEY_LEFTPAREN = sdl2.SDLK_LEFTPAREN
-        self.KEY_RIGHTPAREN = sdl2.SDLK_RIGHTPAREN
-        self.KEY_ASTERISK = sdl2.SDLK_ASTERISK
-        self.KEY_PLUS = sdl2.SDLK_PLUS
-        self.KEY_COMMA = sdl2.SDLK_COMMA
-        self.KEY_MINUS = sdl2.SDLK_MINUS
-        self.KEY_PERIOD = sdl2.SDLK_PERIOD
-        self.KEY_SLASH = sdl2.SDLK_SLASH
-        self.KEY_0 = sdl2.SDLK_0
-        self.KEY_1 = sdl2.SDLK_1
-        self.KEY_2 = sdl2.SDLK_2
-        self.KEY_3 = sdl2.SDLK_3
-        self.KEY_4 = sdl2.SDLK_4
-        self.KEY_5 = sdl2.SDLK_5
-        self.KEY_6 = sdl2.SDLK_6
-        self.KEY_7 = sdl2.SDLK_7
-        self.KEY_8 = sdl2.SDLK_8
-        self.KEY_9 = sdl2.SDLK_9
-        self.KEY_COLON = sdl2.SDLK_COLON
-        self.KEY_SEMICOLON = sdl2.SDLK_SEMICOLON
-        self.KEY_LESS = sdl2.SDLK_LESS
-        self.KEY_EQUALS = sdl2.SDLK_EQUALS
-        self.KEY_GREATER = sdl2.SDLK_GREATER
-        self.KEY_QUESTION = sdl2.SDLK_QUESTION
-        self.KEY_AT = sdl2.SDLK_AT
-        self.KEY_LEFTBRACKET = sdl2.SDLK_LEFTBRACKET
-        self.KEY_BACKSLASH = sdl2.SDLK_BACKSLASH
-        self.KEY_RIGHTBRACKET = sdl2.SDLK_RIGHTBRACKET
-        self.KEY_CARET = sdl2.SDLK_CARET
-        self.KEY_UNDERSCORE = sdl2.SDLK_UNDERSCORE
-        self.KEY_BACKQUOTE = sdl2.SDLK_BACKQUOTE
-        self.KEY_a = sdl2.SDLK_a
-        self.KEY_b = sdl2.SDLK_b
-        self.KEY_c = sdl2.SDLK_c
-        self.KEY_d = sdl2.SDLK_d
-        self.KEY_e = sdl2.SDLK_e
-        self.KEY_f = sdl2.SDLK_f
-        self.KEY_g = sdl2.SDLK_g
-        self.KEY_h = sdl2.SDLK_h
-        self.KEY_i = sdl2.SDLK_i
-        self.KEY_j = sdl2.SDLK_j
-        self.KEY_k = sdl2.SDLK_k
-        self.KEY_l = sdl2.SDLK_l
-        self.KEY_m = sdl2.SDLK_m
-        self.KEY_n = sdl2.SDLK_n
-        self.KEY_o = sdl2.SDLK_o
-        self.KEY_p = sdl2.SDLK_p
-        self.KEY_q = sdl2.SDLK_q
-        self.KEY_r = sdl2.SDLK_r
-        self.KEY_s = sdl2.SDLK_s
-        self.KEY_t = sdl2.SDLK_t
-        self.KEY_u = sdl2.SDLK_u
-        self.KEY_v = sdl2.SDLK_v
-        self.KEY_w = sdl2.SDLK_w
-        self.KEY_x = sdl2.SDLK_x
-        self.KEY_y = sdl2.SDLK_y
-        self.KEY_z = sdl2.SDLK_z
-        self.KEY_CAPSLOCK = sdl2.SDLK_CAPSLOCK
-        self.KEY_F1 = sdl2.SDLK_F1
-        self.KEY_F2 = sdl2.SDLK_F2
-        self.KEY_F3 = sdl2.SDLK_F3
-        self.KEY_F4 = sdl2.SDLK_F4
-        self.KEY_F5 = sdl2.SDLK_F5
-        self.KEY_F6 = sdl2.SDLK_F6
-        self.KEY_F7 = sdl2.SDLK_F7
-        self.KEY_F8 = sdl2.SDLK_F8
-        self.KEY_F9 = sdl2.SDLK_F9
-        self.KEY_F10 = sdl2.SDLK_F10
-        self.KEY_F11 = sdl2.SDLK_F11
-        self.KEY_F12 = sdl2.SDLK_F12
-        self.KEY_PRINTSCREEN = sdl2.SDLK_PRINTSCREEN
-        self.KEY_SCROLLLOCK = sdl2.SDLK_SCROLLLOCK
-        self.KEY_PAUSE = sdl2.SDLK_PAUSE
-        self.KEY_INSERT = sdl2.SDLK_INSERT
-        self.KEY_HOME = sdl2.SDLK_HOME
-        self.KEY_PAGEUP = sdl2.SDLK_PAGEUP
-        self.KEY_DELETE = sdl2.SDLK_DELETE
-        self.KEY_END = sdl2.SDLK_END
-        self.KEY_PAGEDOWN = sdl2.SDLK_PAGEDOWN
-        self.KEY_RIGHT = sdl2.SDLK_RIGHT
-        self.KEY_LEFT = sdl2.SDLK_LEFT
-        self.KEY_DOWN = sdl2.SDLK_DOWN
-        self.KEY_UP = sdl2.SDLK_UP
-        self.KEY_NUMLOCKCLEAR = sdl2.SDLK_NUMLOCKCLEAR
-        self.KEY_KP_DIVIDE = sdl2.SDLK_KP_DIVIDE
-        self.KEY_KP_MULTIPLY = sdl2.SDLK_KP_MULTIPLY
-        self.KEY_KP_MINUS = sdl2.SDLK_KP_MINUS
-        self.KEY_KP_PLUS = sdl2.SDLK_KP_PLUS
-        self.KEY_KP_ENTER = sdl2.SDLK_KP_ENTER
-        self.KEY_KP_1 = sdl2.SDLK_KP_1
-        self.KEY_KP_2 = sdl2.SDLK_KP_2
-        self.KEY_KP_3 = sdl2.SDLK_KP_3
-        self.KEY_KP_4 = sdl2.SDLK_KP_4
-        self.KEY_KP_5 = sdl2.SDLK_KP_5
-        self.KEY_KP_6 = sdl2.SDLK_KP_6
-        self.KEY_KP_7 = sdl2.SDLK_KP_7
-        self.KEY_KP_8 = sdl2.SDLK_KP_8
-        self.KEY_KP_9 = sdl2.SDLK_KP_9
-        self.KEY_KP_0 = sdl2.SDLK_KP_0
-        self.KEY_KP_PERIOD = sdl2.SDLK_KP_PERIOD
-        self.KEY_APPLICATION = sdl2.SDLK_APPLICATION
-        self.KEY_POWER = sdl2.SDLK_POWER
-        self.KEY_KP_EQUALS = sdl2.SDLK_KP_EQUALS
-        self.KEY_F13 = sdl2.SDLK_F13
-        self.KEY_F14 = sdl2.SDLK_F14
-        self.KEY_F15 = sdl2.SDLK_F15
-        self.KEY_F16 = sdl2.SDLK_F16
-        self.KEY_F17 = sdl2.SDLK_F17
-        self.KEY_F18 = sdl2.SDLK_F18
-        self.KEY_F19 = sdl2.SDLK_F19
-        self.KEY_F20 = sdl2.SDLK_F20
-        self.KEY_F21 = sdl2.SDLK_F21
-        self.KEY_F22 = sdl2.SDLK_F22
-        self.KEY_F23 = sdl2.SDLK_F23
-        self.KEY_F24 = sdl2.SDLK_F24
-        self.KEY_EXECUTE = sdl2.SDLK_EXECUTE
-        self.KEY_HELP = sdl2.SDLK_HELP
-        self.KEY_MENU = sdl2.SDLK_MENU
-        self.KEY_SELECT = sdl2.SDLK_SELECT
-        self.KEY_STOP = sdl2.SDLK_STOP
-        self.KEY_AGAIN = sdl2.SDLK_AGAIN
-        self.KEY_UNDO = sdl2.SDLK_UNDO
-        self.KEY_CUT = sdl2.SDLK_CUT
-        self.KEY_COPY = sdl2.SDLK_COPY
-        self.KEY_PASTE = sdl2.SDLK_PASTE
-        self.KEY_FIND = sdl2.SDLK_FIND
-        self.KEY_MUTE = sdl2.SDLK_MUTE
-        self.KEY_VOLUMEUP = sdl2.SDLK_VOLUMEUP
-        self.KEY_VOLUMEDOWN = sdl2.SDLK_VOLUMEDOWN
-        self.KEY_KP_COMMA = sdl2.SDLK_KP_COMMA
-        self.KEY_KP_EQUALSAS400 = sdl2.SDLK_KP_EQUALSAS400
-        self.KEY_ALTERASE = sdl2.SDLK_ALTERASE
-        self.KEY_SYSREQ = sdl2.SDLK_SYSREQ
-        self.KEY_CANCEL = sdl2.SDLK_CANCEL
-        self.KEY_CLEAR = sdl2.SDLK_CLEAR
-        self.KEY_PRIOR = sdl2.SDLK_PRIOR
-        self.KEY_RETURN2 = sdl2.SDLK_RETURN2
-        self.KEY_SEPARATOR = sdl2.SDLK_SEPARATOR
-        self.KEY_OUT = sdl2.SDLK_OUT
-        self.KEY_OPER = sdl2.SDLK_OPER
-        self.KEY_CLEARAGAIN = sdl2.SDLK_CLEARAGAIN
-        self.KEY_CRSEL = sdl2.SDLK_CRSEL
-        self.KEY_EXSEL = sdl2.SDLK_EXSEL
-        self.KEY_KP_00 = sdl2.SDLK_KP_00
-        self.KEY_KP_000 = sdl2.SDLK_KP_000
-        self.KEY_THOUSANDSSEPARATOR = sdl2.SDLK_THOUSANDSSEPARATOR
-        self.KEY_DECIMALSEPARATOR = sdl2.SDLK_DECIMALSEPARATOR
-        self.KEY_CURRENCYUNIT = sdl2.SDLK_CURRENCYUNIT
-        self.KEY_CURRENCYSUBUNIT = sdl2.SDLK_CURRENCYSUBUNIT
-        self.KEY_KP_LEFTPAREN = sdl2.SDLK_KP_LEFTPAREN
-        self.KEY_KP_RIGHTPAREN = sdl2.SDLK_KP_RIGHTPAREN
-        self.KEY_KP_LEFTBRACE = sdl2.SDLK_KP_LEFTBRACE
-        self.KEY_KP_RIGHTBRACE = sdl2.SDLK_KP_RIGHTBRACE
-        self.KEY_KP_TAB = sdl2.SDLK_KP_TAB
-        self.KEY_KP_BACKSPACE = sdl2.SDLK_KP_BACKSPACE
-        self.KEY_KP_A = sdl2.SDLK_KP_A
-        self.KEY_KP_B = sdl2.SDLK_KP_B
-        self.KEY_KP_C = sdl2.SDLK_KP_C
-        self.KEY_KP_D = sdl2.SDLK_KP_D
-        self.KEY_KP_E = sdl2.SDLK_KP_E
-        self.KEY_KP_F = sdl2.SDLK_KP_F
-        self.KEY_KP_XOR = sdl2.SDLK_KP_XOR
-        self.KEY_KP_POWER = sdl2.SDLK_KP_POWER
-        self.KEY_KP_PERCENT = sdl2.SDLK_KP_PERCENT
-        self.KEY_KP_LESS = sdl2.SDLK_KP_LESS
-        self.KEY_KP_GREATER = sdl2.SDLK_KP_GREATER
-        self.KEY_KP_AMPERSAND = sdl2.SDLK_KP_AMPERSAND
-        self.KEY_KP_DBLAMPERSAND = sdl2.SDLK_KP_DBLAMPERSAND
-        self.KEY_KP_VERTICALBAR = sdl2.SDLK_KP_VERTICALBAR
-        self.KEY_KP_DBLVERTICALBAR = sdl2.SDLK_KP_DBLVERTICALBAR
-        self.KEY_KP_COLON = sdl2.SDLK_KP_COLON
-        self.KEY_KP_HASH = sdl2.SDLK_KP_HASH
-        self.KEY_KP_SPACE = sdl2.SDLK_KP_SPACE
-        self.KEY_KP_AT = sdl2.SDLK_KP_AT
-        self.KEY_KP_EXCLAM = sdl2.SDLK_KP_EXCLAM
-        self.KEY_KP_MEMSTORE = sdl2.SDLK_KP_MEMSTORE
-        self.KEY_KP_MEMRECALL = sdl2.SDLK_KP_MEMRECALL
-        self.KEY_KP_MEMCLEAR = sdl2.SDLK_KP_MEMCLEAR
-        self.KEY_KP_MEMADD = sdl2.SDLK_KP_MEMADD
-        self.KEY_KP_MEMSUBTRACT = sdl2.SDLK_KP_MEMSUBTRACT
-        self.KEY_KP_MEMMULTIPLY = sdl2.SDLK_KP_MEMMULTIPLY
-        self.KEY_KP_MEMDIVIDE = sdl2.SDLK_KP_MEMDIVIDE
-        self.KEY_KP_PLUSMINUS = sdl2.SDLK_KP_PLUSMINUS
-        self.KEY_KP_CLEAR = sdl2.SDLK_KP_CLEAR
-        self.KEY_KP_CLEARENTRY = sdl2.SDLK_KP_CLEARENTRY
-        self.KEY_KP_BINARY = sdl2.SDLK_KP_BINARY
-        self.KEY_KP_OCTAL = sdl2.SDLK_KP_OCTAL
-        self.KEY_KP_DECIMAL = sdl2.SDLK_KP_DECIMAL
-        self.KEY_KP_HEXADECIMAL = sdl2.SDLK_KP_HEXADECIMAL
-        self.KEY_LCTRL = sdl2.SDLK_LCTRL
-        self.KEY_LSHIFT = sdl2.SDLK_LSHIFT
-        self.KEY_LALT = sdl2.SDLK_LALT
-        self.KEY_LGUI = sdl2.SDLK_LGUI
-        self.KEY_RCTRL = sdl2.SDLK_RCTRL
-        self.KEY_RSHIFT = sdl2.SDLK_RSHIFT
-        self.KEY_RALT = sdl2.SDLK_RALT
-        self.KEY_RGUI = sdl2.SDLK_RGUI
-        self.KEY_MODE = sdl2.SDLK_MODE
-        self.KEY_AUDIONEXT = sdl2.SDLK_AUDIONEXT
-        self.KEY_AUDIOPREV = sdl2.SDLK_AUDIOPREV
-        self.KEY_AUDIOSTOP = sdl2.SDLK_AUDIOSTOP
-        self.KEY_AUDIOPLAY = sdl2.SDLK_AUDIOPLAY
-        self.KEY_AUDIOMUTE = sdl2.SDLK_AUDIOMUTE
-        self.KEY_MEDIASELECT = sdl2.SDLK_MEDIASELECT
-        self.KEY_WWW = sdl2.SDLK_WWW
-        self.KEY_MAIL = sdl2.SDLK_MAIL
-        self.KEY_CALCULATOR = sdl2.SDLK_CALCULATOR
-        self.KEY_COMPUTER = sdl2.SDLK_COMPUTER
-        self.KEY_AC_SEARCH = sdl2.SDLK_AC_SEARCH
-        self.KEY_AC_HOME = sdl2.SDLK_AC_HOME
-        self.KEY_AC_BACK = sdl2.SDLK_AC_BACK
-        self.KEY_AC_FORWARD = sdl2.SDLK_AC_FORWARD
-        self.KEY_AC_STOP = sdl2.SDLK_AC_STOP
-        self.KEY_AC_REFRESH = sdl2.SDLK_AC_REFRESH
-        self.KEY_AC_BOOKMARKS = sdl2.SDLK_AC_BOOKMARKS
-        self.KEY_BRIGHTNESSDOWN = sdl2.SDLK_BRIGHTNESSDOWN
-        self.KEY_BRIGHTNESSUP = sdl2.SDLK_BRIGHTNESSUP
-        self.KEY_DISPLAYSWITCH = sdl2.SDLK_DISPLAYSWITCH
-        self.KEY_KBDILLUMTOGGLE = sdl2.SDLK_KBDILLUMTOGGLE
-        self.KEY_KBDILLUMDOWN = sdl2.SDLK_KBDILLUMDOWN
-        self.KEY_KBDILLUMUP = sdl2.SDLK_KBDILLUMUP
-        self.KEY_EJECT = sdl2.SDLK_EJECT
-        self.KEY_SLEEP = sdl2.SDLK_SLEEP
+from fusionengine.files.imports import *
+import fusionengine.files.window as window
+
+class Event:
+    def __init__(self) -> None:
+        pass
+
+    def keyDown(self, key: int, window: window._CustomRenderer) -> bool:
+        event = window.event
+        if event.type == sdl2.SDL_KEYDOWN:
+            if event.key.keysym.sym == key:
+                return True
+        return False
+    def keyDownOnce(self, key: int, window: window._CustomRenderer) -> bool:
+        pass
+
+
+class Keys:
+    def __init__(self):
+        self.KEY_UNKNOWN = sdl2.SDLK_UNKNOWN
+        self.KEY_RETURN = sdl2.SDLK_RETURN
+        self.KEY_ESCAPE = sdl2.SDLK_ESCAPE
+        self.KEY_BACKSPACE = sdl2.SDLK_BACKSPACE
+        self.KEY_TAB = sdl2.SDLK_TAB
+        self.KEY_SPACE = sdl2.SDLK_SPACE
+        self.KEY_EXCLAIM = sdl2.SDLK_EXCLAIM
+        self.KEY_QUOTEDBL = sdl2.SDLK_QUOTEDBL
+        self.KEY_HASH = sdl2.SDLK_HASH
+        self.KEY_PERCENT = sdl2.SDLK_PERCENT
+        self.KEY_DOLLAR = sdl2.SDLK_DOLLAR
+        self.KEY_AMPERSAND = sdl2.SDLK_AMPERSAND
+        self.KEY_QUOTE = sdl2.SDLK_QUOTE
+        self.KEY_LEFTPAREN = sdl2.SDLK_LEFTPAREN
+        self.KEY_RIGHTPAREN = sdl2.SDLK_RIGHTPAREN
+        self.KEY_ASTERISK = sdl2.SDLK_ASTERISK
+        self.KEY_PLUS = sdl2.SDLK_PLUS
+        self.KEY_COMMA = sdl2.SDLK_COMMA
+        self.KEY_MINUS = sdl2.SDLK_MINUS
+        self.KEY_PERIOD = sdl2.SDLK_PERIOD
+        self.KEY_SLASH = sdl2.SDLK_SLASH
+        self.KEY_0 = sdl2.SDLK_0
+        self.KEY_1 = sdl2.SDLK_1
+        self.KEY_2 = sdl2.SDLK_2
+        self.KEY_3 = sdl2.SDLK_3
+        self.KEY_4 = sdl2.SDLK_4
+        self.KEY_5 = sdl2.SDLK_5
+        self.KEY_6 = sdl2.SDLK_6
+        self.KEY_7 = sdl2.SDLK_7
+        self.KEY_8 = sdl2.SDLK_8
+        self.KEY_9 = sdl2.SDLK_9
+        self.KEY_COLON = sdl2.SDLK_COLON
+        self.KEY_SEMICOLON = sdl2.SDLK_SEMICOLON
+        self.KEY_LESS = sdl2.SDLK_LESS
+        self.KEY_EQUALS = sdl2.SDLK_EQUALS
+        self.KEY_GREATER = sdl2.SDLK_GREATER
+        self.KEY_QUESTION = sdl2.SDLK_QUESTION
+        self.KEY_AT = sdl2.SDLK_AT
+        self.KEY_LEFTBRACKET = sdl2.SDLK_LEFTBRACKET
+        self.KEY_BACKSLASH = sdl2.SDLK_BACKSLASH
+        self.KEY_RIGHTBRACKET = sdl2.SDLK_RIGHTBRACKET
+        self.KEY_CARET = sdl2.SDLK_CARET
+        self.KEY_UNDERSCORE = sdl2.SDLK_UNDERSCORE
+        self.KEY_BACKQUOTE = sdl2.SDLK_BACKQUOTE
+        self.KEY_a = sdl2.SDLK_a
+        self.KEY_b = sdl2.SDLK_b
+        self.KEY_c = sdl2.SDLK_c
+        self.KEY_d = sdl2.SDLK_d
+        self.KEY_e = sdl2.SDLK_e
+        self.KEY_f = sdl2.SDLK_f
+        self.KEY_g = sdl2.SDLK_g
+        self.KEY_h = sdl2.SDLK_h
+        self.KEY_i = sdl2.SDLK_i
+        self.KEY_j = sdl2.SDLK_j
+        self.KEY_k = sdl2.SDLK_k
+        self.KEY_l = sdl2.SDLK_l
+        self.KEY_m = sdl2.SDLK_m
+        self.KEY_n = sdl2.SDLK_n
+        self.KEY_o = sdl2.SDLK_o
+        self.KEY_p = sdl2.SDLK_p
+        self.KEY_q = sdl2.SDLK_q
+        self.KEY_r = sdl2.SDLK_r
+        self.KEY_s = sdl2.SDLK_s
+        self.KEY_t = sdl2.SDLK_t
+        self.KEY_u = sdl2.SDLK_u
+        self.KEY_v = sdl2.SDLK_v
+        self.KEY_w = sdl2.SDLK_w
+        self.KEY_x = sdl2.SDLK_x
+        self.KEY_y = sdl2.SDLK_y
+        self.KEY_z = sdl2.SDLK_z
+        self.KEY_CAPSLOCK = sdl2.SDLK_CAPSLOCK
+        self.KEY_F1 = sdl2.SDLK_F1
+        self.KEY_F2 = sdl2.SDLK_F2
+        self.KEY_F3 = sdl2.SDLK_F3
+        self.KEY_F4 = sdl2.SDLK_F4
+        self.KEY_F5 = sdl2.SDLK_F5
+        self.KEY_F6 = sdl2.SDLK_F6
+        self.KEY_F7 = sdl2.SDLK_F7
+        self.KEY_F8 = sdl2.SDLK_F8
+        self.KEY_F9 = sdl2.SDLK_F9
+        self.KEY_F10 = sdl2.SDLK_F10
+        self.KEY_F11 = sdl2.SDLK_F11
+        self.KEY_F12 = sdl2.SDLK_F12
+        self.KEY_PRINTSCREEN = sdl2.SDLK_PRINTSCREEN
+        self.KEY_SCROLLLOCK = sdl2.SDLK_SCROLLLOCK
+        self.KEY_PAUSE = sdl2.SDLK_PAUSE
+        self.KEY_INSERT = sdl2.SDLK_INSERT
+        self.KEY_HOME = sdl2.SDLK_HOME
+        self.KEY_PAGEUP = sdl2.SDLK_PAGEUP
+        self.KEY_DELETE = sdl2.SDLK_DELETE
+        self.KEY_END = sdl2.SDLK_END
+        self.KEY_PAGEDOWN = sdl2.SDLK_PAGEDOWN
+        self.KEY_RIGHT = sdl2.SDLK_RIGHT
+        self.KEY_LEFT = sdl2.SDLK_LEFT
+        self.KEY_DOWN = sdl2.SDLK_DOWN
+        self.KEY_UP = sdl2.SDLK_UP
+        self.KEY_NUMLOCKCLEAR = sdl2.SDLK_NUMLOCKCLEAR
+        self.KEY_KP_DIVIDE = sdl2.SDLK_KP_DIVIDE
+        self.KEY_KP_MULTIPLY = sdl2.SDLK_KP_MULTIPLY
+        self.KEY_KP_MINUS = sdl2.SDLK_KP_MINUS
+        self.KEY_KP_PLUS = sdl2.SDLK_KP_PLUS
+        self.KEY_KP_ENTER = sdl2.SDLK_KP_ENTER
+        self.KEY_KP_1 = sdl2.SDLK_KP_1
+        self.KEY_KP_2 = sdl2.SDLK_KP_2
+        self.KEY_KP_3 = sdl2.SDLK_KP_3
+        self.KEY_KP_4 = sdl2.SDLK_KP_4
+        self.KEY_KP_5 = sdl2.SDLK_KP_5
+        self.KEY_KP_6 = sdl2.SDLK_KP_6
+        self.KEY_KP_7 = sdl2.SDLK_KP_7
+        self.KEY_KP_8 = sdl2.SDLK_KP_8
+        self.KEY_KP_9 = sdl2.SDLK_KP_9
+        self.KEY_KP_0 = sdl2.SDLK_KP_0
+        self.KEY_KP_PERIOD = sdl2.SDLK_KP_PERIOD
+        self.KEY_APPLICATION = sdl2.SDLK_APPLICATION
+        self.KEY_POWER = sdl2.SDLK_POWER
+        self.KEY_KP_EQUALS = sdl2.SDLK_KP_EQUALS
+        self.KEY_F13 = sdl2.SDLK_F13
+        self.KEY_F14 = sdl2.SDLK_F14
+        self.KEY_F15 = sdl2.SDLK_F15
+        self.KEY_F16 = sdl2.SDLK_F16
+        self.KEY_F17 = sdl2.SDLK_F17
+        self.KEY_F18 = sdl2.SDLK_F18
+        self.KEY_F19 = sdl2.SDLK_F19
+        self.KEY_F20 = sdl2.SDLK_F20
+        self.KEY_F21 = sdl2.SDLK_F21
+        self.KEY_F22 = sdl2.SDLK_F22
+        self.KEY_F23 = sdl2.SDLK_F23
+        self.KEY_F24 = sdl2.SDLK_F24
+        self.KEY_EXECUTE = sdl2.SDLK_EXECUTE
+        self.KEY_HELP = sdl2.SDLK_HELP
+        self.KEY_MENU = sdl2.SDLK_MENU
+        self.KEY_SELECT = sdl2.SDLK_SELECT
+        self.KEY_STOP = sdl2.SDLK_STOP
+        self.KEY_AGAIN = sdl2.SDLK_AGAIN
+        self.KEY_UNDO = sdl2.SDLK_UNDO
+        self.KEY_CUT = sdl2.SDLK_CUT
+        self.KEY_COPY = sdl2.SDLK_COPY
+        self.KEY_PASTE = sdl2.SDLK_PASTE
+        self.KEY_FIND = sdl2.SDLK_FIND
+        self.KEY_MUTE = sdl2.SDLK_MUTE
+        self.KEY_VOLUMEUP = sdl2.SDLK_VOLUMEUP
+        self.KEY_VOLUMEDOWN = sdl2.SDLK_VOLUMEDOWN
+        self.KEY_KP_COMMA = sdl2.SDLK_KP_COMMA
+        self.KEY_KP_EQUALSAS400 = sdl2.SDLK_KP_EQUALSAS400
+        self.KEY_ALTERASE = sdl2.SDLK_ALTERASE
+        self.KEY_SYSREQ = sdl2.SDLK_SYSREQ
+        self.KEY_CANCEL = sdl2.SDLK_CANCEL
+        self.KEY_CLEAR = sdl2.SDLK_CLEAR
+        self.KEY_PRIOR = sdl2.SDLK_PRIOR
+        self.KEY_RETURN2 = sdl2.SDLK_RETURN2
+        self.KEY_SEPARATOR = sdl2.SDLK_SEPARATOR
+        self.KEY_OUT = sdl2.SDLK_OUT
+        self.KEY_OPER = sdl2.SDLK_OPER
+        self.KEY_CLEARAGAIN = sdl2.SDLK_CLEARAGAIN
+        self.KEY_CRSEL = sdl2.SDLK_CRSEL
+        self.KEY_EXSEL = sdl2.SDLK_EXSEL
+        self.KEY_KP_00 = sdl2.SDLK_KP_00
+        self.KEY_KP_000 = sdl2.SDLK_KP_000
+        self.KEY_THOUSANDSSEPARATOR = sdl2.SDLK_THOUSANDSSEPARATOR
+        self.KEY_DECIMALSEPARATOR = sdl2.SDLK_DECIMALSEPARATOR
+        self.KEY_CURRENCYUNIT = sdl2.SDLK_CURRENCYUNIT
+        self.KEY_CURRENCYSUBUNIT = sdl2.SDLK_CURRENCYSUBUNIT
+        self.KEY_KP_LEFTPAREN = sdl2.SDLK_KP_LEFTPAREN
+        self.KEY_KP_RIGHTPAREN = sdl2.SDLK_KP_RIGHTPAREN
+        self.KEY_KP_LEFTBRACE = sdl2.SDLK_KP_LEFTBRACE
+        self.KEY_KP_RIGHTBRACE = sdl2.SDLK_KP_RIGHTBRACE
+        self.KEY_KP_TAB = sdl2.SDLK_KP_TAB
+        self.KEY_KP_BACKSPACE = sdl2.SDLK_KP_BACKSPACE
+        self.KEY_KP_A = sdl2.SDLK_KP_A
+        self.KEY_KP_B = sdl2.SDLK_KP_B
+        self.KEY_KP_C = sdl2.SDLK_KP_C
+        self.KEY_KP_D = sdl2.SDLK_KP_D
+        self.KEY_KP_E = sdl2.SDLK_KP_E
+        self.KEY_KP_F = sdl2.SDLK_KP_F
+        self.KEY_KP_XOR = sdl2.SDLK_KP_XOR
+        self.KEY_KP_POWER = sdl2.SDLK_KP_POWER
+        self.KEY_KP_PERCENT = sdl2.SDLK_KP_PERCENT
+        self.KEY_KP_LESS = sdl2.SDLK_KP_LESS
+        self.KEY_KP_GREATER = sdl2.SDLK_KP_GREATER
+        self.KEY_KP_AMPERSAND = sdl2.SDLK_KP_AMPERSAND
+        self.KEY_KP_DBLAMPERSAND = sdl2.SDLK_KP_DBLAMPERSAND
+        self.KEY_KP_VERTICALBAR = sdl2.SDLK_KP_VERTICALBAR
+        self.KEY_KP_DBLVERTICALBAR = sdl2.SDLK_KP_DBLVERTICALBAR
+        self.KEY_KP_COLON = sdl2.SDLK_KP_COLON
+        self.KEY_KP_HASH = sdl2.SDLK_KP_HASH
+        self.KEY_KP_SPACE = sdl2.SDLK_KP_SPACE
+        self.KEY_KP_AT = sdl2.SDLK_KP_AT
+        self.KEY_KP_EXCLAM = sdl2.SDLK_KP_EXCLAM
+        self.KEY_KP_MEMSTORE = sdl2.SDLK_KP_MEMSTORE
+        self.KEY_KP_MEMRECALL = sdl2.SDLK_KP_MEMRECALL
+        self.KEY_KP_MEMCLEAR = sdl2.SDLK_KP_MEMCLEAR
+        self.KEY_KP_MEMADD = sdl2.SDLK_KP_MEMADD
+        self.KEY_KP_MEMSUBTRACT = sdl2.SDLK_KP_MEMSUBTRACT
+        self.KEY_KP_MEMMULTIPLY = sdl2.SDLK_KP_MEMMULTIPLY
+        self.KEY_KP_MEMDIVIDE = sdl2.SDLK_KP_MEMDIVIDE
+        self.KEY_KP_PLUSMINUS = sdl2.SDLK_KP_PLUSMINUS
+        self.KEY_KP_CLEAR = sdl2.SDLK_KP_CLEAR
+        self.KEY_KP_CLEARENTRY = sdl2.SDLK_KP_CLEARENTRY
+        self.KEY_KP_BINARY = sdl2.SDLK_KP_BINARY
+        self.KEY_KP_OCTAL = sdl2.SDLK_KP_OCTAL
+        self.KEY_KP_DECIMAL = sdl2.SDLK_KP_DECIMAL
+        self.KEY_KP_HEXADECIMAL = sdl2.SDLK_KP_HEXADECIMAL
+        self.KEY_LCTRL = sdl2.SDLK_LCTRL
+        self.KEY_LSHIFT = sdl2.SDLK_LSHIFT
+        self.KEY_LALT = sdl2.SDLK_LALT
+        self.KEY_LGUI = sdl2.SDLK_LGUI
+        self.KEY_RCTRL = sdl2.SDLK_RCTRL
+        self.KEY_RSHIFT = sdl2.SDLK_RSHIFT
+        self.KEY_RALT = sdl2.SDLK_RALT
+        self.KEY_RGUI = sdl2.SDLK_RGUI
+        self.KEY_MODE = sdl2.SDLK_MODE
+        self.KEY_AUDIONEXT = sdl2.SDLK_AUDIONEXT
+        self.KEY_AUDIOPREV = sdl2.SDLK_AUDIOPREV
+        self.KEY_AUDIOSTOP = sdl2.SDLK_AUDIOSTOP
+        self.KEY_AUDIOPLAY = sdl2.SDLK_AUDIOPLAY
+        self.KEY_AUDIOMUTE = sdl2.SDLK_AUDIOMUTE
+        self.KEY_MEDIASELECT = sdl2.SDLK_MEDIASELECT
+        self.KEY_WWW = sdl2.SDLK_WWW
+        self.KEY_MAIL = sdl2.SDLK_MAIL
+        self.KEY_CALCULATOR = sdl2.SDLK_CALCULATOR
+        self.KEY_COMPUTER = sdl2.SDLK_COMPUTER
+        self.KEY_AC_SEARCH = sdl2.SDLK_AC_SEARCH
+        self.KEY_AC_HOME = sdl2.SDLK_AC_HOME
+        self.KEY_AC_BACK = sdl2.SDLK_AC_BACK
+        self.KEY_AC_FORWARD = sdl2.SDLK_AC_FORWARD
+        self.KEY_AC_STOP = sdl2.SDLK_AC_STOP
+        self.KEY_AC_REFRESH = sdl2.SDLK_AC_REFRESH
+        self.KEY_AC_BOOKMARKS = sdl2.SDLK_AC_BOOKMARKS
+        self.KEY_BRIGHTNESSDOWN = sdl2.SDLK_BRIGHTNESSDOWN
+        self.KEY_BRIGHTNESSUP = sdl2.SDLK_BRIGHTNESSUP
+        self.KEY_DISPLAYSWITCH = sdl2.SDLK_DISPLAYSWITCH
+        self.KEY_KBDILLUMTOGGLE = sdl2.SDLK_KBDILLUMTOGGLE
+        self.KEY_KBDILLUMDOWN = sdl2.SDLK_KBDILLUMDOWN
+        self.KEY_KBDILLUMUP = sdl2.SDLK_KBDILLUMUP
+        self.KEY_EJECT = sdl2.SDLK_EJECT
+        self.KEY_SLEEP = sdl2.SDLK_SLEEP
```

### Comparing `fusion-engine-0.1.0/src/fusionengine/files/storage.py` & `fusion-engine-0.1.1/src/fusionengine/files/storage.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-import json
-import typing
-from pathlib import Path
-
-from fusionengine.files.exceptions import InvalidType, JsonStorageInvalidIndex
-
-class JsonStorage:
-    """JsonStorage is a storage class for saving json databases, currently all data is loaded from
-    disk and saved to memory when you done with the storage you can just save it to the disk file
-    using save method
-    
-    Attributes:
-        file_path (str): The path to the storage file on disk
-        storage (list): The storage variable saved to memory
-    """
-
-    def __init__(self, file_path: str):
-        self.storage = []
-        self.file_path = Path(file_path)
-
-        if self.file_path.exists():
-            with open(self.file_path, mode="r", encoding="utf8") as file:
-                self.storage = json.load(file)
-    def insert(self, _dict: dict[typing.Any, typing.Any]) -> bool:
-        try:
-            if not isinstance(_dict, dict):
-                raise InvalidType(f"_dict excepted to be dict not {type(_dict)}")
-
-            self.storage.append(_dict)
-            return True
-        except:
-            return False
-    def search(self, search_dict: dict[typing.Any, typing.Any],
-        first: bool = False,
-        get_index: bool = False) -> typing.Union[dict, list, tuple, None]:
-        """Search for a entry based on the search_dict
-        
-        Args:
-            search_dict (dict): search_dict is a dictionary describing keys:values to search for
-            in the entries
-            first (bool, optional): only return the first result that found
-            nested_search (bool, optional): if its true if will search for keys and values
-            based on search_dict in nested data structures (like another dictionary in the
-            parent main dict entry)
-        
-        Returns:
-            typing.Union[dict, list, tuple, None]: The entries that found if
-            first is False otherwise the first entry that found 
-            if get_index is true then it will return a tuple
-            containing two values which being the index of the entry
-            aside the value of it(returns None if nothing found)
-        """
-        if first:
-            # Only search for the first entry
-            for index, entry in enumerate(self.storage):
-                passed_every_search = True
-                for sk, sv in search_dict.items():
-                    if entry.get(sk) != sv:
-                        passed_every_search = False
-                if passed_every_search:
-                    if get_index:
-                        return (entry, index)
-                    else:
-                        return entry
-        else:
-            # Search for all entries
-            founded_entries = []
-            for index, entry in enumerate(self.storage):
-                passed_every_search = True
-                for sk, sv in search_dict.items():
-
-                    if entry.get(sk) != sv:
-                        passed_every_search = False
-                if passed_every_search:
-                    if get_index:
-                        founded_entries.append((entry, index))
-                    else:
-                        founded_entries.append(entry)
-            return founded_entries
-    def update(self, index: int, new_entry: dict[typing.Any, typing.Any]) -> bool:
-        """Update the entry based on the index to new_dict
-        
-        Args:
-            index (int): The index of the entry you want to update
-            new_entry (dict): The new updated entry
-        
-        Returns:
-            bool: Wether the action was successful or not
-        
-        Raises:
-            InvalidType: In case the index parameter is not an integer or new_entry
-            is not a dict
-            JsonStorageInvalidIndex: In case the index is out of range and couldn't be find
-            in the entries
-        """
-        if not isinstance(index, int):
-            raise InvalidType(f"index excepted to be integer not {type(index)}")
-        if not isinstance(new_entry, dict):
-            raise InvalidType(f"new_entry excepted to be dict not {type(new_entry)}")
-        try:
-            self.storage[index] = new_entry
-            return True
-        except IndexError:
-            raise JsonStorageInvalidIndex("Invalid index, couldn't find the index in entries")
-        except:
-            return False
-    def delete(self, index: int) -> bool:
-
-        """Delete an entry based on the index given
-        
-        Args:
-            index (int): The index of the entry you want to delete
-        
-        Returns:
-            bool: Wether the action was successful or not
-        
-        Raises:
-            InvalidType: In case the index parameter is not an integer
-            JsonStorageInvalidIndex: In case the index is out of range and couldn't be find
-            in the entries
-        """
-        if not isinstance(index, int):
-            raise InvalidType(f"index excepted to be integer not {type(index)}")
-        try:
-            del self.storage[index]
-            return True
-        except IndexError:
-            raise JsonStorageInvalidIndex("Invalid index, couldn't find the index in entries")
-        except:
-            return False
-    def save(self) -> bool:
-        """Saves the storage variable into disk
-        
-        Returns:
-            bool: Wether the action was successful or not
-        """
-        try:
-            with open(self.file_path, mode="w", encoding="utf8") as file:
-                json.dump(self.storage, file)
-            return True
-        except:
-            return False
+import json
+import typing
+from pathlib import Path
+
+from fusionengine.files.exceptions import InvalidType, JsonStorageInvalidIndex
+
+class JsonStorage:
+    """JsonStorage is a storage class for saving json databases, currently all data is loaded from
+    disk and saved to memory when you done with the storage you can just save it to the disk file
+    using save method
+    
+    Attributes:
+        file_path (str): The path to the storage file on disk
+        storage (list): The storage variable saved to memory
+    """
+
+    def __init__(self, file_path: str):
+        self.storage = []
+        self.file_path = Path(file_path)
+
+        if self.file_path.exists():
+            with open(self.file_path, mode="r", encoding="utf8") as file:
+                self.storage = json.load(file)
+    def insert(self, _dict: dict[typing.Any, typing.Any]) -> bool:
+        try:
+            if not isinstance(_dict, dict):
+                raise InvalidType(f"_dict excepted to be dict not {type(_dict)}")
+
+            self.storage.append(_dict)
+            return True
+        except:
+            return False
+    def search(self, search_dict: dict[typing.Any, typing.Any],
+        first: bool = False,
+        get_index: bool = False) -> typing.Union[dict, list, tuple, None]:
+        """Search for a entry based on the search_dict
+        
+        Args:
+            search_dict (dict): search_dict is a dictionary describing keys:values to search for
+            in the entries
+            first (bool, optional): only return the first result that found
+            nested_search (bool, optional): if its true if will search for keys and values
+            based on search_dict in nested data structures (like another dictionary in the
+            parent main dict entry)
+        
+        Returns:
+            typing.Union[dict, list, tuple, None]: The entries that found if
+            first is False otherwise the first entry that found 
+            if get_index is true then it will return a tuple
+            containing two values which being the index of the entry
+            aside the value of it(returns None if nothing found)
+        """
+        if first:
+            # Only search for the first entry
+            for index, entry in enumerate(self.storage):
+                passed_every_search = True
+                for sk, sv in search_dict.items():
+                    if entry.get(sk) != sv:
+                        passed_every_search = False
+                if passed_every_search:
+                    if get_index:
+                        return (entry, index)
+                    else:
+                        return entry
+        else:
+            # Search for all entries
+            founded_entries = []
+            for index, entry in enumerate(self.storage):
+                passed_every_search = True
+                for sk, sv in search_dict.items():
+
+                    if entry.get(sk) != sv:
+                        passed_every_search = False
+                if passed_every_search:
+                    if get_index:
+                        founded_entries.append((entry, index))
+                    else:
+                        founded_entries.append(entry)
+            return founded_entries
+    def update(self, index: int, new_entry: dict[typing.Any, typing.Any]) -> bool:
+        """Update the entry based on the index to new_dict
+        
+        Args:
+            index (int): The index of the entry you want to update
+            new_entry (dict): The new updated entry
+        
+        Returns:
+            bool: Wether the action was successful or not
+        
+        Raises:
+            InvalidType: In case the index parameter is not an integer or new_entry
+            is not a dict
+            JsonStorageInvalidIndex: In case the index is out of range and couldn't be find
+            in the entries
+        """
+        if not isinstance(index, int):
+            raise InvalidType(f"index excepted to be integer not {type(index)}")
+        if not isinstance(new_entry, dict):
+            raise InvalidType(f"new_entry excepted to be dict not {type(new_entry)}")
+        try:
+            self.storage[index] = new_entry
+            return True
+        except IndexError:
+            raise JsonStorageInvalidIndex("Invalid index, couldn't find the index in entries")
+        except:
+            return False
+    def delete(self, index: int) -> bool:
+
+        """Delete an entry based on the index given
+        
+        Args:
+            index (int): The index of the entry you want to delete
+        
+        Returns:
+            bool: Wether the action was successful or not
+        
+        Raises:
+            InvalidType: In case the index parameter is not an integer
+            JsonStorageInvalidIndex: In case the index is out of range and couldn't be find
+            in the entries
+        """
+        if not isinstance(index, int):
+            raise InvalidType(f"index excepted to be integer not {type(index)}")
+        try:
+            del self.storage[index]
+            return True
+        except IndexError:
+            raise JsonStorageInvalidIndex("Invalid index, couldn't find the index in entries")
+        except:
+            return False
+    def save(self) -> bool:
+        """Saves the storage variable into disk
+        
+        Returns:
+            bool: Wether the action was successful or not
+        """
+        try:
+            with open(self.file_path, mode="w", encoding="utf8") as file:
+                json.dump(self.storage, file)
+            return True
+        except:
+            return False
```

### Comparing `fusion-engine-0.1.0/src/fusionengine/files/systems.py` & `fusion-engine-0.1.1/src/fusionengine/files/systems.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from fusionengine.files.enums import RendererFlag
-from fusionengine.files.imports import *
-
-class RendererOptions:
-    def __init__(self) -> None:
-        self.rendererflag = SDL_RENDERER_ACCELERATED
-    def getSurfaceFromWindow(self, window):
-        return window.surface
-    def setRendererFlag(self, flag: RendererFlag) -> None:
-        if flag == RendererFlag.PREVENT_SYNC:
-            self.rendererflag = SDL_RENDERER_PRESENTVSYNC
-        elif flag == RendererFlag.SOFTWARE:
-            self.rendererflag = SDL_RENDERER_SOFTWARE
-        elif flag == RendererFlag.TARGET_TEXTURE:
-            self.rendererflag = SDL_RENDERER_TARGETTEXTURE
-        else:
-            self.rendererflag = SDL_RENDERER_ACCELERATED
-
-class System:
-    def __init__(self):
-        pass
+from fusionengine.files.enums import RendererFlag
+from fusionengine.files.imports import *
+
+class RendererOptions:
+    def __init__(self) -> None:
+        self.rendererflag = SDL_RENDERER_ACCELERATED
+    def getSurfaceFromWindow(self, window):
+        return window.surface
+    def setRendererFlag(self, flag: RendererFlag) -> None:
+        if flag == RendererFlag.PREVENT_SYNC:
+            self.rendererflag = SDL_RENDERER_PRESENTVSYNC
+        elif flag == RendererFlag.SOFTWARE:
+            self.rendererflag = SDL_RENDERER_SOFTWARE
+        elif flag == RendererFlag.TARGET_TEXTURE:
+            self.rendererflag = SDL_RENDERER_TARGETTEXTURE
+        else:
+            self.rendererflag = SDL_RENDERER_ACCELERATED
+
+class System:
+    def __init__(self):
+        pass
```

### Comparing `fusion-engine-0.1.0/src/fusionengine/files/window.py` & `fusion-engine-0.1.1/src/fusionengine/files/window.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import fusionengine.files.systems as sysconfig
-
-from fusionengine.files.imports import *
-
-class _CustomRenderer:
-    def __init__(self, window) -> None:
-        self.window = window
-        self.event = SDL_Event()
-        self.renderer = SDL_CreateRenderer(self.window, -1, sysconfig.RendererOptions().rendererflag)
-
-class Window:
-    def __init__(self) -> None:
-        self.window = None
-        self._running = False
-        self._NOW = SDL_GetPerformanceCounter();
-        self._LAST = 0;
-        self.DELTATIME = 0;   
-    
-    def newWindow(self, title: str, width: int, height: int) -> _CustomRenderer:
-        encoded_title = title.encode('utf-8')
-        self.window = SDL_CreateWindow(encoded_title,
-                                       SDL_WINDOWPOS_CENTERED,
-                                       SDL_WINDOWPOS_CENTERED,
-                                       width, height,
-                                       SDL_WINDOW_SHOWN
-                                       )
-        self._running = True
-        return _CustomRenderer(self.window)
-    
-    def running(self, window) -> bool:
-        self._refresh(window)
-        return self._running
-    
-    def _refresh(self, window) -> None:
-        SDL_UpdateWindowSurface(window.window)
-        SDL_RenderPresent(window.renderer)
-        
-        self._LAST = self._NOW;
-        self._NOW = SDL_GetPerformanceCounter();
-
-        self.DELTATIME = (self._NOW - self._LAST)*1000 / SDL_GetPerformanceFrequency()
-                                  
-        if sdl2.SDL_PollEvent(window.event) != 0:
-            if window.event.type == sdl2.SDL_QUIT:
-                self._running = False
-
-        
+import fusionengine.files.systems as sysconfig
+
+from fusionengine.files.imports import *
+
+class _CustomRenderer:
+    def __init__(self, window: SDL_CreateWindow) -> None:
+        self.window = window
+        self.event = SDL_Event()
+        self.renderer = SDL_CreateRenderer(self.window, -1, sysconfig.RendererOptions().rendererflag)
+
+class Window:
+    def __init__(self) -> None:
+        self.window = None
+        self._running = False
+        self._NOW = SDL_GetPerformanceCounter();
+        self._LAST = 0;
+        self.DELTATIME = 0;   
+    
+    def newWindow(self, title: str, width: int, height: int) -> _CustomRenderer:
+        encoded_title = title.encode('utf-8')
+        self.window = SDL_CreateWindow(encoded_title,
+                                       SDL_WINDOWPOS_CENTERED,
+                                       SDL_WINDOWPOS_CENTERED,
+                                       width, height,
+                                       SDL_WINDOW_SHOWN
+                                       )
+        self._running = True
+        return _CustomRenderer(self.window)
+    
+    def running(self, window:_CustomRenderer) -> bool:
+        self._refresh(window)
+        return self._running
+    
+    def _refresh(self, window: _CustomRenderer) -> None:
+        SDL_UpdateWindowSurface(window.window)
+        SDL_RenderPresent(window.renderer)
+        
+        self._LAST = self._NOW;
+        self._NOW = SDL_GetPerformanceCounter();
+
+        self.DELTATIME = (self._NOW - self._LAST)*1000 / SDL_GetPerformanceFrequency()
+                                  
+        if sdl2.SDL_PollEvent(window.event) != 0:
+            if window.event.type == sdl2.SDL_QUIT:
+                self._running = False
+
+
```

