# Comparing `tmp/desktop-notifier-3.5.3.tar.gz` & `tmp/desktop-notifier-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop-notifier-3.5.3.tar", last modified: Fri May 12 08:35:11 2023, max compression
+gzip compressed data, was "desktop-notifier-3.5.4.tar", last modified: Mon Jul  3 18:47:52 2023, max compression
```

## Comparing `desktop-notifier-3.5.3.tar` & `desktop-notifier-3.5.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/src/desktop_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/dbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/macos_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/macos_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/src/desktop_notifier/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/resources/python.png
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/winrt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-12 08:35:11.000000 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-12 08:35:11.000000 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:35:11.000000 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-12 08:35:11.000000 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-12 08:35:11.000000 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:47:52.294218 desktop-notifier-3.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/src/desktop_notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/macos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/macos_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/macos_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/src/desktop_notifier/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/resources/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-03 18:47:39.000000 desktop-notifier-3.5.4/src/desktop_notifier/winrt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:47:52.298218 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-03 18:47:52.000000 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-03 18:47:52.000000 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:47:52.000000 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-03 18:47:52.000000 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 18:47:52.000000 desktop-notifier-3.5.4/src/desktop_notifier.egg-info/top_level.txt
```

### Comparing `desktop-notifier-3.5.3/LICENSE` & `desktop-notifier-3.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.3/PKG-INFO` & `desktop-notifier-3.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.3
+Version: 3.5.4
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -37,50 +37,52 @@
 * [**exprimental**] Windows via the WinRT / Python bridge.
 
 ![gif](screenshots/macOS.gif)
 
 ## Features
 
 `desktop-notifier` aims to be a good citizen of the platforms which it supports. It
-therefore stays within the limits of the native platform APIs and does not try to
-work around limitations which are often deliberate UI choices. For example, on macOS
-and iOS, it is not possible to change the app icon which is shown on notifications.
-There are possible workarounds - that would likely be rejected by an App Store review.
+therefore stays within the limits of the native platform APIs and does not try to work
+around limitations which are often deliberate UI choices. For example, on macOS  and
+iOS, it is not possible to change the app icon which is shown on notifications. There 
+are possible workarounds - that would likely be rejected by an App Store review - and
+desktop-notifier deliberately stays away from those.
 
 Where supported by the native platform APIs, `desktop-notifier` allows for:
 
 * Clickable notifications with callbacks on user interaction
 * Multiple action buttons
 * A single reply field (e.g., for chat notifications)
 * Notification sounds
 * Notification threads (grouping notifications by topic)
-* Limiting maximum number of notifications shown in the notification center
+* Limiting the maximum number of notifications shown in the notification center
 
 An exhaustive list of features and their platform support is provided in the
 [documentation](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html).
 
 Design choices by `desktop-notifier`:
 
-* Asyncio API: The main API consists of async methods and a running event loop
+* Async API: The main API consists of async methods and a running event loop
   is required to respond to user interactions with a notification.
-* Pure Python dependencies only, no extension modules (with the exception of
-  of the Windows backend).
+* Prefer pure Python dependencies over extension modules. We make an exception for
+  Windows because interoperability with the Windows Runtime is difficult to achieve
+  otherwise.
 
 ## Installation
 
 From PyPI:
 
 ```
 pip3 install -U desktop-notifier
 ```
 
 ## Usage
 
 The main API consists of asynchronous methods which need to be awaited. Basic usage only
-requires the user to specify a notification title and message. For instance:
+requires the user to specify a notification title and message. For example:
 
 ```Python
 import asyncio
 from desktop_notifier import DesktopNotifier
 
 notifier = DesktopNotifier()
 
@@ -91,16 +93,16 @@
 
     await notifier.clear(n)  # removes the notification
     await notifier.clear_all()  # removes all notifications for this app
 
 asyncio.run(main())
 ```
 
-For convenience, the is also a synchronous method ``send_sync()`` to send notifications
-which does not require a running asyncio loop:
+For convenience, there is also a synchronous method ``send_sync()`` to send 
+notifications without manually starting an asyncio event loop:
 
 ```Python
 notifier.send_sync(title="Hello world!", message="Sent from Python")
 ```
 
 By default, "Python" will be used as the app name for all notifications, but you can
 manually specify an app name and icon in the ``DesktopNotifier`` constructor. Advanced
@@ -137,24 +139,23 @@
 
 loop = asyncio.get_event_loop()
 loop.create_task(main())
 loop.run_forever()
 ```
 
 Note that some platforms may not support all options. For instance, some Linux desktop
-environments may not support notifications with buttons. macOS does not support
-manually setting the app icon or name. Instead, both are always determined by the
-application which uses the Library. This can be Python itself, when used interactively,
-or a frozen app bundle when packaged with PyInstaller or similar solutions. Please refer
-to the [Platform Support](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html)
+environments may not support notifications with buttons. macOS does not support manually
+setting the app icon or name. Instead, both are always determined by the application
+which uses the Library. This can be Python itself, or a frozen app bundle when packaged
+with PyInstaller or similar solutions. Please refer to the
+[Platform Support](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html)
 chapter of the documentation for more information on limitations for certain platforms.
 
 Any options or configurations which are not supported by the platform will be silently
-ignored. Please refer to the documentation on [Read the Docs](https://desktop-notifier.readthedocs.io)
-for more information on platform support.
+ignored.
 
 ## Event loop integration
 
 Using the asynchronous API is highly recommended to prevent multiple milliseconds of
 blocking IO from DBus or Cocoa APIs. In addition, execution of callbacks requires a
 running event loop. On Linux, an asyncio event loop will be sufficient but macOS
 requires a running [CFRunLoop](https://developer.apple.com/documentation/corefoundation/cfrunloop-rht).
@@ -170,17 +171,17 @@
 asyncio.set_event_loop_policy(EventLoopPolicy())
 
 # Get an event loop, and run it!
 loop = asyncio.get_event_loop()
 loop.run_forever()
 ```
 
-Desktop-notifier itself uses Rubicon Objective-C to interface with Cocoa APIs so you
-will not be adding a new dependency. A full example integrating with the CFRunLoop is
-given in [examples/eventloop.py](examples/eventloop.py). Please refer to the
+Desktop-notifier itself uses Rubicon Objective-C to interface with Cocoa APIs. A full
+example integrating with the CFRunLoop is given in
+[examples/eventloop.py](examples/eventloop.py). Please refer to the
 [Rubicon Objective-C docs](https://rubicon-objc.readthedocs.io/en/latest/how-to/async.html)
 for more information.
 
 Likewise, you can integrate the asyncio event loop with a Gtk main loop on Gnome using
 [gbulb](https://pypi.org/project/gbulb). This is not required for full functionality
 but may be convenient when developing a Gtk app.
 
@@ -188,15 +189,15 @@
 
 On macOS 10.14 and higher, the implementation uses the `UNUserNotificationCenter`
 instead of the deprecated `NSUserNotificationCenter`. `UNUserNotificationCenter`
 only allows signed executables to send desktop notifications. This means that
 notifications will only work if the Python executable or bundled app has been signed.
 Note that the installer from [python.org](https://python.org) provides a properly signed
 Python framework but **homebrew does not** (manually signing the executable installed
-by homebrew _should_ work as well).
+by homebrew *should* work as well).
 
 If you freeze your code with PyInstaller or a similar packaging solution, you must sign 
 the resulting app bundle for notifications to work. An ad-hoc signature will be
 sufficient but signing with an Apple developer certificate is recommended for
 distribution and may be required on future releases of macOS.
 
 ## Requirements
@@ -204,7 +205,8 @@
 * macOS 10.13 or higher
 * Linux desktop environment providing a dbus desktop notifications service
 
 ## Dependencies
 
 * [dbus-next](https://github.com/altdesktop/python-dbus-next) on Linux
 * [rubicon-objc](https://github.com/beeware/rubicon-objc) on macOS
+* [winsdk](https://github.com/pywinrt/python-winsdk) on Windows
```

### Comparing `desktop-notifier-3.5.3/README.md` & `desktop-notifier-3.5.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,50 +12,52 @@
 * [**exprimental**] Windows via the WinRT / Python bridge.
 
 ![gif](screenshots/macOS.gif)
 
 ## Features
 
 `desktop-notifier` aims to be a good citizen of the platforms which it supports. It
-therefore stays within the limits of the native platform APIs and does not try to
-work around limitations which are often deliberate UI choices. For example, on macOS
-and iOS, it is not possible to change the app icon which is shown on notifications.
-There are possible workarounds - that would likely be rejected by an App Store review.
+therefore stays within the limits of the native platform APIs and does not try to work
+around limitations which are often deliberate UI choices. For example, on macOS  and
+iOS, it is not possible to change the app icon which is shown on notifications. There 
+are possible workarounds - that would likely be rejected by an App Store review - and
+desktop-notifier deliberately stays away from those.
 
 Where supported by the native platform APIs, `desktop-notifier` allows for:
 
 * Clickable notifications with callbacks on user interaction
 * Multiple action buttons
 * A single reply field (e.g., for chat notifications)
 * Notification sounds
 * Notification threads (grouping notifications by topic)
-* Limiting maximum number of notifications shown in the notification center
+* Limiting the maximum number of notifications shown in the notification center
 
 An exhaustive list of features and their platform support is provided in the
 [documentation](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html).
 
 Design choices by `desktop-notifier`:
 
-* Asyncio API: The main API consists of async methods and a running event loop
+* Async API: The main API consists of async methods and a running event loop
   is required to respond to user interactions with a notification.
-* Pure Python dependencies only, no extension modules (with the exception of
-  of the Windows backend).
+* Prefer pure Python dependencies over extension modules. We make an exception for
+  Windows because interoperability with the Windows Runtime is difficult to achieve
+  otherwise.
 
 ## Installation
 
 From PyPI:
 
 ```
 pip3 install -U desktop-notifier
 ```
 
 ## Usage
 
 The main API consists of asynchronous methods which need to be awaited. Basic usage only
-requires the user to specify a notification title and message. For instance:
+requires the user to specify a notification title and message. For example:
 
 ```Python
 import asyncio
 from desktop_notifier import DesktopNotifier
 
 notifier = DesktopNotifier()
 
@@ -66,16 +68,16 @@
 
     await notifier.clear(n)  # removes the notification
     await notifier.clear_all()  # removes all notifications for this app
 
 asyncio.run(main())
 ```
 
-For convenience, the is also a synchronous method ``send_sync()`` to send notifications
-which does not require a running asyncio loop:
+For convenience, there is also a synchronous method ``send_sync()`` to send 
+notifications without manually starting an asyncio event loop:
 
 ```Python
 notifier.send_sync(title="Hello world!", message="Sent from Python")
 ```
 
 By default, "Python" will be used as the app name for all notifications, but you can
 manually specify an app name and icon in the ``DesktopNotifier`` constructor. Advanced
@@ -112,24 +114,23 @@
 
 loop = asyncio.get_event_loop()
 loop.create_task(main())
 loop.run_forever()
 ```
 
 Note that some platforms may not support all options. For instance, some Linux desktop
-environments may not support notifications with buttons. macOS does not support
-manually setting the app icon or name. Instead, both are always determined by the
-application which uses the Library. This can be Python itself, when used interactively,
-or a frozen app bundle when packaged with PyInstaller or similar solutions. Please refer
-to the [Platform Support](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html)
+environments may not support notifications with buttons. macOS does not support manually
+setting the app icon or name. Instead, both are always determined by the application
+which uses the Library. This can be Python itself, or a frozen app bundle when packaged
+with PyInstaller or similar solutions. Please refer to the
+[Platform Support](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html)
 chapter of the documentation for more information on limitations for certain platforms.
 
 Any options or configurations which are not supported by the platform will be silently
-ignored. Please refer to the documentation on [Read the Docs](https://desktop-notifier.readthedocs.io)
-for more information on platform support.
+ignored.
 
 ## Event loop integration
 
 Using the asynchronous API is highly recommended to prevent multiple milliseconds of
 blocking IO from DBus or Cocoa APIs. In addition, execution of callbacks requires a
 running event loop. On Linux, an asyncio event loop will be sufficient but macOS
 requires a running [CFRunLoop](https://developer.apple.com/documentation/corefoundation/cfrunloop-rht).
@@ -145,17 +146,17 @@
 asyncio.set_event_loop_policy(EventLoopPolicy())
 
 # Get an event loop, and run it!
 loop = asyncio.get_event_loop()
 loop.run_forever()
 ```
 
-Desktop-notifier itself uses Rubicon Objective-C to interface with Cocoa APIs so you
-will not be adding a new dependency. A full example integrating with the CFRunLoop is
-given in [examples/eventloop.py](examples/eventloop.py). Please refer to the
+Desktop-notifier itself uses Rubicon Objective-C to interface with Cocoa APIs. A full
+example integrating with the CFRunLoop is given in
+[examples/eventloop.py](examples/eventloop.py). Please refer to the
 [Rubicon Objective-C docs](https://rubicon-objc.readthedocs.io/en/latest/how-to/async.html)
 for more information.
 
 Likewise, you can integrate the asyncio event loop with a Gtk main loop on Gnome using
 [gbulb](https://pypi.org/project/gbulb). This is not required for full functionality
 but may be convenient when developing a Gtk app.
 
@@ -163,15 +164,15 @@
 
 On macOS 10.14 and higher, the implementation uses the `UNUserNotificationCenter`
 instead of the deprecated `NSUserNotificationCenter`. `UNUserNotificationCenter`
 only allows signed executables to send desktop notifications. This means that
 notifications will only work if the Python executable or bundled app has been signed.
 Note that the installer from [python.org](https://python.org) provides a properly signed
 Python framework but **homebrew does not** (manually signing the executable installed
-by homebrew _should_ work as well).
+by homebrew *should* work as well).
 
 If you freeze your code with PyInstaller or a similar packaging solution, you must sign 
 the resulting app bundle for notifications to work. An ad-hoc signature will be
 sufficient but signing with an Apple developer certificate is recommended for
 distribution and may be required on future releases of macOS.
 
 ## Requirements
@@ -179,7 +180,8 @@
 * macOS 10.13 or higher
 * Linux desktop environment providing a dbus desktop notifications service
 
 ## Dependencies
 
 * [dbus-next](https://github.com/altdesktop/python-dbus-next) on Linux
 * [rubicon-objc](https://github.com/beeware/rubicon-objc) on macOS
+* [winsdk](https://github.com/pywinrt/python-winsdk) on Windows
```

### Comparing `desktop-notifier-3.5.3/pyproject.toml` & `desktop-notifier-3.5.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "desktop-notifier"
-version = "3.5.3"
+version = "3.5.4"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Python library for cross-platform desktop notifications"
 keywords = ["desktop-notifier"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
@@ -20,17 +20,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 requires-python = ">=3.7"
 dependencies = [
-    "dbus-next;sys_platform=='linux'",
-    "importlib_resources;python_version<'3.9'",
     "packaging",
+    "importlib_resources",
+    "dbus-next;sys_platform=='linux'",
     "rubicon-objc;sys_platform=='darwin'",
     "winsdk==1.0.0b9;sys_platform=='win32'",
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
@@ -46,18 +46,18 @@
     "flake8-pyproject",
     "mypy",
     "pre-commit",
     "pytest",
     "pytest-cov",
 ]
 docs = [
-    "sphinx",
-    "sphinx-autoapi",
-    "sphinx-mdinclude",
-    "sphinx_rtd_theme",
+    "furo==2023.5.20",
+    "sphinx==7.0.1",
+    "sphinx-autoapi==2.1.1",
+    "sphinx-mdinclude==0.5.3",
 ]
 
 [tool.setuptools.package-data]
 desktop_notifier = ["**/*.png"]
 
 [tool.flake8]
 ignore = "E203,E501,W503,H306"
@@ -68,8 +68,8 @@
 [tool.mypy]
 ignore_missing_imports = true
 strict = true
 files = ["src"]
 
 [tool.black]
 line-length = 88
-target-version = ["py37", "py38", "py39", "py310"]
+target-version = ["py37", "py38", "py39", "py310", "py311"]
```

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier/base.py` & `desktop-notifier-3.5.4/src/desktop_notifier/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,35 +4,26 @@
 must inherit from :class:`DesktopNotifierBase`.
 """
 
 from __future__ import annotations
 
 # system imports
 import logging
-import pathlib
 from enum import Enum
 from collections import deque
 from typing import (
     Dict,
     Callable,
     Any,
     Deque,
     List,
     Sequence,
-    ContextManager,
 )
 
-try:
-    from importlib.resources import as_file, files
-
-    def resource_path(package: str, resource: str) -> ContextManager[pathlib.Path]:
-        return as_file(files(package) / resource)
-
-except ImportError:
-    from importlib.resources import path as resource_path
+from importlib_resources import path as resource_path
 
 
 logger = logging.getLogger(__name__)
 
 PYTHON_ICON_PATH = resource_path("desktop_notifier.resources", "python.png").__enter__()
```

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier/dbus.py` & `desktop-notifier-3.5.4/src/desktop_notifier/dbus.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,16 +113,25 @@
             self.interface = await self._init_dbus()
 
         if notification_to_replace:
             replaces_nid = notification_to_replace.identifier
         else:
             replaces_nid = 0
 
-        # Create list of actions with default and user-supplied.
-        actions = ["default", "default"]
+        # Create list of actions for a user interacting with the notification.
+        actions = []
+
+        if notification.on_clicked:
+            # The "default" action is typically invoked when clicking on the
+            # notification body itself, see
+            # https://specifications.freedesktop.org/notification-spec. There are some
+            # exceptions though, such as XFCE, where this will result in a separate
+            # button. If no label name is provided in XFCE, it will result in a default
+            # symbol being used. We therefore don't specify a label name.
+            actions = ["default", ""]
 
         for n, button in enumerate(notification.buttons):
             actions += [str(n), button.title]
 
         hints = {"urgency": self._to_native_urgency[notification.urgency]}
 
         # sound
```

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier/dummy.py` & `desktop-notifier-3.5.4/src/desktop_notifier/dummy.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier/macos.py` & `desktop-notifier-3.5.4/src/desktop_notifier/macos.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier/macos_legacy.py` & `desktop-notifier-3.5.4/src/desktop_notifier/macos_legacy.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier/macos_support.py` & `desktop-notifier-3.5.4/src/desktop_notifier/macos_support.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier/main.py` & `desktop-notifier-3.5.4/src/desktop_notifier/main.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier/resources/python.png` & `desktop-notifier-3.5.4/src/desktop_notifier/resources/python.png`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier/winrt.py` & `desktop-notifier-3.5.4/src/desktop_notifier/winrt.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier.egg-info/PKG-INFO` & `desktop-notifier-3.5.4/src/desktop_notifier.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.3
+Version: 3.5.4
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -37,50 +37,52 @@
 * [**exprimental**] Windows via the WinRT / Python bridge.
 
 ![gif](screenshots/macOS.gif)
 
 ## Features
 
 `desktop-notifier` aims to be a good citizen of the platforms which it supports. It
-therefore stays within the limits of the native platform APIs and does not try to
-work around limitations which are often deliberate UI choices. For example, on macOS
-and iOS, it is not possible to change the app icon which is shown on notifications.
-There are possible workarounds - that would likely be rejected by an App Store review.
+therefore stays within the limits of the native platform APIs and does not try to work
+around limitations which are often deliberate UI choices. For example, on macOS  and
+iOS, it is not possible to change the app icon which is shown on notifications. There 
+are possible workarounds - that would likely be rejected by an App Store review - and
+desktop-notifier deliberately stays away from those.
 
 Where supported by the native platform APIs, `desktop-notifier` allows for:
 
 * Clickable notifications with callbacks on user interaction
 * Multiple action buttons
 * A single reply field (e.g., for chat notifications)
 * Notification sounds
 * Notification threads (grouping notifications by topic)
-* Limiting maximum number of notifications shown in the notification center
+* Limiting the maximum number of notifications shown in the notification center
 
 An exhaustive list of features and their platform support is provided in the
 [documentation](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html).
 
 Design choices by `desktop-notifier`:
 
-* Asyncio API: The main API consists of async methods and a running event loop
+* Async API: The main API consists of async methods and a running event loop
   is required to respond to user interactions with a notification.
-* Pure Python dependencies only, no extension modules (with the exception of
-  of the Windows backend).
+* Prefer pure Python dependencies over extension modules. We make an exception for
+  Windows because interoperability with the Windows Runtime is difficult to achieve
+  otherwise.
 
 ## Installation
 
 From PyPI:
 
 ```
 pip3 install -U desktop-notifier
 ```
 
 ## Usage
 
 The main API consists of asynchronous methods which need to be awaited. Basic usage only
-requires the user to specify a notification title and message. For instance:
+requires the user to specify a notification title and message. For example:
 
 ```Python
 import asyncio
 from desktop_notifier import DesktopNotifier
 
 notifier = DesktopNotifier()
 
@@ -91,16 +93,16 @@
 
     await notifier.clear(n)  # removes the notification
     await notifier.clear_all()  # removes all notifications for this app
 
 asyncio.run(main())
 ```
 
-For convenience, the is also a synchronous method ``send_sync()`` to send notifications
-which does not require a running asyncio loop:
+For convenience, there is also a synchronous method ``send_sync()`` to send 
+notifications without manually starting an asyncio event loop:
 
 ```Python
 notifier.send_sync(title="Hello world!", message="Sent from Python")
 ```
 
 By default, "Python" will be used as the app name for all notifications, but you can
 manually specify an app name and icon in the ``DesktopNotifier`` constructor. Advanced
@@ -137,24 +139,23 @@
 
 loop = asyncio.get_event_loop()
 loop.create_task(main())
 loop.run_forever()
 ```
 
 Note that some platforms may not support all options. For instance, some Linux desktop
-environments may not support notifications with buttons. macOS does not support
-manually setting the app icon or name. Instead, both are always determined by the
-application which uses the Library. This can be Python itself, when used interactively,
-or a frozen app bundle when packaged with PyInstaller or similar solutions. Please refer
-to the [Platform Support](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html)
+environments may not support notifications with buttons. macOS does not support manually
+setting the app icon or name. Instead, both are always determined by the application
+which uses the Library. This can be Python itself, or a frozen app bundle when packaged
+with PyInstaller or similar solutions. Please refer to the
+[Platform Support](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html)
 chapter of the documentation for more information on limitations for certain platforms.
 
 Any options or configurations which are not supported by the platform will be silently
-ignored. Please refer to the documentation on [Read the Docs](https://desktop-notifier.readthedocs.io)
-for more information on platform support.
+ignored.
 
 ## Event loop integration
 
 Using the asynchronous API is highly recommended to prevent multiple milliseconds of
 blocking IO from DBus or Cocoa APIs. In addition, execution of callbacks requires a
 running event loop. On Linux, an asyncio event loop will be sufficient but macOS
 requires a running [CFRunLoop](https://developer.apple.com/documentation/corefoundation/cfrunloop-rht).
@@ -170,17 +171,17 @@
 asyncio.set_event_loop_policy(EventLoopPolicy())
 
 # Get an event loop, and run it!
 loop = asyncio.get_event_loop()
 loop.run_forever()
 ```
 
-Desktop-notifier itself uses Rubicon Objective-C to interface with Cocoa APIs so you
-will not be adding a new dependency. A full example integrating with the CFRunLoop is
-given in [examples/eventloop.py](examples/eventloop.py). Please refer to the
+Desktop-notifier itself uses Rubicon Objective-C to interface with Cocoa APIs. A full
+example integrating with the CFRunLoop is given in
+[examples/eventloop.py](examples/eventloop.py). Please refer to the
 [Rubicon Objective-C docs](https://rubicon-objc.readthedocs.io/en/latest/how-to/async.html)
 for more information.
 
 Likewise, you can integrate the asyncio event loop with a Gtk main loop on Gnome using
 [gbulb](https://pypi.org/project/gbulb). This is not required for full functionality
 but may be convenient when developing a Gtk app.
 
@@ -188,15 +189,15 @@
 
 On macOS 10.14 and higher, the implementation uses the `UNUserNotificationCenter`
 instead of the deprecated `NSUserNotificationCenter`. `UNUserNotificationCenter`
 only allows signed executables to send desktop notifications. This means that
 notifications will only work if the Python executable or bundled app has been signed.
 Note that the installer from [python.org](https://python.org) provides a properly signed
 Python framework but **homebrew does not** (manually signing the executable installed
-by homebrew _should_ work as well).
+by homebrew *should* work as well).
 
 If you freeze your code with PyInstaller or a similar packaging solution, you must sign 
 the resulting app bundle for notifications to work. An ad-hoc signature will be
 sufficient but signing with an Apple developer certificate is recommended for
 distribution and may be required on future releases of macOS.
 
 ## Requirements
@@ -204,7 +205,8 @@
 * macOS 10.13 or higher
 * Linux desktop environment providing a dbus desktop notifications service
 
 ## Dependencies
 
 * [dbus-next](https://github.com/altdesktop/python-dbus-next) on Linux
 * [rubicon-objc](https://github.com/beeware/rubicon-objc) on macOS
+* [winsdk](https://github.com/pywinrt/python-winsdk) on Windows
```

### Comparing `desktop-notifier-3.5.3/src/desktop_notifier.egg-info/SOURCES.txt` & `desktop-notifier-3.5.4/src/desktop_notifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

