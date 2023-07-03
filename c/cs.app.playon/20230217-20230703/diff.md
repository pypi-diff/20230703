# Comparing `tmp/cs.app.playon-20230217.tar.gz` & `tmp/cs.app.playon-20230703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.app.playon-20230217.tar", last modified: Fri Feb 17 00:55:00 2023, max compression
+gzip compressed data, was "cs.app.playon-20230703.tar", last modified: Mon Jul  3 10:17:17 2023, max compression
```

## Comparing `cs.app.playon-20230217.tar` & `cs.app.playon-20230703.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:55:00.963257 cs.app.playon-20230217/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-02-17 00:54:48.000000 cs.app.playon-20230217/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     6025 2023-02-17 00:55:00.963365 cs.app.playon-20230217/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    11852 2023-02-17 00:54:49.000000 cs.app.playon-20230217/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:55:00.959076 cs.app.playon-20230217/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:55:00.959377 cs.app.playon-20230217/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:55:00.959491 cs.app.playon-20230217/lib/python/cs/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:55:00.962982 cs.app.playon-20230217/lib/python/cs/app/
--rw-r--r--   0 cameron    (501) cameron    (502)    31674 2023-02-17 00:54:37.000000 cs.app.playon-20230217/lib/python/cs/app/playon.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:55:00.962699 cs.app.playon-20230217/lib/python/cs.app.playon.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     6025 2023-02-17 00:55:00.000000 cs.app.playon-20230217/lib/python/cs.app.playon.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      373 2023-02-17 00:55:00.000000 cs.app.playon-20230217/lib/python/cs.app.playon.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-02-17 00:55:00.000000 cs.app.playon-20230217/lib/python/cs.app.playon.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       46 2023-02-17 00:55:00.000000 cs.app.playon-20230217/lib/python/cs.app.playon.egg-info/entry_points.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      337 2023-02-17 00:55:00.000000 cs.app.playon-20230217/lib/python/cs.app.playon.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-02-17 00:55:00.000000 cs.app.playon-20230217/lib/python/cs.app.playon.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     6632 2023-02-17 00:54:53.000000 cs.app.playon-20230217/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1273 2023-02-17 00:55:00.964012 cs.app.playon-20230217/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-02-17 00:54:49.000000 cs.app.playon-20230217/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.080803 cs.app.playon-20230703/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-07-03 10:17:01.000000 cs.app.playon-20230703/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6847 2023-07-03 10:17:17.080931 cs.app.playon-20230703/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    13326 2023-07-03 10:17:03.000000 cs.app.playon-20230703/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.075575 cs.app.playon-20230703/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.075927 cs.app.playon-20230703/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.076059 cs.app.playon-20230703/lib/python/cs/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.080431 cs.app.playon-20230703/lib/python/cs/app/
+-rw-r--r--   0 cameron    (501) cameron    (502)    32942 2023-07-03 10:16:46.000000 cs.app.playon-20230703/lib/python/cs/app/playon.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.080067 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6847 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      373 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       46 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      327 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     7444 2023-07-03 10:17:07.000000 cs.app.playon-20230703/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1263 2023-07-03 10:17:17.081639 cs.app.playon-20230703/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-07-03 10:17:03.000000 cs.app.playon-20230703/setup.py
```

### Comparing `cs.app.playon-20230217/PKG-INFO` & `cs.app.playon-20230703/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.app.playon
-Version: 20230217
+Version: 20230703
 Summary: PlayOn facilities, primarily access to the download API. Includes a nice command line tool.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -17,20 +17,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 PlayOn facilities, primarily access to the download API.
 Includes a nice command line tool.
 
-*Latest release 20230217*:
-* Move some core stuff off into cs.service_api.HTTPServiceAPI.
-* Move core Recording.is_stale() method to TagSet.is_stale(), leave override method behind.
-* Persist login tokens in a db for reuse while still fresh.
-* "playon dl": allow interrupting downloads.
-* Cleaner handling of playon.Name having a leading SNNeNN prefix.
+*Latest release 20230703*:
+* PlayOnAPI: features, feature, featured_image_url, service_image_url.
+* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
+* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
+* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
+* PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
 
 ## Function `main(argv=None)`
 
 Playon command line mode;
 see the `PlayOnCommand` class below.
 
 ## Class `PlayOnAPI(cs.service_api.HTTPServiceAPI, cs.service_api.ServiceAPI, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -74,14 +74,18 @@
             content
             content/provider-name
         dl [-j jobs] [-n] [recordings...]
           Download the specified recordings, default "pending".
           -j jobs   Run this many downloads in parallel.
                     The default is 2.
           -n        No download. List the specified recordings.
+        downloaded recordings...
+          Mark the specified recordings as downloaded and no longer pending.
+        feature [feature_id]
+          List features.
         help [-l] [subcommand-names...]
           Print the full help for the named subcommands,
           or for all subcommands if no names are specified.
           -l  Long help even if no subcommand-names provided.
         ls [-l] [recordings...]
           List available downloads.
           -l        Long listing: list tags below each entry.
@@ -98,27 +102,36 @@
           -l        Long listing: list tags below each entry.
           -o format Format string for each entry.
           Default format: {playon.ID} {playon.Series} {playon.Name} {playon.ProviderID}
         refresh [queue] [recordings]
           Update the db state from the PlayOn service.
         service [service_id]
           List services.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
 ## Class `PlayOnSQLTags(cs.sqltags.SQLTags, cs.tagset.BaseTagSets, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, collections.abc.MutableMapping, collections.abc.Mapping, collections.abc.Collection, collections.abc.Sized, collections.abc.Iterable, collections.abc.Container, cs.deco.Promotable)`
 
 `SQLTags` subclass with PlayOn related methods.
 
 ## Class `Recording(cs.sqltags.SQLTagSet, cs.obj.SingletonMixin, cs.tagset.TagSet, builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter, cs.mappings.AttrableMappingMixin)`
 
 An `SQLTagSet` with knowledge about PlayOn recordings.
 
 # Release Log
 
 
 
+*Release 20230703*:
+* PlayOnAPI: features, feature, featured_image_url, service_image_url.
+* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
+* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
+* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
+* PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
+
 *Release 20230217*:
 * Move some core stuff off into cs.service_api.HTTPServiceAPI.
 * Move core Recording.is_stale() method to TagSet.is_stale(), leave override method behind.
 * Persist login tokens in a db for reuse while still fresh.
 * "playon dl": allow interrupting downloads.
 * Cleaner handling of playon.Name having a leading SNNeNN prefix.
```

### Comparing `cs.app.playon-20230217/README.md` & `cs.app.playon-20230703/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 PlayOn facilities, primarily access to the download API.
 Includes a nice command line tool.
 
-*Latest release 20230217*:
-* Move some core stuff off into cs.service_api.HTTPServiceAPI.
-* Move core Recording.is_stale() method to TagSet.is_stale(), leave override method behind.
-* Persist login tokens in a db for reuse while still fresh.
-* "playon dl": allow interrupting downloads.
-* Cleaner handling of playon.Name having a leading SNNeNN prefix.
+*Latest release 20230703*:
+* PlayOnAPI: features, feature, featured_image_url, service_image_url.
+* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
+* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
+* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
+* PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
 
 ## Function `main(argv=None)`
 
 Playon command line mode;
 see the `PlayOnCommand` class below.
 
 ## Class `PlayOnAPI(cs.service_api.HTTPServiceAPI, cs.service_api.ServiceAPI, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -54,14 +54,23 @@
 
 The default `filename` is the basename of the filename
 from the download.
 If the filename is supplied with a trailing dot (`'.'`)
 then the file extension will be taken from the filename
 of the download URL.
 
+*Method `PlayOnAPI.feature(self, feature_id)`*:
+Return the feature `SQLTags` instance for `feature_id`.
+
+*Method `PlayOnAPI.featured_image_url(self, feature_name: str)`*:
+URL of the image for a featured show.
+
+*Method `PlayOnAPI.features(self)`*:
+Fetch the list of featured shows.
+
 *Method `PlayOnAPI.from_playon_date(date_s)`*:
 The PlayOn API seems to use UTC date strings.
 
 *Property `PlayOnAPI.jwt`*:
 The JWT token.
 
 *Method `PlayOnAPI.login(self)`*:
@@ -79,21 +88,21 @@
 
 *Method `PlayOnAPI.recordings(self)`*:
 Return the `TagSet` instances for the available recordings.
 
 *Method `PlayOnAPI.renew_jwt(self)`*:
 UNUSED
 
-*Method `PlayOnAPI.service(self, service_id)`*:
+*Method `PlayOnAPI.service(self, service_id: str)`*:
 Return the service `SQLTags` instance for `service_id`.
 
 *Method `PlayOnAPI.services(self)`*:
 Fetch the list of services.
 
-*Method `PlayOnAPI.suburl(self, suburl, headers=None, **kw)`*:
+*Method `PlayOnAPI.suburl(self, suburl, *, api_version=None, headers=None, _base_url=None, **kw)`*:
 Override `HTTPServiceAPI.suburl` with default
 `headers={'Authorization':self.jwt}`.
 
 *Method `PlayOnAPI.suburl_data(self, suburl, *, raw=False, **kw)`*:
 Call `suburl` and return the `'data'` component on success.
 
 Parameters:
@@ -140,14 +149,18 @@
             content
             content/provider-name
         dl [-j jobs] [-n] [recordings...]
           Download the specified recordings, default "pending".
           -j jobs   Run this many downloads in parallel.
                     The default is 2.
           -n        No download. List the specified recordings.
+        downloaded recordings...
+          Mark the specified recordings as downloaded and no longer pending.
+        feature [feature_id]
+          List features.
         help [-l] [subcommand-names...]
           Print the full help for the named subcommands,
           or for all subcommands if no names are specified.
           -l  Long help even if no subcommand-names provided.
         ls [-l] [recordings...]
           List available downloads.
           -l        Long listing: list tags below each entry.
@@ -164,14 +177,18 @@
           -l        Long listing: list tags below each entry.
           -o format Format string for each entry.
           Default format: {playon.ID} {playon.Series} {playon.Name} {playon.ProviderID}
         refresh [queue] [recordings]
           Update the db state from the PlayOn service.
         service [service_id]
           List services.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
+
+*`PlayOnCommand.Options`*
 
 *Method `PlayOnCommand.cmd_account(self, argv)`*:
 Usage: {cmd}
 Report account state.
 
 *Method `PlayOnCommand.cmd_api(self, argv)`*:
 Usage: {cmd} suburl
@@ -187,14 +204,22 @@
 *Method `PlayOnCommand.cmd_dl(self, argv)`*:
 Usage: {cmd} [-j jobs] [-n] [recordings...]
 Download the specified recordings, default "pending".
 -j jobs   Run this many downloads in parallel.
           The default is {DEFAULT_DL_PARALLELISM}.
 -n        No download. List the specified recordings.
 
+*Method `PlayOnCommand.cmd_downloaded(self, argv, locale='en_US')`*:
+Usage: {cmd} recordings...
+Mark the specified recordings as downloaded and no longer pending.
+
+*Method `PlayOnCommand.cmd_feature(self, argv, locale='en_US')`*:
+Usage: {cmd} [feature_id]
+List features.
+
 *Method `PlayOnCommand.cmd_ls(self, argv)`*:
 Usage: {cmd} [-l] [recordings...]
 List available downloads.
 -l        Long listing: list tags below each entry.
 -o format Format string for each entry.
 Default format: {LS_FORMAT}
 
@@ -256,15 +281,16 @@
 An `SQLTagSet` with knowledge about PlayOn recordings.
 
 *Method `Recording.is_available(self)`*:
 Is a recording available for download?
 
 *Method `Recording.is_downloaded(self)`*:
 Test whether this recording has been downloaded
-based on the presence of a `download_path` `Tag`.
+based on the presence of a `download_path` `Tag`
+or a true `downloaded` `Tag`.
 
 *Method `Recording.is_expired(self)`*:
 Test whether this recording is expired,
 which implies that it is no longer available for download.
 
 *Method `Recording.is_pending(self)`*:
 A pending download: available and not already downloaded.
@@ -298,14 +324,21 @@
 *Method `Recording.status(self)`*:
 Return a short status string.
 
 # Release Log
 
 
 
+*Release 20230703*:
+* PlayOnAPI: features, feature, featured_image_url, service_image_url.
+* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
+* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
+* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
+* PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
+
 *Release 20230217*:
 * Move some core stuff off into cs.service_api.HTTPServiceAPI.
 * Move core Recording.is_stale() method to TagSet.is_stale(), leave override method behind.
 * Persist login tokens in a db for reuse while still fresh.
 * "playon dl": allow interrupting downloads.
 * Cleaner handling of playon.Name having a leading SNNeNN prefix.
```

### Comparing `cs.app.playon-20230217/lib/python/cs/app/playon.py` & `cs.app.playon-20230703/lib/python/cs/app/playon.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,53 +4,52 @@
 #
 
 ''' PlayOn facilities, primarily access to the download API.
     Includes a nice command line tool.
 '''
 
 from contextlib import contextmanager
+from dataclasses import dataclass, field
 from datetime import datetime, timezone
-from functools import partial
 from getopt import getopt, GetoptError
-from json import JSONDecodeError
 from netrc import netrc
 import os
 from os import environ
 from os.path import (
     basename, exists as pathexists, expanduser, realpath, splitext
 )
 from pprint import pformat, pprint
 import re
 import sys
 from threading import Semaphore
 import time
-from typing import Set
+from typing import Optional, Set
 from urllib.parse import unquote as unpercent
 
+from icontract import require
 import requests
 from typeguard import typechecked
 
 from cs.cmdutils import BaseCommand
 from cs.context import stackattrs
 from cs.deco import fmtdoc
-from cs.fstags import FSTags
 from cs.fileutils import atomic_filename
 from cs.lex import has_format_attributes, format_attribute, get_prefix_n
 from cs.logutils import warning
 from cs.pfx import Pfx, pfx_method, pfx_call
 from cs.progress import progressbar
 from cs.resources import RunState, uses_runstate
 from cs.result import bg as bg_result, report as report_results, CancellationError
 from cs.service_api import HTTPServiceAPI, RequestsNoAuth
 from cs.sqltags import SQLTags, SQLTagSet
 from cs.threads import monitor, bg as bg_thread
 from cs.units import BINARY_BYTES_SCALE
-from cs.upd import uses_upd, print  # pylint: disable=redefined-builtin
+from cs.upd import print  # pylint: disable=redefined-builtin
 
-__version__ = '20230217'
+__version__ = '20230703'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Programming Language :: Python",
@@ -61,26 +60,26 @@
         'console_scripts': ['playon = cs.app.playon:main'],
     },
     'install_requires': [
         'cs.cmdutils',
         'cs.context',
         'cs.deco',
         'cs.fileutils>=atomic_filename',
-        'cs.fstags',
         'cs.lex',
         'cs.logutils',
         'cs.pfx>=pfx_call',
         'cs.progress',
         'cs.resources',
         'cs.result',
         'cs.service_api',
         'cs.sqltags',
         'cs.threads',
         'cs.units',
         'cs.upd',
+        'icontract',
         'requests',
         'typeguard',
     ],
 }
 
 DBURL_ENVVAR = 'PLAYON_TAGS_DBURL'
 DBURL_DEFAULT = '~/var/playon.sqlite'
@@ -139,20 +138,26 @@
       downloaded    Recordings already downloaded.
       expired       Recording which are no longer available.
       pending       Recordings not already downloaded.
       /regexp       Recordings whose Series or Name match the regexp,
                     case insensitive.
   '''
 
-  def apply_defaults(self):
-    options = self.options
-    options.user = environ.get('PLAYON_USER', environ.get('EMAIL'))
-    options.password = environ.get('PLAYON_PASSWORD')
-    options.filename_format = environ.get(
-        'PLAYON_FILENAME_FORMAT', DEFAULT_FILENAME_FORMAT
+  @dataclass
+  class Options(BaseCommand.Options):
+    user: Optional[str] = field(
+        default_factory=lambda: environ.
+        get('PLAYON_USER', environ.get('EMAIL'))
+    )
+    password: Optional[str] = field(
+        default_factory=lambda: environ.get('PLAYON_PASSWORD')
+    )
+    filename_format: str = field(
+        default_factory=lambda: environ.
+        get('PLAYON_FILENAME_FORMAT', DEFAULT_FILENAME_FORMAT)
     )
 
   @contextmanager
   def run_context(self):
     ''' Prepare the `PlayOnAPI` around each command invocation.
     '''
     with super().run_context():
@@ -288,15 +293,14 @@
               sem.acquire()  # pylint: disable=consider-using-with
               Rs.append(bg_result(_dl, dl_id, sem, _extra=dict(dl_id=dl_id)))
 
     if Rs:
       for R in report_results(Rs):
         dl_id = R.extra['dl_id']
         recording = sqltags[dl_id]
-        warning("RECORDING = %s", recording)
         try:
           dl = R()
         except CancellationError as e:
           warning("%s: download interrupted: %s", recording.nice_name(), e)
           xit = 1
         else:
           if not dl:
@@ -356,14 +360,64 @@
           continue
         for dl_id in recording_ids:
           recording = sqltags[dl_id]
           with Pfx(recording.name):
             recording.ls(ls_format=listing_format, long_mode=long_mode)
     return xit
 
+  def cmd_downloaded(self, argv, locale='en_US'):
+    ''' Usage: {cmd} recordings...
+          Mark the specified recordings as downloaded and no longer pending.
+    '''
+    if not argv:
+      raise GetoptError("missing recordings")
+    sqltags = self.options.sqltags
+    xit = 0
+    for spec in argv:
+      with Pfx(spec):
+        recording_ids = sqltags.recording_ids_from_str(spec)
+        if not recording_ids:
+          warning("no recording ids")
+          xit = 1
+          continue
+        for dl_id in recording_ids:
+          with Pfx("%s", dl_id):
+            recording = sqltags[dl_id]
+            print(dl_id, '+ downloaded')
+            recording.add("downloaded")
+
+  def cmd_feature(self, argv, locale='en_US'):
+    ''' Usage: {cmd} [feature_id]
+          List features.
+    '''
+    long_mode = False
+    opts, argv = getopt(argv, 'l', '')
+    for opt, val in opts:
+      if opt == '-l':
+        long_mode = True
+      else:
+        raise RuntimeError("unhandled option: %r" % (opt,))
+    if argv:
+      feature_id = argv.pop(0)
+    else:
+      feature_id = None
+    if argv:
+      raise GetoptError("extra arguments: %r" % (argv,))
+    api = self.options.api
+    for feature in sorted(api.features(), key=lambda svc: svc['playon.ID']):
+      playon = feature.subtags('playon', as_tagset=True)
+      if feature_id is not None and playon.ID != feature_id:
+        print("skip", playon.ID)
+        continue
+      print(playon.ID)
+      if feature_id is None and not long_mode:
+        continue
+      for tag in playon:
+        print(" ", tag)
+
   def cmd_ls(self, argv):
     ''' Usage: {cmd} [-l] [recordings...]
           List available downloads.
           -l        Long listing: list tags below each entry.
           -o format Format string for each entry.
           Default format: {LS_FORMAT}
     '''
@@ -512,17 +566,18 @@
     ''' Is a recording still in the queue?
     '''
     return 'playon.Created' not in self
 
   @format_attribute
   def is_downloaded(self):
     ''' Test whether this recording has been downloaded
-        based on the presence of a `download_path` `Tag`.
+        based on the presence of a `download_path` `Tag`
+        or a true `downloaded` `Tag`.
     '''
-    return self.download_path is not None
+    return self.download_path is not None or 'downloaded' in self
 
   @format_attribute
   def is_pending(self):
     ''' A pending download: available and not already downloaded.
     '''
     return self.is_available() and not self.is_downloaded()
 
@@ -774,21 +829,25 @@
 
   @typechecked
   def __getitem__(self, download_id: int):
     ''' Return the recording `TagSet` associated with the recording `download_id`.
     '''
     return self.sqltags[download_id]
 
-  def suburl(self, suburl, headers=None, **kw):
+  def suburl(
+      self, suburl, *, api_version=None, headers=None, _base_url=None, **kw
+  ):
     ''' Override `HTTPServiceAPI.suburl` with default
         `headers={'Authorization':self.jwt}`.
     '''
+    if _base_url is None:
+      _base_url = None if api_version is None else f'api/v{api_version}'
     if headers is None:
       headers = dict(Authorization=self.jwt)
-    return super().suburl(suburl, headers=headers, **kw)
+    return super().suburl(suburl, _base_url=_base_url, headers=headers, **kw)
 
   def suburl_data(self, suburl, *, raw=False, **kw):
     ''' Call `suburl` and return the `'data'` component on success.
 
         Parameters:
         * `suburl`: the API subURL designating the endpoint.
         * `raw`: if true, return the whole decoded JSON result;
@@ -825,134 +884,126 @@
         _method=_method,
         headers=headers,
         raw=True,
         **kw
     )
 
   @pfx_method
-  def _recordings_from_entries(self, entries) -> Set[SQLTagSet]:
-    ''' Return the recording `TagSet` instances from PlayOn data entries.
-    '''
-    with self.sqltags:
-      now = time.time()
-      recordings = set()
-      for entry in entries:
-        entry_id = entry['ID']
-        with Pfx(entry_id):
-          for field, conv in sorted(dict(
-              Episode=int,
-              ReleaseYear=int,
-              Season=int,
-              ##Created=self.from_playon_date,
-              ##Expires=self.from_playon_date,
-              ##Updated=self.from_playon_date,
-          ).items()):
-            try:
-              value = entry[field]
-            except KeyError:
-              pass
-            else:
-              with Pfx("%s=%r", field, value):
-                if value is None:
-                  del entry[field]
-                else:
-                  try:
-                    value2 = conv(value)
-                  except ValueError as e:
-                    warning("%r: %s", value, e)
-                  else:
-                    entry[field] = value2
-          recording = self[entry_id]
-          # sometimes the name is spuriously prefixed with the seaon and episode
-          playon_name = entry['Name']
-          season = entry.get('Season')
-          spfx, sn, offset = get_prefix_n(playon_name, 's', season)
-          if spfx:
-            episode = entry.get('Episode')
-            epfx, en, offset = get_prefix_n(
-                playon_name, 'e', episode, offset=offset
-            )
-            if epfx:
-              entry['Season'] = sn
-              entry['Episode'] = en
-              entry['Name'] = playon_name[offset:].lstrip(' -')
-          recording.update(entry, prefix='playon')
-          recording.update(dict(last_updated=now))
-          recordings.add(recording)
-      return recordings
-
-  @pfx_method
   def queue(self):
     ''' Return the `TagSet` instances for the queued recordings.
     '''
     with self.sqltags.db_session():
       data = self.suburl_data('queue')
       entries = data['entries']
-      return self._recordings_from_entries(entries)
+      return self._entry_tagsets(
+          entries, 'recording', dict(
+              Episode=int,
+              ReleaseYear=int,
+              Season=int,
+          )
+      )
 
   @pfx_method
   def recordings(self):
     ''' Return the `TagSet` instances for the available recordings.
     '''
     with self.sqltags.db_session():
       data = self.suburl_data('library/all')
       entries = data['entries']
-      return self._recordings_from_entries(entries)
+      return self._entry_tagsets(
+          entries, 'recording', dict(
+              Episode=int,
+              ReleaseYear=int,
+              Season=int,
+          )
+      )
 
   available = recordings
 
   @pfx_method
-  def _services_from_entries(self, entries):
-    ''' Return the service `TagSet` instances from PlayOn data entries.
+  @require(lambda type: type in ('feature', 'recording', 'service'))
+  def _entry_tagsets(
+      self, entries, type: str, conversions: Optional[dict] = None
+  ) -> set:
+    ''' Return a `set` of `TagSet` instances from PlayOn data entries.
     '''
     with self.sqltags:
       now = time.time()
-      services = set()
+      tes = set()
       for entry in entries:
         entry_id = entry['ID']
         with Pfx(entry_id):
           # pylint: disable=use-dict-literal
-          for field, conv in sorted(dict(
-              ##Created=self.from_playon_date,
-              ##Expires=self.from_playon_date,
-              ##Updated=self.from_playon_date,
-          ).items()):
-            try:
-              value = entry[field]
-            except KeyError:
-              pass
-            else:
-              with Pfx("%s=%r", field, value):
-                if value is None:
-                  del entry[field]
-                else:
-                  try:
-                    value2 = conv(value)
-                  except ValueError as e:
-                    warning("%r: %s", value, e)
+          if conversions:
+            for e_field, conv in sorted(conversions.items()):
+              try:
+                value = entry[e_field]
+              except KeyError:
+                pass
+              else:
+                with Pfx("%s=%r", e_field, value):
+                  if value is None:
+                    del entry[e_field]
                   else:
-                    entry[field] = value2
-          service = self.service(entry_id)
-          service.update(entry, prefix='playon')
-          service.update(dict(last_updated=now))
-          services.add(service)
-      return services
+                    try:
+                      value2 = conv(value)
+                    except ValueError as e:
+                      warning("%r: %s", value, e)
+                    else:
+                      entry[e_field] = value2
+          te = self.sqltags[f'{type}.{entry_id}']
+          te.update(entry, prefix='playon')
+          te.update(dict(last_updated=now))
+          tes.add(te)
+      return tes
+
+  @pfx_method
+  def _services_from_entries(self, entries):
+    ''' Return the service `TagSet` instances from PlayOn data entries.
+    '''
+    return self._entry_tagsets(entries, 'service')
 
   @pfx_method
   def services(self):
     ''' Fetch the list of services.
     '''
     entries = self.cdsurl_data('content')
     return self._services_from_entries(entries)
 
-  def service(self, service_id):
+  def service(self, service_id: str):
     ''' Return the service `SQLTags` instance for `service_id`.
     '''
     return self.sqltags[f'service.{service_id}']
 
+  @pfx_method
+  def features(self):
+    ''' Fetch the list of featured shows.
+    '''
+    entries = self.cdsurl_data('content/featured')
+    return self._entry_tagsets(entries, 'feature')
+
+  def feature(self, feature_id):
+    ''' Return the feature `SQLTags` instance for `feature_id`.
+    '''
+    return self.sqltags[f'feature.{feature_id}']
+
+  def featured_image_url(self, feature_name: str):
+    ''' URL of the image for a featured show. '''
+    return self.suburl(
+        self, f'content/featured/{feature_name}/image', api_version=9
+    )
+
+  def service_image_url(self, service_id, large=True):
+    return self.suburl(
+        self,
+        f'content/{service_id}/image?size={"large" if large else "small"}',
+        _base_url=self.CDS_HOSTNAME,
+        api_version=9,
+    )
+
   # pylint: disable=too-many-locals
   @pfx_method
   @uses_runstate
   @typechecked
   def download(self, download_id: int, filename=None, *, runstate: RunState):
     ''' Download the file with `download_id` to `filename_basis`.
         Return the `TagSet` for the recording.
```

### Comparing `cs.app.playon-20230217/lib/python/cs.app.playon.egg-info/PKG-INFO` & `cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.app.playon
-Version: 20230217
+Version: 20230703
 Summary: PlayOn facilities, primarily access to the download API. Includes a nice command line tool.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -17,20 +17,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 PlayOn facilities, primarily access to the download API.
 Includes a nice command line tool.
 
-*Latest release 20230217*:
-* Move some core stuff off into cs.service_api.HTTPServiceAPI.
-* Move core Recording.is_stale() method to TagSet.is_stale(), leave override method behind.
-* Persist login tokens in a db for reuse while still fresh.
-* "playon dl": allow interrupting downloads.
-* Cleaner handling of playon.Name having a leading SNNeNN prefix.
+*Latest release 20230703*:
+* PlayOnAPI: features, feature, featured_image_url, service_image_url.
+* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
+* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
+* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
+* PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
 
 ## Function `main(argv=None)`
 
 Playon command line mode;
 see the `PlayOnCommand` class below.
 
 ## Class `PlayOnAPI(cs.service_api.HTTPServiceAPI, cs.service_api.ServiceAPI, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -74,14 +74,18 @@
             content
             content/provider-name
         dl [-j jobs] [-n] [recordings...]
           Download the specified recordings, default "pending".
           -j jobs   Run this many downloads in parallel.
                     The default is 2.
           -n        No download. List the specified recordings.
+        downloaded recordings...
+          Mark the specified recordings as downloaded and no longer pending.
+        feature [feature_id]
+          List features.
         help [-l] [subcommand-names...]
           Print the full help for the named subcommands,
           or for all subcommands if no names are specified.
           -l  Long help even if no subcommand-names provided.
         ls [-l] [recordings...]
           List available downloads.
           -l        Long listing: list tags below each entry.
@@ -98,27 +102,36 @@
           -l        Long listing: list tags below each entry.
           -o format Format string for each entry.
           Default format: {playon.ID} {playon.Series} {playon.Name} {playon.ProviderID}
         refresh [queue] [recordings]
           Update the db state from the PlayOn service.
         service [service_id]
           List services.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
 ## Class `PlayOnSQLTags(cs.sqltags.SQLTags, cs.tagset.BaseTagSets, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, collections.abc.MutableMapping, collections.abc.Mapping, collections.abc.Collection, collections.abc.Sized, collections.abc.Iterable, collections.abc.Container, cs.deco.Promotable)`
 
 `SQLTags` subclass with PlayOn related methods.
 
 ## Class `Recording(cs.sqltags.SQLTagSet, cs.obj.SingletonMixin, cs.tagset.TagSet, builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter, cs.mappings.AttrableMappingMixin)`
 
 An `SQLTagSet` with knowledge about PlayOn recordings.
 
 # Release Log
 
 
 
+*Release 20230703*:
+* PlayOnAPI: features, feature, featured_image_url, service_image_url.
+* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
+* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
+* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
+* PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
+
 *Release 20230217*:
 * Move some core stuff off into cs.service_api.HTTPServiceAPI.
 * Move core Recording.is_stale() method to TagSet.is_stale(), leave override method behind.
 * Persist login tokens in a db for reuse while still fresh.
 * "playon dl": allow interrupting downloads.
 * Cleaner handling of playon.Name having a leading SNNeNN prefix.
```

### Comparing `cs.app.playon-20230217/pyproject.toml` & `cs.app.playon-20230703/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,62 +4,62 @@
 authors = [
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python3",
 ]
 dependencies = [
-    "cs.cmdutils>=20230212",
-    "cs.context>=20230212",
-    "cs.deco>=20230212",
+    "cs.cmdutils>=20230703",
+    "cs.context>=20230331",
+    "cs.deco>=20230331",
     "cs.fileutils>=20210731",
-    "cs.fstags>=20230217",
-    "cs.lex>=20230217",
+    "cs.lex>=20230401",
     "cs.logutils>=20230212",
     "cs.pfx>=20210731",
-    "cs.progress>=20230212",
-    "cs.resources>=20230217",
-    "cs.result>=20230212",
-    "cs.service_api>=20230217",
-    "cs.sqltags>=20230217",
-    "cs.threads>=20230212",
+    "cs.progress>=20230401",
+    "cs.resources>=20230503",
+    "cs.result>=20230331",
+    "cs.service_api>=20230703",
+    "cs.sqltags>=20230612",
+    "cs.threads>=20230331",
     "cs.units",
-    "cs.upd>=20230217",
+    "cs.upd>=20230401",
+    "icontract",
     "requests",
     "typeguard",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230217"
+version = "20230703"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 PlayOn facilities, primarily access to the download API.
 Includes a nice command line tool.
 
-*Latest release 20230217*:
-* Move some core stuff off into cs.service_api.HTTPServiceAPI.
-* Move core Recording.is_stale() method to TagSet.is_stale(), leave override method behind.
-* Persist login tokens in a db for reuse while still fresh.
-* \"playon dl\": allow interrupting downloads.
-* Cleaner handling of playon.Name having a leading SNNeNN prefix.
+*Latest release 20230703*:
+* PlayOnAPI: features, feature, featured_image_url, service_image_url.
+* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
+* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
+* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
+* PlayOnCommand.cmd_downloaded: add 'downloaded\" tag to specified recordings.
 
 ## Function `main(argv=None)`
 
 Playon command line mode;
 see the `PlayOnCommand` class below.
 
 ## Class `PlayOnAPI(cs.service_api.HTTPServiceAPI, cs.service_api.ServiceAPI, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -103,14 +103,18 @@
             content
             content/provider-name
         dl [-j jobs] [-n] [recordings...]
           Download the specified recordings, default \"pending\".
           -j jobs   Run this many downloads in parallel.
                     The default is 2.
           -n        No download. List the specified recordings.
+        downloaded recordings...
+          Mark the specified recordings as downloaded and no longer pending.
+        feature [feature_id]
+          List features.
         help [-l] [subcommand-names...]
           Print the full help for the named subcommands,
           or for all subcommands if no names are specified.
           -l  Long help even if no subcommand-names provided.
         ls [-l] [recordings...]
           List available downloads.
           -l        Long listing: list tags below each entry.
@@ -127,27 +131,36 @@
           -l        Long listing: list tags below each entry.
           -o format Format string for each entry.
           Default format: {playon.ID} {playon.Series} {playon.Name} {playon.ProviderID}
         refresh [queue] [recordings]
           Update the db state from the PlayOn service.
         service [service_id]
           List services.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
 ## Class `PlayOnSQLTags(cs.sqltags.SQLTags, cs.tagset.BaseTagSets, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, collections.abc.MutableMapping, collections.abc.Mapping, collections.abc.Collection, collections.abc.Sized, collections.abc.Iterable, collections.abc.Container, cs.deco.Promotable)`
 
 `SQLTags` subclass with PlayOn related methods.
 
 ## Class `Recording(cs.sqltags.SQLTagSet, cs.obj.SingletonMixin, cs.tagset.TagSet, builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter, cs.mappings.AttrableMappingMixin)`
 
 An `SQLTagSet` with knowledge about PlayOn recordings.
 
 # Release Log
 
 
 
+*Release 20230703*:
+* PlayOnAPI: features, feature, featured_image_url, service_image_url.
+* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
+* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
+* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
+* PlayOnCommand.cmd_downloaded: add 'downloaded\" tag to specified recordings.
+
 *Release 20230217*:
 * Move some core stuff off into cs.service_api.HTTPServiceAPI.
 * Move core Recording.is_stale() method to TagSet.is_stale(), leave override method behind.
 * Persist login tokens in a db for reuse while still fresh.
 * \"playon dl\": allow interrupting downloads.
 * Cleaner handling of playon.Name having a leading SNNeNN prefix.
```

### Comparing `cs.app.playon-20230217/setup.cfg` & `cs.app.playon-20230703/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.app.playon
-version = 20230217
+version = 20230703
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = PlayOn facilities, primarily access to the download API. Includes a nice command line tool.
 keywords = python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
@@ -19,30 +19,30 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
-	cs.cmdutils>=20230212
-	cs.context>=20230212
-	cs.deco>=20230212
+	cs.cmdutils>=20230703
+	cs.context>=20230331
+	cs.deco>=20230331
 	cs.fileutils>=20210731
-	cs.fstags>=20230217
-	cs.lex>=20230217
+	cs.lex>=20230401
 	cs.logutils>=20230212
 	cs.pfx>=20210731
-	cs.progress>=20230212
-	cs.resources>=20230217
-	cs.result>=20230212
-	cs.service_api>=20230217
-	cs.sqltags>=20230217
-	cs.threads>=20230212
+	cs.progress>=20230401
+	cs.resources>=20230503
+	cs.result>=20230331
+	cs.service_api>=20230703
+	cs.sqltags>=20230612
+	cs.threads>=20230331
 	cs.units
-	cs.upd>=20230217
+	cs.upd>=20230401
+	icontract
 	requests
 	typeguard
 
 [options.entry_points]
 console_scripts = 
 	playon = cs.app.playon:main
```

