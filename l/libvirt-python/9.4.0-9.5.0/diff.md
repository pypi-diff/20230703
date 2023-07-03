# Comparing `tmp/libvirt-python-9.4.0.tar.gz` & `tmp/libvirt-python-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvirt-python-9.4.0.tar", last modified: Thu Jun  1 09:50:26 2023, max compression
+gzip compressed data, was "libvirt-python-9.5.0.tar", last modified: Mon Jul  3 10:17:22 2023, max compression
```

## Comparing `libvirt-python-9.4.0.tar` & `libvirt-python-9.5.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.515809 libvirt-python-9.4.0/
--rw-rw-r--   0 jirka      (500) jirka      (500)       27 2014-06-19 09:18:44.000000 libvirt-python-9.4.0/.ctags
--rw-rw-r--   0 jirka      (500) jirka      (500)      171 2014-06-19 09:18:44.000000 libvirt-python-9.4.0/.dir-locals.el
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.502476 libvirt-python-9.4.0/.github/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.509142 libvirt-python-9.4.0/.github/workflows/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1486 2021-12-01 09:53:22.000000 libvirt-python-9.4.0/.github/workflows/lockdown.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      100 2023-01-16 10:59:44.000000 libvirt-python-9.4.0/.gitignore
--rw-rw-r--   0 jirka      (500) jirka      (500)     2693 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/.gitlab-ci.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      554 2016-10-04 07:42:23.000000 libvirt-python-9.4.0/.mailmap
--rw-rw-r--   0 jirka      (500) jirka      (500)     4008 2023-06-01 09:50:26.000000 libvirt-python-9.4.0/AUTHORS
--rw-rw-r--   0 jirka      (500) jirka      (500)      236 2014-06-19 09:18:44.000000 libvirt-python-9.4.0/AUTHORS.in
--rw-rw-r--   0 jirka      (500) jirka      (500)     1023 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 jirka      (500) jirka      (500)    18092 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/COPYING
--rw-rw-r--   0 jirka      (500) jirka      (500)    26530 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/COPYING.LESSER
--rw-rw-r--   0 jirka      (500) jirka      (500)   406729 2023-06-01 09:50:26.000000 libvirt-python-9.4.0/ChangeLog
--rw-rw-r--   0 jirka      (500) jirka      (500)     1491 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/HACKING
--rw-rw-r--   0 jirka      (500) jirka      (500)     1283 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/MANIFEST
--rw-rw-r--   0 jirka      (500) jirka      (500)     1704 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/MANIFEST.in
--rw-rw-r--   0 jirka      (500) jirka      (500)      260 2016-10-04 07:42:23.000000 libvirt-python-9.4.0/Makefile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1162 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/PKG-INFO
--rw-rw-r--   0 jirka      (500) jirka      (500)     1384 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/README
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.502476 libvirt-python-9.4.0/build/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/build/libvirt_python.egg-info/
--rw-rw-r--   0 jirka      (500) jirka      (500)     2326 2023-06-01 09:50:26.000000 libvirt-python-9.4.0/build/libvirt_python.egg-info/SOURCES.txt
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.509142 libvirt-python-9.4.0/ci/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.509142 libvirt-python-9.4.0/ci/buildenv/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1407 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/centos-stream-8.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      965 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/centos-stream-9.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/debian-10.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/debian-sid.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      798 2023-01-16 10:59:44.000000 libvirt-python-9.4.0/ci/buildenv/fedora-37.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      798 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/buildenv/fedora-38.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      850 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/fedora-rawhide.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      846 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/buildenv/opensuse-leap-15.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      852 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/opensuse-tumbleweed.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/ubuntu-2004.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/ubuntu-2204.sh
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.509142 libvirt-python-9.4.0/ci/containers/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1499 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/centos-stream-8.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/centos-stream-9.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1370 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/debian-10.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1371 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/debian-sid.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1281 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/ci/containers/fedora-37.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1281 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/containers/fedora-38.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1343 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/ci/containers/fedora-rawhide.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)      905 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/containers/opensuse-leap-15.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)      919 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/opensuse-tumbleweed.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1368 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/ubuntu-2004.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1368 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/ubuntu-2204.Dockerfile
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/ci/gitlab/
--rw-rw-r--   0 jirka      (500) jirka      (500)     6071 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/ci/gitlab/build-templates.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     5844 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/gitlab/builds.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1573 2023-01-16 10:59:44.000000 libvirt-python-9.4.0/ci/gitlab/container-templates.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1445 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/gitlab/containers.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      938 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/ci/gitlab/sanity-checks.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     2754 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/ci/gitlab.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1474 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/manifest.yml
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/examples/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1592 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/README
--rw-rw-r--   0 jirka      (500) jirka      (500)     3300 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/consolecallback.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1663 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/dhcpleases.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     2107 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/dominfo.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1568 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/domipaddrs.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)      690 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/domrestore.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)      762 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/domsave.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1239 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/domstart.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     5066 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/esxlist.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)    35898 2022-07-01 09:27:33.000000 libvirt-python-9.4.0/examples/event-test.py
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/examples/guest-vcpus/
--rwxrwxr-x   0 jirka      (500) jirka      (500)     3880 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/guest-vcpus/guest-vcpu-daemon.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1588 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/guest-vcpus/guest-vcpu.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     2782 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/nodestats.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     3857 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/sparsestream.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1235 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/topology.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)    70037 2023-01-16 10:59:44.000000 libvirt-python-9.4.0/generator.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      737 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-lxc-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)     3276 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-lxc-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    59229 2022-06-01 07:30:40.000000 libvirt-python-9.4.0/libvirt-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)    31114 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virConnect.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     5628 2023-01-16 10:59:44.000000 libvirt-python-9.4.0/libvirt-override-virDomain.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      716 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virDomainCheckpoint.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      702 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virDomainSnapshot.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      381 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virNetwork.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      396 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virStoragePool.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    11453 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virStream.py
--rw-rw-r--   0 jirka      (500) jirka      (500)   329987 2023-06-01 09:50:22.000000 libvirt-python-9.4.0/libvirt-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    10085 2022-05-02 11:37:45.000000 libvirt-python-9.4.0/libvirt-override.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     2759 2023-06-01 09:50:26.000000 libvirt-python-9.4.0/libvirt-python.spec
--rw-rw-r--   0 jirka      (500) jirka      (500)     2766 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/libvirt-python.spec.in
--rw-rw-r--   0 jirka      (500) jirka      (500)     1135 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-qemu-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)    14037 2023-03-01 10:15:08.000000 libvirt-python-9.4.0/libvirt-qemu-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)     3452 2022-05-02 11:37:45.000000 libvirt-python-9.4.0/libvirt-qemu-override.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    16182 2022-07-11 21:25:49.000000 libvirt-python-9.4.0/libvirt-utils.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    13274 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-utils.h
--rw-rw-r--   0 jirka      (500) jirka      (500)    16957 2022-07-01 09:27:33.000000 libvirt-python-9.4.0/libvirtaio.py
--rw-rw-r--   0 jirka      (500) jirka      (500)       10 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/requirements-test.txt
--rw-rw-r--   0 jirka      (500) jirka      (500)       38 2023-06-01 09:50:26.515809 libvirt-python-9.4.0/setup.cfg
--rwxrwxr-x   0 jirka      (500) jirka      (500)    11863 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/setup.py
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/tests/
--rw-rw-r--   0 jirka      (500) jirka      (500)     2774 2022-07-01 09:27:33.000000 libvirt-python-9.4.0/tests/eventmock.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     6016 2022-07-01 09:27:33.000000 libvirt-python-9.4.0/tests/test_aio.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    16198 2022-05-02 11:37:45.000000 libvirt-python-9.4.0/tests/test_api_coverage.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     2884 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_conn.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      758 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_domain.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      552 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_domain_checkpoint.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      398 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_domain_snapshot.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      367 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_interface.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      363 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_network.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      380 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_nodedev.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      600 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_storage.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      114 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tox.ini
--rw-rw-r--   0 jirka      (500) jirka      (500)    10721 2023-03-01 10:15:08.000000 libvirt-python-9.4.0/typewrappers.c
--rw-rw-r--   0 jirka      (500) jirka      (500)     9234 2022-09-20 16:28:07.000000 libvirt-python-9.4.0/typewrappers.h
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.751372 libvirt-python-9.5.0/
+-rw-rw-r--   0 jirka      (500) jirka      (500)       27 2014-06-19 09:18:44.000000 libvirt-python-9.5.0/.ctags
+-rw-rw-r--   0 jirka      (500) jirka      (500)      171 2014-06-19 09:18:44.000000 libvirt-python-9.5.0/.dir-locals.el
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.741372 libvirt-python-9.5.0/.github/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.744705 libvirt-python-9.5.0/.github/workflows/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1486 2021-12-01 09:53:22.000000 libvirt-python-9.5.0/.github/workflows/lockdown.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      100 2023-01-16 10:59:44.000000 libvirt-python-9.5.0/.gitignore
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2745 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/.gitlab-ci.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      554 2016-10-04 07:42:23.000000 libvirt-python-9.5.0/.mailmap
+-rw-rw-r--   0 jirka      (500) jirka      (500)      227 2023-07-03 10:17:22.000000 libvirt-python-9.5.0/AUTHORS
+-rw-rw-r--   0 jirka      (500) jirka      (500)      236 2014-06-19 09:18:44.000000 libvirt-python-9.5.0/AUTHORS.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1023 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 jirka      (500) jirka      (500)    26521 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/COPYING
+-rw-rw-r--   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.000000 libvirt-python-9.5.0/ChangeLog
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1491 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/HACKING
+-rw-rw-r--   0 jirka      (500) jirka      (500)      326 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/MANIFEST.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)      304 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/Makefile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2542 2023-07-03 10:17:22.751372 libvirt-python-9.5.0/PKG-INFO
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1988 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/README
+-rw-rw-r--   0 jirka      (500) jirka      (500)        6 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/VERSION
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.741372 libvirt-python-9.5.0/build/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.751372 libvirt-python-9.5.0/build/libvirt_python.egg-info/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2335 2023-07-03 10:17:22.000000 libvirt-python-9.5.0/build/libvirt_python.egg-info/SOURCES.txt
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.744705 libvirt-python-9.5.0/ci/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.748039 libvirt-python-9.5.0/ci/buildenv/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1463 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/centos-stream-8.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1021 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/centos-stream-9.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1145 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/debian-10.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1113 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/debian-sid.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      822 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/fedora-37.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      822 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/fedora-38.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      874 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/fedora-rawhide.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      905 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/opensuse-leap-15.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      911 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/opensuse-tumbleweed.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1145 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/ubuntu-2004.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1145 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/buildenv/ubuntu-2204.sh
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.748039 libvirt-python-9.5.0/ci/containers/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1556 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/centos-stream-8.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1115 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/centos-stream-9.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1478 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/debian-10.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1446 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/debian-sid.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1312 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/fedora-37.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1312 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/fedora-38.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1374 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/fedora-rawhide.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)      965 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/opensuse-leap-15.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)      979 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/opensuse-tumbleweed.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1476 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/ubuntu-2004.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1476 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/containers/ubuntu-2204.Dockerfile
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.748039 libvirt-python-9.5.0/ci/gitlab/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     6071 2023-05-02 11:04:38.000000 libvirt-python-9.5.0/ci/gitlab/build-templates.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     5842 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/gitlab/builds.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1573 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/gitlab/container-templates.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1445 2023-05-17 07:45:20.000000 libvirt-python-9.5.0/ci/gitlab/containers.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      938 2023-05-02 11:04:38.000000 libvirt-python-9.5.0/ci/gitlab/sanity-checks.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2754 2023-05-02 11:04:38.000000 libvirt-python-9.5.0/ci/gitlab.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1473 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/ci/manifest.yml
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.751372 libvirt-python-9.5.0/examples/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1592 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/README
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3300 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/consolecallback.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1663 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/dhcpleases.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     2107 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/dominfo.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1568 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/domipaddrs.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)      690 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/domrestore.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)      762 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/domsave.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1239 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/domstart.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     5066 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/esxlist.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)    35898 2022-07-01 09:27:33.000000 libvirt-python-9.5.0/examples/event-test.py
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.751372 libvirt-python-9.5.0/examples/guest-vcpus/
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     3880 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/guest-vcpus/guest-vcpu-daemon.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1588 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/guest-vcpus/guest-vcpu.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     2782 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/nodestats.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     3857 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/sparsestream.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1235 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/examples/topology.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)    70037 2023-01-16 10:59:44.000000 libvirt-python-9.5.0/generator.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      737 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/libvirt-lxc-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3276 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/libvirt-lxc-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    59229 2022-06-01 07:30:40.000000 libvirt-python-9.5.0/libvirt-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)    31114 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/libvirt-override-virConnect.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     5628 2023-01-16 10:59:44.000000 libvirt-python-9.5.0/libvirt-override-virDomain.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      716 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/libvirt-override-virDomainCheckpoint.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      702 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/libvirt-override-virDomainSnapshot.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      381 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/libvirt-override-virNetwork.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      396 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/libvirt-override-virStoragePool.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    11453 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/libvirt-override-virStream.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)   329987 2023-06-01 09:50:22.000000 libvirt-python-9.5.0/libvirt-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    10085 2022-05-02 11:37:45.000000 libvirt-python-9.5.0/libvirt-override.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2725 2023-07-03 10:17:22.000000 libvirt-python-9.5.0/libvirt-python.spec
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2732 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/libvirt-python.spec.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1135 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/libvirt-qemu-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)    14037 2023-03-01 10:15:08.000000 libvirt-python-9.5.0/libvirt-qemu-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3452 2022-05-02 11:37:45.000000 libvirt-python-9.5.0/libvirt-qemu-override.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16182 2022-07-11 21:25:49.000000 libvirt-python-9.5.0/libvirt-utils.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    13274 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/libvirt-utils.h
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16957 2022-07-01 09:27:33.000000 libvirt-python-9.5.0/libvirtaio.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)       81 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/pyproject.toml
+-rw-rw-r--   0 jirka      (500) jirka      (500)       10 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/requirements-test.txt
+-rw-rw-r--   0 jirka      (500) jirka      (500)      639 2023-07-03 10:17:22.751372 libvirt-python-9.5.0/setup.cfg
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     9313 2023-07-03 10:05:49.000000 libvirt-python-9.5.0/setup.py
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-07-03 10:17:22.751372 libvirt-python-9.5.0/tests/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2774 2022-07-01 09:27:33.000000 libvirt-python-9.5.0/tests/eventmock.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     6016 2022-07-01 09:27:33.000000 libvirt-python-9.5.0/tests/test_aio.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16198 2022-05-02 11:37:45.000000 libvirt-python-9.5.0/tests/test_api_coverage.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2884 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/tests/test_conn.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      758 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/tests/test_domain.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      552 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/tests/test_domain_checkpoint.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      398 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/tests/test_domain_snapshot.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      367 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/tests/test_interface.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      363 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/tests/test_network.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      380 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/tests/test_nodedev.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      600 2022-04-01 10:30:02.000000 libvirt-python-9.5.0/tests/test_storage.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)       89 2023-07-03 08:16:56.000000 libvirt-python-9.5.0/tox.ini
+-rw-rw-r--   0 jirka      (500) jirka      (500)    10721 2023-03-01 10:15:08.000000 libvirt-python-9.5.0/typewrappers.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)     9234 2022-09-20 16:28:07.000000 libvirt-python-9.5.0/typewrappers.h
```

### Comparing `libvirt-python-9.4.0/.github/workflows/lockdown.yml` & `libvirt-python-9.5.0/.github/workflows/lockdown.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/.gitlab-ci.yml` & `libvirt-python-9.5.0/.gitlab-ci.yml`

 * *Files 15% similar despite different names*

```diff
@@ -21,18 +21,17 @@
     - mkdir -p "$SCRATCH_DIR"
     - cd "$SCRATCH_DIR"
     - git clone --depth 1 https://gitlab.com/libvirt/libvirt.git
     - cd libvirt
     - meson build -Ddriver_libvirtd=disabled "--prefix=$VROOT" "--libdir=$LIBDIR"
     - ninja -C build install
     - popd
-    - $PYTHON setup.py build
-    - $PYTHON -m pip ${PIP_INSTALL:-install} .
-    - $PYTHON setup.py test
-    - $PYTHON setup.py sdist
+    - $PYTHON -m build
+    - $PYTHON -m pip ${PIP_INSTALL:-install} dist/libvirt_python*.whl
+    - $PYTHON -m pytest tests
     - if test -x /usr/bin/rpmbuild && test "$RPM" != "skip" ;
       then
           rpmbuild --clean --nodeps --define "_topdir $PWD/rpmbuild" -ta dist/libvirt-python*tar.gz ;
           mv rpmbuild/RPMS/x86_64/ libvirt-python-rpms ;
       fi
 
 .native_git_build_job_prebuilt_env:
@@ -45,18 +44,17 @@
     - .native_git_build_job
     - .gitlab_native_build_job_local_env
 
 .native_build_job:
   script:
     - export MAKEFLAGS="-j$(getconf _NPROCESSORS_ONLN)"
     - export CFLAGS="-Werror"
-    - $PYTHON setup.py build
-    - $PYTHON -m pip ${PIP_INSTALL:-install} .
-    - $PYTHON setup.py test
-    - $PYTHON setup.py sdist
+    - $PYTHON -m build
+    - $PYTHON -m pip ${PIP_INSTALL:-install} dist/libvirt_python*.whl
+    - $PYTHON -m pytest tests
     - if test -x /usr/bin/rpmbuild && test "$RPM" != "skip" ;
       then
           rpmbuild --clean --nodeps --define "_topdir $PWD/rpmbuild" -ta dist/libvirt-python*tar.gz ;
           mv rpmbuild/RPMS/x86_64/ libvirt-python-rpms ;
       fi
 
 .native_build_job_prebuilt_env:
@@ -71,15 +69,16 @@
 
 include: '/ci/gitlab.yml'
 
 .api_coverage_job:
   stage: sanity_checks
   script:
     - *git_build_vars
-    - LIBVIRT_API_COVERAGE=1 $PYTHON setup.py test
+    - $PYTHON -m pip ${PIP_INSTALL:-install} dist/libvirt_python*.whl
+    - LIBVIRT_API_COVERAGE=1 $PYTHON -m pytest tests
   allow_failure: true
 
 api_coverage_prebuilt_env:
   extends:
     - .gitlab_native_build_job_prebuilt_env
     - .api_coverage_job
   needs:
```

### Comparing `libvirt-python-9.4.0/.mailmap` & `libvirt-python-9.5.0/.mailmap`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/CONTRIBUTING.rst` & `libvirt-python-9.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/COPYING` & `libvirt-python-9.5.0/COPYING`

 * *Files 24% similar despite different names*

```diff
@@ -1,339 +1,502 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 2, June 1991
+                  GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 2.1, February 1999
 
- Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
- 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+ Copyright (C) 1991, 1999 Free Software Foundation, Inc.
+ 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
+[This is the first released version of the Lesser GPL.  It also counts
+ as the successor of the GNU Library Public License, version 2, hence
+ the version number 2.1.]
+
                             Preamble
 
   The licenses for most software are designed to take away your
 freedom to share and change it.  By contrast, the GNU General Public
-License is intended to guarantee your freedom to share and change free
-software--to make sure the software is free for all its users.  This
-General Public License applies to most of the Free Software
-Foundation's software and to any other program whose authors commit to
-using it.  (Some other Free Software Foundation software is covered by
-the GNU Lesser General Public License instead.)  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-this service if you wish), that you receive source code or can get it
-if you want it, that you can change the software or use pieces of it
-in new free programs; and that you know you can do these things.
+Licenses are intended to guarantee your freedom to share and change
+free software--to make sure the software is free for all its users.
+
+  This license, the Lesser General Public License, applies to some
+specially designated software packages--typically libraries--of the
+Free Software Foundation and other authors who decide to use it.  You
+can use it too, but we suggest you first think carefully about whether
+this license or the ordinary General Public License is the better
+strategy to use in any particular case, based on the explanations below.
+
+  When we speak of free software, we are referring to freedom of use,
+not price.  Our General Public Licenses are designed to make sure that
+you have the freedom to distribute copies of free software (and charge
+for this service if you wish); that you receive source code or can get
+it if you want it; that you can change the software and use pieces of
+it in new free programs; and that you are informed that you can do
+these things.
 
   To protect your rights, we need to make restrictions that forbid
-anyone to deny you these rights or to ask you to surrender the rights.
-These restrictions translate to certain responsibilities for you if you
-distribute copies of the software, or if you modify it.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must give the recipients all the rights that
-you have.  You must make sure that they, too, receive or can get the
-source code.  And you must show them these terms so they know their
-rights.
-
-  We protect your rights with two steps: (1) copyright the software, and
-(2) offer you this license which gives you legal permission to copy,
-distribute and/or modify the software.
-
-  Also, for each author's protection and ours, we want to make certain
-that everyone understands that there is no warranty for this free
-software.  If the software is modified by someone else and passed on, we
-want its recipients to know that what they have is not the original, so
-that any problems introduced by others will not reflect on the original
-authors' reputations.
-
-  Finally, any free program is threatened constantly by software
-patents.  We wish to avoid the danger that redistributors of a free
-program will individually obtain patent licenses, in effect making the
-program proprietary.  To prevent this, we have made it clear that any
-patent must be licensed for everyone's free use or not licensed at all.
+distributors to deny you these rights or to ask you to surrender these
+rights.  These restrictions translate to certain responsibilities for
+you if you distribute copies of the library or if you modify it.
+
+  For example, if you distribute copies of the library, whether gratis
+or for a fee, you must give the recipients all the rights that we gave
+you.  You must make sure that they, too, receive or can get the source
+code.  If you link other code with the library, you must provide
+complete object files to the recipients, so that they can relink them
+with the library after making changes to the library and recompiling
+it.  And you must show them these terms so they know their rights.
+
+  We protect your rights with a two-step method: (1) we copyright the
+library, and (2) we offer you this license, which gives you legal
+permission to copy, distribute and/or modify the library.
+
+  To protect each distributor, we want to make it very clear that
+there is no warranty for the free library.  Also, if the library is
+modified by someone else and passed on, the recipients should know
+that what they have is not the original version, so that the original
+author's reputation will not be affected by problems that might be
+introduced by others.
+
+  Finally, software patents pose a constant threat to the existence of
+any free program.  We wish to make sure that a company cannot
+effectively restrict the users of a free program by obtaining a
+restrictive license from a patent holder.  Therefore, we insist that
+any patent license obtained for a version of the library must be
+consistent with the full freedom of use specified in this license.
+
+  Most GNU software, including some libraries, is covered by the
+ordinary GNU General Public License.  This license, the GNU Lesser
+General Public License, applies to certain designated libraries, and
+is quite different from the ordinary General Public License.  We use
+this license for certain libraries in order to permit linking those
+libraries into non-free programs.
+
+  When a program is linked with a library, whether statically or using
+a shared library, the combination of the two is legally speaking a
+combined work, a derivative of the original library.  The ordinary
+General Public License therefore permits such linking only if the
+entire combination fits its criteria of freedom.  The Lesser General
+Public License permits more lax criteria for linking other code with
+the library.
+
+  We call this license the "Lesser" General Public License because it
+does Less to protect the user's freedom than the ordinary General
+Public License.  It also provides other free software developers Less
+of an advantage over competing non-free programs.  These disadvantages
+are the reason we use the ordinary General Public License for many
+libraries.  However, the Lesser license provides advantages in certain
+special circumstances.
+
+  For example, on rare occasions, there may be a special need to
+encourage the widest possible use of a certain library, so that it becomes
+a de-facto standard.  To achieve this, non-free programs must be
+allowed to use the library.  A more frequent case is that a free
+library does the same job as widely used non-free libraries.  In this
+case, there is little to gain by limiting the free library to free
+software only, so we use the Lesser General Public License.
+
+  In other cases, permission to use a particular library in non-free
+programs enables a greater number of people to use a large body of
+free software.  For example, permission to use the GNU C Library in
+non-free programs enables many more people to use the whole GNU
+operating system, as well as its variant, the GNU/Linux operating
+system.
+
+  Although the Lesser General Public License is Less protective of the
+users' freedom, it does ensure that the user of a program that is
+linked with the Library has the freedom and the wherewithal to run
+that program using a modified version of the Library.
 
   The precise terms and conditions for copying, distribution and
-modification follow.
+modification follow.  Pay close attention to the difference between a
+"work based on the library" and a "work that uses the library".  The
+former contains code derived from the library, whereas the latter must
+be combined with the library in order to run.
 
-                    GNU GENERAL PUBLIC LICENSE
+                  GNU LESSER GENERAL PUBLIC LICENSE
    TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
 
-  0. This License applies to any program or other work which contains
-a notice placed by the copyright holder saying it may be distributed
-under the terms of this General Public License.  The "Program", below,
-refers to any such program or work, and a "work based on the Program"
-means either the Program or any derivative work under copyright law:
-that is to say, a work containing the Program or a portion of it,
-either verbatim or with modifications and/or translated into another
-language.  (Hereinafter, translation is included without limitation in
-the term "modification".)  Each licensee is addressed as "you".
+  0. This License Agreement applies to any software library or other
+program which contains a notice placed by the copyright holder or
+other authorized party saying it may be distributed under the terms of
+this Lesser General Public License (also called "this License").
+Each licensee is addressed as "you".
+
+  A "library" means a collection of software functions and/or data
+prepared so as to be conveniently linked with application programs
+(which use some of those functions and data) to form executables.
+
+  The "Library", below, refers to any such software library or work
+which has been distributed under these terms.  A "work based on the
+Library" means either the Library or any derivative work under
+copyright law: that is to say, a work containing the Library or a
+portion of it, either verbatim or with modifications and/or translated
+straightforwardly into another language.  (Hereinafter, translation is
+included without limitation in the term "modification".)
+
+  "Source code" for a work means the preferred form of the work for
+making modifications to it.  For a library, complete source code means
+all the source code for all modules it contains, plus any associated
+interface definition files, plus the scripts used to control compilation
+and installation of the library.
 
-Activities other than copying, distribution and modification are not
+  Activities other than copying, distribution and modification are not
 covered by this License; they are outside its scope.  The act of
-running the Program is not restricted, and the output from the Program
-is covered only if its contents constitute a work based on the
-Program (independent of having been made by running the Program).
-Whether that is true depends on what the Program does.
-
-  1. You may copy and distribute verbatim copies of the Program's
-source code as you receive it, in any medium, provided that you
-conspicuously and appropriately publish on each copy an appropriate
-copyright notice and disclaimer of warranty; keep intact all the
-notices that refer to this License and to the absence of any warranty;
-and give any other recipients of the Program a copy of this License
-along with the Program.
+running a program using the Library is not restricted, and output from
+such a program is covered only if its contents constitute a work based
+on the Library (independent of the use of the Library in a tool for
+writing it).  Whether that is true depends on what the Library does
+and what the program that uses the Library does.
+
+  1. You may copy and distribute verbatim copies of the Library's
+complete source code as you receive it, in any medium, provided that
+you conspicuously and appropriately publish on each copy an
+appropriate copyright notice and disclaimer of warranty; keep intact
+all the notices that refer to this License and to the absence of any
+warranty; and distribute a copy of this License along with the
+Library.
+
+  You may charge a fee for the physical act of transferring a copy,
+and you may at your option offer warranty protection in exchange for a
+fee.
 
-You may charge a fee for the physical act of transferring a copy, and
-you may at your option offer warranty protection in exchange for a fee.
-
-  2. You may modify your copy or copies of the Program or any portion
-of it, thus forming a work based on the Program, and copy and
+  2. You may modify your copy or copies of the Library or any portion
+of it, thus forming a work based on the Library, and copy and
 distribute such modifications or work under the terms of Section 1
 above, provided that you also meet all of these conditions:
 
-    a) You must cause the modified files to carry prominent notices
+    a) The modified work must itself be a software library.
+
+    b) You must cause the files modified to carry prominent notices
     stating that you changed the files and the date of any change.
 
-    b) You must cause any work that you distribute or publish, that in
-    whole or in part contains or is derived from the Program or any
-    part thereof, to be licensed as a whole at no charge to all third
-    parties under the terms of this License.
-
-    c) If the modified program normally reads commands interactively
-    when run, you must cause it, when started running for such
-    interactive use in the most ordinary way, to print or display an
-    announcement including an appropriate copyright notice and a
-    notice that there is no warranty (or else, saying that you provide
-    a warranty) and that users may redistribute the program under
-    these conditions, and telling the user how to view a copy of this
-    License.  (Exception: if the Program itself is interactive but
-    does not normally print such an announcement, your work based on
-    the Program is not required to print an announcement.)
+    c) You must cause the whole of the work to be licensed at no
+    charge to all third parties under the terms of this License.
+
+    d) If a facility in the modified Library refers to a function or a
+    table of data to be supplied by an application program that uses
+    the facility, other than as an argument passed when the facility
+    is invoked, then you must make a good faith effort to ensure that,
+    in the event an application does not supply such function or
+    table, the facility still operates, and performs whatever part of
+    its purpose remains meaningful.
+
+    (For example, a function in a library to compute square roots has
+    a purpose that is entirely well-defined independent of the
+    application.  Therefore, Subsection 2d requires that any
+    application-supplied function or table used by this function must
+    be optional: if the application does not supply it, the square
+    root function must still compute square roots.)
 
 These requirements apply to the modified work as a whole.  If
-identifiable sections of that work are not derived from the Program,
+identifiable sections of that work are not derived from the Library,
 and can be reasonably considered independent and separate works in
 themselves, then this License, and its terms, do not apply to those
 sections when you distribute them as separate works.  But when you
 distribute the same sections as part of a whole which is a work based
-on the Program, the distribution of the whole must be on the terms of
+on the Library, the distribution of the whole must be on the terms of
 this License, whose permissions for other licensees extend to the
-entire whole, and thus to each and every part regardless of who wrote it.
+entire whole, and thus to each and every part regardless of who wrote
+it.
 
 Thus, it is not the intent of this section to claim rights or contest
 your rights to work written entirely by you; rather, the intent is to
 exercise the right to control the distribution of derivative or
-collective works based on the Program.
+collective works based on the Library.
 
-In addition, mere aggregation of another work not based on the Program
-with the Program (or with a work based on the Program) on a volume of
+In addition, mere aggregation of another work not based on the Library
+with the Library (or with a work based on the Library) on a volume of
 a storage or distribution medium does not bring the other work under
 the scope of this License.
 
-  3. You may copy and distribute the Program (or a work based on it,
-under Section 2) in object code or executable form under the terms of
-Sections 1 and 2 above provided that you also do one of the following:
-
-    a) Accompany it with the complete corresponding machine-readable
-    source code, which must be distributed under the terms of Sections
-    1 and 2 above on a medium customarily used for software interchange; or,
-
-    b) Accompany it with a written offer, valid for at least three
-    years, to give any third party, for a charge no more than your
-    cost of physically performing source distribution, a complete
-    machine-readable copy of the corresponding source code, to be
-    distributed under the terms of Sections 1 and 2 above on a medium
-    customarily used for software interchange; or,
-
-    c) Accompany it with the information you received as to the offer
-    to distribute corresponding source code.  (This alternative is
-    allowed only for noncommercial distribution and only if you
-    received the program in object code or executable form with such
-    an offer, in accord with Subsection b above.)
-
-The source code for a work means the preferred form of the work for
-making modifications to it.  For an executable work, complete source
-code means all the source code for all modules it contains, plus any
-associated interface definition files, plus the scripts used to
-control compilation and installation of the executable.  However, as a
-special exception, the source code distributed need not include
-anything that is normally distributed (in either source or binary
-form) with the major components (compiler, kernel, and so on) of the
-operating system on which the executable runs, unless that component
-itself accompanies the executable.
-
-If distribution of executable or object code is made by offering
-access to copy from a designated place, then offering equivalent
-access to copy the source code from the same place counts as
-distribution of the source code, even though third parties are not
+  3. You may opt to apply the terms of the ordinary GNU General Public
+License instead of this License to a given copy of the Library.  To do
+this, you must alter all the notices that refer to this License, so
+that they refer to the ordinary GNU General Public License, version 2,
+instead of to this License.  (If a newer version than version 2 of the
+ordinary GNU General Public License has appeared, then you can specify
+that version instead if you wish.)  Do not make any other change in
+these notices.
+
+  Once this change is made in a given copy, it is irreversible for
+that copy, so the ordinary GNU General Public License applies to all
+subsequent copies and derivative works made from that copy.
+
+  This option is useful when you wish to copy part of the code of
+the Library into a program that is not a library.
+
+  4. You may copy and distribute the Library (or a portion or
+derivative of it, under Section 2) in object code or executable form
+under the terms of Sections 1 and 2 above provided that you accompany
+it with the complete corresponding machine-readable source code, which
+must be distributed under the terms of Sections 1 and 2 above on a
+medium customarily used for software interchange.
+
+  If distribution of object code is made by offering access to copy
+from a designated place, then offering equivalent access to copy the
+source code from the same place satisfies the requirement to
+distribute the source code, even though third parties are not
 compelled to copy the source along with the object code.
 
-  4. You may not copy, modify, sublicense, or distribute the Program
-except as expressly provided under this License.  Any attempt
-otherwise to copy, modify, sublicense or distribute the Program is
-void, and will automatically terminate your rights under this License.
-However, parties who have received copies, or rights, from you under
-this License will not have their licenses terminated so long as such
-parties remain in full compliance.
+  5. A program that contains no derivative of any portion of the
+Library, but is designed to work with the Library by being compiled or
+linked with it, is called a "work that uses the Library".  Such a
+work, in isolation, is not a derivative work of the Library, and
+therefore falls outside the scope of this License.
+
+  However, linking a "work that uses the Library" with the Library
+creates an executable that is a derivative of the Library (because it
+contains portions of the Library), rather than a "work that uses the
+library".  The executable is therefore covered by this License.
+Section 6 states terms for distribution of such executables.
+
+  When a "work that uses the Library" uses material from a header file
+that is part of the Library, the object code for the work may be a
+derivative work of the Library even though the source code is not.
+Whether this is true is especially significant if the work can be
+linked without the Library, or if the work is itself a library.  The
+threshold for this to be true is not precisely defined by law.
+
+  If such an object file uses only numerical parameters, data
+structure layouts and accessors, and small macros and small inline
+functions (ten lines or less in length), then the use of the object
+file is unrestricted, regardless of whether it is legally a derivative
+work.  (Executables containing this object code plus portions of the
+Library will still fall under Section 6.)
+
+  Otherwise, if the work is a derivative of the Library, you may
+distribute the object code for the work under the terms of Section 6.
+Any executables containing that work also fall under Section 6,
+whether or not they are linked directly with the Library itself.
+
+  6. As an exception to the Sections above, you may also combine or
+link a "work that uses the Library" with the Library to produce a
+work containing portions of the Library, and distribute that work
+under terms of your choice, provided that the terms permit
+modification of the work for the customer's own use and reverse
+engineering for debugging such modifications.
+
+  You must give prominent notice with each copy of the work that the
+Library is used in it and that the Library and its use are covered by
+this License.  You must supply a copy of this License.  If the work
+during execution displays copyright notices, you must include the
+copyright notice for the Library among them, as well as a reference
+directing the user to the copy of this License.  Also, you must do one
+of these things:
+
+    a) Accompany the work with the complete corresponding
+    machine-readable source code for the Library including whatever
+    changes were used in the work (which must be distributed under
+    Sections 1 and 2 above); and, if the work is an executable linked
+    with the Library, with the complete machine-readable "work that
+    uses the Library", as object code and/or source code, so that the
+    user can modify the Library and then relink to produce a modified
+    executable containing the modified Library.  (It is understood
+    that the user who changes the contents of definitions files in the
+    Library will not necessarily be able to recompile the application
+    to use the modified definitions.)
+
+    b) Use a suitable shared library mechanism for linking with the
+    Library.  A suitable mechanism is one that (1) uses at run time a
+    copy of the library already present on the user's computer system,
+    rather than copying library functions into the executable, and (2)
+    will operate properly with a modified version of the library, if
+    the user installs one, as long as the modified version is
+    interface-compatible with the version that the work was made with.
+
+    c) Accompany the work with a written offer, valid for at
+    least three years, to give the same user the materials
+    specified in Subsection 6a, above, for a charge no more
+    than the cost of performing this distribution.
+
+    d) If distribution of the work is made by offering access to copy
+    from a designated place, offer equivalent access to copy the above
+    specified materials from the same place.
+
+    e) Verify that the user has already received a copy of these
+    materials or that you have already sent this user a copy.
+
+  For an executable, the required form of the "work that uses the
+Library" must include any data and utility programs needed for
+reproducing the executable from it.  However, as a special exception,
+the materials to be distributed need not include anything that is
+normally distributed (in either source or binary form) with the major
+components (compiler, kernel, and so on) of the operating system on
+which the executable runs, unless that component itself accompanies
+the executable.
+
+  It may happen that this requirement contradicts the license
+restrictions of other proprietary libraries that do not normally
+accompany the operating system.  Such a contradiction means you cannot
+use both them and the Library together in an executable that you
+distribute.
+
+  7. You may place library facilities that are a work based on the
+Library side-by-side in a single library together with other library
+facilities not covered by this License, and distribute such a combined
+library, provided that the separate distribution of the work based on
+the Library and of the other library facilities is otherwise
+permitted, and provided that you do these two things:
+
+    a) Accompany the combined library with a copy of the same work
+    based on the Library, uncombined with any other library
+    facilities.  This must be distributed under the terms of the
+    Sections above.
+
+    b) Give prominent notice with the combined library of the fact
+    that part of it is a work based on the Library, and explaining
+    where to find the accompanying uncombined form of the same work.
+
+  8. You may not copy, modify, sublicense, link with, or distribute
+the Library except as expressly provided under this License.  Any
+attempt otherwise to copy, modify, sublicense, link with, or
+distribute the Library is void, and will automatically terminate your
+rights under this License.  However, parties who have received copies,
+or rights, from you under this License will not have their licenses
+terminated so long as such parties remain in full compliance.
 
-  5. You are not required to accept this License, since you have not
+  9. You are not required to accept this License, since you have not
 signed it.  However, nothing else grants you permission to modify or
-distribute the Program or its derivative works.  These actions are
+distribute the Library or its derivative works.  These actions are
 prohibited by law if you do not accept this License.  Therefore, by
-modifying or distributing the Program (or any work based on the
-Program), you indicate your acceptance of this License to do so, and
+modifying or distributing the Library (or any work based on the
+Library), you indicate your acceptance of this License to do so, and
 all its terms and conditions for copying, distributing or modifying
-the Program or works based on it.
+the Library or works based on it.
 
-  6. Each time you redistribute the Program (or any work based on the
-Program), the recipient automatically receives a license from the
-original licensor to copy, distribute or modify the Program subject to
-these terms and conditions.  You may not impose any further
+  10. Each time you redistribute the Library (or any work based on the
+Library), the recipient automatically receives a license from the
+original licensor to copy, distribute, link with or modify the Library
+subject to these terms and conditions.  You may not impose any further
 restrictions on the recipients' exercise of the rights granted herein.
-You are not responsible for enforcing compliance by third parties to
+You are not responsible for enforcing compliance by third parties with
 this License.
 
-  7. If, as a consequence of a court judgment or allegation of patent
+  11. If, as a consequence of a court judgment or allegation of patent
 infringement or for any other reason (not limited to patent issues),
 conditions are imposed on you (whether by court order, agreement or
 otherwise) that contradict the conditions of this License, they do not
 excuse you from the conditions of this License.  If you cannot
 distribute so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you
-may not distribute the Program at all.  For example, if a patent
-license would not permit royalty-free redistribution of the Program by
+may not distribute the Library at all.  For example, if a patent
+license would not permit royalty-free redistribution of the Library by
 all those who receive copies directly or indirectly through you, then
 the only way you could satisfy both it and this License would be to
-refrain entirely from distribution of the Program.
+refrain entirely from distribution of the Library.
 
-If any portion of this section is held invalid or unenforceable under
-any particular circumstance, the balance of the section is intended to
-apply and the section as a whole is intended to apply in other
-circumstances.
+If any portion of this section is held invalid or unenforceable under any
+particular circumstance, the balance of the section is intended to apply,
+and the section as a whole is intended to apply in other circumstances.
 
 It is not the purpose of this section to induce you to infringe any
 patents or other property right claims or to contest validity of any
 such claims; this section has the sole purpose of protecting the
-integrity of the free software distribution system, which is
+integrity of the free software distribution system which is
 implemented by public license practices.  Many people have made
 generous contributions to the wide range of software distributed
 through that system in reliance on consistent application of that
 system; it is up to the author/donor to decide if he or she is willing
 to distribute software through any other system and a licensee cannot
 impose that choice.
 
 This section is intended to make thoroughly clear what is believed to
 be a consequence of the rest of this License.
 
-  8. If the distribution and/or use of the Program is restricted in
+  12. If the distribution and/or use of the Library is restricted in
 certain countries either by patents or by copyrighted interfaces, the
-original copyright holder who places the Program under this License
-may add an explicit geographical distribution limitation excluding
-those countries, so that distribution is permitted only in or among
-countries not thus excluded.  In such case, this License incorporates
-the limitation as if written in the body of this License.
-
-  9. The Free Software Foundation may publish revised and/or new versions
-of the General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-Each version is given a distinguishing version number.  If the Program
-specifies a version number of this License which applies to it and "any
-later version", you have the option of following the terms and conditions
-either of that version or of any later version published by the Free
-Software Foundation.  If the Program does not specify a version number of
-this License, you may choose any version ever published by the Free Software
-Foundation.
-
-  10. If you wish to incorporate parts of the Program into other free
-programs whose distribution conditions are different, write to the author
-to ask for permission.  For software which is copyrighted by the Free
-Software Foundation, write to the Free Software Foundation; we sometimes
-make exceptions for this.  Our decision will be guided by the two goals
-of preserving the free status of all derivatives of our free software and
-of promoting the sharing and reuse of software generally.
+original copyright holder who places the Library under this License may add
+an explicit geographical distribution limitation excluding those countries,
+so that distribution is permitted only in or among countries not thus
+excluded.  In such case, this License incorporates the limitation as if
+written in the body of this License.
+
+  13. The Free Software Foundation may publish revised and/or new
+versions of the Lesser General Public License from time to time.
+Such new versions will be similar in spirit to the present version,
+but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number.  If the Library
+specifies a version number of this License which applies to it and
+"any later version", you have the option of following the terms and
+conditions either of that version or of any later version published by
+the Free Software Foundation.  If the Library does not specify a
+license version number, you may choose any version ever published by
+the Free Software Foundation.
+
+  14. If you wish to incorporate parts of the Library into other free
+programs whose distribution conditions are incompatible with these,
+write to the author to ask for permission.  For software which is
+copyrighted by the Free Software Foundation, write to the Free
+Software Foundation; we sometimes make exceptions for this.  Our
+decision will be guided by the two goals of preserving the free status
+of all derivatives of our free software and of promoting the sharing
+and reuse of software generally.
 
                             NO WARRANTY
 
-  11. BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY
-FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW.  EXCEPT WHEN
-OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES
-PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED
-OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
-MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.  THE ENTIRE RISK AS
-TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU.  SHOULD THE
-PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING,
-REPAIR OR CORRECTION.
-
-  12. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR
-REDISTRIBUTE THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
-INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING
-OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED
-TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
-YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
-PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGES.
+  15. BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
+WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
+EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
+OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
+KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
+LIBRARY IS WITH YOU.  SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
+THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
+WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
+AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
+FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
+CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
+LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
+RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
+FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
+SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
+DAMAGES.
 
                      END OF TERMS AND CONDITIONS
 
-            How to Apply These Terms to Your New Programs
+           How to Apply These Terms to Your New Libraries
 
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-convey the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
+  If you develop a new library, and you want it to be of the greatest
+possible use to the public, we recommend making it free software that
+everyone can redistribute and change.  You can do so by permitting
+redistribution under these terms (or, alternatively, under the terms of the
+ordinary General Public License).
+
+  To apply these terms, attach the following notices to the library.  It is
+safest to attach them to the start of each source file to most effectively
+convey the exclusion of warranty; and each file should have at least the
+"copyright" line and a pointer to where the full notice is found.
 
-    <one line to give the program's name and a brief idea of what it does.>
+    <one line to give the library's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
-    This program is free software; you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation; either version 2 of the License, or
-    (at your option) any later version.
+    This library is free software; you can redistribute it and/or
+    modify it under the terms of the GNU Lesser General Public
+    License as published by the Free Software Foundation; either
+    version 2.1 of the License, or (at your option) any later version.
 
-    This program is distributed in the hope that it will be useful,
+    This library is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+    Lesser General Public License for more details.
 
-    You should have received a copy of the GNU General Public License along
-    with this program; if not, write to the Free Software Foundation, Inc.,
-    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+    You should have received a copy of the GNU Lesser General Public
+    License along with this library; if not, write to the Free Software
+    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 Also add information on how to contact you by electronic and paper mail.
 
-If the program is interactive, make it output a short notice like this
-when it starts in an interactive mode:
-
-    Gnomovision version 69, Copyright (C) year name of author
-    Gnomovision comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, the commands you use may
-be called something other than `show w' and `show c'; they could even be
-mouse-clicks or menu items--whatever suits your program.
-
 You should also get your employer (if you work as a programmer) or your
-school, if any, to sign a "copyright disclaimer" for the program, if
+school, if any, to sign a "copyright disclaimer" for the library, if
 necessary.  Here is a sample; alter the names:
 
-  Yoyodyne, Inc., hereby disclaims all copyright interest in the program
-  `Gnomovision' (which makes passes at compilers) written by James Hacker.
+  Yoyodyne, Inc., hereby disclaims all copyright interest in the
+  library `Frob' (a library for tweaking knobs) written by James Random Hacker.
 
-  <signature of Ty Coon>, 1 April 1989
+  <signature of Ty Coon>, 1 April 1990
   Ty Coon, President of Vice
 
-This General Public License does not permit incorporating your program into
-proprietary programs.  If your program is a subroutine library, you may
-consider it more useful to permit linking proprietary applications with the
-library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.
+That's all there is to it!
```

### Comparing `libvirt-python-9.4.0/HACKING` & `libvirt-python-9.5.0/HACKING`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/build/libvirt_python.egg-info/SOURCES.txt` & `libvirt-python-9.5.0/build/libvirt_python.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 .gitignore
 .gitlab-ci.yml
 .mailmap
 AUTHORS
 AUTHORS.in
 CONTRIBUTING.rst
 COPYING
-COPYING.LESSER
 ChangeLog
 HACKING
-MANIFEST
 MANIFEST.in
 Makefile
 README
+VERSION
 generator.py
 libvirt-lxc-override-api.xml
 libvirt-lxc-override.c
 libvirt-override-api.xml
 libvirt-override-virConnect.py
 libvirt-override-virDomain.py
 libvirt-override-virDomainCheckpoint.py
@@ -31,15 +30,17 @@
 libvirt-python.spec.in
 libvirt-qemu-override-api.xml
 libvirt-qemu-override.c
 libvirt-qemu-override.py
 libvirt-utils.c
 libvirt-utils.h
 libvirtaio.py
+pyproject.toml
 requirements-test.txt
+setup.cfg
 setup.py
 tox.ini
 typewrappers.c
 typewrappers.h
 .github/workflows/lockdown.yml
 ci/gitlab.yml
 ci/manifest.yml
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/centos-stream-8.sh` & `libvirt-python-9.5.0/ci/containers/centos-stream-8.Dockerfile`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
-function install_buildenv() {
-    dnf distro-sync -y
-    dnf install 'dnf-command(config-manager)' -y
-    dnf config-manager --set-enabled -y powertools
-    dnf install -y centos-release-advanced-virtualization
-    dnf install -y epel-release
-    dnf install -y epel-next-release
+FROM quay.io/centos/centos:stream8
+
+RUN dnf distro-sync -y && \
+    dnf install 'dnf-command(config-manager)' -y && \
+    dnf config-manager --set-enabled -y powertools && \
+    dnf install -y centos-release-advanced-virtualization && \
+    dnf install -y epel-release && \
+    dnf install -y epel-next-release && \
     dnf install -y \
         ca-certificates \
         ccache \
         cpp \
         gcc \
         gettext \
         git \
@@ -36,20 +37,24 @@
         python3 \
         python3-devel \
         python3-docutils \
         python3-lxml \
         python3-pip \
         python3-pytest \
         python3-setuptools \
+        python3-wheel \
         rpcgen \
-        rpm-build
-    rpm -qa | sort > /packages.txt
-    mkdir -p /usr/libexec/ccache-wrappers
-    ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc
+        rpm-build && \
+    dnf autoremove -y && \
+    dnf clean all -y && \
+    rpm -qa | sort > /packages.txt && \
+    mkdir -p /usr/libexec/ccache-wrappers && \
+    ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
-}
 
-export CCACHE_WRAPPERSDIR="/usr/libexec/ccache-wrappers"
-export LANG="en_US.UTF-8"
-export MAKE="/usr/bin/make"
-export NINJA="/usr/bin/ninja"
-export PYTHON="/usr/bin/python3"
+RUN /usr/bin/pip3 install build
+
+ENV CCACHE_WRAPPERSDIR "/usr/libexec/ccache-wrappers"
+ENV LANG "en_US.UTF-8"
+ENV MAKE "/usr/bin/make"
+ENV NINJA "/usr/bin/ninja"
+ENV PYTHON "/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/centos-stream-9.sh` & `libvirt-python-9.5.0/ci/buildenv/centos-stream-9.sh`

 * *Files 12% similar despite different names*

```diff
@@ -20,17 +20,19 @@
         pkgconfig \
         python3 \
         python3-devel \
         python3-lxml \
         python3-pip \
         python3-pytest \
         python3-setuptools \
+        python3-wheel \
         rpm-build
     rpm -qa | sort > /packages.txt
     mkdir -p /usr/libexec/ccache-wrappers
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
+    /usr/bin/pip3 install build
 }
 
 export CCACHE_WRAPPERSDIR="/usr/libexec/ccache-wrappers"
 export LANG="en_US.UTF-8"
 export PYTHON="/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/debian-10.sh` & `libvirt-python-9.5.0/ci/buildenv/debian-10.sh`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,22 @@
             locales \
             pkgconf \
             python3 \
             python3-dev \
             python3-lxml \
             python3-pip \
             python3-pytest \
-            python3-setuptools
+            python3-setuptools \
+            python3-venv \
+            python3-wheel
     sed -Ei 's,^# (en_US\.UTF-8 .*)$,\1,' /etc/locale.gen
     dpkg-reconfigure locales
     dpkg-query --showformat '${Package}_${Version}_${Architecture}\n' --show > /packages.txt
     mkdir -p /usr/libexec/ccache-wrappers
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
+    /usr/bin/pip3 install build
 }
 
 export CCACHE_WRAPPERSDIR="/usr/libexec/ccache-wrappers"
 export LANG="en_US.UTF-8"
 export PYTHON="/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/debian-sid.sh` & `libvirt-python-9.5.0/ci/buildenv/ubuntu-2004.sh`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,22 @@
             locales \
             pkgconf \
             python3 \
             python3-dev \
             python3-lxml \
             python3-pip \
             python3-pytest \
-            python3-setuptools
+            python3-setuptools \
+            python3-venv \
+            python3-wheel
     sed -Ei 's,^# (en_US\.UTF-8 .*)$,\1,' /etc/locale.gen
     dpkg-reconfigure locales
     dpkg-query --showformat '${Package}_${Version}_${Architecture}\n' --show > /packages.txt
     mkdir -p /usr/libexec/ccache-wrappers
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
+    /usr/bin/pip3 install build
 }
 
 export CCACHE_WRAPPERSDIR="/usr/libexec/ccache-wrappers"
 export LANG="en_US.UTF-8"
 export PYTHON="/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/fedora-37.sh` & `libvirt-python-9.5.0/ci/buildenv/opensuse-leap-15.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
 function install_buildenv() {
-    dnf update -y
-    dnf install -y \
-        ca-certificates \
-        ccache \
-        gcc \
-        git \
-        glibc-langpack-en \
-        libvirt-devel \
-        pkgconfig \
-        python3 \
-        python3-devel \
-        python3-lxml \
-        python3-pip \
-        python3-pytest \
-        python3-setuptools \
-        rpm-build
+    zypper update -y
+    zypper install -y \
+           ca-certificates \
+           ccache \
+           gcc \
+           git \
+           glibc-locale \
+           libvirt-devel \
+           pkgconfig \
+           python3-base \
+           python3-devel \
+           python3-lxml \
+           python3-pip \
+           python3-pytest \
+           python3-setuptools \
+           python3-wheel \
+           rpm-build
     rpm -qa | sort > /packages.txt
     mkdir -p /usr/libexec/ccache-wrappers
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
+    /usr/bin/pip3 install build
 }
 
 export CCACHE_WRAPPERSDIR="/usr/libexec/ccache-wrappers"
 export LANG="en_US.UTF-8"
 export PYTHON="/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/fedora-38.sh` & `libvirt-python-9.5.0/ci/buildenv/fedora-rawhide.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
 function install_buildenv() {
-    dnf update -y
+    dnf update -y --nogpgcheck fedora-gpg-keys
+    dnf distro-sync -y
     dnf install -y \
         ca-certificates \
         ccache \
         gcc \
         git \
         glibc-langpack-en \
         libvirt-devel \
         pkgconfig \
         python3 \
+        python3-build \
         python3-devel \
         python3-lxml \
         python3-pip \
         python3-pytest \
         python3-setuptools \
         rpm-build
     rpm -qa | sort > /packages.txt
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/fedora-rawhide.sh` & `libvirt-python-9.5.0/ci/buildenv/fedora-37.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
 function install_buildenv() {
-    dnf update -y --nogpgcheck fedora-gpg-keys
-    dnf distro-sync -y
+    dnf update -y
     dnf install -y \
         ca-certificates \
         ccache \
         gcc \
         git \
         glibc-langpack-en \
         libvirt-devel \
         pkgconfig \
         python3 \
+        python3-build \
         python3-devel \
         python3-lxml \
         python3-pip \
         python3-pytest \
         python3-setuptools \
         rpm-build
     rpm -qa | sort > /packages.txt
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/opensuse-leap-15.sh` & `libvirt-python-9.5.0/ci/buildenv/opensuse-tumbleweed.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
 function install_buildenv() {
-    zypper update -y
+    zypper dist-upgrade -y
     zypper install -y \
            ca-certificates \
            ccache \
            gcc \
            git \
            glibc-locale \
            libvirt-devel \
            pkgconfig \
            python3-base \
            python3-devel \
            python3-lxml \
            python3-pip \
            python3-pytest \
            python3-setuptools \
+           python3-wheel \
            rpm-build
     rpm -qa | sort > /packages.txt
     mkdir -p /usr/libexec/ccache-wrappers
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
+    /usr/bin/pip3 install build
 }
 
 export CCACHE_WRAPPERSDIR="/usr/libexec/ccache-wrappers"
 export LANG="en_US.UTF-8"
 export PYTHON="/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/opensuse-tumbleweed.sh` & `libvirt-python-9.5.0/ci/buildenv/fedora-38.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
 function install_buildenv() {
-    zypper dist-upgrade -y
-    zypper install -y \
-           ca-certificates \
-           ccache \
-           gcc \
-           git \
-           glibc-locale \
-           libvirt-devel \
-           pkgconfig \
-           python3-base \
-           python3-devel \
-           python3-lxml \
-           python3-pip \
-           python3-pytest \
-           python3-setuptools \
-           rpm-build
+    dnf update -y
+    dnf install -y \
+        ca-certificates \
+        ccache \
+        gcc \
+        git \
+        glibc-langpack-en \
+        libvirt-devel \
+        pkgconfig \
+        python3 \
+        python3-build \
+        python3-devel \
+        python3-lxml \
+        python3-pip \
+        python3-pytest \
+        python3-setuptools \
+        rpm-build
     rpm -qa | sort > /packages.txt
     mkdir -p /usr/libexec/ccache-wrappers
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
 }
 
 export CCACHE_WRAPPERSDIR="/usr/libexec/ccache-wrappers"
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/ubuntu-2004.sh` & `libvirt-python-9.5.0/ci/buildenv/ubuntu-2204.sh`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,22 @@
             locales \
             pkgconf \
             python3 \
             python3-dev \
             python3-lxml \
             python3-pip \
             python3-pytest \
-            python3-setuptools
+            python3-setuptools \
+            python3-venv \
+            python3-wheel
     sed -Ei 's,^# (en_US\.UTF-8 .*)$,\1,' /etc/locale.gen
     dpkg-reconfigure locales
     dpkg-query --showformat '${Package}_${Version}_${Architecture}\n' --show > /packages.txt
     mkdir -p /usr/libexec/ccache-wrappers
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
+    /usr/bin/pip3 install build
 }
 
 export CCACHE_WRAPPERSDIR="/usr/libexec/ccache-wrappers"
 export LANG="en_US.UTF-8"
 export PYTHON="/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/buildenv/ubuntu-2204.sh` & `libvirt-python-9.5.0/ci/buildenv/debian-sid.sh`

 * *Files 7% similar despite different names*

```diff
@@ -13,19 +13,21 @@
             ccache \
             gcc \
             git \
             libvirt-dev \
             locales \
             pkgconf \
             python3 \
+            python3-build \
             python3-dev \
             python3-lxml \
             python3-pip \
             python3-pytest \
-            python3-setuptools
+            python3-setuptools \
+            python3-venv
     sed -Ei 's,^# (en_US\.UTF-8 .*)$,\1,' /etc/locale.gen
     dpkg-reconfigure locales
     dpkg-query --showformat '${Package}_${Version}_${Architecture}\n' --show > /packages.txt
     mkdir -p /usr/libexec/ccache-wrappers
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
 }
```

### Comparing `libvirt-python-9.4.0/ci/containers/centos-stream-8.Dockerfile` & `libvirt-python-9.5.0/ci/buildenv/centos-stream-8.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
-FROM quay.io/centos/centos:stream8
-
-RUN dnf distro-sync -y && \
-    dnf install 'dnf-command(config-manager)' -y && \
-    dnf config-manager --set-enabled -y powertools && \
-    dnf install -y centos-release-advanced-virtualization && \
-    dnf install -y epel-release && \
-    dnf install -y epel-next-release && \
+function install_buildenv() {
+    dnf distro-sync -y
+    dnf install 'dnf-command(config-manager)' -y
+    dnf config-manager --set-enabled -y powertools
+    dnf install -y centos-release-advanced-virtualization
+    dnf install -y epel-release
+    dnf install -y epel-next-release
     dnf install -y \
         ca-certificates \
         ccache \
         cpp \
         gcc \
         gettext \
         git \
@@ -37,21 +36,22 @@
         python3 \
         python3-devel \
         python3-docutils \
         python3-lxml \
         python3-pip \
         python3-pytest \
         python3-setuptools \
+        python3-wheel \
         rpcgen \
-        rpm-build && \
-    dnf autoremove -y && \
-    dnf clean all -y && \
-    rpm -qa | sort > /packages.txt && \
-    mkdir -p /usr/libexec/ccache-wrappers && \
-    ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc && \
+        rpm-build
+    rpm -qa | sort > /packages.txt
+    mkdir -p /usr/libexec/ccache-wrappers
+    ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
+    /usr/bin/pip3 install build
+}
 
-ENV CCACHE_WRAPPERSDIR "/usr/libexec/ccache-wrappers"
-ENV LANG "en_US.UTF-8"
-ENV MAKE "/usr/bin/make"
-ENV NINJA "/usr/bin/ninja"
-ENV PYTHON "/usr/bin/python3"
+export CCACHE_WRAPPERSDIR="/usr/libexec/ccache-wrappers"
+export LANG="en_US.UTF-8"
+export MAKE="/usr/bin/make"
+export NINJA="/usr/bin/ninja"
+export PYTHON="/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/containers/centos-stream-9.Dockerfile` & `libvirt-python-9.5.0/ci/containers/centos-stream-9.Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,21 @@
         pkgconfig \
         python3 \
         python3-devel \
         python3-lxml \
         python3-pip \
         python3-pytest \
         python3-setuptools \
+        python3-wheel \
         rpm-build && \
     dnf autoremove -y && \
     dnf clean all -y && \
     rpm -qa | sort > /packages.txt && \
     mkdir -p /usr/libexec/ccache-wrappers && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
 
+RUN /usr/bin/pip3 install build
+
 ENV CCACHE_WRAPPERSDIR "/usr/libexec/ccache-wrappers"
 ENV LANG "en_US.UTF-8"
 ENV PYTHON "/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/containers/debian-10.Dockerfile` & `libvirt-python-9.5.0/ci/containers/debian-10.Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,24 @@
                       locales \
                       pkgconf \
                       python3 \
                       python3-dev \
                       python3-lxml \
                       python3-pip \
                       python3-pytest \
-                      python3-setuptools && \
+                      python3-setuptools \
+                      python3-venv \
+                      python3-wheel && \
     eatmydata apt-get autoremove -y && \
     eatmydata apt-get autoclean -y && \
     sed -Ei 's,^# (en_US\.UTF-8 .*)$,\1,' /etc/locale.gen && \
     dpkg-reconfigure locales && \
     dpkg-query --showformat '${Package}_${Version}_${Architecture}\n' --show > /packages.txt && \
     mkdir -p /usr/libexec/ccache-wrappers && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
 
+RUN /usr/bin/pip3 install build
+
 ENV CCACHE_WRAPPERSDIR "/usr/libexec/ccache-wrappers"
 ENV LANG "en_US.UTF-8"
 ENV PYTHON "/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/containers/debian-sid.Dockerfile` & `libvirt-python-9.5.0/ci/containers/ubuntu-2004.Dockerfile`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
-FROM docker.io/library/debian:sid-slim
+FROM docker.io/library/ubuntu:20.04
 
 RUN export DEBIAN_FRONTEND=noninteractive && \
     apt-get update && \
     apt-get install -y eatmydata && \
     eatmydata apt-get dist-upgrade -y && \
     eatmydata apt-get install --no-install-recommends -y \
                       ca-certificates \
@@ -19,20 +19,24 @@
                       locales \
                       pkgconf \
                       python3 \
                       python3-dev \
                       python3-lxml \
                       python3-pip \
                       python3-pytest \
-                      python3-setuptools && \
+                      python3-setuptools \
+                      python3-venv \
+                      python3-wheel && \
     eatmydata apt-get autoremove -y && \
     eatmydata apt-get autoclean -y && \
     sed -Ei 's,^# (en_US\.UTF-8 .*)$,\1,' /etc/locale.gen && \
     dpkg-reconfigure locales && \
     dpkg-query --showformat '${Package}_${Version}_${Architecture}\n' --show > /packages.txt && \
     mkdir -p /usr/libexec/ccache-wrappers && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
 
+RUN /usr/bin/pip3 install build
+
 ENV CCACHE_WRAPPERSDIR "/usr/libexec/ccache-wrappers"
 ENV LANG "en_US.UTF-8"
 ENV PYTHON "/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/containers/fedora-37.Dockerfile` & `libvirt-python-9.5.0/ci/containers/fedora-37.Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
                ccache \
                gcc \
                git \
                glibc-langpack-en \
                libvirt-devel \
                pkgconfig \
                python3 \
+               python3-build \
                python3-devel \
                python3-lxml \
                python3-pip \
                python3-pytest \
                python3-setuptools \
                rpm-build && \
     nosync dnf autoremove -y && \
```

### Comparing `libvirt-python-9.4.0/ci/containers/fedora-38.Dockerfile` & `libvirt-python-9.5.0/ci/containers/fedora-38.Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
                ccache \
                gcc \
                git \
                glibc-langpack-en \
                libvirt-devel \
                pkgconfig \
                python3 \
+               python3-build \
                python3-devel \
                python3-lxml \
                python3-pip \
                python3-pytest \
                python3-setuptools \
                rpm-build && \
     nosync dnf autoremove -y && \
```

### Comparing `libvirt-python-9.4.0/ci/containers/fedora-rawhide.Dockerfile` & `libvirt-python-9.5.0/ci/containers/fedora-rawhide.Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
                ccache \
                gcc \
                git \
                glibc-langpack-en \
                libvirt-devel \
                pkgconfig \
                python3 \
+               python3-build \
                python3-devel \
                python3-lxml \
                python3-pip \
                python3-pytest \
                python3-setuptools \
                rpm-build && \
     nosync dnf autoremove -y && \
```

### Comparing `libvirt-python-9.4.0/ci/containers/opensuse-leap-15.Dockerfile` & `libvirt-python-9.5.0/ci/containers/opensuse-tumbleweed.Dockerfile`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
-FROM registry.opensuse.org/opensuse/leap:15.4
+FROM registry.opensuse.org/opensuse/tumbleweed:latest
 
-RUN zypper update -y && \
+RUN zypper dist-upgrade -y && \
     zypper install -y \
            ca-certificates \
            ccache \
            gcc \
            git \
            glibc-locale \
            libvirt-devel \
            pkgconfig \
            python3-base \
            python3-devel \
            python3-lxml \
            python3-pip \
            python3-pytest \
            python3-setuptools \
+           python3-wheel \
            rpm-build && \
     zypper clean --all && \
     rpm -qa | sort > /packages.txt && \
     mkdir -p /usr/libexec/ccache-wrappers && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
 
+RUN /usr/bin/pip3 install build
+
 ENV CCACHE_WRAPPERSDIR "/usr/libexec/ccache-wrappers"
 ENV LANG "en_US.UTF-8"
 ENV PYTHON "/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/containers/opensuse-tumbleweed.Dockerfile` & `libvirt-python-9.5.0/ci/containers/opensuse-leap-15.Dockerfile`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
-FROM registry.opensuse.org/opensuse/tumbleweed:latest
+FROM registry.opensuse.org/opensuse/leap:15.5
 
-RUN zypper dist-upgrade -y && \
+RUN zypper update -y && \
     zypper install -y \
            ca-certificates \
            ccache \
            gcc \
            git \
            glibc-locale \
            libvirt-devel \
            pkgconfig \
            python3-base \
            python3-devel \
            python3-lxml \
            python3-pip \
            python3-pytest \
            python3-setuptools \
+           python3-wheel \
            rpm-build && \
     zypper clean --all && \
     rpm -qa | sort > /packages.txt && \
     mkdir -p /usr/libexec/ccache-wrappers && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
 
+RUN /usr/bin/pip3 install build
+
 ENV CCACHE_WRAPPERSDIR "/usr/libexec/ccache-wrappers"
 ENV LANG "en_US.UTF-8"
 ENV PYTHON "/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/containers/ubuntu-2004.Dockerfile` & `libvirt-python-9.5.0/ci/containers/ubuntu-2204.Dockerfile`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
-FROM docker.io/library/ubuntu:20.04
+FROM docker.io/library/ubuntu:22.04
 
 RUN export DEBIAN_FRONTEND=noninteractive && \
     apt-get update && \
     apt-get install -y eatmydata && \
     eatmydata apt-get dist-upgrade -y && \
     eatmydata apt-get install --no-install-recommends -y \
                       ca-certificates \
@@ -19,20 +19,24 @@
                       locales \
                       pkgconf \
                       python3 \
                       python3-dev \
                       python3-lxml \
                       python3-pip \
                       python3-pytest \
-                      python3-setuptools && \
+                      python3-setuptools \
+                      python3-venv \
+                      python3-wheel && \
     eatmydata apt-get autoremove -y && \
     eatmydata apt-get autoclean -y && \
     sed -Ei 's,^# (en_US\.UTF-8 .*)$,\1,' /etc/locale.gen && \
     dpkg-reconfigure locales && \
     dpkg-query --showformat '${Package}_${Version}_${Architecture}\n' --show > /packages.txt && \
     mkdir -p /usr/libexec/ccache-wrappers && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/gcc
 
+RUN /usr/bin/pip3 install build
+
 ENV CCACHE_WRAPPERSDIR "/usr/libexec/ccache-wrappers"
 ENV LANG "en_US.UTF-8"
 ENV PYTHON "/usr/bin/python3"
```

### Comparing `libvirt-python-9.4.0/ci/containers/ubuntu-2204.Dockerfile` & `libvirt-python-9.5.0/ci/containers/debian-sid.Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
-FROM docker.io/library/ubuntu:22.04
+FROM docker.io/library/debian:sid-slim
 
 RUN export DEBIAN_FRONTEND=noninteractive && \
     apt-get update && \
     apt-get install -y eatmydata && \
     eatmydata apt-get dist-upgrade -y && \
     eatmydata apt-get install --no-install-recommends -y \
                       ca-certificates \
                       ccache \
                       gcc \
                       git \
                       libvirt-dev \
                       locales \
                       pkgconf \
                       python3 \
+                      python3-build \
                       python3-dev \
                       python3-lxml \
                       python3-pip \
                       python3-pytest \
-                      python3-setuptools && \
+                      python3-setuptools \
+                      python3-venv && \
     eatmydata apt-get autoremove -y && \
     eatmydata apt-get autoclean -y && \
     sed -Ei 's,^# (en_US\.UTF-8 .*)$,\1,' /etc/locale.gen && \
     dpkg-reconfigure locales && \
     dpkg-query --showformat '${Package}_${Version}_${Architecture}\n' --show > /packages.txt && \
     mkdir -p /usr/libexec/ccache-wrappers && \
     ln -s /usr/bin/ccache /usr/libexec/ccache-wrappers/cc && \
```

### Comparing `libvirt-python-9.4.0/ci/gitlab/build-templates.yml` & `libvirt-python-9.5.0/ci/gitlab/build-templates.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/ci/gitlab/builds.yml` & `libvirt-python-9.5.0/ci/gitlab/builds.yml`

 * *Files 1% similar despite different names*

```diff
@@ -41,28 +41,28 @@
   allow_failure: false
   variables:
     NAME: centos-stream-8
   artifacts:
     expire_in: 2 days
     paths:
       - scratch
-      - build
+      - dist
 
 x86_64-centos-stream-8-git-local-env:
   extends: .native_git_build_job_local_env
   needs: []
   allow_failure: false
   variables:
     IMAGE: quay.io/centos/centos:stream8
     NAME: centos-stream-8
   artifacts:
     expire_in: 2 days
     paths:
       - scratch
-      - build
+      - dist
 
 
 x86_64-centos-stream-9-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
     - job: x86_64-centos-stream-9-container
       optional: true
@@ -206,15 +206,15 @@
     RPM: skip
 
 x86_64-opensuse-leap-15-local-env:
   extends: .native_build_job_local_env
   needs: []
   allow_failure: false
   variables:
-    IMAGE: registry.opensuse.org/opensuse/leap:15.4
+    IMAGE: registry.opensuse.org/opensuse/leap:15.5
     NAME: opensuse-leap-15
     RPM: skip
 
 
 x86_64-opensuse-tumbleweed-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
```

### Comparing `libvirt-python-9.4.0/ci/gitlab/container-templates.yml` & `libvirt-python-9.5.0/ci/gitlab/container-templates.yml`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  - In upstream, for push to default branch with CI changes.
 #  - In upstream, on request, for scheduled/manual pipelines
 #    against default branch
 #
 # Note: never publish from merge requests since they have non-committed code
 #
 .container_job:
-  image: docker:stable
+  image: docker:latest
   stage: containers
   interruptible: false
   needs: []
   services:
     - docker:dind
   before_script:
     - export TAG="$CI_REGISTRY_IMAGE/ci-$NAME:latest"
```

### Comparing `libvirt-python-9.4.0/ci/gitlab/containers.yml` & `libvirt-python-9.5.0/ci/gitlab/containers.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/ci/gitlab/sanity-checks.yml` & `libvirt-python-9.5.0/ci/gitlab/sanity-checks.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/ci/gitlab.yml` & `libvirt-python-9.5.0/ci/gitlab.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/ci/manifest.yml` & `libvirt-python-9.5.0/ci/manifest.yml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       - arch: x86_64
         template: .native_git_build_job
         suffix: -git
         artifacts:
           expire_in: 2 days
           paths:
             - scratch
-            - build
+            - dist
 
   centos-stream-9:
     jobs:
       - arch: x86_64
         artifacts:
           expire_in: 1 hour
           paths:
```

### Comparing `libvirt-python-9.4.0/examples/README` & `libvirt-python-9.5.0/examples/README`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/consolecallback.py` & `libvirt-python-9.5.0/examples/consolecallback.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/dhcpleases.py` & `libvirt-python-9.5.0/examples/dhcpleases.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/dominfo.py` & `libvirt-python-9.5.0/examples/dominfo.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/domipaddrs.py` & `libvirt-python-9.5.0/examples/domipaddrs.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/domrestore.py` & `libvirt-python-9.5.0/examples/domrestore.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/domsave.py` & `libvirt-python-9.5.0/examples/domsave.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/domstart.py` & `libvirt-python-9.5.0/examples/domstart.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/esxlist.py` & `libvirt-python-9.5.0/examples/esxlist.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/event-test.py` & `libvirt-python-9.5.0/examples/event-test.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/guest-vcpus/guest-vcpu-daemon.py` & `libvirt-python-9.5.0/examples/guest-vcpus/guest-vcpu-daemon.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/guest-vcpus/guest-vcpu.py` & `libvirt-python-9.5.0/examples/guest-vcpus/guest-vcpu.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/nodestats.py` & `libvirt-python-9.5.0/examples/nodestats.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/sparsestream.py` & `libvirt-python-9.5.0/examples/sparsestream.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/examples/topology.py` & `libvirt-python-9.5.0/examples/topology.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/generator.py` & `libvirt-python-9.5.0/generator.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-lxc-override-api.xml` & `libvirt-python-9.5.0/libvirt-lxc-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-lxc-override.c` & `libvirt-python-9.5.0/libvirt-lxc-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-override-api.xml` & `libvirt-python-9.5.0/libvirt-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-override-virConnect.py` & `libvirt-python-9.5.0/libvirt-override-virConnect.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-override-virDomain.py` & `libvirt-python-9.5.0/libvirt-override-virDomain.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-override-virDomainCheckpoint.py` & `libvirt-python-9.5.0/libvirt-override-virDomainCheckpoint.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-override-virDomainSnapshot.py` & `libvirt-python-9.5.0/libvirt-override-virDomainSnapshot.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-override-virStream.py` & `libvirt-python-9.5.0/libvirt-override-virStream.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-override.c` & `libvirt-python-9.5.0/libvirt-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-override.py` & `libvirt-python-9.5.0/libvirt-override.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-python.spec` & `libvirt-python-9.5.0/libvirt-python.spec`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     %define supported_platform 1
 %else
     %define supported_platform 0
 %endif
 
 Summary: The libvirt virtualization API python3 binding
 Name: libvirt-python
-Version: 9.4.0
+Version: 9.5.0
 Release: 1%{?dist}
 Source0: https://libvirt.org/sources/python/%{name}-%{version}.tar.gz
 Url: https://libvirt.org
 License: LGPL-2.1-or-later
 BuildRequires: libvirt-devel == %{version}
 BuildRequires: python3-devel
 BuildRequires: python3-pytest
@@ -66,18 +66,18 @@
 
 %py3_build
 
 %install
 %py3_install
 
 %check
-%{__python3} setup.py test
+%pytest
 
 %files -n python3-libvirt
-%doc ChangeLog AUTHORS README COPYING COPYING.LESSER examples/
+%doc ChangeLog AUTHORS README COPYING examples/
 %{python3_sitearch}/libvirt.py*
 %{python3_sitearch}/libvirtaio.py*
 %{python3_sitearch}/libvirt_qemu.py*
 %{python3_sitearch}/libvirt_lxc.py*
 %{python3_sitearch}/__pycache__/libvirt.cpython-*.py*
 %{python3_sitearch}/__pycache__/libvirt_qemu.cpython-*.py*
 %{python3_sitearch}/__pycache__/libvirt_lxc.cpython-*.py*
```

### Comparing `libvirt-python-9.4.0/libvirt-python.spec.in` & `libvirt-python-9.5.0/libvirt-python.spec.in`

 * *Files 8% similar despite different names*

```diff
@@ -66,18 +66,18 @@
 
 %py3_build
 
 %install
 %py3_install
 
 %check
-%{__python3} setup.py test
+%pytest
 
 %files -n python3-libvirt
-%doc ChangeLog AUTHORS README COPYING COPYING.LESSER examples/
+%doc ChangeLog AUTHORS README COPYING examples/
 %{python3_sitearch}/libvirt.py*
 %{python3_sitearch}/libvirtaio.py*
 %{python3_sitearch}/libvirt_qemu.py*
 %{python3_sitearch}/libvirt_lxc.py*
 %{python3_sitearch}/__pycache__/libvirt.cpython-*.py*
 %{python3_sitearch}/__pycache__/libvirt_qemu.cpython-*.py*
 %{python3_sitearch}/__pycache__/libvirt_lxc.cpython-*.py*
```

### Comparing `libvirt-python-9.4.0/libvirt-qemu-override-api.xml` & `libvirt-python-9.5.0/libvirt-qemu-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-qemu-override.c` & `libvirt-python-9.5.0/libvirt-qemu-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-qemu-override.py` & `libvirt-python-9.5.0/libvirt-qemu-override.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-utils.c` & `libvirt-python-9.5.0/libvirt-utils.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirt-utils.h` & `libvirt-python-9.5.0/libvirt-utils.h`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/libvirtaio.py` & `libvirt-python-9.5.0/libvirtaio.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/tests/eventmock.py` & `libvirt-python-9.5.0/tests/eventmock.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/tests/test_aio.py` & `libvirt-python-9.5.0/tests/test_aio.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/tests/test_api_coverage.py` & `libvirt-python-9.5.0/tests/test_api_coverage.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/tests/test_conn.py` & `libvirt-python-9.5.0/tests/test_conn.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/tests/test_domain.py` & `libvirt-python-9.5.0/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/tests/test_domain_checkpoint.py` & `libvirt-python-9.5.0/tests/test_domain_checkpoint.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/tests/test_storage.py` & `libvirt-python-9.5.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/typewrappers.c` & `libvirt-python-9.5.0/typewrappers.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.4.0/typewrappers.h` & `libvirt-python-9.5.0/typewrappers.h`

 * *Files identical despite different names*

