# Comparing `tmp/gitlab-runner-tart-driver-0.1.7.tar.gz` & `tmp/gitlab-runner-tart-driver-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-runner-tart-driver-0.1.7.tar", last modified: Mon Jun 26 18:01:57 2023, max compression
+gzip compressed data, was "gitlab-runner-tart-driver-0.2.0.tar", last modified: Mon Jul  3 12:51:24 2023, max compression
```

## Comparing `gitlab-runner-tart-driver-0.1.7.tar` & `gitlab-runner-tart-driver-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:01:57.900614 gitlab-runner-tart-driver-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     3303 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    18448 2023-06-26 18:01:57.900614 gitlab-runner-tart-driver-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    17927 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:01:57.897614 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:01:57.899614 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/commands/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/commands/config.py
--rw-rw-rw-   0 root         (0) root         (0)    11270 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/commands/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     2654 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/commands/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:01:57.899614 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8703 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/modules/tart.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/modules/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:01:57.900614 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2533 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:01:57.898614 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18448 2023-06-26 18:01:57.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2023-06-26 18:01:57.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 18:01:57.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-26 18:01:57.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 18:01:57.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-26 18:01:57.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-26 18:01:57.000000 gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 18:01:57.900614 gitlab-runner-tart-driver-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-06-26 18:01:50.000000 gitlab-runner-tart-driver-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.679694 gitlab-runner-tart-driver-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    20528 2023-07-03 12:51:24.679694 gitlab-runner-tart-driver-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    20007 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.675694 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.678694 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10415 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.678694 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8937 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/tart.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.679694 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2533 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.677694 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20528 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 12:51:24.679694 gitlab-runner-tart-driver-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/setup.py
```

### Comparing `gitlab-runner-tart-driver-0.1.7/LICENSE.txt` & `gitlab-runner-tart-driver-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.7/PKG-INFO` & `gitlab-runner-tart-driver-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.7
+Version: 0.2.0
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 # Gitlab Runner Custom Tart Driver
 
 - [Gitlab Runner Custom Tart Driver](#gitlab-runner-custom-tart-driver)
   - [About](#about)
   - [Setup](#setup)
     - [GitLab Runner Configuration](#gitlab-runner-configuration)
   - [GitLab CI](#gitlab-ci)
+    - [Supported Environment Variables](#supported-environment-variables)
     - [Private OCI Registries](#private-oci-registries)
     - [Configuring the SSH Credentials](#configuring-the-ssh-credentials)
   - [Advanced Configuration](#advanced-configuration)
     - [GitLab Runner Installation](#gitlab-runner-installation)
     - [Concurrency](#concurrency)
     - [Host Cache and Builds directories](#host-cache-and-builds-directories)
     - [Volume Mounts](#volume-mounts)
@@ -173,14 +174,32 @@
   script:
     - echo "This is brought to you by tart" >> artifact.txt
   artifacts:
     paths:
       - artifact.txt
 ```
 
+### Supported Environment Variables
+
+| **Name**                              | **Default**    | **Description**                                                                                               |
+| ------------------------------------- | -------------- | ------------------------------------------------------------------------------------------------------------- |
+| `TART_REGISTRY_USERNAME`              |                | Username to login to private OCI registry                                                                     |
+| `TART_REGISTRY_PASSWORD`              |                | Password to login to private OCI registry                                                                     |
+| `TART_REGISTRY`                       |                | Private OCI registry                                                                                          |
+| `TART_PULL_POLICY`                    | if-not-present | define how runners pull tart images from registries. Options are `always`,`if-not-present`,`never`            |
+| `TART_SSH_USERNAME`                   | admin          | Username to use to login to VM                                                                                |
+| `TART_SSH_PASSWORD`                   | admin          | Password to use to login to VM                                                                                |
+| `TART_EXECUTOR_HEADLESS`              | true           | Don't open a UI window.                                                                                       |
+| `TART_EXECUTOR_SOFTNET_ENABLED`       | false          | Use software networking instead of the default shared (NAT) networking                                        |
+| `TART_EXECUTOR_VNC_ENABLED`           | false          | Use screen sharing instead of the built-in UI. Note that Remote Login option should be enabled inside the VM. |
+| `TART_EXECUTOR_INSTALL_GITLAB_RUNNER` | false          | Install a GitLabRunner into the VM to ensure full CI/CD functionality                                         |
+| `TART_EXECUTOR_SHELL`                 | /bin/zsh       | The shell that should be used when running commands                                                           |
+| `TART_EXECUTOR_TIMEOUT`               | 60             | Timeout for `tart ip` to respond with a valid IP                                                              |
+| `TART_EXECUTOR_DISPLAY`               | 1920x1200      | Display resolution in format `WxH`                                                                            |
+
 ### Private OCI Registries
 
 Oftentimes you might want to provide your own OCI-compliant images created with [Packer](https://www.packer.io) and the official [Tart Builder](https://developer.hashicorp.com/packer/plugins/builders/tart). If you push your images to a private registry you will need to provide the credentials for the `gitlab-runner-tart-driver` to login there first.
 
 You can provide a default login registry using the `CLI` parameters (see **Command `prepare`**) but also provide the credentials from with each job variable definition
 
 ```yaml
@@ -342,17 +361,15 @@
 
 You can use a custom shell to execute your commands. The default ist `/bin/zsh`
 
 see **Command `run`**
 
 ### Custom `pull_policy`
 
-You can use a custom `pull_policy`. The default policy is `if-not-present`
-
-see **Command `prepare`**
+You can use a custom `pull_policy`. The default policy is `if-not-present`. Use `TART_PULL_POLICY` to override the default pull policy
 
 ## CLI
 
 ### CLI Parameters for `config.toml`
 
 The `gitlab-runner-tart-driver` gives a number of advanced configuration options. Use `gitlab-runner-tart-driver [stage] --help` to get a full list of options that you can pass to the exectuable using your `config.toml` file.
 
@@ -387,22 +404,14 @@
 
 ```
 Usage: gitlab-runner-tart-driver prepare [OPTIONS]
 
   Prepare the environment and start the tart VM.
 
 Options:
-  --default-ssh-username TEXT     username to login to a tart vm
-  --default-ssh-password TEXT     password to login to a tart vm
-  --pull-policy [always|if-not-present|never]
-                                  define how runners pull tart images from
-                                  registries
-  --registry-username TEXT        username to login to a oci registry
-  --registry-password TEXT        password to login to a oci registry
-  --registry TEXT                 username to login to a oci registry
   --cpu INTEGER                   Number of CPUs associated to VM
   --memory INTEGER                VM memory size in megabytes associated to VM
   --display TEXT                  VM display resolution in a format of
                                   <width>x<height>. For example, 1200x800
   --auto-resources / --no-auto-resources
                                   If enabled, the driver will divide system
                                   resources equally to the concurrent VMs.
@@ -430,16 +439,14 @@
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
   Run commands.
 
 Options:
-  --default-ssh-username TEXT  username to login to a tart vm
-  --default-ssh-password TEXT  password to login to a tart vm
   --timeout INTEGER            SSH connection timeout in seconds
   -x, --tart-executable TEXT   Path to the tart executable.
   --shell TEXT                 Path to the shell to be used for commands over
                                ssh.
   --help                       Show this message and exit.
 ```
```

### Comparing `gitlab-runner-tart-driver-0.1.7/README.md` & `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,30 @@
+Metadata-Version: 2.1
+Name: gitlab-runner-tart-driver
+Version: 0.2.0
+Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
+Author: Matthias Schmieder
+Author-email: schmieder.matthias@gmail.com
+License: BSD
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Version Control
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Gitlab Runner Custom Tart Driver
 
 - [Gitlab Runner Custom Tart Driver](#gitlab-runner-custom-tart-driver)
   - [About](#about)
   - [Setup](#setup)
     - [GitLab Runner Configuration](#gitlab-runner-configuration)
   - [GitLab CI](#gitlab-ci)
+    - [Supported Environment Variables](#supported-environment-variables)
     - [Private OCI Registries](#private-oci-registries)
     - [Configuring the SSH Credentials](#configuring-the-ssh-credentials)
   - [Advanced Configuration](#advanced-configuration)
     - [GitLab Runner Installation](#gitlab-runner-installation)
     - [Concurrency](#concurrency)
     - [Host Cache and Builds directories](#host-cache-and-builds-directories)
     - [Volume Mounts](#volume-mounts)
@@ -158,14 +174,32 @@
   script:
     - echo "This is brought to you by tart" >> artifact.txt
   artifacts:
     paths:
       - artifact.txt
 ```
 
+### Supported Environment Variables
+
+| **Name**                              | **Default**    | **Description**                                                                                               |
+| ------------------------------------- | -------------- | ------------------------------------------------------------------------------------------------------------- |
+| `TART_REGISTRY_USERNAME`              |                | Username to login to private OCI registry                                                                     |
+| `TART_REGISTRY_PASSWORD`              |                | Password to login to private OCI registry                                                                     |
+| `TART_REGISTRY`                       |                | Private OCI registry                                                                                          |
+| `TART_PULL_POLICY`                    | if-not-present | define how runners pull tart images from registries. Options are `always`,`if-not-present`,`never`            |
+| `TART_SSH_USERNAME`                   | admin          | Username to use to login to VM                                                                                |
+| `TART_SSH_PASSWORD`                   | admin          | Password to use to login to VM                                                                                |
+| `TART_EXECUTOR_HEADLESS`              | true           | Don't open a UI window.                                                                                       |
+| `TART_EXECUTOR_SOFTNET_ENABLED`       | false          | Use software networking instead of the default shared (NAT) networking                                        |
+| `TART_EXECUTOR_VNC_ENABLED`           | false          | Use screen sharing instead of the built-in UI. Note that Remote Login option should be enabled inside the VM. |
+| `TART_EXECUTOR_INSTALL_GITLAB_RUNNER` | false          | Install a GitLabRunner into the VM to ensure full CI/CD functionality                                         |
+| `TART_EXECUTOR_SHELL`                 | /bin/zsh       | The shell that should be used when running commands                                                           |
+| `TART_EXECUTOR_TIMEOUT`               | 60             | Timeout for `tart ip` to respond with a valid IP                                                              |
+| `TART_EXECUTOR_DISPLAY`               | 1920x1200      | Display resolution in format `WxH`                                                                            |
+
 ### Private OCI Registries
 
 Oftentimes you might want to provide your own OCI-compliant images created with [Packer](https://www.packer.io) and the official [Tart Builder](https://developer.hashicorp.com/packer/plugins/builders/tart). If you push your images to a private registry you will need to provide the credentials for the `gitlab-runner-tart-driver` to login there first.
 
 You can provide a default login registry using the `CLI` parameters (see **Command `prepare`**) but also provide the credentials from with each job variable definition
 
 ```yaml
@@ -327,17 +361,15 @@
 
 You can use a custom shell to execute your commands. The default ist `/bin/zsh`
 
 see **Command `run`**
 
 ### Custom `pull_policy`
 
-You can use a custom `pull_policy`. The default policy is `if-not-present`
-
-see **Command `prepare`**
+You can use a custom `pull_policy`. The default policy is `if-not-present`. Use `TART_PULL_POLICY` to override the default pull policy
 
 ## CLI
 
 ### CLI Parameters for `config.toml`
 
 The `gitlab-runner-tart-driver` gives a number of advanced configuration options. Use `gitlab-runner-tart-driver [stage] --help` to get a full list of options that you can pass to the exectuable using your `config.toml` file.
 
@@ -372,22 +404,14 @@
 
 ```
 Usage: gitlab-runner-tart-driver prepare [OPTIONS]
 
   Prepare the environment and start the tart VM.
 
 Options:
-  --default-ssh-username TEXT     username to login to a tart vm
-  --default-ssh-password TEXT     password to login to a tart vm
-  --pull-policy [always|if-not-present|never]
-                                  define how runners pull tart images from
-                                  registries
-  --registry-username TEXT        username to login to a oci registry
-  --registry-password TEXT        password to login to a oci registry
-  --registry TEXT                 username to login to a oci registry
   --cpu INTEGER                   Number of CPUs associated to VM
   --memory INTEGER                VM memory size in megabytes associated to VM
   --display TEXT                  VM display resolution in a format of
                                   <width>x<height>. For example, 1200x800
   --auto-resources / --no-auto-resources
                                   If enabled, the driver will divide system
                                   resources equally to the concurrent VMs.
@@ -415,16 +439,14 @@
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
   Run commands.
 
 Options:
-  --default-ssh-username TEXT  username to login to a tart vm
-  --default-ssh-password TEXT  password to login to a tart vm
   --timeout INTEGER            SSH connection timeout in seconds
   -x, --tart-executable TEXT   Path to the tart executable.
   --shell TEXT                 Path to the shell to be used for commands over
                                ssh.
   --help                       Show this message and exit.
 ```
 
@@ -434,8 +456,8 @@
 Usage: gitlab-runner-tart-driver cleanup [OPTIONS]
 
   Command to greet a user.
 
 Options:
   -x, --tart-executable TEXT  Path to the tart executable.
   --help                      Show this message and exit.
-```
+```
```

### Comparing `gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/cli.py` & `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/commands/cleanup.py` & `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/commands/config.py` & `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/commands/prepare.py` & `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/prepare.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,14 @@
 from gitlab_runner_tart_driver.modules.tart import Tart
 from gitlab_runner_tart_driver.modules.tart import TartVolume
 from gitlab_runner_tart_driver.modules.utils import get_host_spec
 from gitlab_runner_tart_driver.modules.utils import print_host_spec
 
 
 @click.command()
-@click.option(
-    "--default-ssh-username", default="admin", required=False, type=str, help="username to login to a tart vm"
-)
-@click.option(
-    "--default-ssh-password", default="admin", required=False, type=str, help="password to login to a tart vm"
-)
-@click.option(
-    "--pull-policy",
-    default="if-not-present",
-    type=click.Choice(["always", "if-not-present", "never"]),
-    help="define how runners pull tart images from registries",
-)
-@click.option("--registry-username", required=False, default=None, type=str, help="username to login to a oci registry")
-@click.option("--registry-password", required=False, default=None, type=str, help="password to login to a oci registry")
-@click.option("--registry", required=False, default=None, type=str, help="username to login to a oci registry")
 @click.option("--cpu", required=False, default=None, type=int, help="Number of CPUs associated to VM")
 @click.option("--memory", required=False, default=None, type=int, help="VM memory size in megabytes associated to VM")
 @click.option(
     "--display",
     required=False,
     default=None,
     type=str,
@@ -99,23 +84,17 @@
     required=False,
     type=str,
     default="latest",
     help="The version of the GitLab Runner to be installed. Example '15.11.0'",
 )
 @click.option("-x", "--tart-executable", required=False, default="tart", type=str, help="Path to the tart executable.")
 def prepare(
-    default_ssh_username,
-    default_ssh_password,
-    registry_username,
-    registry_password,
-    registry,
     cpu,
     memory,
     display,
-    pull_policy,
     auto_resources,
     concurrency,
     cache_dir,
     builds_dir,
     timeout,
     volumes,
     install_gitlab_runner,
@@ -125,67 +104,66 @@
 ):
     """Prepare the environment and start the tart VM."""
 
     print_host_spec()
 
     p = GitLabCustomCommandConfig()
 
-    if not p.tart_ssh_username:
-        p.tart_ssh_username = default_ssh_username
-    if not p.tart_ssh_password:
-        p.tart_ssh_password = default_ssh_password
+    if not p.tart_executor_display:
+        p.tart_executor_display = display
+    if not p.tart_executor_install_gitlab_runner:
+        p.tart_executor_install_gitlab_runner = install_gitlab_runner
+    if not p.tart_executor_timeout:
+        p.tart_executor_timeout = timeout
 
     tart = Tart(exec_path=tart_executable)
     tart_images = tart.list()
     tart_vm_map = {}
     for i in tart_images:
         tart_vm_map[i.name] = i
 
-    # for k,v in os.environ.items():
-    #     click.echo(f'{k}={v}')
-
     ######################################################################
     # OCI LOGIN
     ######################################################################
     click.echo(f"[INFO] Logging into GitLab Registry '{p.ci_registry}'")
     try:
         tart.login(username=p.ci_registry_user, password=p.ci_registry_password, host=p.ci_registry)
     except:
         click.secho(f"[ERROR] Failed to login to '{p.ci_registry}'", fg="red")
 
-    if registry_username and registry_password and registry:
-        click.echo(f"[INFO] Logging into OCI Registry '{registry}'")
+    if p.registry_username and p.registry_password and p.registry:
+        click.echo(f"[INFO] Logging into OCI Registry '{p.registry}'")
         try:
-            tart.login(username=registry_username, password=registry_password, host=registry)
+            tart.login(username=p.registry_username, password=p.registry_password, host=p.registry)
         except:
-            click.secho(f"[ERROR] Failed to login to '{registry}'", fg="red")
+            click.secho(f"[ERROR] Failed to login to '{p.registry}'", fg="red")
 
     if p.tart_registry_username and p.tart_registry_password and p.tart_registry:
         click.echo(f"[INFO] Logging into custom OCI Registry '{p.tart_registry}'")
         try:
             tart.login(username=p.tart_registry_username, password=p.tart_registry_password, host=p.tart_registry)
         except:
             click.secho(f"[ERROR] Failed to login to '{p.tart_registry}'", fg="red")
 
     ######################################################################
     # PULL
     ######################################################################
     if (
-        (pull_policy == "always")
-        or (p.ci_job_image not in tart_vm_map and pull_policy != "never")
-        or (p.ci_job_image not in tart_vm_map and pull_policy == "if-not-present")
+        (p.pull_policy == "always")
+        or (p.ci_job_image not in tart_vm_map and p.pull_policy != "never")
+        or (p.ci_job_image not in tart_vm_map and p.pull_policy == "if-not-present")
     ):
-        click.echo(f"[INFO] Pulling '{p.ci_job_image}' [pull_policy={pull_policy}]")
+        click.echo(f"[INFO] Pulling '{p.ci_job_image}' [pull_policy={p.pull_policy}]")
         try:
             tart.pull(p.ci_job_image)
         except:
             click.secho(f"[ERROR] Failed to pull image '{p.ci_job_image}'", fg="red")
             sys.exit(1)
     else:
-        click.echo(f"[INFO] Skipping '{p.ci_job_image}' [pull_policy={pull_policy}]")
+        click.echo(f"[INFO] Skipping '{p.ci_job_image}' [pull_policy={p.pull_policy}]")
 
     ######################################################################
     # Create VM
     ######################################################################
     tart_vm_name = p.vm_name()
     if tart_vm_name in tart_vm_map:
         if tart_vm_map[tart_vm_name].running:
@@ -207,18 +185,18 @@
     click.echo(f"[INFO] Cloning VM instance '{tart_vm_name}' from '{p.ci_job_image}'")
     try:
         tart.clone(p.ci_job_image, tart_vm_name)
     except:
         click.secho(f"[ERROR] failed to clone image f'{p.ci_job_image}'", fg="red")
         sys.exit(1)
 
-    if cpu or memory or display:
+    if cpu or memory or p.display:
         click.echo(f"[INFO] Configuring instance '{tart_vm_name}' from '{p.ci_job_image}'")
         click.echo(
-            f"[INFO] {tart_vm_name} [cpu={cpu if cpu else 'default'}, memory={memory if memory else 'default'}, display={display if display else 'default'}]"
+            f"[INFO] {tart_vm_name} [cpu={cpu if cpu else 'default'}, memory={memory if memory else 'default'}, display={p.display if p.display else 'default'}]"
         )
         tart.set(tart_vm_name, cpu=cpu, memory=memory, display=display)
     elif auto_resources:
         click.echo("[INFO] Auto resource-disribution enabled.")
         host_spec = get_host_spec()
         tart.set(tart_vm_name, cpu=int(host_spec.cpu_count / concurrency), memory=int(host_spec.memory / concurrency))
 
@@ -245,61 +223,61 @@
         click.echo(f"[INFO] Builds directory set to '{builds_dir}'")
         volume_mounts.append(TartVolume(source=builds_dir, dest=remote_build_dir, name="builds", ro=False))
 
     for v in volumes:
         volume_mounts.append(TartVolume.from_string(v))
 
     try:
-        tart.run(tart_vm_name, volume_mounts)
+        tart.run(tart_vm_name, volume_mounts, no_graphics=p.headless, softnet=p.softnet_enabled)
     except:
         click.secho(f"[ERROR] Failed to start VM '{tart_vm_name}'", fg="red")
         sys.exit(1)
 
     try:
-        ip = tart.ip(tart_vm_name, timeout=timeout)
+        ip = tart.ip(tart_vm_name, timeout=p.timeout)
     except:
         click.secho(f"[ERROR] Failed to get IP of VM '{tart_vm_name}'", fg="red")
         sys.exit(1)
 
     if not ip:
-        click.echo(f"[ERROR] Error, VM was not reacheable after '{timeout}' seconds")
+        click.echo(f"[ERROR] Error, VM was not reacheable after '{p.timeout}' seconds")
         sys.exit(1)
 
     try:
-        ssh_session = tart.ssh_session(name=p.vm_name(), username=p.tart_ssh_username, password=p.tart_ssh_password)
+        ssh_session = tart.ssh_session(name=p.vm_name(), username=p.ssh_username, password=p.ssh_password)
         ssh_session.exec_ssh_command(
-            f"sudo mkdir -p {remote_script_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_script_dir}",
+            f"sudo mkdir -p {remote_script_dir} && sudo chown {p.ssh_username}:{p.ssh_username} {remote_script_dir}",
         )
 
         for volume in volume_mounts:
             click.echo(f"[INFO] Setting up volume mount '{volume.name}'")
             ssh_session.exec_ssh_command(
                 f"sudo mkdir -p $(dirname {volume.dest}); sudo ln -sf '/Volumes/My Shared Files/{volume.name}' {volume.dest}",
             )
 
         # if cache and builds volumes are not mounted, make sure to create them locally inside the VM
         if not cache_dir:
             ssh_session.exec_ssh_command(
-                f"sudo mkdir -p {remote_cache_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_cache_dir}",
+                f"sudo mkdir -p {remote_cache_dir} && sudo chown {p.ssh_username}:{p.ssh_username} {remote_cache_dir}",
             )
 
         if not builds_dir:
             ssh_session.exec_ssh_command(
-                f"sudo mkdir -p {remote_build_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_build_dir}",
+                f"sudo mkdir -p {remote_build_dir} && sudo chown {p.ssh_username}:{p.ssh_username} {remote_build_dir}",
             )
     except:
         click.secho(f"[ERROR] Failed so prepare VM '{tart_vm_name}'", fg="red")
         sys.exit(1)
 
-    if install_gitlab_runner:
+    if p.install_gitlab_runner:
         click.echo(
             f"[INFO] Installing GitLab Runner '{gitlab_runner_version}' [force: '{force_install_gitlab_runner}']"
         )
         try:
-            tart.install_gitlab_runner(name=tart_vm_name, username=p.tart_ssh_username, password=p.tart_ssh_password)
+            tart.install_gitlab_runner(name=tart_vm_name, username=p.ssh_username, password=p.ssh_password)
         except:
             click.secho(f"[ERROR] Failed to install GitLab Runner '{gitlab_runner_version}'", fg="red")
             sys.exit(1)
 
     tart.print_spec(tart_vm_name)
 
     sys.exit(0)
```

### Comparing `gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/commands/run.py` & `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/run.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 
 from gitlab_runner_tart_driver.modules.gitlab_custom_command_config import GitLabCustomCommandConfig
 from gitlab_runner_tart_driver.modules.tart import Tart
 
 
 @click.command()
 @click.option(
-    "--default-ssh-username", default="admin", required=False, type=str, help="username to login to a tart vm"
-)
-@click.option(
-    "--default-ssh-password", default="admin", required=False, type=str, help="password to login to a tart vm"
-)
-@click.option(
     "--timeout", "ssh_timeout", default=60, required=False, type=int, help="SSH connection timeout in seconds"
 )
 @click.option(
     "-x",
     "--tart-executable",
     required=False,
     default="tart",
@@ -30,51 +24,47 @@
     required=False,
     default="/bin/zsh",
     type=str,
     help="Path to the shell to be used for commands over ssh.",
 )
 @click.argument("script")
 @click.argument("stage")
-def run(default_ssh_username, default_ssh_password, ssh_timeout, tart_executable, shell, script, stage):
+def run(ssh_timeout, tart_executable, shell, script, stage):
     """Run commands."""
     p = GitLabCustomCommandConfig()
 
-    if not p.tart_ssh_username:
-        p.tart_ssh_username = default_ssh_username
-    if not p.tart_ssh_password:
-        p.tart_ssh_password = default_ssh_password
-
+    if not p.tart_executor_shell:
+        p.tart_executor_shell = shell
     ######################################################################
     # Connect to VM
     ######################################################################
     tart = Tart(exec_path=tart_executable)
     tart_vm_name = p.vm_name()
 
     try:
         tart_ip = tart.ip(tart_vm_name, timeout=ssh_timeout)
-        click.echo(f"[INFO] Establishing SSH conntection to '{p.tart_ssh_username}@{tart_ip}'")
+        click.echo(f"[{stage}][INFO] Establishing SSH conntection to '{p.ssh_username}@{tart_ip}'")
     except:
         click.secho(
-            f"[ERROR] Could not establish SSH conntection to '{tart_vm_name}' after '{ssh_timeout}' seconds.", fg="red"
+            f"[{stage}][ERROR] Could not establish SSH conntection to '{tart_vm_name}' after '{ssh_timeout}' seconds.",
+            fg="red",
         )
         sys.exit(1)
 
     try:
-        ssh_session = tart.ssh_session(name=p.vm_name(), username=p.tart_ssh_username, password=p.tart_ssh_password)
+        ssh_session = tart.ssh_session(name=p.vm_name(), username=p.ssh_username, password=p.ssh_password)
     except:
-        click.secho(f"[ERROR] Could not establish SSH session with '{p.tart_ssh_username}@{tart_ip}'", fg="red")
+        click.secho(f"[{stage}][ERROR] Could not establish SSH session with '{p.ssh_username}@{tart_ip}'", fg="red")
         sys.exit(1)
 
-    click.echo("[INFO] Preparing workspace")
     remote_temp_dir = "/opt/temp"
-
     script_name = os.path.basename(script)
     remote_script_path = os.path.join(remote_temp_dir, stage + "-" + script_name)
 
     sftp = ssh_session.ssh_client.open_sftp()
     sftp.put(script, remote_script_path)
     sftp.close()
 
     # ssh_session.exec_ssh_command(f"cd {remote_build_dir}")
-    script_exit_code = ssh_session.exec_ssh_command(f"{shell} -l {remote_script_path}", get_pty=True)
+    script_exit_code = ssh_session.exec_ssh_command(f"{p.shell} -l {remote_script_path}", get_pty=True)
 
     sys.exit(script_exit_code)
```

### Comparing `gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/modules/tart.py` & `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/tart.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,27 +149,33 @@
         ]
         print(tabulate(data, headers=["CPU", "Memory", "Disk", "Display", "Running", "IP Address"], tablefmt=tablefmt))
 
     def stop(self, name) -> None:
         """stops a given tart VM"""
         self.exec(["stop", name])
 
-    def run(self, name: str, volumes: list[TartVolume] = [], no_graphics=True) -> None:
+    def run(self, name: str, volumes: list[TartVolume] = [], no_graphics=True, softnet=False, vnc=False) -> None:
         """starts a given tart VM"""
         args = ["run", name]
         if no_graphics:
             args.append("--no-graphics")
+        if softnet:
+            args.append("--net-softnet")
+        if vnc:
+            args.append("--vnc")
 
         if volumes:
             for d in volumes:
                 source_path = os.path.abspath(os.path.expanduser(d.source))
                 if d.ro:
                     source_path = f"{source_path}:ro"
                 args.extend(["--dir", f"{d.name}:{source_path}"])
         try:
+            print(f"Starting VM '{name}'")
+            print(f"Command: 'tart {' '.join(args)}'")
             self.spawn_exec(args)
         except Exception as e:
             print(f"Error when running VM {name}")
             raise e
 
     def ip(self, name, timeout=30, resolver="dhcp") -> str:
         """return the IP adress of a given tart VM"""
```

### Comparing `gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/modules/utils.py` & `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2` & `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver.egg-info/PKG-INFO` & `gitlab-runner-tart-driver-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,15 @@
-Metadata-Version: 2.1
-Name: gitlab-runner-tart-driver
-Version: 0.1.7
-Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
-Author: Matthias Schmieder
-Author-email: schmieder.matthias@gmail.com
-License: BSD
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Version Control
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Gitlab Runner Custom Tart Driver
 
 - [Gitlab Runner Custom Tart Driver](#gitlab-runner-custom-tart-driver)
   - [About](#about)
   - [Setup](#setup)
     - [GitLab Runner Configuration](#gitlab-runner-configuration)
   - [GitLab CI](#gitlab-ci)
+    - [Supported Environment Variables](#supported-environment-variables)
     - [Private OCI Registries](#private-oci-registries)
     - [Configuring the SSH Credentials](#configuring-the-ssh-credentials)
   - [Advanced Configuration](#advanced-configuration)
     - [GitLab Runner Installation](#gitlab-runner-installation)
     - [Concurrency](#concurrency)
     - [Host Cache and Builds directories](#host-cache-and-builds-directories)
     - [Volume Mounts](#volume-mounts)
@@ -173,14 +159,32 @@
   script:
     - echo "This is brought to you by tart" >> artifact.txt
   artifacts:
     paths:
       - artifact.txt
 ```
 
+### Supported Environment Variables
+
+| **Name**                              | **Default**    | **Description**                                                                                               |
+| ------------------------------------- | -------------- | ------------------------------------------------------------------------------------------------------------- |
+| `TART_REGISTRY_USERNAME`              |                | Username to login to private OCI registry                                                                     |
+| `TART_REGISTRY_PASSWORD`              |                | Password to login to private OCI registry                                                                     |
+| `TART_REGISTRY`                       |                | Private OCI registry                                                                                          |
+| `TART_PULL_POLICY`                    | if-not-present | define how runners pull tart images from registries. Options are `always`,`if-not-present`,`never`            |
+| `TART_SSH_USERNAME`                   | admin          | Username to use to login to VM                                                                                |
+| `TART_SSH_PASSWORD`                   | admin          | Password to use to login to VM                                                                                |
+| `TART_EXECUTOR_HEADLESS`              | true           | Don't open a UI window.                                                                                       |
+| `TART_EXECUTOR_SOFTNET_ENABLED`       | false          | Use software networking instead of the default shared (NAT) networking                                        |
+| `TART_EXECUTOR_VNC_ENABLED`           | false          | Use screen sharing instead of the built-in UI. Note that Remote Login option should be enabled inside the VM. |
+| `TART_EXECUTOR_INSTALL_GITLAB_RUNNER` | false          | Install a GitLabRunner into the VM to ensure full CI/CD functionality                                         |
+| `TART_EXECUTOR_SHELL`                 | /bin/zsh       | The shell that should be used when running commands                                                           |
+| `TART_EXECUTOR_TIMEOUT`               | 60             | Timeout for `tart ip` to respond with a valid IP                                                              |
+| `TART_EXECUTOR_DISPLAY`               | 1920x1200      | Display resolution in format `WxH`                                                                            |
+
 ### Private OCI Registries
 
 Oftentimes you might want to provide your own OCI-compliant images created with [Packer](https://www.packer.io) and the official [Tart Builder](https://developer.hashicorp.com/packer/plugins/builders/tart). If you push your images to a private registry you will need to provide the credentials for the `gitlab-runner-tart-driver` to login there first.
 
 You can provide a default login registry using the `CLI` parameters (see **Command `prepare`**) but also provide the credentials from with each job variable definition
 
 ```yaml
@@ -342,17 +346,15 @@
 
 You can use a custom shell to execute your commands. The default ist `/bin/zsh`
 
 see **Command `run`**
 
 ### Custom `pull_policy`
 
-You can use a custom `pull_policy`. The default policy is `if-not-present`
-
-see **Command `prepare`**
+You can use a custom `pull_policy`. The default policy is `if-not-present`. Use `TART_PULL_POLICY` to override the default pull policy
 
 ## CLI
 
 ### CLI Parameters for `config.toml`
 
 The `gitlab-runner-tart-driver` gives a number of advanced configuration options. Use `gitlab-runner-tart-driver [stage] --help` to get a full list of options that you can pass to the exectuable using your `config.toml` file.
 
@@ -387,22 +389,14 @@
 
 ```
 Usage: gitlab-runner-tart-driver prepare [OPTIONS]
 
   Prepare the environment and start the tart VM.
 
 Options:
-  --default-ssh-username TEXT     username to login to a tart vm
-  --default-ssh-password TEXT     password to login to a tart vm
-  --pull-policy [always|if-not-present|never]
-                                  define how runners pull tart images from
-                                  registries
-  --registry-username TEXT        username to login to a oci registry
-  --registry-password TEXT        password to login to a oci registry
-  --registry TEXT                 username to login to a oci registry
   --cpu INTEGER                   Number of CPUs associated to VM
   --memory INTEGER                VM memory size in megabytes associated to VM
   --display TEXT                  VM display resolution in a format of
                                   <width>x<height>. For example, 1200x800
   --auto-resources / --no-auto-resources
                                   If enabled, the driver will divide system
                                   resources equally to the concurrent VMs.
@@ -430,16 +424,14 @@
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
   Run commands.
 
 Options:
-  --default-ssh-username TEXT  username to login to a tart vm
-  --default-ssh-password TEXT  password to login to a tart vm
   --timeout INTEGER            SSH connection timeout in seconds
   -x, --tart-executable TEXT   Path to the tart executable.
   --shell TEXT                 Path to the shell to be used for commands over
                                ssh.
   --help                       Show this message and exit.
 ```
 
@@ -449,8 +441,8 @@
 Usage: gitlab-runner-tart-driver cleanup [OPTIONS]
 
   Command to greet a user.
 
 Options:
   -x, --tart-executable TEXT  Path to the tart executable.
   --help                      Show this message and exit.
-```
+```
```

### Comparing `gitlab-runner-tart-driver-0.1.7/gitlab_runner_tart_driver.egg-info/SOURCES.txt` & `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.7/setup.py` & `gitlab-runner-tart-driver-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.1.7"
+version = "0.2.0"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
```

