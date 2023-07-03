# Comparing `tmp/git_changelog-1.0.1.tar.gz` & `tmp/git_changelog-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_changelog-1.0.1.tar", last modified: Wed May 10 15:56:33 2023, max compression
+gzip compressed data, was "git_changelog-2.0.0.tar", last modified: Mon Jul  3 13:07:07 2023, max compression
```

## Comparing `git_changelog-1.0.1.tar` & `git_changelog-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,25 @@
--rw-r--r--   0        0        0      754 2023-05-10 15:37:31.957872 git_changelog-1.0.1/LICENSE
--rw-r--r--   0        0        0     7863 2023-05-10 15:37:31.957872 git_changelog-1.0.1/README.md
--rw-r--r--   0        0        0     2697 2023-05-10 15:56:33.713125 git_changelog-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      254 2023-05-10 15:37:31.957872 git_changelog-1.0.1/src/git_changelog/__init__.py
--rw-r--r--   0        0        0      387 2023-05-10 15:37:31.957872 git_changelog-1.0.1/src/git_changelog/__main__.py
--rw-r--r--   0        0        0    14779 2023-05-10 15:20:51.179724 git_changelog-1.0.1/src/git_changelog/build.py
--rw-r--r--   0        0        0    13174 2023-05-10 15:51:30.408729 git_changelog-1.0.1/src/git_changelog/cli.py
--rw-r--r--   0        0        0    13748 2023-05-10 15:20:51.179724 git_changelog-1.0.1/src/git_changelog/commit.py
--rw-r--r--   0        0        0    11212 2023-05-10 15:20:51.179724 git_changelog-1.0.1/src/git_changelog/providers.py
--rw-r--r--   0        0        0        0 2023-05-10 15:37:29.431312 git_changelog-1.0.1/src/git_changelog/py.typed
--rw-r--r--   0        0        0     1122 2023-02-03 19:05:40.815432 git_changelog-1.0.1/src/git_changelog/templates/__init__.py
--rw-r--r--   0        0        0     1588 2023-02-04 13:50:13.931438 git_changelog-1.0.1/src/git_changelog/templates/angular.md.jinja
--rw-r--r--   0        0        0     2213 2023-02-04 13:49:16.982323 git_changelog-1.0.1/src/git_changelog/templates/keepachangelog.md.jinja
--rw-r--r--   0        0        0       37 2021-11-14 15:27:29.516885 git_changelog-1.0.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2021-11-14 15:27:29.516885 git_changelog-1.0.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2021-11-14 15:27:29.516885 git_changelog-1.0.1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2021-11-14 15:32:24.789513 git_changelog-1.0.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2021-11-14 15:32:24.789513 git_changelog-1.0.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       10 2021-11-14 15:32:24.236192 git_changelog-1.0.1/tests/.pytest_cache/v/randomly_seed
--rw-r--r--   0        0        0      166 2023-05-10 15:37:29.424645 git_changelog-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-05-10 15:37:29.421312 git_changelog-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0     2361 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_angular_style.py
--rw-r--r--   0        0        0     2308 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_basic_style.py
--rw-r--r--   0        0        0     1172 2023-05-10 15:37:31.957872 git_changelog-1.0.1/tests/test_cli.py
--rw-r--r--   0        0        0     1079 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_commit.py
--rw-r--r--   0        0        0     5483 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_conventional_commit_style.py
--rw-r--r--   0        0        0     6039 2023-05-10 15:52:36.028834 git_changelog-1.0.1/tests/test_end_to_end.py
--rw-r--r--   0        0        0     1207 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_providers.py
--rw-r--r--   0        0        0     2297 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_version.py
--rw-r--r--   0        0        0     9526 1970-01-01 00:00:00.000000 git_changelog-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-07-01 10:51:08.684355 git_changelog-2.0.0/LICENSE
+-rw-r--r--   0        0        0     8453 2023-07-03 13:00:29.469919 git_changelog-2.0.0/README.md
+-rw-r--r--   0        0        0     2723 2023-07-03 13:07:07.133360 git_changelog-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      254 2023-07-01 10:51:08.684355 git_changelog-2.0.0/src/git_changelog/__init__.py
+-rw-r--r--   0        0        0      387 2023-07-01 10:51:08.684355 git_changelog-2.0.0/src/git_changelog/__main__.py
+-rw-r--r--   0        0        0    15261 2023-07-03 12:39:27.374475 git_changelog-2.0.0/src/git_changelog/build.py
+-rw-r--r--   0        0        0    16161 2023-07-03 12:44:30.582591 git_changelog-2.0.0/src/git_changelog/cli.py
+-rw-r--r--   0        0        0    13926 2023-07-01 11:37:50.518284 git_changelog-2.0.0/src/git_changelog/commit.py
+-rw-r--r--   0        0        0    11252 2023-07-01 11:07:50.369403 git_changelog-2.0.0/src/git_changelog/providers.py
+-rw-r--r--   0        0        0        0 2023-07-01 10:51:06.314370 git_changelog-2.0.0/src/git_changelog/py.typed
+-rw-r--r--   0        0        0     1122 2023-02-03 19:05:40.815432 git_changelog-2.0.0/src/git_changelog/templates/__init__.py
+-rw-r--r--   0        0        0     1588 2023-02-04 13:50:13.931438 git_changelog-2.0.0/src/git_changelog/templates/angular.md.jinja
+-rw-r--r--   0        0        0     2213 2023-02-04 13:49:16.982323 git_changelog-2.0.0/src/git_changelog/templates/keepachangelog.md.jinja
+-rw-r--r--   0        0        0      166 2023-07-01 10:51:06.304370 git_changelog-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-01 10:51:06.304370 git_changelog-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     2361 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_angular_style.py
+-rw-r--r--   0        0        0     2308 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_basic_style.py
+-rw-r--r--   0        0        0     1172 2023-07-01 10:51:08.684355 git_changelog-2.0.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1079 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_commit.py
+-rw-r--r--   0        0        0     5483 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_conventional_commit_style.py
+-rw-r--r--   0        0        0     6708 2023-07-03 12:39:27.101147 git_changelog-2.0.0/tests/test_end_to_end.py
+-rw-r--r--   0        0        0     1207 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_providers.py
+-rw-r--r--   0        0        0      897 2023-07-03 12:39:27.097813 git_changelog-2.0.0/tests/test_release_notes.py
+-rw-r--r--   0        0        0     2297 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_version.py
+-rw-r--r--   0        0        0    10008 1970-01-01 00:00:00.000000 git_changelog-2.0.0/PKG-INFO
```

### Comparing `git_changelog-1.0.1/LICENSE` & `git_changelog-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/README.md` & `git_changelog-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -57,24 +57,24 @@
 With `pip`:
 ```bash
 pip install git-changelog
 ```
 
 With [`pipx`](https://github.com/pipxproject/pipx):
 ```bash
-python3.7 -m pip install --user pipx
+python3.8 -m pip install --user pipx
 pipx install git-changelog
 ```
 
 ## Usage (command-line)
 
 ```
 usage: git-changelog [-b] [-h] [-i] [-g VERSION_REGEX] [-m MARKER_LINE]
-                     [-o OUTPUT] [-R] [-c {angular,atom,conventional,basic}]
-                     [-S SECTIONS [SECTIONS ...]]
+                     [-o OUTPUT] [-r] [-R] [-I INPUT]
+                     [-c {angular,atom,conventional,basic}] [-s SECTIONS]
                      [-t {angular,keepachangelog}] [-T] [-v]
                      [REPOSITORY]
 
 Automatic Changelog generator using Jinja2 templates.
 
 This tool parses your commit messages to extract useful data
 that is then rendered using Jinja2 templates, for example to
@@ -130,54 +130,63 @@
 - ci: Continuous Integration
 - deps: Dependencies
 - doc, docs: Docs
 - style: Style
 - test, tests: Tests
 
 positional arguments:
-  REPOSITORY            The repository path, relative or absolute.
+  REPOSITORY            The repository path, relative or absolute. Default: .
 
 options:
-  -b, --bump            Guess the new latest version by bumping the previous
+  -b, --bump-latest     Guess the new latest version by bumping the previous
                         one based on the set of unreleased commits. For
                         example, if a commit contains breaking changes, bump
                         the major number (or the minor number for 0.x
                         versions). Else if there are new features, bump the
                         minor number. Else just bump the patch number.
+                        Default: False.
   -h, --help            Show this help message and exit.
   -i, --in-place        Insert new entries (versions missing from changelog)
                         in-place. An output file must be specified. With
                         custom templates, you can pass two additional
                         arguments: --version-regex and --marker-line. When
                         writing in-place, an 'in_place' variable will be
                         injected in the Jinja context, allowing to adapt the
                         generated contents (for example to skip changelog
-                        headers or footers).
+                        headers or footers). Default: False.
   -g, --version-regex VERSION_REGEX
                         A regular expression to match versions in the existing
                         changelog (used to find the latest release) when
                         writing in-place. The regular expression must be a
-                        Python regex with a 'version' named group.
+                        Python regex with a 'version' named group. Default:
+                        ^## \[(?P<version>v?[^\]]+).
   -m, --marker-line MARKER_LINE
                         A marker line at which to insert new entries (versions
                         missing from changelog). If two marker lines are
                         present in the changelog, the contents between those
                         two lines will be overwritten (useful to update an
-                        'Unreleased' entry for example).
-  -o OUTPUT, --output OUTPUT
-                        Output to given file. Default: stdout.
-  -r, --parse-refs      Parse provider-specific references in commit
-                        messages (GitHub/GitLab issues, PRs, etc.).
-  -c, -s, --style, --commit-style,  --convention {angular,atom,conventional,basic}
-                        The commit convention to match against. Default: basic.
-  -S, --sections SECTIONS [SECTIONS ...]
-                        The sections to render. See the available sections for
-                        each supported convention in the description.
-  -t, --template {angular,keepachangelog}
+                        'Unreleased' entry for example). Default: <!--
+                        insertion marker -->.
+  -o, --output OUTPUT   Output to given file. Default: stdout.
+  -r, --parse-refs      Parse provider-specific references in commit messages
+                        (GitHub/GitLab issues, PRs, etc.). Default: False.
+  -R, --release-notes   Output release notes to stdout based on the last entry
+                        in the changelog. Default: False.
+  -I, --input INPUT     Read from given file when creating release notes.
+                        Default: CHANGELOG.md.
+  -c, --style, --commit-style, --convention {angular,atom,conventional,basic}
+                        The commit convention to match against. Default:
+                        basic.
+  -s, --sections SECTIONS
+                        A comma-separated list of sections to render. See the
+                        available sections for each supported convention in
+                        the description. Default: None.
+  -t {angular,keepachangelog}, --template {angular,keepachangelog}
                         The Jinja2 template to use. Prefix with "path:" to
                         specify the path to a directory containing a file
-                        named "changelog.md".
+                        named "changelog.md". Default: keepachangelog.
   -T, --trailers, --git-trailers
                         Parse Git trailers in the commit message. See
                         https://git-scm.com/docs/git-interpret-trailers.
+                        Default: False.
   -v, --version         Show the current version of the program and exit.
 ```
```

### Comparing `git_changelog-1.0.1/pyproject.toml` & `git_changelog-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,46 +7,44 @@
 [project]
 name = "git-changelog"
 description = "Automatic Changelog generator using Jinja2 templates."
 authors = [
     { name = "Timothée Mazzucotelli", email = "pawamoy@pm.me" },
 ]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = [
     "git",
     "changelog",
     "changelog-generator",
     "commit-style",
     "commit-convention",
 ]
 dynamic = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Documentation",
     "Topic :: Software Development",
     "Topic :: Software Development :: Documentation",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "Jinja2>=2.10,<4",
-    "semver~=2.13",
-    "importlib-metadata; python_version < '3.8'",
+    "semver>=2.13",
 ]
-version = "1.0.1"
+version = "2.0.0"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/git-changelog"
 Documentation = "https://pawamoy.github.io/git-changelog"
@@ -72,14 +70,20 @@
 package-dir = "src"
 editable-backend = "editables"
 
 [tool.pdm.dev-dependencies]
 duty = [
     "duty>=0.10",
 ]
+ci-quality = [
+    "git-changelog[duty,docs,quality,typing,security]",
+]
+ci-tests = [
+    "git-changelog[duty,tests]",
+]
 docs = [
     "black>=23.1",
     "markdown-callouts>=0.2",
     "markdown-exec>=0.5",
     "mkdocs>=1.3",
     "mkdocs-coverage>=0.2",
     "mkdocs-gen-files>=0.3",
```

### Comparing `git_changelog-1.0.1/src/git_changelog/build.py` & `git_changelog-2.0.0/src/git_changelog/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """The module responsible for building the data."""
 
 from __future__ import annotations
 
 import datetime
 import os
+import re
 import sys
 from contextlib import suppress
 from subprocess import check_output  # (we trust the commands we run)
-from typing import TYPE_CHECKING, Type, Union
+from typing import TYPE_CHECKING, ClassVar, Type, Union
 
 from semver import VersionInfo
 
 from git_changelog.commit import (
     AngularConvention,
     AtomConvention,
     BasicConvention,
@@ -136,28 +137,28 @@
         """
         return bool(self.tag.split(".", 2)[2])
 
 
 class Changelog:
     """The main changelog class."""
 
-    MARKER: str = "--GIT-CHANGELOG MARKER--"
-    FORMAT: str = (
+    MARKER: ClassVar[str] = "--GIT-CHANGELOG MARKER--"
+    FORMAT: ClassVar[str] = (
         r"%H%n"  # commit commit_hash
         r"%an%n"  # author name
         r"%ae%n"  # author email
         r"%ad%n"  # author date
         r"%cn%n"  # committer name
         r"%ce%n"  # committer email
         r"%cd%n"  # committer date
         r"%D%n"  # tag
         r"%s%n"  # subject
         r"%b%n" + MARKER  # body
     )
-    CONVENTION: dict[str, type[CommitConvention]] = {
+    CONVENTION: ClassVar[dict[str, type[CommitConvention]]] = {
         "basic": BasicConvention,
         "angular": AngularConvention,
         "atom": AtomConvention,
         "conventional": ConventionalCommitConvention,
     }
 
     def __init__(
@@ -257,15 +258,21 @@
         """
         remote = "remote." + os.environ.get("GIT_CHANGELOG_REMOTE", "origin") + ".url"
         git_url = self.run_git("config", "--get", remote).rstrip("\n")
         if git_url.startswith("git@"):
             git_url = git_url.replace(":", "/", 1).replace("git@", "https://", 1)
         if git_url.endswith(".git"):
             git_url = git_url[:-4]
-        return git_url
+
+        # Remove GitHub token from the URL.
+        # See https://gist.github.com/magnetikonline/073afe7909ffdd6f10ef06a00bc3bc88.
+        # Personal access tokens (classic): ^ghp_[a-zA-Z0-9]{36}$
+        # Personal access tokens (fine-grained): ^github_pat_[a-zA-Z0-9]{22}_[a-zA-Z0-9]{59}$
+        # GitHub Actions tokens: ^ghs_[a-zA-Z0-9]{36}$
+        return re.sub(r"(gh[ps]_[a-zA-Z0-9]{36}|github_pat_[a-zA-Z0-9]{22}_[a-zA-Z0-9]{59})@", "", git_url)
 
     def get_log(self) -> str:
         """Get the `git log` output.
 
         Returns:
             The output of the `git log` command, with a particular format.
         """
```

### Comparing `git_changelog-1.0.1/src/git_changelog/cli.py` & `git_changelog-2.0.0/src/git_changelog/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,31 +12,30 @@
 #   there's no `git_changelog.__main__` in `sys.modules`.
 
 from __future__ import annotations
 
 import argparse
 import re
 import sys
-from typing import Pattern, TextIO
+from importlib import metadata
+from typing import TYPE_CHECKING, Pattern, TextIO
 
 from jinja2.exceptions import TemplateNotFound
 
 from git_changelog import templates
 from git_changelog.build import Changelog, Version
 from git_changelog.commit import (
     AngularConvention,
     BasicConvention,
     CommitConvention,
     ConventionalCommitConvention,
 )
 
-if sys.version_info < (3, 8):
-    import importlib_metadata as metadata
-else:
-    from importlib import metadata
+if TYPE_CHECKING:
+    from pathlib import Path
 
 DEFAULT_VERSION_REGEX = r"^## \[(?P<version>v?[^\]]+)"
 DEFAULT_MARKER_LINE = "<!-- insertion marker -->"
 CONVENTIONS = ("angular", "atom", "conventional", "basic")
 
 
 class Templates(tuple):  # (subclassing tuple)
@@ -97,26 +96,26 @@
     )
 
     parser.add_argument(
         "repository",
         metavar="REPOSITORY",
         nargs="?",
         default=".",
-        help="The repository path, relative or absolute.",
+        help="The repository path, relative or absolute. Default: %(default)s.",
     )
 
     parser.add_argument(
         "-b",
         "--bump-latest",
         action="store_true",
         dest="bump_latest",
         default=False,
         help="Guess the new latest version by bumping the previous one based on the set of unreleased commits. "
         "For example, if a commit contains breaking changes, bump the major number (or the minor number for 0.x versions). "
-        "Else if there are new features, bump the minor number. Else just bump the patch number.",
+        "Else if there are new features, bump the minor number. Else just bump the patch number. Default: %(default)s.",
     )
     parser.add_argument(
         "-h",
         "--help",
         action="help",
         default=argparse.SUPPRESS,
         help="Show this help message and exit.",
@@ -129,38 +128,38 @@
         default=False,
         help="Insert new entries (versions missing from changelog) in-place. "
         "An output file must be specified. With custom templates, "
         "you can pass two additional arguments: --version-regex and --marker-line. "
         "When writing in-place, an 'in_place' variable "
         "will be injected in the Jinja context, "
         "allowing to adapt the generated contents "
-        "(for example to skip changelog headers or footers).",
+        "(for example to skip changelog headers or footers). Default: %(default)s.",
     )
     parser.add_argument(
         "-g",
         "--version-regex",
         action="store",
         dest="version_regex",
         default=DEFAULT_VERSION_REGEX,
         help="A regular expression to match versions in the existing changelog "
         "(used to find the latest release) when writing in-place. "
-        "The regular expression must be a Python regex with a 'version' named group. ",
+        "The regular expression must be a Python regex with a 'version' named group. Default: %(default)s.",
     )
 
     parser.add_argument(
         "-m",
         "--marker-line",
         action="store",
         dest="marker_line",
         default=DEFAULT_MARKER_LINE,
         help="A marker line at which to insert new entries "
         "(versions missing from changelog). "
         "If two marker lines are present in the changelog, "
         "the contents between those two lines will be overwritten "
-        "(useful to update an 'Unreleased' entry for example).",
+        "(useful to update an 'Unreleased' entry for example). Default: %(default)s.",
     )
     parser.add_argument(
         "-o",
         "--output",
         action="store",
         dest="output",
         default=sys.stdout,
@@ -168,53 +167,68 @@
     )
     parser.add_argument(
         "-r",
         "--parse-refs",
         action="store_true",
         dest="parse_refs",
         default=False,
-        help="Parse provider-specific references in commit messages (GitHub/GitLab issues, PRs, etc.).",
+        help="Parse provider-specific references in commit messages (GitHub/GitLab issues, PRs, etc.). Default: %(default)s.",
+    )
+    parser.add_argument(
+        "-R",
+        "--release-notes",
+        action="store_true",
+        dest="release_notes",
+        default=False,
+        help="Output release notes to stdout based on the last entry in the changelog. Default: %(default)s.",
+    )
+    parser.add_argument(
+        "-I",
+        "--input",
+        dest="input",
+        default="CHANGELOG.md",
+        help="Read from given file when creating release notes. Default: %(default)s.",
     )
     parser.add_argument(
         "-c",
         "--style",
         "--commit-style",
         "--convention",
         choices=CONVENTIONS,
         default="basic",
         dest="convention",
-        help="The commit convention to match against. Default: basic.",
+        help="The commit convention to match against. Default: %(default)s.",
     )
     parser.add_argument(
         "-s",
         "--sections",
         action="store",
         type=_comma_separated_list,
         default=None,
         dest="sections",
         help="A comma-separated list of sections to render. "
-        "See the available sections for each supported convention in the description.",
+        "See the available sections for each supported convention in the description. Default: %(default)s.",
     )
     parser.add_argument(
         "-t",
         "--template",
         choices=Templates(("angular", "keepachangelog")),
         default="keepachangelog",
         dest="template",
         help='The Jinja2 template to use. Prefix with "path:" to specify the path '
-        'to a directory containing a file named "changelog.md".',
+        'to a directory containing a file named "changelog.md". Default: %(default)s.',
     )
     parser.add_argument(
         "-T",
         "--trailers",
         "--git-trailers",
         action="store_true",
         default=False,
         dest="parse_trailers",
-        help="Parse Git trailers in the commit message. See https://git-scm.com/docs/git-interpret-trailers.",
+        help="Parse Git trailers in the commit message. See https://git-scm.com/docs/git-interpret-trailers. Default: %(default)s.",
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
         version="%(prog)s " + get_version(),  # (%)
         help="Show the current version of the program and exit.",
@@ -233,49 +247,14 @@
 def _unreleased(versions: list[Version], last_release: str) -> list[Version]:
     for index, version in enumerate(versions):
         if version.tag == last_release:
             return versions[:index]
     return versions
 
 
-def main(args: list[str] | None = None) -> int:
-    """Run the main program.
-
-    This function is executed when you type `git-changelog` or `python -m git_changelog`.
-
-    Arguments:
-        args: Arguments passed from the command line.
-
-    Returns:
-        An exit code.
-    """
-    parser = get_parser()
-    opts = parser.parse_args(args=args)
-
-    try:
-        build_and_render(
-            repository=opts.repository,
-            template=opts.template,
-            convention=opts.convention,
-            parse_refs=opts.parse_refs,
-            parse_trailers=opts.parse_trailers,
-            sections=opts.sections,
-            in_place=opts.in_place,
-            output=opts.output,
-            version_regex=opts.version_regex,
-            marker_line=opts.marker_line,
-            bump_latest=opts.bump_latest,
-        )
-    except ValueError as error:
-        print(f"git-changelog: {error}", file=sys.stderr)
-        return 1
-
-    return 0
-
-
 def build_and_render(
     repository: str,
     template: str,
     convention: str | CommitConvention,
     parse_refs: bool = False,  # noqa: FBT001,FBT002
     parse_trailers: bool = False,  # noqa: FBT001,FBT002
     sections: list[str] | None = None,
@@ -387,7 +366,113 @@
         if output is sys.stdout:
             sys.stdout.write(rendered)
         else:
             with open(output, "w") as stream:  # type: ignore[arg-type]
                 stream.write(rendered)
 
     return changelog, rendered
+
+
+def get_release_notes(
+    input_file: str | Path = "CHANGELOG.md",
+    version_regex: str = DEFAULT_VERSION_REGEX,
+    marker_line: str = DEFAULT_MARKER_LINE,
+) -> str:
+    """Get release notes from existing changelog.
+
+    This will return the latest entry in the changelog.
+
+    Parameters:
+        input_file: The changelog to read from.
+        version_regex: A regular expression to match version entries.
+        marker_line: The insertion marker line in the changelog.
+
+    Returns:
+        The latest changelog entry.
+    """
+    release_notes = []
+    found_marker = False
+    found_version = False
+    with open(input_file) as changelog:
+        for line in changelog:
+            line = line.strip()  # noqa: PLW2901
+            if not found_marker:
+                if line == marker_line:
+                    found_marker = True
+                continue
+            if re.search(version_regex, line):
+                if found_version:
+                    break
+                found_version = True
+            release_notes.append(line)
+    result = "\n".join(release_notes).strip()
+    if result.endswith(marker_line):
+        result = result[: -len(marker_line)].strip()
+    return result
+
+
+def output_release_notes(
+    input_file: str = "CHANGELOG.md",
+    version_regex: str = DEFAULT_VERSION_REGEX,
+    marker_line: str = DEFAULT_MARKER_LINE,
+    output_file: str | TextIO = sys.stdout,
+) -> None:
+    """Print release notes from existing changelog.
+
+    This will print the latest entry in the changelog.
+
+    Parameters:
+        input_file: The changelog to read from.
+        version_regex: A regular expression to match version entries.
+        marker_line: The insertion marker line in the changelog.
+        output_file: Where to print/write the release notes.
+    """
+    release_notes = get_release_notes(input_file, version_regex, marker_line)
+    try:
+        output_file.write(release_notes)  # type: ignore[union-attr]
+    except AttributeError:
+        with open(output_file, "w") as file:  # type: ignore[arg-type]
+            file.write(release_notes)
+
+
+def main(args: list[str] | None = None) -> int:
+    """Run the main program.
+
+    This function is executed when you type `git-changelog` or `python -m git_changelog`.
+
+    Arguments:
+        args: Arguments passed from the command line.
+
+    Returns:
+        An exit code.
+    """
+    parser = get_parser()
+    opts = parser.parse_args(args=args)
+
+    if opts.release_notes:
+        output_release_notes(
+            input_file=opts.input,
+            version_regex=opts.version_regex,
+            marker_line=opts.marker_line,
+            output_file=opts.output,
+        )
+        return 0
+
+    try:
+        build_and_render(
+            repository=opts.repository,
+            template=opts.template,
+            convention=opts.convention,
+            parse_refs=opts.parse_refs,
+            parse_trailers=opts.parse_trailers,
+            sections=opts.sections,
+            in_place=opts.in_place,
+            output=opts.output,
+            version_regex=opts.version_regex,
+            marker_line=opts.marker_line,
+            bump_latest=opts.bump_latest,
+        )
+    except ValueError as error:
+        print(f"git-changelog: {error}", file=sys.stderr)
+        return 1
+
+    return 0
```

### Comparing `git_changelog-1.0.1/src/git_changelog/commit.py` & `git_changelog-2.0.0/src/git_changelog/commit.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import re
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from contextlib import suppress
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Pattern
+from typing import TYPE_CHECKING, Any, ClassVar, Pattern
 
 if TYPE_CHECKING:
     from git_changelog.providers import ProviderRefParser, Ref
 
 
 def _clean_body(lines: list[str]) -> list[str]:
     while lines and not lines[0].strip():
@@ -153,18 +153,18 @@
             trailers[title] = value.strip()
         return trailers  # or raise ValueError due to split unpacking
 
 
 class CommitConvention(ABC):
     """A base class for a convention of commit messages."""
 
-    TYPES: dict[str, str]
-    TYPE_REGEX: Pattern
-    BREAK_REGEX: Pattern
-    DEFAULT_RENDER: list[str]
+    TYPES: ClassVar[dict[str, str]]
+    TYPE_REGEX: ClassVar[Pattern]
+    BREAK_REGEX: ClassVar[Pattern]
+    DEFAULT_RENDER: ClassVar[list[str]]
 
     @abstractmethod
     def parse_commit(self, commit: Commit) -> dict[str, str | bool]:
         """Parse the commit to extract information.
 
         Arguments:
             commit: The commit to parse.
@@ -184,43 +184,43 @@
         additional = "- " + "\n- ".join(
             f"{', '.join(types)}: {title}" for title, types in reversed_map.items() if title not in default_sections
         )
         return re.sub(
             r"\n *",
             "\n",
             f"""
-            {cls.__name__.replace('Convention', '').upper()} CONVENTION
+            {cls.__name__.replace('Convention', ' Convention').upper().strip()}
 
             Default sections:
             {default}
 
             Additional sections:
             {additional}
             """,
         )
 
 
 class BasicConvention(CommitConvention):
     """Basic commit message convention."""
 
-    TYPES: dict[str, str] = {
+    TYPES: ClassVar[dict[str, str]] = {
         "add": "Added",
         "fix": "Fixed",
         "change": "Changed",
         "remove": "Removed",
         "merge": "Merged",
         "doc": "Documented",
     }
 
-    TYPE_REGEX: Pattern = re.compile(r"^(?P<type>(%s))" % "|".join(TYPES.keys()), re.I)
-    BREAK_REGEX: Pattern = re.compile(
+    TYPE_REGEX: ClassVar[Pattern] = re.compile(r"^(?P<type>(%s))" % "|".join(TYPES.keys()), re.I)
+    BREAK_REGEX: ClassVar[Pattern] = re.compile(
         r"^break(s|ing changes?)?[ :].+$",
         re.I | re.MULTILINE,
     )
-    DEFAULT_RENDER: list[str] = [
+    DEFAULT_RENDER: ClassVar[list[str]] = [
         TYPES["add"],
         TYPES["fix"],
         TYPES["change"],
         TYPES["remove"],
     ]
 
     def parse_commit(self, commit: Commit) -> dict[str, str | bool]:  # noqa: D102
@@ -273,15 +273,15 @@
         """
         return bool(self.BREAK_REGEX.search(commit_message))
 
 
 class AngularConvention(CommitConvention):
     """Angular commit message convention."""
 
-    TYPES: dict[str, str] = {
+    TYPES: ClassVar[dict[str, str]] = {
         "build": "Build",
         "chore": "Chore",
         "ci": "Continuous Integration",
         "deps": "Dependencies",
         "doc": "Docs",
         "docs": "Docs",
         "feat": "Features",
@@ -290,22 +290,22 @@
         "ref": "Code Refactoring",
         "refactor": "Code Refactoring",
         "revert": "Reverts",
         "style": "Style",
         "test": "Tests",
         "tests": "Tests",
     }
-    SUBJECT_REGEX: Pattern = re.compile(
+    SUBJECT_REGEX: ClassVar[Pattern] = re.compile(
         r"^(?P<type>(%s))(?:\((?P<scope>.+)\))?: (?P<subject>.+)$" % ("|".join(TYPES.keys())),  # (%)
     )
-    BREAK_REGEX: Pattern = re.compile(
+    BREAK_REGEX: ClassVar[Pattern] = re.compile(
         r"^break(s|ing changes?)?[ :].+$",
         re.I | re.MULTILINE,
     )
-    DEFAULT_RENDER: list[str] = [
+    DEFAULT_RENDER: ClassVar[list[str]] = [
         TYPES["feat"],
         TYPES["fix"],
         TYPES["revert"],
         TYPES["refactor"],
         TYPES["perf"],
     ]
 
@@ -363,17 +363,17 @@
         """
         return bool(self.BREAK_REGEX.search(commit_message))
 
 
 class ConventionalCommitConvention(AngularConvention):
     """Conventional commit message convention."""
 
-    TYPES: dict[str, str] = AngularConvention.TYPES
-    DEFAULT_RENDER: list[str] = AngularConvention.DEFAULT_RENDER
-    SUBJECT_REGEX: Pattern = re.compile(
+    TYPES: ClassVar[dict[str, str]] = AngularConvention.TYPES
+    DEFAULT_RENDER: ClassVar[list[str]] = AngularConvention.DEFAULT_RENDER
+    SUBJECT_REGEX: ClassVar[Pattern] = re.compile(
         r"^(?P<type>(%s))(?:\((?P<scope>.+)\))?(?P<breaking>!)?: (?P<subject>.+)$" % ("|".join(TYPES.keys())),  # (%)
     )
 
     def parse_commit(self, commit: Commit) -> dict[str, str | bool]:  # noqa: D102
         subject = self.parse_subject(commit.subject)
         message = "\n".join([commit.subject, *commit.body])
         is_major = self.is_major(message) or subject.get("breaking") == "!"
@@ -389,15 +389,15 @@
             "is_patch": is_patch,
         }
 
 
 class AtomConvention(CommitConvention):
     """Atom commit message convention."""
 
-    TYPES: dict[str, str] = {
+    TYPES: ClassVar[dict[str, str]] = {
         ":art:": "",  # when improving the format/structure of the code
         ":racehorse:": "",  # when improving performance
         ":non-potable_water:": "",  # when plugging memory leaks
         ":memo:": "",  # when writing docs
         ":penguin:": "",  # when fixing something on Linux
         ":apple:": "",  # when fixing something on Mac OS
         ":checkered_flag:": "",  # when fixing something on Windows
```

### Comparing `git_changelog-1.0.1/src/git_changelog/providers.py` & `git_changelog-2.0.0/src/git_changelog/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module containing the parsing utilities for git providers."""
 
 from __future__ import annotations
 
 import re
 from abc import ABC, abstractmethod
-from typing import Match, Pattern
+from typing import ClassVar, Match, Pattern
 
 
 class RefRe:
     """An enum helper to store parts of regular expressions for references."""
 
     BB = r"(?:^|[\s,])"  # blank before
     BA = r"(?:[\s,]|$)"  # blank after
@@ -54,15 +54,15 @@
 
 class ProviderRefParser(ABC):
     """A base class for specific providers reference parsers."""
 
     url: str
     namespace: str
     project: str
-    REF: dict[str, RefDef] = {}
+    REF: ClassVar[dict[str, RefDef]] = {}
 
     def get_refs(self, ref_type: str, text: str) -> list[Ref]:
         """Find all references in the given text.
 
         Arguments:
             ref_type: The reference type.
             text: The text in which to search references.
@@ -134,15 +134,15 @@
     url: str = "https://github.com"
     project_url: str = "{base_url}/{namespace}/{project}"
     tag_url: str = "{base_url}/{namespace}/{project}/releases/tag/{ref}"
 
     commit_min_length = 8
     commit_max_length = 40
 
-    REF: dict[str, RefDef] = {
+    REF: ClassVar[dict[str, RefDef]] = {
         "issues": RefDef(
             regex=re.compile(RefRe.BB + RefRe.NP + "?" + RefRe.ID.format(symbol="#"), re.I),
             url_string="{base_url}/{namespace}/{project}/issues/{ref}",
         ),
         "commits": RefDef(
             regex=re.compile(
                 RefRe.BB
@@ -202,15 +202,15 @@
     url: str = "https://gitlab.com"
     project_url: str = "{base_url}/{namespace}/{project}"
     tag_url: str = "{base_url}/{namespace}/{project}/tags/{ref}"
 
     commit_min_length = 8
     commit_max_length = 40
 
-    REF: dict[str, RefDef] = {
+    REF: ClassVar[dict[str, RefDef]] = {
         "issues": RefDef(
             regex=re.compile(RefRe.BB + RefRe.NP + "?" + RefRe.ID.format(symbol="#"), re.I),
             url_string="{base_url}/{namespace}/{project}/issues/{ref}",
         ),
         "merge_requests": RefDef(
             regex=re.compile(RefRe.BB + RefRe.NP + "?" + RefRe.ID.format(symbol=r"!"), re.I),
             url_string="{base_url}/{namespace}/{project}/merge_requests/{ref}",
```

### Comparing `git_changelog-1.0.1/src/git_changelog/templates/__init__.py` & `git_changelog-2.0.0/src/git_changelog/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/src/git_changelog/templates/angular.md.jinja` & `git_changelog-2.0.0/src/git_changelog/templates/angular.md.jinja`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/src/git_changelog/templates/keepachangelog.md.jinja` & `git_changelog-2.0.0/src/git_changelog/templates/keepachangelog.md.jinja`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/tests/test_angular_style.py` & `git_changelog-2.0.0/tests/test_angular_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/tests/test_basic_style.py` & `git_changelog-2.0.0/tests/test_basic_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/tests/test_cli.py` & `git_changelog-2.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/tests/test_commit.py` & `git_changelog-2.0.0/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/tests/test_conventional_commit_style.py` & `git_changelog-2.0.0/tests/test_conventional_commit_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/tests/test_end_to_end.py` & `git_changelog-2.0.0/tests/test_end_to_end.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     for version in versions:
         for section in AngularConvention.TYPES:
             commit(section)
             commit(section)
         if version:
             git("tag", version)
     yield tmp_path
-    shutil.rmtree(tmp_path)
+    shutil.rmtree(tmp_path, ignore_errors=True)
 
 
 def test_bumping_latest(repo: Path) -> None:
     """Bump latest version.
 
     Parameters:
         repo: Path to a temporary repository.
@@ -183,7 +183,25 @@
             template="keepachangelog",
             in_place=True,
         )
 
     rendered = output.read_text()
     # The latest tag should still appear exactly three times in the changelog
     assert rendered.count(latest_tag) == 3
+
+
+def test_removing_tokens_from_remotes(repo: Path) -> None:
+    """Remove GitHub tokens from remotes.
+
+    Parameters:
+        repo: Temporary Git repository (fixture).
+    """
+    git = partial(_git, "-C", str(repo))
+    tokens = [
+        "ghp_abcdefghijklmnOPQRSTUVWXYZ0123456789",
+        "ghs_abcdefghijklmnOPQRSTUVWXYZ0123456789",
+        "github_pat_abcdefgOPQRS0123456789_abcdefghijklmnOPQRSTUVWXYZ0123456789abcdefgOPQRS0123456789A",
+    ]
+    for token in tokens:
+        git("remote", "set-url", "origin", f"https://{token}@github.com:example/example")
+        changelog = Changelog(repo)
+        assert token not in changelog.remote_url
```

### Comparing `git_changelog-1.0.1/tests/test_providers.py` & `git_changelog-2.0.0/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/tests/test_version.py` & `git_changelog-2.0.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `git_changelog-1.0.1/PKG-INFO` & `git_changelog-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: git-changelog
-Version: 1.0.1
+Version: 2.0.0
 Summary: Automatic Changelog generator using Jinja2 templates.
 Keywords: git changelog changelog-generator commit-style commit-convention
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
@@ -24,18 +23,17 @@
 Project-URL: Documentation, https://pawamoy.github.io/git-changelog
 Project-URL: Changelog, https://pawamoy.github.io/git-changelog/changelog
 Project-URL: Repository, https://github.com/pawamoy/git-changelog
 Project-URL: Issues, https://github.com/pawamoy/git-changelog/issues
 Project-URL: Discussions, https://github.com/pawamoy/git-changelog/discussions
 Project-URL: Gitter, https://gitter.im/git-changelog/community
 Project-URL: Funding, https://github.com/sponsors/pawamoy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: Jinja2<4,>=2.10
-Requires-Dist: semver~=2.13
-Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: semver>=2.13
 Description-Content-Type: text/markdown
 
 # git-changelog
 
 [![ci](https://github.com/pawamoy/git-changelog/workflows/ci/badge.svg)](https://github.com/pawamoy/git-changelog/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/git-changelog/)
 [![pypi version](https://img.shields.io/pypi/v/git-changelog.svg)](https://pypi.org/project/git-changelog/)
@@ -93,24 +91,24 @@
 With `pip`:
 ```bash
 pip install git-changelog
 ```
 
 With [`pipx`](https://github.com/pipxproject/pipx):
 ```bash
-python3.7 -m pip install --user pipx
+python3.8 -m pip install --user pipx
 pipx install git-changelog
 ```
 
 ## Usage (command-line)
 
 ```
 usage: git-changelog [-b] [-h] [-i] [-g VERSION_REGEX] [-m MARKER_LINE]
-                     [-o OUTPUT] [-R] [-c {angular,atom,conventional,basic}]
-                     [-S SECTIONS [SECTIONS ...]]
+                     [-o OUTPUT] [-r] [-R] [-I INPUT]
+                     [-c {angular,atom,conventional,basic}] [-s SECTIONS]
                      [-t {angular,keepachangelog}] [-T] [-v]
                      [REPOSITORY]
 
 Automatic Changelog generator using Jinja2 templates.
 
 This tool parses your commit messages to extract useful data
 that is then rendered using Jinja2 templates, for example to
@@ -166,54 +164,63 @@
 - ci: Continuous Integration
 - deps: Dependencies
 - doc, docs: Docs
 - style: Style
 - test, tests: Tests
 
 positional arguments:
-  REPOSITORY            The repository path, relative or absolute.
+  REPOSITORY            The repository path, relative or absolute. Default: .
 
 options:
-  -b, --bump            Guess the new latest version by bumping the previous
+  -b, --bump-latest     Guess the new latest version by bumping the previous
                         one based on the set of unreleased commits. For
                         example, if a commit contains breaking changes, bump
                         the major number (or the minor number for 0.x
                         versions). Else if there are new features, bump the
                         minor number. Else just bump the patch number.
+                        Default: False.
   -h, --help            Show this help message and exit.
   -i, --in-place        Insert new entries (versions missing from changelog)
                         in-place. An output file must be specified. With
                         custom templates, you can pass two additional
                         arguments: --version-regex and --marker-line. When
                         writing in-place, an 'in_place' variable will be
                         injected in the Jinja context, allowing to adapt the
                         generated contents (for example to skip changelog
-                        headers or footers).
+                        headers or footers). Default: False.
   -g, --version-regex VERSION_REGEX
                         A regular expression to match versions in the existing
                         changelog (used to find the latest release) when
                         writing in-place. The regular expression must be a
-                        Python regex with a 'version' named group.
+                        Python regex with a 'version' named group. Default:
+                        ^## \[(?P<version>v?[^\]]+).
   -m, --marker-line MARKER_LINE
                         A marker line at which to insert new entries (versions
                         missing from changelog). If two marker lines are
                         present in the changelog, the contents between those
                         two lines will be overwritten (useful to update an
-                        'Unreleased' entry for example).
-  -o OUTPUT, --output OUTPUT
-                        Output to given file. Default: stdout.
-  -r, --parse-refs      Parse provider-specific references in commit
-                        messages (GitHub/GitLab issues, PRs, etc.).
-  -c, -s, --style, --commit-style,  --convention {angular,atom,conventional,basic}
-                        The commit convention to match against. Default: basic.
-  -S, --sections SECTIONS [SECTIONS ...]
-                        The sections to render. See the available sections for
-                        each supported convention in the description.
-  -t, --template {angular,keepachangelog}
+                        'Unreleased' entry for example). Default: <!--
+                        insertion marker -->.
+  -o, --output OUTPUT   Output to given file. Default: stdout.
+  -r, --parse-refs      Parse provider-specific references in commit messages
+                        (GitHub/GitLab issues, PRs, etc.). Default: False.
+  -R, --release-notes   Output release notes to stdout based on the last entry
+                        in the changelog. Default: False.
+  -I, --input INPUT     Read from given file when creating release notes.
+                        Default: CHANGELOG.md.
+  -c, --style, --commit-style, --convention {angular,atom,conventional,basic}
+                        The commit convention to match against. Default:
+                        basic.
+  -s, --sections SECTIONS
+                        A comma-separated list of sections to render. See the
+                        available sections for each supported convention in
+                        the description. Default: None.
+  -t {angular,keepachangelog}, --template {angular,keepachangelog}
                         The Jinja2 template to use. Prefix with "path:" to
                         specify the path to a directory containing a file
-                        named "changelog.md".
+                        named "changelog.md". Default: keepachangelog.
   -T, --trailers, --git-trailers
                         Parse Git trailers in the commit message. See
                         https://git-scm.com/docs/git-interpret-trailers.
+                        Default: False.
   -v, --version         Show the current version of the program and exit.
 ```
```

