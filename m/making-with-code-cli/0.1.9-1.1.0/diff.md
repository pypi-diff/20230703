# Comparing `tmp/making-with-code-cli-0.1.9.tar.gz` & `tmp/making_with_code_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "making-with-code-cli-0.1.9.tar", max compression
+gzip compressed data, was "making_with_code_cli-1.1.0.tar", max compression
```

## Comparing `making-with-code-cli-0.1.9.tar` & `making_with_code_cli-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1342 2022-01-28 16:04:53.371574 making-with-code-cli-0.1.9/README.md
--rw-r--r--   0        0        0     6353 2023-02-08 18:49:16.807000 making-with-code-cli-0.1.9/making_with_code_cli/cli.py
--rw-r--r--   0        0        0    15649 2023-02-08 18:48:40.038349 making-with-code-cli-0.1.9/making_with_code_cli/cli_setup.py
--rw-r--r--   0        0        0      255 2022-01-26 22:46:15.444811 making-with-code-cli-0.1.9/making_with_code_cli/curriculum.py
--rw-r--r--   0        0        0      213 2022-08-22 21:39:48.144079 making-with-code-cli-0.1.9/making_with_code_cli/git_backend/__init__.py
--rw-r--r--   0        0        0     2674 2022-02-18 18:05:17.002213 making-with-code-cli-0.1.9/making_with_code_cli/git_backend/base_backend.py
--rw-r--r--   0        0        0     3834 2022-04-13 23:45:49.390638 making-with-code-cli-0.1.9/making_with_code_cli/git_backend/github_backend.py
--rw-r--r--   0        0        0     4218 2022-08-22 21:54:54.411188 making-with-code-cli-0.1.9/making_with_code_cli/git_backend/github_org_backend.py
--rw-r--r--   0        0        0      266 2022-01-28 14:38:32.561937 making-with-code-cli-0.1.9/making_with_code_cli/helpers.py
--rw-r--r--   0        0        0     2285 2022-01-25 20:02:26.726590 making-with-code-cli-0.1.9/making_with_code_cli/mwc_api.py
--rw-r--r--   0        0        0     1629 2022-09-13 14:24:43.726870 making-with-code-cli-0.1.9/making_with_code_cli/settings.py
--rw-r--r--   0        0        0     1682 2023-02-08 18:47:05.565571 making-with-code-cli-0.1.9/making_with_code_cli/styles.py
--rw-r--r--   0        0        0      662 2023-02-08 18:49:24.423489 making-with-code-cli-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2286 2023-02-08 18:49:27.422459 making-with-code-cli-0.1.9/setup.py
--rw-r--r--   0        0        0     2094 2023-02-08 18:49:27.422792 making-with-code-cli-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.1.0/README.md
+-rw-r--r--   0        0        0     6410 2023-07-03 00:30:08.092007 making_with_code_cli-1.1.0/making_with_code_cli/cli.py
+-rw-r--r--   0        0        0    14782 2023-07-03 01:17:43.683351 making_with_code_cli-1.1.0/making_with_code_cli/cli_setup.py
+-rw-r--r--   0        0        0      530 2023-07-02 19:59:44.714590 making_with_code_cli-1.1.0/making_with_code_cli/curriculum.py
+-rw-r--r--   0        0        0      277 2023-07-02 20:00:38.095929 making_with_code_cli-1.1.0/making_with_code_cli/errors.py
+-rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.1.0/making_with_code_cli/git_backend/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.1.0/making_with_code_cli/git_backend/base_backend.py
+-rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.1.0/making_with_code_cli/git_backend/github_backend.py
+-rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.1.0/making_with_code_cli/git_backend/github_org_backend.py
+-rw-r--r--   0        0        0     2470 2023-06-05 21:06:58.811653 making_with_code_cli-1.1.0/making_with_code_cli/git_backend/mwc_backend.py
+-rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.1.0/making_with_code_cli/helpers.py
+-rw-r--r--   0        0        0     2285 2023-05-30 14:14:06.615841 making_with_code_cli-1.1.0/making_with_code_cli/mwc_api.py
+-rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.1.0/making_with_code_cli/settings.py
+-rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.1.0/making_with_code_cli/styles.py
+-rw-r--r--   0        0        0      663 2023-07-03 01:21:16.549208 making_with_code_cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.1.0/PKG-INFO
```

### Comparing `making-with-code-cli-0.1.9/README.md` & `making_with_code_cli-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `making-with-code-cli-0.1.9/making_with_code_cli/cli.py` & `making_with_code_cli-1.1.0/making_with_code_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     iter_settings,
     write_settings,
 )
 from making_with_code_cli.cli_setup import (
     INTRO_MESSAGE,
     INTRO_NOTES,
     WORK_DIR_PERMISSIONS,
+    Platform,
     choose_mwc_username,
     choose_work_dir,
     choose_mwc_site_url,
     choose_course,
     choose_editor,
     MWCShellConfig,
     InstallCurl,
@@ -40,15 +41,14 @@
     InstallPoetry,
     InstallGit,
     InstallTree,
     InstallVSCode,
     InstallImageMagick,
     InstallHttpie,
     InstallScipy,
-    GHAuthentication,
     GitConfiguration,
 )
 from making_with_code_cli.curriculum import (
     get_curriculum,
 )
 from making_with_code_cli.git_backend import (
     get_backend,
@@ -87,15 +87,16 @@
     settings['mwc_site_url'] = choose_mwc_site_url(settings.get('mwc_site_url'))
     curriculum = get_curriculum(settings)
     settings['course'] = choose_course(
         [course['name'] for course in curriculum['courses']], 
         default=settings.get('course')
     )
     course = [c for c in curriculum['courses'] if c['name'] == settings['course']][0]
-    settings['editor'] = choose_editor(settings.get('editor', 'atom'))
+    if Platform.detect() & (Platform.MAC | Platform.UBUNTU):
+        settings['editor'] = choose_editor(settings.get('editor', 'atom'))
     G = get_backend(course['git_backend'])
     settings = G.extend_settings(settings)
     if yes:
         click.echo(info("Updated settings:"))
         click.echo(info(yaml.dump(settings), preformatted=True))
     else:
         click.echo(info(yaml.dump(settings), preformatted=True))
```

### Comparing `making-with-code-cli-0.1.9/making_with_code_cli/cli_setup.py` & `making_with_code_cli-1.1.0/making_with_code_cli/cli_setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from pathlib import Path
 from enum import Flag, auto
 from stat import *
 import sys
+import os
+import platform
 from making_with_code_cli.styles import (
     address,
     question,
     confirm,
     info,
     success,
     warn,
     error,
 )
+from making_with_code_cli.errors import (
+    CurriculumSiteNotAvailable,
+    NoCurriculaAvailable,
+)
 import click
 import requests
 from subprocess import run
 import yaml
 
 INTRO_MESSAGE = (
     "Welcome to Making with Code setup. This program will ask you for some settings "
@@ -29,27 +35,30 @@
     "The setup may ask for your password. As a security measure, you won't see any characters when you type it in.",
     "If you get stuck or have any questions, ask a teacher.",
 ]
 WORK_DIR_PERMISSIONS = S_IRWXU | S_IXGRP | S_IXOTH
 
 class Platform(Flag):
     MAC = auto()
-    DEBIAN = auto()
-    WSL = auto()
-    SUPPORTED = MAC | DEBIAN | WSL
+    UBUNTU = auto()
+    REPLIT = auto()
+    SUPPORTED = MAC | UBUNTU | REPLIT
     UNSUPPORTED = 0
 
     @classmethod
     def detect(self):
-        if Path("/proc/version").exists() and "WSL" in Path("/proc/version").read_text():
-            return self.WSL
-        if sys.platform.startswith("darwin"):
+        if os.environ.get('REPL_ID'):
+            return self.REPLIT
+        system_name = platform.system()
+        if system_name == "Darwin":
             return self.MAC
-        if sys.platform.startswith("linux") and Path("/etc/debian_version").exists():
-            return self.DEBIAN
+        if system_name == "Linux" and platform.freedesktop_os_release().get('NAME'):
+            release_name = (platform.freedesktop_os_release() or {}).get('NAME')
+            if release_name == "Ubuntu":
+                return self.UBUNTU
         return self.UNSUPPORTED
 
 def default_work_dir():
     if (Path.home() / "Desktop").exists():
         return Path.home() / "Desktop" / "making_with_code"
     else:
         return Path.home() / "making_with_code"
@@ -88,31 +97,26 @@
         url = click.prompt(
             question("What's the URL of your Making With Code website?"),
             default=default,
         )
         if url.endswith('/'):
             url = url[:-1]
         try:
-            if not requests.get(url).ok:
-                click.echo(error("Hmm, couldn't reach that site..."))
-            else:
-                if not requests.get(url + "/index.json"):
-                    click.echo(error("Found the site, but it's not responding properly. " + 
-                            "Please ask your teacher for help."))
-                else:
-                    return url
+            curriculum = get_curriculum({'mwc_site_url': url})
+        except CurriculumSiteNotAvailable as err:
+            click.echo(error(str(err)))
         except requests.exceptions.MissingSchema as e:
             click.echo(error(str(e)))
 
 def choose_course(options, default=None):
     """Asks the user which course they are part of"""
     if len(options) == 0:
         err = "There is a problem with the MWC site. Please ask a teacher for help."
-        error(err)
-        raise ValueError(err)
+        click.echo(error(err))
+        raise NoCurriculaAvailable(err)
     elif len(options) == 1:
         if default and default not in options:
             confirm(f"Changing your course from '{default}' to '{options[0]}'")
         else:
             confirm(f"You are part of the course '{options[0]}'.")
         return options[0]
     else:
@@ -210,14 +214,15 @@
         for sh, rc in candidates:
             if shell == sh and rc.exists():
                 return rc
         raise IOError("Can't find an rc file.")
 
 class InstallHomebrew(SetupTask):
     description = "Install homebrew"
+    platform = Platform.MAC
 
     def is_complete(self):
         return self.executable_on_path("brew")
 
     def run_task(self):
         click.echo(address("Installing homebrew... (this may take a while)"))
         cmd = '/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"'
@@ -281,27 +286,21 @@
         f += "## Add Poetry to $PATH\n"
         f += 'export PATH="$HOME/.local/bin:$PATH"\n\n'
         if Platform.detect() == Platform.MAC:
             if self.settings['editor'] == "subl":
                 f += "## Add subl to $PATH\n"
                 subldir = "/Applications/Sublime Text.app/Contents/SharedSupport/bin"
                 f += f'export PATH="{subldir}:$PATH"\n\n'
-        if Platform.detect() == Platform.WSL:
-            if self.settings['editor'] == "subl":
-                f += "## Create subl alias for Sublime Text\n"
-                f += 'alias subl=\'"/mnt/c/Program Files/Sublime Text 3/subl.exe"\''
-            if self.settings['editor'] == "atom":
-                f += "## Create atom alias\n"
-                f += 'alias atom=”/mnt/c/Windows/System32/cmd.exe /c \'atom\'"\n\n'
         return f
 
 class InstallPackage(SetupTask):
     package_name = "package"
     brew_name = "package"
     apt_name = "package"
+    nix_name = "package"
     cask = False
 
     def __init__(self, *args, **kwargs):
         self.description = f"Install {self.package_name}"
         super().__init__(*args, **kwargs)
 
     def is_complete(self):
@@ -311,86 +310,69 @@
         platform = Platform.detect()
         click.echo(address(f"Installing {self.package_name}..."))
         if platform & Platform.MAC:
             if self.cask:
                 run(f"brew install {self.brew_name}", shell=True, check=True)
             else:
                 run(f"brew install --cask {self.brew_name}", shell=True, check=True)
-        elif platform & (Platform.DEBIAN | Platform.WSL):
-            run(f"apt install {pkg}", shell=True, check=True)
+        elif platform & Platform.UBUNTU:
+            run(f"apt install {self.apt_name}", shell=True, check=True)
+        elif platform & Platform.REPLIT:
+            run(f"nix-env -iA nixpkgs.{self.nix_name}", shell=True, check=True)
         else:
             raise IOError(f"Platform {platform} not supported...")
 
 class InstallCurl(InstallPackage):
+    platform = Platform.UBUNTU
     package_name = brew_name = apt_name = "curl"
 
 class InstallPython3(InstallPackage):
+    platform = Platform.MAC | Platform.UBUNTU
     package_name = brew_name = apt_name = "python3"
 
 class InstallGit(InstallPackage):
+    platform = Platform.MAC | Platform.UBUNTU
     package_name = brew_name = apt_name = "git"
 
 class InstallTree(InstallPackage):
-    package_name = brew_name = apt_name = "tree"
-
-class InstallAtom(InstallPackage):
-    platform = Platform.MAC
-    package_name = brew_name = apt_name = "atom"
+    package_name = brew_name = apt_name = nix_name = "tree"
 
 class InstallVSCode(InstallPackage):
-    platform = Platform.MAC
-    package_name = brew_name = "visual-studio-code"
+    platform = Platform.MAC | Platform.UBUNTU
+    package_name = "code"
+    brew_name = "visual-studio-code"
     cask = True
 
-class InstallGh(InstallPackage):
-    package_name = brew_name = "gh"
-
-    def package_installer(self):
-        return "brew"
+    def run_task(self):
+        platform = Platform.detect()
+        if platform & Platform.UBUNTU:
+            run("sudo snap install --classic code", shell=True, check=True)
+        else:
+            return super().run_task()
 
 class InstallImageMagick(InstallPackage):
-    package_name = brew_name = apt_name = "imagemagick"
-
-    def is_complete(self):
-        return self.executable_on_path("magick")
+    package_name = "magick"
+    brew_name = apt_name = nix_name = "imagemagick"
 
 class InstallHttpie(InstallPackage):
-    package_name = brew_name = apt_name = "httpie"
+    package_name = "http"
+    brew_name = apt_name = nix_name = "httpie"
 
 class InstallScipy(InstallPackage):
     package_name = brew_name = apt_name = "scipy"
 
     def is_complete(self):
         return True
         try:
             import scipy
             return True
         except ModuleNotFoundError as e:
             print(e)
             return False
 
-class GHAuthentication(SetupTask):
-    description = "Sign in to github"
-    gh_auth_file = Path.home() / ".config/gh/hosts.yml"
-
-    def is_complete(self):
-        return "github.com" in self.gh_auth_data()
-
-    def run_task(self):
-        click.echo(address("You will now be prompted to log in to github.com (or to create an account)."))
-        click.echo(address(" - Choose 'GitHub.com' when asked which account you want to log into."))
-        click.echo(address(" - Choose 'HTTPS' when asked which protocol to use"))
-        run("gh auth login", shell=True, check=True)
-
-    def gh_auth_data(self):
-        if self.gh_auth_file.exists():
-            return yaml.safe_load(self.gh_auth_file.read_text())
-        else:
-            return {}
-
 class GitConfiguration(SetupTask):
     """Configure global git settings.
     Can be skipped by setting `skip_git_config: true` in settings.
     """
     description = "Configure git"
 
     editorcmds = {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `making-with-code-cli-0.1.9/making_with_code_cli/git_backend/base_backend.py` & `making_with_code_cli-1.1.0/making_with_code_cli/git_backend/base_backend.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,49 +10,24 @@
 )
 
 class GitBackend:
     """Base class interface to backend git server.
     All Making With Code deployments are backed by a git server, but the nature of the
     server and the strategies for completing tasks vary by backend. 
     """
-    INIT_ACTIONS = [
-        'create_from_template',
-        'clone',
-        'mkdir'
-    ]
 
     @classmethod
     def extend_settings(self, settings):
         "A hook for git backends to collect additional information from the user"
         return settings
 
     def __init__(self, settings):
         self.settings = settings
 
     def init_module(self, module, modpath):
-        if not 'init_action' in module:
-            raise ValueError(f"There is a problem with the website. Can't initialize module {module['slug']} " + 
-                    "without an init action.")
-        if not module['init_action'] in self.INIT_ACTIONS:
-            raise ValueError(f"There is a problem with the website. Can't initialize module {module['slug']} " + 
-                    f"with init action '{module['init_action']}'.")
-        if module['init_action'] == "mkdir":
-            self.init_mkdir(module, modpath)
-        if module['init_action'] == "clone":
-            self.init_clone(module, modpath)
-        if module['init_action'] == "create_from_template":
-            self.init_create_from_template(module, modpath)
-
-    def init_mkdir(self, module, modpath):
-        modpath.mkdir(mode=WORK_DIR_PERMISSIONS)
-
-    def init_clone(self, module, modpath):
-        raise NotImplemented()
-
-    def init_create_from_template(self, module, modpath):
         raise NotImplemented()
 
     def update(self, module, modpath):
         if (modpath / ".git").is_dir():
             with cd(modpath):
                 relpath = self.relative_path(modpath)
                 try:
```

### Comparing `making-with-code-cli-0.1.9/making_with_code_cli/git_backend/github_backend.py` & `making_with_code_cli-1.1.0/making_with_code_cli/git_backend/github_org_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,82 +7,79 @@
 from making_with_code_cli.helpers import cd
 from making_with_code_cli.styles import (
     confirm,
 )
 
 COMMIT_TEMPLATE = ".commit_template"
 
-class GithubBackend(GitBackend):
-    """A Github backend. Students own their own repos and grant teachers access via token.
-    Note that this gives the teacher account access to the student's entire github account, 
-    within scope.
+class GithubOrgBackend(GitBackend):
+    """A Github backend which uses github organizations.  
+    Students own their own repos but create them from within the organization.
     """
 
     @classmethod
     def extend_settings(self, settings):
         "Asks for the user's github username and email address"
         def choose_github_username(github_username):
             msg = "What is your GitHub username? "
             return click.prompt(msg, default=github_username)
+        def choose_github_org(github_org):
+            msg = "What is the name of the course's GitHub organization? "
+            return click.prompt(msg, default=github_org)
         def choose_github_email(github_email):
             msg = "What is the email address associated with your GitHub account? "
             return click.prompt(msg, default=github_email)
         def choose_git_name(git_name):
             msg = "What name do you want to use in your git commits? "
             return click.prompt(msg, default=git_name)
         if settings.get('github_username') or click.confirm("Do you have a GitHub account?"):
             settings['github_username'] = choose_github_username(settings.get("github_username"))
+            settings['github_org'] = choose_github_org(settings.get("github_org"))
             settings['github_email'] = choose_github_email(settings.get("github_email"))
             settings['git_name'] = choose_git_name(settings.get("git_name"))
         return settings
 
-    def init_clone(self, module, modpath):
-        url = module["repo_url"]
-        cmd = f'gh repo clone "{url}" "{modpath.name}"'
-        with cd(modpath.parent):
-            run(cmd, shell=True, check=True)
-        if (modpath / COMMIT_TEMPLATE).exists():
-            with cd(modpath):
-                run(f"git config commit.template {COMMIT_TEMPLATE}")
-
-    def init_create_from_template(self, module, modpath):
+    def init_module(self, module, modpath):
         """Creates the named repo from a template, or clones an existing repo with. 
         """
         repo_name = self.get_repo_name_from_template_repo_url(module["repo_url"])
         url = module["repo_url"]
 
         if self.user_has_repo(repo_name):
             cmd = f'gh repo clone "{url}" "{modpath.name}"'
         else:
             if modpath.exists():
                 self.relocate_existing_directory(modpath)
-            cmd = f'gh repo create {repo_name} --clone --private --template "{url}"'
+            usr = self.settings['username']
+            org = self.settings['github_org']
+            cmd = f'gh repo create "{org}/{repo_name}" --clone --private --template "{url}"'
         with cd(modpath.parent):
             run(cmd, shell=True, check=True)
             run(f"mv {repo_name} {modpath.name}", shell=True, check=True) 
         if (modpath / COMMIT_TEMPLATE).exists():
             with cd(modpath):
                 run(f"git config commit.template {COMMIT_TEMPLATE}")
 
     def get_repo_name_from_template_repo_url(self, url):
         """Parses the template repo URL and returns the name of a repo to create.
         Expects a GitHub url like "https://github.com/cproctor/mwc-pedprog-unit00-project-drawing.git"
         """
         parts = url.split('/')
         name, suffix = parts[-1][:-4], parts[-1][-4:]
-        return name
+        return name + '-' + self.settings['github_username']
 
     def relocate_existing_directory(self, path):
         """Moves an existing directory out of the way.
         """
         new_path = path.parent / path.name + '_old'
         while new_path.exists():
             new_path = new_path.parent / new_path.name + '_old'
         click.echo(confirm(f"Moving existing directory {path} to {new_path}."))
         os.rename(path, new_path)
 
     def user_has_repo(self, name):
         "Checks to see whether the user already has the named repo."
-        cmd = f"gh repo list --json name --limit 10000"
+        org = self.settings['github_org']
+        cmd = f"gh repo list {org} --json name --limit 10000"
         result = run(cmd, shell=True, capture_output=True, text=True).stdout
         repo_names = [obj['name'] for obj in json.loads(result)]
         return name in repo_names
```

### Comparing `making-with-code-cli-0.1.9/making_with_code_cli/mwc_api.py` & `making_with_code_cli-1.1.0/making_with_code_cli/mwc_api.py`

 * *Files identical despite different names*

### Comparing `making-with-code-cli-0.1.9/making_with_code_cli/settings.py` & `making_with_code_cli-1.1.0/making_with_code_cli/settings.py`

 * *Files identical despite different names*

### Comparing `making-with-code-cli-0.1.9/making_with_code_cli/styles.py` & `making_with_code_cli-1.1.0/making_with_code_cli/styles.py`

 * *Files identical despite different names*

### Comparing `making-with-code-cli-0.1.9/pyproject.toml` & `making_with_code_cli-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "making-with-code-cli"
-version = "0.1.9"
+version = "1.1.0"
 description = "Courseware for Making With Code"
 authors = ["Chris Proctor <chris@chrisproctor.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cproctor/making-with-code-courseware"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 PyYAML = "^6.0"
 click = "^8.0.3"
 requests = "^2.27.1"
 toml = "^0.10.2"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `making-with-code-cli-0.1.9/PKG-INFO` & `making_with_code_cli-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: making-with-code-cli
-Version: 0.1.9
+Version: 1.1.0
 Summary: Courseware for Making With Code
 Home-page: https://github.com/cproctor/making-with-code-courseware
 License: MIT
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: issues, https://github.com/cproctor/making-with-code-courseware/issues
 Description-Content-Type: text/markdown
```

