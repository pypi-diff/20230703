# Comparing `tmp/PyFakeDados-0.0.5.1.tar.gz` & `tmp/PyFakeDados-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFakeDados-0.0.5.1.tar", last modified: Fri Jun 30 19:06:38 2023, max compression
+gzip compressed data, was "PyFakeDados-0.0.5.2.tar", last modified: Mon Jul  3 01:04:56 2023, max compression
```

## Comparing `PyFakeDados-0.0.5.1.tar` & `PyFakeDados-0.0.5.2.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 19:06:38.869212 PyFakeDados-0.0.5.1/
--rw-rw-rw-   0        0        0    35821 2023-06-29 17:33:57.000000 PyFakeDados-0.0.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0       29 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3486 2023-06-30 19:06:38.870066 PyFakeDados-0.0.5.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 19:06:38.829006 PyFakeDados-0.0.5.1/PyFakeDados/
--rw-rw-rw-   0        0        0       23 2023-06-30 19:01:18.000000 PyFakeDados-0.0.5.1/PyFakeDados/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/bairro.py
--rw-rw-rw-   0        0        0     1711 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/cep.py
--rw-rw-rw-   0        0        0     1823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/cnpj.py
--rw-rw-rw-   0        0        0     1533 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/cpf.py
--rw-rw-rw-   0        0        0      184 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/ctps.py
--rw-rw-rw-   0        0        0      849 2023-06-30 17:24:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/email.py
--rw-rw-rw-   0        0        0     5379 2023-06-30 18:58:05.000000 PyFakeDados-0.0.5.1/PyFakeDados/empresa.py
--rw-rw-rw-   0        0        0     1798 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/estado.py
--rw-rw-rw-   0        0        0      170 2023-06-29 19:04:37.000000 PyFakeDados-0.0.5.1/PyFakeDados/inscricao_estadual.py
--rw-rw-rw-   0        0        0      823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/logradouro.py
--rw-rw-rw-   0        0        0     1417 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/municipio.py
--rw-rw-rw-   0        0        0     3360 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/nome.py
--rw-rw-rw-   0        0        0     2965 2023-06-30 18:29:17.000000 PyFakeDados-0.0.5.1/PyFakeDados/pessoa.py
--rw-rw-rw-   0        0        0      177 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/pis.py
--rw-rw-rw-   0        0        0      657 2023-06-30 15:02:53.000000 PyFakeDados-0.0.5.1/PyFakeDados/rg.py
--rw-rw-rw-   0        0        0      400 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/senha.py
--rw-rw-rw-   0        0        0      411 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/site.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:06:38.865958 PyFakeDados-0.0.5.1/PyFakeDados/src/
--rw-rw-rw-   0        0        0     1043 2023-06-29 20:04:40.000000 PyFakeDados-0.0.5.1/PyFakeDados/src/estados.csv
--rw-rw-rw-   0        0        0   358545 2023-06-29 20:09:31.000000 PyFakeDados-0.0.5.1/PyFakeDados/src/municipios.csv
--rw-rw-rw-   0        0        0     1886 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/telefone.py
--rw-rw-rw-   0        0        0     2145 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:06:38.859601 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/
--rw-rw-rw-   0        0        0     3486 2023-06-30 19:06:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      759 2023-06-30 19:06:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 19:06:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 13:11:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-30 19:06:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 19:06:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2841 2023-06-30 15:02:58.000000 PyFakeDados-0.0.5.1/README.md
--rw-rw-rw-   0        0        0      848 2023-06-30 19:06:38.871083 PyFakeDados-0.0.5.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-06-29 17:33:57.000000 PyFakeDados-0.0.5.1/setup.py
+drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-07-03 01:04:56.811155 PyFakeDados-0.0.5.2/
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)    35148 2023-06-29 22:25:25.000000 PyFakeDados-0.0.5.2/LICENSE.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       29 2023-06-30 02:34:23.000000 PyFakeDados-0.0.5.2/MANIFEST.in
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3406 2023-07-03 01:04:56.811155 PyFakeDados-0.0.5.2/PKG-INFO
+drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-07-03 01:04:56.811155 PyFakeDados-0.0.5.2/PyFakeDados/
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)   922861 2023-07-03 00:37:28.000000 PyFakeDados-0.0.5.2/PyFakeDados/CONSTANTS.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       23 2023-07-03 01:02:38.000000 PyFakeDados-0.0.5.2/PyFakeDados/__init__.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      857 2023-06-29 22:47:13.000000 PyFakeDados-0.0.5.2/PyFakeDados/bairro.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1661 2023-06-30 03:02:42.000000 PyFakeDados-0.0.5.2/PyFakeDados/cep.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1771 2023-06-29 23:29:37.000000 PyFakeDados-0.0.5.2/PyFakeDados/cnpj.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1487 2023-06-29 23:59:11.000000 PyFakeDados-0.0.5.2/PyFakeDados/cpf.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      177 2023-06-30 00:10:57.000000 PyFakeDados-0.0.5.2/PyFakeDados/ctps.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      823 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/PyFakeDados/email.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     5250 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/PyFakeDados/empresa.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      489 2023-07-03 00:41:15.000000 PyFakeDados-0.0.5.2/PyFakeDados/estado.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      164 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/PyFakeDados/inscricao_estadual.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      798 2023-06-29 22:57:01.000000 PyFakeDados-0.0.5.2/PyFakeDados/logradouro.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      446 2023-07-03 00:29:57.000000 PyFakeDados-0.0.5.2/PyFakeDados/municipio.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3278 2023-06-30 00:32:32.000000 PyFakeDados-0.0.5.2/PyFakeDados/nome.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2872 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/PyFakeDados/pessoa.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      170 2023-06-30 00:12:54.000000 PyFakeDados-0.0.5.2/PyFakeDados/pis.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      630 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/PyFakeDados/rg.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      389 2023-06-30 00:36:02.000000 PyFakeDados-0.0.5.2/PyFakeDados/senha.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      399 2023-06-30 03:01:14.000000 PyFakeDados-0.0.5.2/PyFakeDados/site.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1820 2023-06-30 03:00:58.000000 PyFakeDados-0.0.5.2/PyFakeDados/telefone.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2119 2023-07-03 00:42:12.000000 PyFakeDados-0.0.5.2/PyFakeDados/utils.py
+drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-07-03 01:04:56.811155 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3406 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/PKG-INFO
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      725 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/SOURCES.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)        1 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/dependency_links.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)        1 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/not-zip-safe
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       10 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/requires.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       12 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/top_level.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2777 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/README.md
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      819 2023-07-03 01:04:56.811155 PyFakeDados-0.0.5.2/setup.cfg
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       38 2023-06-29 22:25:25.000000 PyFakeDados-0.0.5.2/setup.py
```

### Comparing `PyFakeDados-0.0.5.1/LICENSE.txt` & `PyFakeDados-0.0.5.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `PyFakeDados-0.0.5.1/PKG-INFO` & `PyFakeDados-0.0.5.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-Metadata-Version: 2.1
-Name: PyFakeDados
-Version: 0.0.5.1
-Summary: Generic generator fake data for application and api development.
-Home-page: https://github.com/juliansantosinfo/PyFakeDados
-Author: Julian de Almeida Santos
-Author-email: julian.santos.info@gmail.com
-License: GPLv3
-Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
-Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# PyFakeDados
-
-![PyFakeDados](https://github.com/juliansantosinfo/PyFakeDados/logo.png)
-
-PyFakeDados é uma ferramenta em Python que auxilia desenvolvedores na geração de dados falsos (fake) aleatórios para bancos de dados de teste ou APIs. Com essa ferramenta, é possível gerar uma variedade de informações, como nomes, telefones, CPFs, e-mails, senhas e muito mais.
-
-O PyFakeDados oferece uma ampla gama de recursos para gerar dados em diversos formatos, como nomes, endereços, números de telefone, documentos como CPFs e CNPJs, e-mails, senhas, entre outros. Além disso, a ferramenta permite criar identidades completas de pessoas e empresas, fornecendo informações consistentes e realistas.
-
-A biblioteca é de fácil utilização e pode ser integrada facilmente a projetos em Python. Com uma simples chamada de função, você pode gerar quantidades massivas de dados falsos para preencher suas necessidades de teste. A diversidade dos dados gerados e a capacidade de personalização tornam o PyFakeDados uma ferramenta indispensável para qualquer desenvolvedor que precise de dados fictícios em seus projetos.
-
-Este repositório também fornece documentação completa sobre como usar a biblioteca e exemplos práticos para ajudá-lo a aproveitar ao máximo todas as funcionalidades do PyFakeDados.
-
-Experimente o PyFakeDados agora e torne o processo de geração de dados falsos mais eficiente e realista em seus projetos!
-
-## Recursos
-
-PyFakeDados é capaz de gerar os seguintes tipos de dados:
-
-- Nome
-- Sobrenome
-- Nome completo
-- Nome com filiação
-- Telefone fixo
-- Telefone celular
-- CPF
-- RG
-- PIS
-- CTPS
-- CNPJ
-- Inscrição estadual
-- E-mail
-- Site
-- Senhas
-
-Além disso, a ferramenta também é capaz de gerar agrupamentos de dados, formando identidades de pessoas e empresas.
-
-## Instalação
-
-Você pode instalar o PyFakeDados através do pip, executando o seguinte comando:
-
-```shell
-pip install PyFakeDados
-```
-
-## Uso
-
-Para utilizar o PyFakeDados em seu projeto, importe o pacote e utilize as funções correspondentes aos tipos de dados que deseja gerar. Por exemplo, para gerar um nome completo, utilize a função `gerar_nome_completo()`.
-
-```python
-from pyfakedados import gerar_nome_completo
-
-nome_completo = gerar_nome_completo()
-print(nome_completo)
-```
-
-Para mais exemplos de uso, consulte a documentação disponível em [link_da_documentacao](https://github.com/seu-usuario/repositorio/documentacao.md).
-
-## Contribuição
-
-Contribuições são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request* com melhorias, correções de bugs ou novos recursos.
-
-## Licença
-
-Este projeto é licenciado sob a [GPL-3.0 License](https://raw.githubusercontent.com/juliansantosinfo/PyFakeDados/main/LICENSE.txt).
+Metadata-Version: 2.1
+Name: PyFakeDados
+Version: 0.0.5.2
+Summary: Generic generator fake data for application and api development.
+Home-page: https://github.com/juliansantosinfo/PyFakeDados
+Author: Julian de Almeida Santos
+Author-email: julian.santos.info@gmail.com
+License: GPLv3
+Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
+Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# PyFakeDados
+
+![PyFakeDados](https://github.com/juliansantosinfo/PyFakeDados/logo.png)
+
+PyFakeDados é uma ferramenta em Python que auxilia desenvolvedores na geração de dados falsos (fake) aleatórios para bancos de dados de teste ou APIs. Com essa ferramenta, é possível gerar uma variedade de informações, como nomes, telefones, CPFs, e-mails, senhas e muito mais.
+
+O PyFakeDados oferece uma ampla gama de recursos para gerar dados em diversos formatos, como nomes, endereços, números de telefone, documentos como CPFs e CNPJs, e-mails, senhas, entre outros. Além disso, a ferramenta permite criar identidades completas de pessoas e empresas, fornecendo informações consistentes e realistas.
+
+A biblioteca é de fácil utilização e pode ser integrada facilmente a projetos em Python. Com uma simples chamada de função, você pode gerar quantidades massivas de dados falsos para preencher suas necessidades de teste. A diversidade dos dados gerados e a capacidade de personalização tornam o PyFakeDados uma ferramenta indispensável para qualquer desenvolvedor que precise de dados fictícios em seus projetos.
+
+Este repositório também fornece documentação completa sobre como usar a biblioteca e exemplos práticos para ajudá-lo a aproveitar ao máximo todas as funcionalidades do PyFakeDados.
+
+Experimente o PyFakeDados agora e torne o processo de geração de dados falsos mais eficiente e realista em seus projetos!
+
+## Recursos
+
+PyFakeDados é capaz de gerar os seguintes tipos de dados:
+
+- Nome
+- Sobrenome
+- Nome completo
+- Nome com filiação
+- Telefone fixo
+- Telefone celular
+- CPF
+- RG
+- PIS
+- CTPS
+- CNPJ
+- Inscrição estadual
+- E-mail
+- Site
+- Senhas
+
+Além disso, a ferramenta também é capaz de gerar agrupamentos de dados, formando identidades de pessoas e empresas.
+
+## Instalação
+
+Você pode instalar o PyFakeDados através do pip, executando o seguinte comando:
+
+```shell
+pip install PyFakeDados
+```
+
+## Uso
+
+Para utilizar o PyFakeDados em seu projeto, importe o pacote e utilize as funções correspondentes aos tipos de dados que deseja gerar. Por exemplo, para gerar um nome completo, utilize a função `gerar_nome_completo()`.
+
+```python
+from pyfakedados import gerar_nome_completo
+
+nome_completo = gerar_nome_completo()
+print(nome_completo)
+```
+
+Para mais exemplos de uso, consulte a documentação disponível em [link_da_documentacao](https://github.com/seu-usuario/repositorio/documentacao.md).
+
+## Contribuição
+
+Contribuições são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request* com melhorias, correções de bugs ou novos recursos.
+
+## Licença
+
+Este projeto é licenciado sob a [GPL-3.0 License](https://raw.githubusercontent.com/juliansantosinfo/PyFakeDados/main/LICENSE.txt).
```

### Comparing `PyFakeDados-0.0.5.1/PyFakeDados/bairro.py` & `PyFakeDados-0.0.5.2/PyFakeDados/bairro.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import random
-
-prefixos = [
-        'Alto', 'Baixo', 'Vila', 'Nova', 'Bela', 'Jardim', 'São', 'Santa', 'Bom', 'Grande',
-        'Sol', 'Mar', 'Cidade', 'Campo', 'Parque', 'Mira', 'Floresta', 'Canto', 'Lagoa', 'Praia',
-        'Verde', 'Dourado', 'Ouro', 'Monte', 'Vista', 'Primavera', 'Cipreste', 'Sereno', 'Vento',
-        'Porto', 'Pedra', 'Aurora', 'Brisa', 'Serrano', 'Sol Nascente', 'Maravilha', 'Celestial', 'Rio',
-        'Vale', 'Aconchego', 'Harmonia', 'Eterno', 'Sorriso', 'Céu Azul', 'Sonho', 'Alegria', 'Encantamento',
-        'Inspiração', 'Doce Lar', 'Azul', 'Estrela', 'Canto do Pássaro'
-    ]
-
-sufixos = ['Vista', 'Flores', 'Alegre', 'Verde', 'Luz', 'Sol', 'Mar', 'Norte', 'Sul', 'Leste', 'Oeste']
-
-def gerar_bairro():
-    
-    prefixo = random.choice(prefixos)
-    sufixo = random.choice(sufixos)
-    
-    return f'{prefixo} {sufixo}'
+import random
+
+prefixos = [
+        'Alto', 'Baixo', 'Vila', 'Nova', 'Bela', 'Jardim', 'São', 'Santa', 'Bom', 'Grande',
+        'Sol', 'Mar', 'Cidade', 'Campo', 'Parque', 'Mira', 'Floresta', 'Canto', 'Lagoa', 'Praia',
+        'Verde', 'Dourado', 'Ouro', 'Monte', 'Vista', 'Primavera', 'Cipreste', 'Sereno', 'Vento',
+        'Porto', 'Pedra', 'Aurora', 'Brisa', 'Serrano', 'Sol Nascente', 'Maravilha', 'Celestial', 'Rio',
+        'Vale', 'Aconchego', 'Harmonia', 'Eterno', 'Sorriso', 'Céu Azul', 'Sonho', 'Alegria', 'Encantamento',
+        'Inspiração', 'Doce Lar', 'Azul', 'Estrela', 'Canto do Pássaro'
+    ]
+
+sufixos = ['Vista', 'Flores', 'Alegre', 'Verde', 'Luz', 'Sol', 'Mar', 'Norte', 'Sul', 'Leste', 'Oeste']
+
+def gerar_bairro():
+    
+    prefixo = random.choice(prefixos)
+    sufixo = random.choice(sufixos)
+    
+    return f'{prefixo} {sufixo}'
```

### Comparing `PyFakeDados-0.0.5.1/PyFakeDados/cnpj.py` & `PyFakeDados-0.0.5.2/PyFakeDados/cpf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,46 @@
-import random
-import itertools
-
-def gerar_cnpj(mask=False):
-    
-    while True:
-
-        # Gera os oito primeiros dígitos do CNPJ de forma aleatória
-        cnpj = [random.randint(0, 9) for _ in range(8)]
-
-        # Gera os quatro dígitos de controle
-        cnpj += [0, 0, 0, 1]
-
-        # Calcula o primeiro dígito verificador
-        soma = sum(x * y for x, y in zip(cnpj, itertools.cycle(range(2, 10))))
-        cnpj.append((11 - (soma % 11)) % 11)
-
-        # Calcula o segundo dígito verificador
-        soma = sum(x * y for x, y in zip(cnpj, itertools.cycle(range(2, 10)))) + 2 * cnpj[8]
-        cnpj.append((11 - (soma % 11)) % 11)
-
-        # Verifica se o CNPJ gerado é válido
-        if validar_cnpj(''.join(map(str, cnpj))):
-            break
-    
-    if mask:
-        cnpj = f"{cnpj[0]}{cnpj[1]}.{cnpj[2]}{cnpj[3]}{cnpj[4]}.{cnpj[5]}{cnpj[6]}{cnpj[7]}/{cnpj[8]}{cnpj[9]}{cnpj[10]}{cnpj[11]}-{cnpj[12]}{cnpj[13]}"
-    else:
-        cnpj = ''.join([str(num) for num in cnpj])
-
-    # Retorna o CNPJ formatado (XX.XXX.XXX/XXXX-XX)
-    return cnpj
-
-def validar_cnpj(cnpj):
-    # Remove caracteres não numéricos do CNPJ
-    cnpj = ''.join(filter(str.isdigit, cnpj))
-
-    # Verifica se o CNPJ possui 14 dígitos
-    if len(cnpj) != 14:
-        return False
-
-    # Calcula o primeiro dígito verificador e compara com o CNPJ fornecido
-    soma = sum(int(x) * y for x, y in zip(cnpj[:12], itertools.cycle(range(2, 10))))
-    if (11 - (soma % 11)) % 11 != int(cnpj[12]):
-        return False
-
-    # Calcula o segundo dígito verificador e compara com o CNPJ fornecido
-    soma = sum(int(x) * y for x, y in zip(cnpj[:13], itertools.cycle(range(2, 10)))) + 2 * int(cnpj[12])
-    if (11 - (soma % 11)) % 11 != int(cnpj[13]):
-        return False
-
-    return True
+import random
+import itertools
+
+def validar_cpf(cpf):
+    # Remove caracteres não numéricos do CPF
+    cpf = ''.join(filter(str.isdigit, cpf))
+
+    # Verifica se o CPF possui 11 dígitos
+    if len(cpf) != 11:
+        return False
+
+    # Verifica se todos os dígitos são iguais
+    if cpf == cpf[0] * 11:
+        return False
+
+    # Calcula o primeiro dígito verificador e compara com o CPF fornecido
+    soma = sum(int(x) * y for x, y in zip(cpf[:9], itertools.count(10, -1)))
+    if (11 - (soma % 11)) % 11 != int(cpf[9]):
+        return False
+
+    # Calcula o segundo dígito verificador e compara com o CPF fornecido
+    soma = sum(int(x) * y for x, y in zip(cpf[:10], itertools.count(11, -1)))
+    if (11 - (soma % 11)) % 11 != int(cpf[10]):
+        return False
+
+    return True
+
+def gerar_cpf(mask=False):
+    # Gera os nove primeiros dígitos do CPF de forma aleatória
+    cpf = [random.randint(0, 9) for _ in range(9)]
+
+    # Calcula o primeiro dígito verificador
+    soma = sum(x * y for x, y in zip(cpf, itertools.count(10, -1)))
+    cpf.append((11 - (soma % 11)) % 11)
+
+    # Calcula o segundo dígito verificador
+    soma = sum(x * y for x, y in zip(cpf, itertools.count(11, -1)))
+    cpf.append((11 - (soma % 11)) % 11)
+
+    if mask:
+        cpf = f"{cpf[0]}{cpf[1]}{cpf[2]}.{cpf[3]}{cpf[4]}{cpf[5]}.{cpf[6]}{cpf[7]}{cpf[8]}-{cpf[9]}{cpf[10]}"
+    else:
+        cpf = ''.join([str(num) for num in cpf])
+
+    # Retorna o CPF formatado (XXX.XXX.XXX-XX)
+    return cpf
```

### Comparing `PyFakeDados-0.0.5.1/PyFakeDados/logradouro.py` & `PyFakeDados-0.0.5.2/PyFakeDados/logradouro.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import random
-
-tipos_logradouros = ['Rua', 'Avenida', 'Estrada', 'Beco', 'Travessa', 'Alameda', 'Viela']
-prefixos = ['Do', 'Dos', 'Das', 'De', 'Doutor', 'Dom', 'Vila', 'Chácara', 'Sítio']
-sufixos = ['Novo', 'Velho', 'Grande', 'Pequeno', 'Alto', 'Baixo', 'Leste', 'Oeste', 'Norte', 'Sul']
-
-def gerar_numero():
-    return str(random.randint(1,2000))
-
-def gerar_logradouro():
-    
-    tipo = random.choice(tipos_logradouros)
-    prefixo = random.choice(prefixos)
-    sufixo = random.choice(sufixos)
-    
-    return f'{tipo} {prefixo} {sufixo}'
-
-def gerar_logradouro_com_numero():
-    
-    tipo = random.choice(tipos_logradouros)
-    prefixo = random.choice(prefixos)
-    sufixo = random.choice(sufixos)
-    numero = str(random.randint(1,2000))
-    
-    return f'{tipo} {prefixo} {sufixo}, {numero}'
+import random
+
+tipos_logradouros = ['Rua', 'Avenida', 'Estrada', 'Beco', 'Travessa', 'Alameda', 'Viela']
+prefixos = ['Do', 'Dos', 'Das', 'De', 'Doutor', 'Dom', 'Vila', 'Chácara', 'Sítio']
+sufixos = ['Novo', 'Velho', 'Grande', 'Pequeno', 'Alto', 'Baixo', 'Leste', 'Oeste', 'Norte', 'Sul']
+
+def gerar_numero():
+    return str(random.randint(1,2000))
+
+def gerar_logradouro():
+    
+    tipo = random.choice(tipos_logradouros)
+    prefixo = random.choice(prefixos)
+    sufixo = random.choice(sufixos)
+    
+    return f'{tipo} {prefixo} {sufixo}'
+
+def gerar_logradouro_com_numero():
+    
+    tipo = random.choice(tipos_logradouros)
+    prefixo = random.choice(prefixos)
+    sufixo = random.choice(sufixos)
+    numero = str(random.randint(1,2000))
+    
+    return f'{tipo} {prefixo} {sufixo}, {numero}'
```

### Comparing `PyFakeDados-0.0.5.1/PyFakeDados/nome.py` & `PyFakeDados-0.0.5.2/PyFakeDados/nome.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import random
-
-SEXO_MASCULINO = 'M'
-SEXO_FEMININO = 'F'
-
-LISTA_SEXO = [SEXO_MASCULINO, SEXO_FEMININO]
-
-LISTA_NOMES_MASCULINOS = [
-    "Alex", "Bernardo", "Caio", "Daniel", "Eduardo", "Felipe", "Gabriel", "Henrique",
-    "Igor", "João", "Kauã", "Leonardo", "Matheus", "Nathan", "Otávio", "Pedro",
-    "Rafael", "Samuel", "Thiago", "Vitor", "Wagner", "Xavier", "Yuri", "Zélio",
-    "André", "Bruno", "Carlos", "Diego", "Erick", "Fernando", "Gustavo", "Hugo",
-    "Ícaro", "Jonathan", "Klaus", "Lucas", "Márcio", "Nícolas", "Orlando", "Paulo",
-    "Ricardo", "Sérgio", "Túlio", "Ulisses", "Valdo", "Walter", "Xande", "Yan", "Zeca"
-]
-
-LISTA_NOMES_FEMININOS = [
-    "Alice", "Bianca", "Carolina", "Daniela", "Eduarda", "Fernanda", "Gabriela", "Helena",
-    "Isabela", "Júlia", "Kamila", "Larissa", "Mariana", "Natália", "Olívia", "Patrícia",
-    "Raquel", "Sara", "Tatiana", "Valentina", "Wendy", "Ximena", "Yasmin", "Zara",
-    "Amanda", "Bruna", "Camila", "Débora", "Eloá", "Fátima", "Giovana", "Heloísa",
-    "Isis", "Jéssica", "Karina", "Lara", "Mirella", "Natasha", "Olga", "Priscila",
-    "Rafaela", "Sabrina", "Talita", "Úrsula", "Vitória", "Wanda", "Xuxa", "Yara", "Zilda"
-]
-
-SOBRENOMES = [
-    "Silva", "Santos", "Oliveira", "Souza", "Pereira", "Rodrigues", "Ferreira", "Almeida",
-    "Costa", "Gomes", "Martins", "Rocha", "Ribeiro", "Carvalho", "Melo", "Sousa",
-    "Alves", "Pinto", "Cardoso", "Teixeira", "Nascimento", "Lima", "Araújo", "Fernandes",
-    "Cavalcanti", "Mendes", "Barbosa", "Dias", "Cunha", "Moreira", "Correia", "Castro",
-    "Monteiro", "Sales", "Reis", "Tavares", "Andrade", "Moura", "Freitas", "Santana",
-    "Marques", "Bezerra", "Vieira", "Freire", "Farias", "Gonçalves", "Vargas", "Ramos",
-    "Pinheiro", "Lopes", "Campos", "Brito", "Montenegro", "Macedo", "Morais", "Viana",
-    "Coutinho", "Leal", "Mota", "Maia", "Pacheco", "Peixoto", "Junqueira", "Machado",
-    "Dantas", "Fonseca", "Azevedo", "Barros", "Miranda", "Mourão", "Valente", "Xavier",
-    "Zanetti", "Amorim", "Borges", "Diniz", "Fraga", "Godoy", "Horta", "Jardim",
-    "Klein", "Luz", "Nogueira", "Otero", "Parreira", "Quintana", "Rangel", "Sampaio",
-    "Toledo", "Uribe", "Vasconcelos", "Wanderley", "Ximenes", "Yoshida", "Zimmermann"
-]
-
-def gerar_sexo():
-    return random.choice(LISTA_SEXO)
-
-def gerar_nome(sexo=None):
-    
-    if sexo is None:
-        sexo = gerar_sexo()
-
-    if sexo == 'M':
-        nome = random.choice(LISTA_NOMES_MASCULINOS)
-    elif sexo == 'F':
-        nome = random.choice(LISTA_NOMES_FEMININOS)
-    else:
-        raise ValueError("Sexo inválido. Use 'M' para masculino ou 'F' para feminino.")
-    
-    return f"{nome}"
-
-def gerar_sobrenome():
-    return random.choice(SOBRENOMES)
-
-def gerar_nome_completo(sexo=None):
-
-    if sexo is None:
-        sexo = gerar_sexo()
-
-    nome = gerar_nome(sexo=sexo)
-    sobrenome = gerar_sobrenome()
-    nome_completo = f"{nome} {sobrenome}"
-
-    return nome_completo
-
-def gerar_nome_com_filiacao():
-
-    nome_mae = gerar_nome_completo(sexo='F')
-    nome_pai = gerar_nome_completo(sexo='M')
-
-    sobrenome_mae = nome_mae.split().pop()
-    sobrenome_pai = nome_pai.split().pop()
-
-    nome = gerar_nome()
-    nome = f"{nome} {sobrenome_mae} {sobrenome_pai}"
-
+import random
+
+SEXO_MASCULINO = 'M'
+SEXO_FEMININO = 'F'
+
+LISTA_SEXO = [SEXO_MASCULINO, SEXO_FEMININO]
+
+LISTA_NOMES_MASCULINOS = [
+    "Alex", "Bernardo", "Caio", "Daniel", "Eduardo", "Felipe", "Gabriel", "Henrique",
+    "Igor", "João", "Kauã", "Leonardo", "Matheus", "Nathan", "Otávio", "Pedro",
+    "Rafael", "Samuel", "Thiago", "Vitor", "Wagner", "Xavier", "Yuri", "Zélio",
+    "André", "Bruno", "Carlos", "Diego", "Erick", "Fernando", "Gustavo", "Hugo",
+    "Ícaro", "Jonathan", "Klaus", "Lucas", "Márcio", "Nícolas", "Orlando", "Paulo",
+    "Ricardo", "Sérgio", "Túlio", "Ulisses", "Valdo", "Walter", "Xande", "Yan", "Zeca"
+]
+
+LISTA_NOMES_FEMININOS = [
+    "Alice", "Bianca", "Carolina", "Daniela", "Eduarda", "Fernanda", "Gabriela", "Helena",
+    "Isabela", "Júlia", "Kamila", "Larissa", "Mariana", "Natália", "Olívia", "Patrícia",
+    "Raquel", "Sara", "Tatiana", "Valentina", "Wendy", "Ximena", "Yasmin", "Zara",
+    "Amanda", "Bruna", "Camila", "Débora", "Eloá", "Fátima", "Giovana", "Heloísa",
+    "Isis", "Jéssica", "Karina", "Lara", "Mirella", "Natasha", "Olga", "Priscila",
+    "Rafaela", "Sabrina", "Talita", "Úrsula", "Vitória", "Wanda", "Xuxa", "Yara", "Zilda"
+]
+
+SOBRENOMES = [
+    "Silva", "Santos", "Oliveira", "Souza", "Pereira", "Rodrigues", "Ferreira", "Almeida",
+    "Costa", "Gomes", "Martins", "Rocha", "Ribeiro", "Carvalho", "Melo", "Sousa",
+    "Alves", "Pinto", "Cardoso", "Teixeira", "Nascimento", "Lima", "Araújo", "Fernandes",
+    "Cavalcanti", "Mendes", "Barbosa", "Dias", "Cunha", "Moreira", "Correia", "Castro",
+    "Monteiro", "Sales", "Reis", "Tavares", "Andrade", "Moura", "Freitas", "Santana",
+    "Marques", "Bezerra", "Vieira", "Freire", "Farias", "Gonçalves", "Vargas", "Ramos",
+    "Pinheiro", "Lopes", "Campos", "Brito", "Montenegro", "Macedo", "Morais", "Viana",
+    "Coutinho", "Leal", "Mota", "Maia", "Pacheco", "Peixoto", "Junqueira", "Machado",
+    "Dantas", "Fonseca", "Azevedo", "Barros", "Miranda", "Mourão", "Valente", "Xavier",
+    "Zanetti", "Amorim", "Borges", "Diniz", "Fraga", "Godoy", "Horta", "Jardim",
+    "Klein", "Luz", "Nogueira", "Otero", "Parreira", "Quintana", "Rangel", "Sampaio",
+    "Toledo", "Uribe", "Vasconcelos", "Wanderley", "Ximenes", "Yoshida", "Zimmermann"
+]
+
+def gerar_sexo():
+    return random.choice(LISTA_SEXO)
+
+def gerar_nome(sexo=None):
+    
+    if sexo is None:
+        sexo = gerar_sexo()
+
+    if sexo == 'M':
+        nome = random.choice(LISTA_NOMES_MASCULINOS)
+    elif sexo == 'F':
+        nome = random.choice(LISTA_NOMES_FEMININOS)
+    else:
+        raise ValueError("Sexo inválido. Use 'M' para masculino ou 'F' para feminino.")
+    
+    return f"{nome}"
+
+def gerar_sobrenome():
+    return random.choice(SOBRENOMES)
+
+def gerar_nome_completo(sexo=None):
+
+    if sexo is None:
+        sexo = gerar_sexo()
+
+    nome = gerar_nome(sexo=sexo)
+    sobrenome = gerar_sobrenome()
+    nome_completo = f"{nome} {sobrenome}"
+
+    return nome_completo
+
+def gerar_nome_com_filiacao():
+
+    nome_mae = gerar_nome_completo(sexo='F')
+    nome_pai = gerar_nome_completo(sexo='M')
+
+    sobrenome_mae = nome_mae.split().pop()
+    sobrenome_pai = nome_pai.split().pop()
+
+    nome = gerar_nome()
+    nome = f"{nome} {sobrenome_mae} {sobrenome_pai}"
+
     return nome, nome_mae, nome_pai
```

### Comparing `PyFakeDados-0.0.5.1/PyFakeDados/pessoa.py` & `PyFakeDados-0.0.5.2/PyFakeDados/pessoa.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import random
-from datetime import datetime, timedelta
-from PyFakeDados.nome import gerar_sexo, gerar_nome, gerar_sobrenome, gerar_nome_completo, gerar_nome_com_filiacao
-from PyFakeDados.cep import gerar_cep
-from PyFakeDados.estado import gerar_estado, gerar_uf, busca_nome_uf
-from PyFakeDados.municipio import gerar_municipio
-from PyFakeDados.bairro import gerar_bairro
-from PyFakeDados.logradouro import gerar_logradouro, gerar_numero
-from PyFakeDados.telefone import gerar_telefone_fixo, gerar_telefone_celular
-from PyFakeDados.email import gerar_email, gerar_email_pessoa
-from PyFakeDados.senha import gerar_senha, gerar_senha_numerica
-from PyFakeDados.site import gerar_site
-from PyFakeDados.cpf import gerar_cpf
-from PyFakeDados.rg import gerar_rg
-from PyFakeDados.ctps import gerar_ctps
-from PyFakeDados.pis import gerar_pis
-from PyFakeDados.utils import gerar_data, gerar_data_nascimento
-from PyFakeDados.utils import remover_acentos
-
-def gerar_pessoa(uf=None, mask=False, idade=None, recem_nascido=False, force_ASCII=False, force_upper=False):
-
-    if uf is None:
-        uf = gerar_uf()
-
-    if idade is None:
-        
-        idade_min = 1
-        idade_max = 99
-
-        if recem_nascido:
-            idade_min = 0
-
-        idade = random.randint(idade_min, idade_max)
-
-    pessoa = {}
-    data_nascimento = gerar_data_nascimento(idade)
-    
-    sexo = gerar_sexo()
-    nome, mae, pai = gerar_nome_com_filiacao()
-    cpf = gerar_cpf(mask=mask)
-    rg = gerar_rg()
-    ctps = gerar_ctps()
-    pis = gerar_pis()
-    data_nascimento = data_nascimento
-    site = gerar_site(nome)
-    email = gerar_email_pessoa(nome)
-    senha = gerar_senha_numerica()
-    senha_forte = gerar_senha(16)
-    cep = gerar_cep(uf, mask=mask)
-    endereco = gerar_logradouro()
-    numero = gerar_numero()
-    bairro = gerar_bairro()
-    municipio = gerar_municipio(uf)
-    estado = busca_nome_uf(uf)
-    telefone = gerar_telefone_fixo(uf, mask=mask)
-    celular = gerar_telefone_celular(uf)
-
-    pessoa = {
-        "sexo": sexo,
-        "nome": nome,
-        "mae": mae,
-        "pai": pai,
-        "cpf": cpf,
-        "rg": rg,
-        "ctps": ctps,
-        "pis": pis,
-        "data_nascimento": data_nascimento.strftime("%d/%m/%Y"),
-        "site": site,
-        "email": email,
-        "senha": senha,
-        "senha_forte": senha_forte,
-        "cep": cep,
-        "endereco": endereco,
-        "numero": numero,
-        "bairro": bairro,
-        "municipio": municipio,
-        "estado": estado,
-        "uf": uf,
-        "telefone": telefone,
-        "celular": celular,
-    }
-
-    if force_ASCII:
-        for i in pessoa:
-            if isinstance(pessoa[i], str):
-                pessoa[i] = remover_acentos(pessoa[i])
-    
-    if force_upper:
-        for i in pessoa:
-            if isinstance(pessoa[i], str):
-                pessoa[i] = pessoa[i].upper()
-
-    return pessoa
+import random
+from datetime import datetime, timedelta
+from PyFakeDados.nome import gerar_sexo, gerar_nome, gerar_sobrenome, gerar_nome_completo, gerar_nome_com_filiacao
+from PyFakeDados.cep import gerar_cep
+from PyFakeDados.estado import gerar_estado, gerar_uf, busca_nome_uf
+from PyFakeDados.municipio import gerar_municipio
+from PyFakeDados.bairro import gerar_bairro
+from PyFakeDados.logradouro import gerar_logradouro, gerar_numero
+from PyFakeDados.telefone import gerar_telefone_fixo, gerar_telefone_celular
+from PyFakeDados.email import gerar_email, gerar_email_pessoa
+from PyFakeDados.senha import gerar_senha, gerar_senha_numerica
+from PyFakeDados.site import gerar_site
+from PyFakeDados.cpf import gerar_cpf
+from PyFakeDados.rg import gerar_rg
+from PyFakeDados.ctps import gerar_ctps
+from PyFakeDados.pis import gerar_pis
+from PyFakeDados.utils import gerar_data, gerar_data_nascimento
+from PyFakeDados.utils import remover_acentos
+
+def gerar_pessoa(uf=None, mask=False, idade=None, recem_nascido=False, force_ASCII=False, force_upper=False):
+
+    if uf is None:
+        uf = gerar_uf()
+
+    if idade is None:
+        
+        idade_min = 1
+        idade_max = 99
+
+        if recem_nascido:
+            idade_min = 0
+
+        idade = random.randint(idade_min, idade_max)
+
+    pessoa = {}
+    data_nascimento = gerar_data_nascimento(idade)
+    
+    sexo = gerar_sexo()
+    nome, mae, pai = gerar_nome_com_filiacao()
+    cpf = gerar_cpf(mask=mask)
+    rg = gerar_rg()
+    ctps = gerar_ctps()
+    pis = gerar_pis()
+    data_nascimento = data_nascimento
+    site = gerar_site(nome)
+    email = gerar_email_pessoa(nome)
+    senha = gerar_senha_numerica()
+    senha_forte = gerar_senha(16)
+    cep = gerar_cep(uf, mask=mask)
+    endereco = gerar_logradouro()
+    numero = gerar_numero()
+    bairro = gerar_bairro()
+    municipio = gerar_municipio(uf)
+    estado = busca_nome_uf(uf)
+    telefone = gerar_telefone_fixo(uf, mask=mask)
+    celular = gerar_telefone_celular(uf)
+
+    pessoa = {
+        "sexo": sexo,
+        "nome": nome,
+        "mae": mae,
+        "pai": pai,
+        "cpf": cpf,
+        "rg": rg,
+        "ctps": ctps,
+        "pis": pis,
+        "data_nascimento": data_nascimento.strftime("%d/%m/%Y"),
+        "site": site,
+        "email": email,
+        "senha": senha,
+        "senha_forte": senha_forte,
+        "cep": cep,
+        "endereco": endereco,
+        "numero": numero,
+        "bairro": bairro,
+        "municipio": municipio,
+        "estado": estado,
+        "uf": uf,
+        "telefone": telefone,
+        "celular": celular,
+    }
+
+    if force_ASCII:
+        for i in pessoa:
+            if isinstance(pessoa[i], str):
+                pessoa[i] = remover_acentos(pessoa[i])
+    
+    if force_upper:
+        for i in pessoa:
+            if isinstance(pessoa[i], str):
+                pessoa[i] = pessoa[i].upper()
+
+    return pessoa
```

### Comparing `PyFakeDados-0.0.5.1/PyFakeDados/telefone.py` & `PyFakeDados-0.0.5.2/PyFakeDados/telefone.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import random
-from PyFakeDados.estado import gerar_uf
-
-LISTA_DDD = {
-        'AC': ['68'],
-        'AL': ['82'],
-        'AM': ['92', '97'],
-        'AP': ['96'],
-        'BA': ['71', '73', '74', '75', '77'],
-        'CE': ['85', '88'],
-        'DF': ['61'],
-        'ES': ['27', '28'],
-        'GO': ['62', '64'],
-        'MA': ['98', '99'],
-        'MG': ['31', '32', '33', '34', '35', '37', '38'],
-        'MS': ['67'],
-        'MT': ['65', '66'],
-        'PA': ['91', '93', '94'],
-        'PB': ['83'],
-        'PE': ['81', '87'],
-        'PI': ['86', '89'],
-        'PR': ['41', '42', '43', '44', '45', '46'],
-        'RJ': ['21', '22', '24'],
-        'RN': ['84'],
-        'RO': ['69'],
-        'RR': ['95'],
-        'RS': ['51', '53', '54', '55'],
-        'SC': ['47', '48', '49'],
-        'SE': ['79'],
-        'SP': ['11', '12', '13', '14', '15', '16', '17', '18', '19'],
-        'TO': ['63']
-    }
-
-def gerar_telefone_fixo(uf=None, mask=False):
-
-    if uf is None:
-        uf = gerar_uf()
-
-    if uf.upper() not in LISTA_DDD:
-        raise ValueError("UF inválida.")
-
-    ddd = random.choice(LISTA_DDD[uf.upper()])
-    numero = ''.join(str(random.randint(0, 9)) for _ in range(8))
-
-    if mask:
-        telefone = f"({ddd}) {numero[:4]}-{numero[4:]}"
-    else:
-        telefone = f"{ddd}{numero[:4]}{numero[4:]}"
-    return telefone
-
-def gerar_telefone_celular(uf=None, mask=False):
-
-    if uf is None:
-        uf = gerar_uf()
-
-    if uf.upper() not in LISTA_DDD:
-        raise ValueError("UF inválida.")
-
-    ddd = random.choice(LISTA_DDD[uf.upper()])
-    numero = f'{str(random.randint(7, 9))}' + (''.join(str(random.randint(0, 9)) for _ in range(7)))
-
-    if mask:
-        telefone = f"({ddd}) 9{numero[:4]}-{numero[4:]}"
-    else:
-        telefone = f"{ddd}9{numero[:4]}{numero[4:]}"
-    return telefone
+import random
+from PyFakeDados.estado import gerar_uf
+
+LISTA_DDD = {
+        'AC': ['68'],
+        'AL': ['82'],
+        'AM': ['92', '97'],
+        'AP': ['96'],
+        'BA': ['71', '73', '74', '75', '77'],
+        'CE': ['85', '88'],
+        'DF': ['61'],
+        'ES': ['27', '28'],
+        'GO': ['62', '64'],
+        'MA': ['98', '99'],
+        'MG': ['31', '32', '33', '34', '35', '37', '38'],
+        'MS': ['67'],
+        'MT': ['65', '66'],
+        'PA': ['91', '93', '94'],
+        'PB': ['83'],
+        'PE': ['81', '87'],
+        'PI': ['86', '89'],
+        'PR': ['41', '42', '43', '44', '45', '46'],
+        'RJ': ['21', '22', '24'],
+        'RN': ['84'],
+        'RO': ['69'],
+        'RR': ['95'],
+        'RS': ['51', '53', '54', '55'],
+        'SC': ['47', '48', '49'],
+        'SE': ['79'],
+        'SP': ['11', '12', '13', '14', '15', '16', '17', '18', '19'],
+        'TO': ['63']
+    }
+
+def gerar_telefone_fixo(uf=None, mask=False):
+
+    if uf is None:
+        uf = gerar_uf()
+
+    if uf.upper() not in LISTA_DDD:
+        raise ValueError("UF inválida.")
+
+    ddd = random.choice(LISTA_DDD[uf.upper()])
+    numero = ''.join(str(random.randint(0, 9)) for _ in range(8))
+
+    if mask:
+        telefone = f"({ddd}) {numero[:4]}-{numero[4:]}"
+    else:
+        telefone = f"{ddd}{numero[:4]}{numero[4:]}"
+    return telefone
+
+def gerar_telefone_celular(uf=None, mask=False):
+
+    if uf is None:
+        uf = gerar_uf()
+
+    if uf.upper() not in LISTA_DDD:
+        raise ValueError("UF inválida.")
+
+    ddd = random.choice(LISTA_DDD[uf.upper()])
+    numero = f'{str(random.randint(7, 9))}' + (''.join(str(random.randint(0, 9)) for _ in range(7)))
+
+    if mask:
+        telefone = f"({ddd}) 9{numero[:4]}-{numero[4:]}"
+    else:
+        telefone = f"{ddd}9{numero[:4]}{numero[4:]}"
+    return telefone
```

### Comparing `PyFakeDados-0.0.5.1/PyFakeDados/utils.py` & `PyFakeDados-0.0.5.2/PyFakeDados/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,76 @@
-import random
-from datetime import date, datetime, timedelta
-from unidecode import unidecode
-
-def remover_acentos(texto):
-    texto_sem_acentos = unidecode(texto)
-    return texto_sem_acentos
-
-def gerar_data(data_inicial=None, data_final=None):
-
-    # Definir um intervalo de datas para gerar datas aleatórias
-    if data_inicial is None:
-        data_inicial = datetime(1970, 1, 1)
-    if data_final is None:
-        data_final = datetime.now() - timedelta(days=30)
-    
-    # Gerar uma data aleatória dentro do intervalo definido
-    diferenca = data_final - data_inicial
-    dias_aleatorios = random.randint(0, diferenca.days)
-    data_aleatoria = data_inicial + timedelta(days=dias_aleatorios)
-    
-    return data_aleatoria
-
-def calcular_idade(data_nascimento):
-    
-    hoje = date.today()
-    ano_atual = hoje.year
-    mes_atual = hoje.month
-    dia_atual = hoje.day
-
-    ano_nascimento = data_nascimento.year
-    mes_nascimento = data_nascimento.month
-    dia_nascimento = data_nascimento.day
-
-    idade = ano_atual - ano_nascimento
-
-    if mes_atual < mes_nascimento or (mes_atual == mes_nascimento and dia_atual < dia_nascimento):
-        idade -= 1
-
-    return idade
-
-def calcular_data_nascimento(idade):
-
-    hoje = date.today()
-    ano_atual = hoje.year
-
-    ano_nascimento = ano_atual - idade
-    data_nascimento = date(ano_nascimento, hoje.month, hoje.day)
-
-    return data_nascimento
-
-def gerar_data_nascimento(idade):
-    
-    hoje = date.today()
-    ano_atual = hoje.year
-
-    ano_nascimento = ano_atual - idade
-    mes_nascimento = random.randint(1, 12)
-    
-    # Considerando meses com 30 dias
-    if mes_nascimento == 2:
-        dia_nascimento = random.randint(1, 28)
-    elif mes_nascimento in [4, 6, 9, 11]:
-        dia_nascimento = random.randint(1, 30)
-    else:
-        dia_nascimento = random.randint(1, 31)
-
-    if mes_nascimento > hoje.month or (mes_nascimento == hoje.month and dia_nascimento >= hoje.day):
-        ano_nascimento -= 1
-
-    data_nascimento = date(ano_nascimento, mes_nascimento, dia_nascimento)
-
-    return data_nascimento
+import json
+import random
+import os
+from pathlib import Path
+from datetime import date, datetime, timedelta
+from unidecode import unidecode
+
+def remover_acentos(texto):
+    texto_sem_acentos = unidecode(texto)
+    return texto_sem_acentos
+
+def gerar_data(data_inicial=None, data_final=None):
+
+    # Definir um intervalo de datas para gerar datas aleatórias
+    if data_inicial is None:
+        data_inicial = datetime(1970, 1, 1)
+    if data_final is None:
+        data_final = datetime.now() - timedelta(days=30)
+    
+    # Gerar uma data aleatória dentro do intervalo definido
+    diferenca = data_final - data_inicial
+    dias_aleatorios = random.randint(0, diferenca.days)
+    data_aleatoria = data_inicial + timedelta(days=dias_aleatorios)
+    
+    return data_aleatoria
+
+def calcular_idade(data_nascimento):
+    
+    hoje = date.today()
+    ano_atual = hoje.year
+    mes_atual = hoje.month
+    dia_atual = hoje.day
+
+    ano_nascimento = data_nascimento.year
+    mes_nascimento = data_nascimento.month
+    dia_nascimento = data_nascimento.day
+
+    idade = ano_atual - ano_nascimento
+
+    if mes_atual < mes_nascimento or (mes_atual == mes_nascimento and dia_atual < dia_nascimento):
+        idade -= 1
+
+    return idade
+
+def calcular_data_nascimento(idade):
+
+    hoje = date.today()
+    ano_atual = hoje.year
+
+    ano_nascimento = ano_atual - idade
+    data_nascimento = date(ano_nascimento, hoje.month, hoje.day)
+
+    return data_nascimento
+
+def gerar_data_nascimento(idade):
+    
+    hoje = date.today()
+    ano_atual = hoje.year
+
+    ano_nascimento = ano_atual - idade
+    mes_nascimento = random.randint(1, 12)
+    
+    # Considerando meses com 30 dias
+    if mes_nascimento == 2:
+        dia_nascimento = random.randint(1, 28)
+    elif mes_nascimento in [4, 6, 9, 11]:
+        dia_nascimento = random.randint(1, 30)
+    else:
+        dia_nascimento = random.randint(1, 31)
+
+    if mes_nascimento > hoje.month or (mes_nascimento == hoje.month and dia_nascimento >= hoje.day):
+        ano_nascimento -= 1
+
+    data_nascimento = date(ano_nascimento, mes_nascimento, dia_nascimento)
+
+    return data_nascimento
```

### Comparing `PyFakeDados-0.0.5.1/PyFakeDados.egg-info/PKG-INFO` & `PyFakeDados-0.0.5.2/PyFakeDados.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-Metadata-Version: 2.1
-Name: PyFakeDados
-Version: 0.0.5.1
-Summary: Generic generator fake data for application and api development.
-Home-page: https://github.com/juliansantosinfo/PyFakeDados
-Author: Julian de Almeida Santos
-Author-email: julian.santos.info@gmail.com
-License: GPLv3
-Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
-Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# PyFakeDados
-
-![PyFakeDados](https://github.com/juliansantosinfo/PyFakeDados/logo.png)
-
-PyFakeDados é uma ferramenta em Python que auxilia desenvolvedores na geração de dados falsos (fake) aleatórios para bancos de dados de teste ou APIs. Com essa ferramenta, é possível gerar uma variedade de informações, como nomes, telefones, CPFs, e-mails, senhas e muito mais.
-
-O PyFakeDados oferece uma ampla gama de recursos para gerar dados em diversos formatos, como nomes, endereços, números de telefone, documentos como CPFs e CNPJs, e-mails, senhas, entre outros. Além disso, a ferramenta permite criar identidades completas de pessoas e empresas, fornecendo informações consistentes e realistas.
-
-A biblioteca é de fácil utilização e pode ser integrada facilmente a projetos em Python. Com uma simples chamada de função, você pode gerar quantidades massivas de dados falsos para preencher suas necessidades de teste. A diversidade dos dados gerados e a capacidade de personalização tornam o PyFakeDados uma ferramenta indispensável para qualquer desenvolvedor que precise de dados fictícios em seus projetos.
-
-Este repositório também fornece documentação completa sobre como usar a biblioteca e exemplos práticos para ajudá-lo a aproveitar ao máximo todas as funcionalidades do PyFakeDados.
-
-Experimente o PyFakeDados agora e torne o processo de geração de dados falsos mais eficiente e realista em seus projetos!
-
-## Recursos
-
-PyFakeDados é capaz de gerar os seguintes tipos de dados:
-
-- Nome
-- Sobrenome
-- Nome completo
-- Nome com filiação
-- Telefone fixo
-- Telefone celular
-- CPF
-- RG
-- PIS
-- CTPS
-- CNPJ
-- Inscrição estadual
-- E-mail
-- Site
-- Senhas
-
-Além disso, a ferramenta também é capaz de gerar agrupamentos de dados, formando identidades de pessoas e empresas.
-
-## Instalação
-
-Você pode instalar o PyFakeDados através do pip, executando o seguinte comando:
-
-```shell
-pip install PyFakeDados
-```
-
-## Uso
-
-Para utilizar o PyFakeDados em seu projeto, importe o pacote e utilize as funções correspondentes aos tipos de dados que deseja gerar. Por exemplo, para gerar um nome completo, utilize a função `gerar_nome_completo()`.
-
-```python
-from pyfakedados import gerar_nome_completo
-
-nome_completo = gerar_nome_completo()
-print(nome_completo)
-```
-
-Para mais exemplos de uso, consulte a documentação disponível em [link_da_documentacao](https://github.com/seu-usuario/repositorio/documentacao.md).
-
-## Contribuição
-
-Contribuições são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request* com melhorias, correções de bugs ou novos recursos.
-
-## Licença
-
-Este projeto é licenciado sob a [GPL-3.0 License](https://raw.githubusercontent.com/juliansantosinfo/PyFakeDados/main/LICENSE.txt).
+Metadata-Version: 2.1
+Name: PyFakeDados
+Version: 0.0.5.2
+Summary: Generic generator fake data for application and api development.
+Home-page: https://github.com/juliansantosinfo/PyFakeDados
+Author: Julian de Almeida Santos
+Author-email: julian.santos.info@gmail.com
+License: GPLv3
+Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
+Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# PyFakeDados
+
+![PyFakeDados](https://github.com/juliansantosinfo/PyFakeDados/logo.png)
+
+PyFakeDados é uma ferramenta em Python que auxilia desenvolvedores na geração de dados falsos (fake) aleatórios para bancos de dados de teste ou APIs. Com essa ferramenta, é possível gerar uma variedade de informações, como nomes, telefones, CPFs, e-mails, senhas e muito mais.
+
+O PyFakeDados oferece uma ampla gama de recursos para gerar dados em diversos formatos, como nomes, endereços, números de telefone, documentos como CPFs e CNPJs, e-mails, senhas, entre outros. Além disso, a ferramenta permite criar identidades completas de pessoas e empresas, fornecendo informações consistentes e realistas.
+
+A biblioteca é de fácil utilização e pode ser integrada facilmente a projetos em Python. Com uma simples chamada de função, você pode gerar quantidades massivas de dados falsos para preencher suas necessidades de teste. A diversidade dos dados gerados e a capacidade de personalização tornam o PyFakeDados uma ferramenta indispensável para qualquer desenvolvedor que precise de dados fictícios em seus projetos.
+
+Este repositório também fornece documentação completa sobre como usar a biblioteca e exemplos práticos para ajudá-lo a aproveitar ao máximo todas as funcionalidades do PyFakeDados.
+
+Experimente o PyFakeDados agora e torne o processo de geração de dados falsos mais eficiente e realista em seus projetos!
+
+## Recursos
+
+PyFakeDados é capaz de gerar os seguintes tipos de dados:
+
+- Nome
+- Sobrenome
+- Nome completo
+- Nome com filiação
+- Telefone fixo
+- Telefone celular
+- CPF
+- RG
+- PIS
+- CTPS
+- CNPJ
+- Inscrição estadual
+- E-mail
+- Site
+- Senhas
+
+Além disso, a ferramenta também é capaz de gerar agrupamentos de dados, formando identidades de pessoas e empresas.
+
+## Instalação
+
+Você pode instalar o PyFakeDados através do pip, executando o seguinte comando:
+
+```shell
+pip install PyFakeDados
+```
+
+## Uso
+
+Para utilizar o PyFakeDados em seu projeto, importe o pacote e utilize as funções correspondentes aos tipos de dados que deseja gerar. Por exemplo, para gerar um nome completo, utilize a função `gerar_nome_completo()`.
+
+```python
+from pyfakedados import gerar_nome_completo
+
+nome_completo = gerar_nome_completo()
+print(nome_completo)
+```
+
+Para mais exemplos de uso, consulte a documentação disponível em [link_da_documentacao](https://github.com/seu-usuario/repositorio/documentacao.md).
+
+## Contribuição
+
+Contribuições são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request* com melhorias, correções de bugs ou novos recursos.
+
+## Licença
+
+Este projeto é licenciado sob a [GPL-3.0 License](https://raw.githubusercontent.com/juliansantosinfo/PyFakeDados/main/LICENSE.txt).
```

### Comparing `PyFakeDados-0.0.5.1/PyFakeDados.egg-info/SOURCES.txt` & `PyFakeDados-0.0.5.2/PyFakeDados.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+PyFakeDados/CONSTANTS.py
 PyFakeDados/__init__.py
 PyFakeDados/bairro.py
 PyFakeDados/cep.py
 PyFakeDados/cnpj.py
 PyFakeDados/cpf.py
 PyFakeDados/ctps.py
 PyFakeDados/email.py
@@ -24,10 +25,8 @@
 PyFakeDados/telefone.py
 PyFakeDados/utils.py
 PyFakeDados.egg-info/PKG-INFO
 PyFakeDados.egg-info/SOURCES.txt
 PyFakeDados.egg-info/dependency_links.txt
 PyFakeDados.egg-info/not-zip-safe
 PyFakeDados.egg-info/requires.txt
-PyFakeDados.egg-info/top_level.txt
-PyFakeDados/src/estados.csv
-PyFakeDados/src/municipios.csv
+PyFakeDados.egg-info/top_level.txt
```

### Comparing `PyFakeDados-0.0.5.1/README.md` & `PyFakeDados-0.0.5.2/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-# PyFakeDados
-
-![PyFakeDados](https://github.com/juliansantosinfo/PyFakeDados/logo.png)
-
-PyFakeDados é uma ferramenta em Python que auxilia desenvolvedores na geração de dados falsos (fake) aleatórios para bancos de dados de teste ou APIs. Com essa ferramenta, é possível gerar uma variedade de informações, como nomes, telefones, CPFs, e-mails, senhas e muito mais.
-
-O PyFakeDados oferece uma ampla gama de recursos para gerar dados em diversos formatos, como nomes, endereços, números de telefone, documentos como CPFs e CNPJs, e-mails, senhas, entre outros. Além disso, a ferramenta permite criar identidades completas de pessoas e empresas, fornecendo informações consistentes e realistas.
-
-A biblioteca é de fácil utilização e pode ser integrada facilmente a projetos em Python. Com uma simples chamada de função, você pode gerar quantidades massivas de dados falsos para preencher suas necessidades de teste. A diversidade dos dados gerados e a capacidade de personalização tornam o PyFakeDados uma ferramenta indispensável para qualquer desenvolvedor que precise de dados fictícios em seus projetos.
-
-Este repositório também fornece documentação completa sobre como usar a biblioteca e exemplos práticos para ajudá-lo a aproveitar ao máximo todas as funcionalidades do PyFakeDados.
-
-Experimente o PyFakeDados agora e torne o processo de geração de dados falsos mais eficiente e realista em seus projetos!
-
-## Recursos
-
-PyFakeDados é capaz de gerar os seguintes tipos de dados:
-
-- Nome
-- Sobrenome
-- Nome completo
-- Nome com filiação
-- Telefone fixo
-- Telefone celular
-- CPF
-- RG
-- PIS
-- CTPS
-- CNPJ
-- Inscrição estadual
-- E-mail
-- Site
-- Senhas
-
-Além disso, a ferramenta também é capaz de gerar agrupamentos de dados, formando identidades de pessoas e empresas.
-
-## Instalação
-
-Você pode instalar o PyFakeDados através do pip, executando o seguinte comando:
-
-```shell
-pip install PyFakeDados
-```
-
-## Uso
-
-Para utilizar o PyFakeDados em seu projeto, importe o pacote e utilize as funções correspondentes aos tipos de dados que deseja gerar. Por exemplo, para gerar um nome completo, utilize a função `gerar_nome_completo()`.
-
-```python
-from pyfakedados import gerar_nome_completo
-
-nome_completo = gerar_nome_completo()
-print(nome_completo)
-```
-
-Para mais exemplos de uso, consulte a documentação disponível em [link_da_documentacao](https://github.com/seu-usuario/repositorio/documentacao.md).
-
-## Contribuição
-
-Contribuições são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request* com melhorias, correções de bugs ou novos recursos.
-
-## Licença
-
-Este projeto é licenciado sob a [GPL-3.0 License](https://raw.githubusercontent.com/juliansantosinfo/PyFakeDados/main/LICENSE.txt).
+# PyFakeDados
+
+![PyFakeDados](https://github.com/juliansantosinfo/PyFakeDados/logo.png)
+
+PyFakeDados é uma ferramenta em Python que auxilia desenvolvedores na geração de dados falsos (fake) aleatórios para bancos de dados de teste ou APIs. Com essa ferramenta, é possível gerar uma variedade de informações, como nomes, telefones, CPFs, e-mails, senhas e muito mais.
+
+O PyFakeDados oferece uma ampla gama de recursos para gerar dados em diversos formatos, como nomes, endereços, números de telefone, documentos como CPFs e CNPJs, e-mails, senhas, entre outros. Além disso, a ferramenta permite criar identidades completas de pessoas e empresas, fornecendo informações consistentes e realistas.
+
+A biblioteca é de fácil utilização e pode ser integrada facilmente a projetos em Python. Com uma simples chamada de função, você pode gerar quantidades massivas de dados falsos para preencher suas necessidades de teste. A diversidade dos dados gerados e a capacidade de personalização tornam o PyFakeDados uma ferramenta indispensável para qualquer desenvolvedor que precise de dados fictícios em seus projetos.
+
+Este repositório também fornece documentação completa sobre como usar a biblioteca e exemplos práticos para ajudá-lo a aproveitar ao máximo todas as funcionalidades do PyFakeDados.
+
+Experimente o PyFakeDados agora e torne o processo de geração de dados falsos mais eficiente e realista em seus projetos!
+
+## Recursos
+
+PyFakeDados é capaz de gerar os seguintes tipos de dados:
+
+- Nome
+- Sobrenome
+- Nome completo
+- Nome com filiação
+- Telefone fixo
+- Telefone celular
+- CPF
+- RG
+- PIS
+- CTPS
+- CNPJ
+- Inscrição estadual
+- E-mail
+- Site
+- Senhas
+
+Além disso, a ferramenta também é capaz de gerar agrupamentos de dados, formando identidades de pessoas e empresas.
+
+## Instalação
+
+Você pode instalar o PyFakeDados através do pip, executando o seguinte comando:
+
+```shell
+pip install PyFakeDados
+```
+
+## Uso
+
+Para utilizar o PyFakeDados em seu projeto, importe o pacote e utilize as funções correspondentes aos tipos de dados que deseja gerar. Por exemplo, para gerar um nome completo, utilize a função `gerar_nome_completo()`.
+
+```python
+from pyfakedados import gerar_nome_completo
+
+nome_completo = gerar_nome_completo()
+print(nome_completo)
+```
+
+Para mais exemplos de uso, consulte a documentação disponível em [link_da_documentacao](https://github.com/seu-usuario/repositorio/documentacao.md).
+
+## Contribuição
+
+Contribuições são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request* com melhorias, correções de bugs ou novos recursos.
+
+## Licença
+
+Este projeto é licenciado sob a [GPL-3.0 License](https://raw.githubusercontent.com/juliansantosinfo/PyFakeDados/main/LICENSE.txt).
```

### Comparing `PyFakeDados-0.0.5.1/setup.cfg` & `PyFakeDados-0.0.5.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2050 7946 616b 6544 6164 6f73 0d0a   = PyFakeDados..
-00000020: 7665 7273 696f 6e20 3d20 6174 7472 3a20  version = attr: 
-00000030: 5079 4661 6b65 4461 646f 732e 5f5f 7665  PyFakeDados.__ve
-00000040: 7273 696f 6e5f 5f0d 0a75 726c 203d 2068  rsion__..url = h
-00000050: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000060: 6d2f 6a75 6c69 616e 7361 6e74 6f73 696e  m/juliansantosin
-00000070: 666f 2f50 7946 616b 6544 6164 6f73 0d0a  fo/PyFakeDados..
-00000080: 6175 7468 6f72 203d 204a 756c 6961 6e20  author = Julian 
-00000090: 6465 2041 6c6d 6569 6461 2053 616e 746f  de Almeida Santo
-000000a0: 730d 0a61 7574 686f 725f 656d 6169 6c20  s..author_email 
-000000b0: 3d20 6a75 6c69 616e 2e73 616e 746f 732e  = julian.santos.
-000000c0: 696e 666f 4067 6d61 696c 2e63 6f6d 0d0a  info@gmail.com..
-000000d0: 6465 7363 7269 7074 696f 6e20 3d20 4765  description = Ge
-000000e0: 6e65 7269 6320 6765 6e65 7261 746f 7220  neric generator 
-000000f0: 6661 6b65 2064 6174 6120 666f 7220 6170  fake data for ap
-00000100: 706c 6963 6174 696f 6e20 616e 6420 6170  plication and ap
-00000110: 6920 6465 7665 6c6f 706d 656e 742e 0d0a  i development...
-00000120: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000130: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-00000140: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-00000150: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-00000160: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000170: 6e0d 0a6b 6579 776f 7264 7320 3d20 6661  n..keywords = fa
-00000180: 6b65 6461 646f 732c 2066 616b 652c 2064  kedados, fake, d
-00000190: 6164 6f73 2c20 6765 7261 646f 722c 2070  ados, gerador, p
-000001a0: 6573 736f 612c 2065 6d70 7265 7361 2c20  essoa, empresa, 
-000001b0: 646f 6375 6d65 6e74 6f0d 0a6c 6963 656e  documento..licen
-000001c0: 7365 203d 2047 504c 7633 0d0a 6c69 6365  se = GPLv3..lice
-000001d0: 6e73 655f 6669 6c65 7320 3d20 4c49 4345  nse_files = LICE
-000001e0: 4e53 452e 7478 740d 0a63 6c61 7373 6966  NSE.txt..classif
-000001f0: 6965 7273 203d 200d 0a09 4c69 6365 6e73  iers = ...Licens
-00000200: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000210: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
-00000220: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-00000230: 7633 2028 4750 4c76 3329 0d0a 0950 726f  v3 (GPLv3)...Pro
-00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000250: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000260: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
-00000270: 200d 0a09 536f 7572 6365 203d 2068 7474   ...Source = htt
-00000280: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000290: 6a75 6c69 616e 7361 6e74 6f73 696e 666f  juliansantosinfo
-000002a0: 2f50 7946 616b 6544 6164 6f73 0d0a 0d0a  /PyFakeDados....
-000002b0: 5b6f 7074 696f 6e73 5d0d 0a7a 6970 5f73  [options]..zip_s
-000002c0: 6166 6520 3d20 6661 6c73 650d 0a70 7974  afe = false..pyt
-000002d0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000002e0: 3d33 2e38 0d0a 696e 636c 7564 655f 7061  =3.8..include_pa
-000002f0: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
-00000300: 650d 0a69 6e73 7461 6c6c 5f72 6571 7569  e..install_requi
-00000310: 7265 7320 3d20 0d0a 0955 6e69 6465 636f  res = ...Unideco
-00000320: 6465 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  de....[egg_info]
-00000330: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000340: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 5079 4661 6b65 4461 646f 730a 7665  = PyFakeDados.ve
+00000020: 7273 696f 6e20 3d20 6174 7472 3a20 5079  rsion = attr: Py
+00000030: 4661 6b65 4461 646f 732e 5f5f 7665 7273  FakeDados.__vers
+00000040: 696f 6e5f 5f0a 7572 6c20 3d20 6874 7470  ion__.url = http
+00000050: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00000060: 756c 6961 6e73 616e 746f 7369 6e66 6f2f  uliansantosinfo/
+00000070: 5079 4661 6b65 4461 646f 730a 6175 7468  PyFakeDados.auth
+00000080: 6f72 203d 204a 756c 6961 6e20 6465 2041  or = Julian de A
+00000090: 6c6d 6569 6461 2053 616e 746f 730a 6175  lmeida Santos.au
+000000a0: 7468 6f72 5f65 6d61 696c 203d 206a 756c  thor_email = jul
+000000b0: 6961 6e2e 7361 6e74 6f73 2e69 6e66 6f40  ian.santos.info@
+000000c0: 676d 6169 6c2e 636f 6d0a 6465 7363 7269  gmail.com.descri
+000000d0: 7074 696f 6e20 3d20 4765 6e65 7269 6320  ption = Generic 
+000000e0: 6765 6e65 7261 746f 7220 6661 6b65 2064  generator fake d
+000000f0: 6174 6120 666f 7220 6170 706c 6963 6174  ata for applicat
+00000100: 696f 6e20 616e 6420 6170 6920 6465 7665  ion and api deve
+00000110: 6c6f 706d 656e 742e 0a6c 6f6e 675f 6465  lopment..long_de
+00000120: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+00000130: 3a20 5245 4144 4d45 2e6d 640a 6c6f 6e67  : README.md.long
+00000140: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+00000150: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+00000160: 2f6d 6172 6b64 6f77 6e0a 6b65 7977 6f72  /markdown.keywor
+00000170: 6473 203d 2066 616b 6564 6164 6f73 2c20  ds = fakedados, 
+00000180: 6661 6b65 2c20 6461 646f 732c 2067 6572  fake, dados, ger
+00000190: 6164 6f72 2c20 7065 7373 6f61 2c20 656d  ador, pessoa, em
+000001a0: 7072 6573 612c 2064 6f63 756d 656e 746f  presa, documento
+000001b0: 0a6c 6963 656e 7365 203d 2047 504c 7633  .license = GPLv3
+000001c0: 0a6c 6963 656e 7365 5f66 696c 6573 203d  .license_files =
+000001d0: 204c 4943 454e 5345 2e74 7874 0a63 6c61   LICENSE.txt.cla
+000001e0: 7373 6966 6965 7273 203d 200a 094c 6963  ssifiers = ..Lic
+000001f0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000200: 6f76 6564 203a 3a20 474e 5520 4765 6e65  oved :: GNU Gene
+00000210: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+00000220: 7365 2076 3320 2847 504c 7633 290a 0950  se v3 (GPLv3)..P
+00000230: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000240: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000250: 2033 0a70 726f 6a65 6374 5f75 726c 7320   3.project_urls 
+00000260: 3d20 0a09 536f 7572 6365 203d 2068 7474  = ..Source = htt
+00000270: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000280: 6a75 6c69 616e 7361 6e74 6f73 696e 666f  juliansantosinfo
+00000290: 2f50 7946 616b 6544 6164 6f73 0a0a 5b6f  /PyFakeDados..[o
+000002a0: 7074 696f 6e73 5d0a 7a69 705f 7361 6665  ptions].zip_safe
+000002b0: 203d 2066 616c 7365 0a70 7974 686f 6e5f   = false.python_
+000002c0: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
+000002d0: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
+000002e0: 5f64 6174 6120 3d20 5472 7565 0a69 6e73  _data = True.ins
+000002f0: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000300: 0a09 556e 6964 6563 6f64 650a 0a5b 6567  ..Unidecode..[eg
+00000310: 675f 696e 666f 5d0a 7461 675f 6275 696c  g_info].tag_buil
+00000320: 6420 3d20 0a74 6167 5f64 6174 6520 3d20  d = .tag_date = 
+00000330: 300a 0a                                  0..
```

