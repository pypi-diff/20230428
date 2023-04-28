# Comparing `tmp/dafne-dl-1.3a3.tar.gz` & `tmp/dafne-dl-1.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dafne-dl-1.3a3.tar", last modified: Wed Dec 28 10:25:13 2022, max compression
+gzip compressed data, was "dafne-dl-1.3a4.tar", last modified: Fri Apr 28 09:03:28 2023, max compression
```

## Comparing `dafne-dl-1.3a3.tar` & `dafne-dl-1.3a4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 francesco  (1000) francesco  (1000)        0 2022-12-28 10:25:13.817431 dafne-dl-1.3a3/
--rw-r--r--   0 francesco  (1000) francesco  (1000)    35149 2017-09-30 07:16:26.000000 dafne-dl-1.3a3/COPYING
--rw-r--r--   0 francesco  (1000) francesco  (1000)     7652 2017-09-30 07:16:26.000000 dafne-dl-1.3a3/COPYING.LESSER
--rw-r--r--   0 francesco  (1000) francesco  (1000)     4600 2022-12-28 10:25:13.817431 dafne-dl-1.3a3/PKG-INFO
--rw-r--r--   0 francesco  (1000) francesco  (1000)     4007 2022-06-15 14:26:58.000000 dafne-dl-1.3a3/README.md
--rw-r--r--   0 francesco  (1000) francesco  (1000)       84 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/pyproject.toml
--rw-r--r--   0 francesco  (1000) francesco  (1000)      889 2022-12-28 10:25:13.817431 dafne-dl-1.3a3/setup.cfg
-drwxr-xr-x   0 francesco  (1000) francesco  (1000)        0 2022-12-28 10:25:13.814098 dafne-dl-1.3a3/src/
-drwxr-xr-x   0 francesco  (1000) francesco  (1000)        0 2022-12-28 10:25:13.817431 dafne-dl-1.3a3/src/dafne_dl/
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)    11713 2022-10-21 09:56:03.000000 dafne-dl-1.3a3/src/dafne_dl/DynamicDLModel.py
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)     4745 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/LocalModelProvider.py
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)    10878 2022-09-21 12:03:54.000000 dafne-dl-1.3a3/src/dafne_dl/RemoteModelProvider.py
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)     1388 2022-12-28 10:23:30.000000 dafne-dl-1.3a3/src/dafne_dl/__init__.py
-drwxr-xr-x   0 francesco  (1000) francesco  (1000)        0 2022-12-28 10:25:13.817431 dafne-dl-1.3a3/src/dafne_dl/common/
--rw-r--r--   0 francesco  (1000) francesco  (1000)     4501 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/common/DataGenerators.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)      690 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/common/__init__.py
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)     2094 2022-12-28 07:42:26.000000 dafne-dl-1.3a3/src/dafne_dl/common/biascorrection.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)     2763 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/common/padorcut.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)    19952 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/common/preprocess_train.py
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)     7105 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/interfaces.py
-drwxr-xr-x   0 francesco  (1000) francesco  (1000)        0 2022-12-28 10:25:13.817431 dafne-dl-1.3a3/src/dafne_dl/labels/
--rw-r--r--   0 francesco  (1000) francesco  (1000)      689 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/labels/__init__.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)     1263 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/labels/leg.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)     1490 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/labels/thigh.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)      894 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/labels/utils.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)     2170 2022-07-04 10:07:43.000000 dafne-dl-1.3a3/src/dafne_dl/misc.py
-drwxr-xr-x   0 francesco  (1000) francesco  (1000)        0 2022-12-28 10:25:13.817431 dafne-dl-1.3a3/src/dafne_dl/resources/
--rw-r--r--   0 francesco  (1000) francesco  (1000)        0 2022-10-03 17:39:23.000000 dafne-dl-1.3a3/src/dafne_dl/resources/__init__.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)      400 2022-12-28 07:43:09.000000 dafne-dl-1.3a3/src/dafne_dl/resources/runtime_dependencies.cfg
-drwxr-xr-x   0 francesco  (1000) francesco  (1000)        0 2022-12-28 10:25:13.817431 dafne-dl-1.3a3/src/dafne_dl.egg-info/
--rw-r--r--   0 francesco  (1000) francesco  (1000)     4600 2022-12-28 10:25:13.000000 dafne-dl-1.3a3/src/dafne_dl.egg-info/PKG-INFO
--rw-r--r--   0 francesco  (1000) francesco  (1000)      791 2022-12-28 10:25:13.000000 dafne-dl-1.3a3/src/dafne_dl.egg-info/SOURCES.txt
--rw-r--r--   0 francesco  (1000) francesco  (1000)        1 2022-12-28 10:25:13.000000 dafne-dl-1.3a3/src/dafne_dl.egg-info/dependency_links.txt
--rw-r--r--   0 francesco  (1000) francesco  (1000)       96 2022-12-28 10:25:13.000000 dafne-dl-1.3a3/src/dafne_dl.egg-info/requires.txt
--rw-r--r--   0 francesco  (1000) francesco  (1000)        9 2022-12-28 10:25:13.000000 dafne-dl-1.3a3/src/dafne_dl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 09:03:28.575357 dafne-dl-1.3a4/
+-rw-rw-rw-   0        0        0    35823 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/COPYING
+-rw-rw-rw-   0        0        0     7817 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/COPYING.LESSER
+-rw-rw-rw-   0        0        0     4647 2023-04-28 09:03:28.575357 dafne-dl-1.3a4/PKG-INFO
+-rw-rw-rw-   0        0        0     4038 2022-06-17 12:00:54.000000 dafne-dl-1.3a4/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/pyproject.toml
+-rw-rw-rw-   0        0        0      930 2023-04-28 09:03:28.578349 dafne-dl-1.3a4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 09:03:28.429923 dafne-dl-1.3a4/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 09:03:28.473800 dafne-dl-1.3a4/src/dafne_dl/
+-rw-rw-rw-   0        0        0    12063 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/DynamicDLModel.py
+-rw-rw-rw-   0        0        0     4874 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/LocalModelProvider.py
+-rw-rw-rw-   0        0        0    11169 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/RemoteModelProvider.py
+-rw-rw-rw-   0        0        0     1450 2023-04-28 08:59:32.000000 dafne-dl-1.3a4/src/dafne_dl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:03:28.535032 dafne-dl-1.3a4/src/dafne_dl/common/
+-rw-rw-rw-   0        0        0     4632 2023-04-28 08:57:17.000000 dafne-dl-1.3a4/src/dafne_dl/common/DataGenerators.py
+-rw-rw-rw-   0        0        0      706 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/common/__init__.py
+-rw-rw-rw-   0        0        0     2149 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/common/biascorrection.py
+-rw-rw-rw-   0        0        0     2839 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/common/padorcut.py
+-rw-rw-rw-   0        0        0    20428 2023-04-28 08:57:17.000000 dafne-dl-1.3a4/src/dafne_dl/common/preprocess_train.py
+-rw-rw-rw-   0        0        0     7359 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/interfaces.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:03:28.566415 dafne-dl-1.3a4/src/dafne_dl/labels/
+-rw-rw-rw-   0        0        0      704 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/labels/__init__.py
+-rw-rw-rw-   0        0        0     1306 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/labels/leg.py
+-rw-rw-rw-   0        0        0     1544 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/labels/thigh.py
+-rw-rw-rw-   0        0        0      914 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/labels/utils.py
+-rw-rw-rw-   0        0        0     2233 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/misc.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:03:28.571368 dafne-dl-1.3a4/src/dafne_dl/resources/
+-rw-rw-rw-   0        0        0        0 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/resources/__init__.py
+-rw-rw-rw-   0        0        0      415 2023-04-21 08:42:23.000000 dafne-dl-1.3a4/src/dafne_dl/resources/runtime_dependencies.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 09:03:28.489988 dafne-dl-1.3a4/src/dafne_dl.egg-info/
+-rw-rw-rw-   0        0        0     4647 2023-04-28 09:03:28.000000 dafne-dl-1.3a4/src/dafne_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2023-04-28 09:03:28.000000 dafne-dl-1.3a4/src/dafne_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:03:28.000000 dafne-dl-1.3a4/src/dafne_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-04-28 09:03:28.000000 dafne-dl-1.3a4/src/dafne_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 09:03:28.000000 dafne-dl-1.3a4/src/dafne_dl.egg-info/top_level.txt
```

### Comparing `dafne-dl-1.3a3/COPYING` & `dafne-dl-1.3a4/COPYING`

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
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
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
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `dafne-dl-1.3a3/COPYING.LESSER` & `dafne-dl-1.3a4/COPYING.LESSER`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-                   GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-
-  This version of the GNU Lesser General Public License incorporates
-the terms and conditions of version 3 of the GNU General Public
-License, supplemented by the additional permissions listed below.
-
-  0. Additional Definitions.
-
-  As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the GNU
-General Public License.
-
-  "The Library" refers to a covered work governed by this License,
-other than an Application or a Combined Work as defined below.
-
-  An "Application" is any work that makes use of an interface provided
-by the Library, but which is not otherwise based on the Library.
-Defining a subclass of a class defined by the Library is deemed a mode
-of using an interface provided by the Library.
-
-  A "Combined Work" is a work produced by combining or linking an
-Application with the Library.  The particular version of the Library
-with which the Combined Work was made is also called the "Linked
-Version".
-
-  The "Minimal Corresponding Source" for a Combined Work means the
-Corresponding Source for the Combined Work, excluding any source code
-for portions of the Combined Work that, considered in isolation, are
-based on the Application, and not on the Linked Version.
-
-  The "Corresponding Application Code" for a Combined Work means the
-object code and/or source code for the Application, including any data
-and utility programs needed for reproducing the Combined Work from the
-Application, but excluding the System Libraries of the Combined Work.
-
-  1. Exception to Section 3 of the GNU GPL.
-
-  You may convey a covered work under sections 3 and 4 of this License
-without being bound by section 3 of the GNU GPL.
-
-  2. Conveying Modified Versions.
-
-  If you modify a copy of the Library, and, in your modifications, a
-facility refers to a function or data to be supplied by an Application
-that uses the facility (other than as an argument passed when the
-facility is invoked), then you may convey a copy of the modified
-version:
-
-   a) under this License, provided that you make a good faith effort to
-   ensure that, in the event an Application does not supply the
-   function or data, the facility still operates, and performs
-   whatever part of its purpose remains meaningful, or
-
-   b) under the GNU GPL, with none of the additional permissions of
-   this License applicable to that copy.
-
-  3. Object Code Incorporating Material from Library Header Files.
-
-  The object code form of an Application may incorporate material from
-a header file that is part of the Library.  You may convey such object
-code under terms of your choice, provided that, if the incorporated
-material is not limited to numerical parameters, data structure
-layouts and accessors, or small macros, inline functions and templates
-(ten or fewer lines in length), you do both of the following:
-
-   a) Give prominent notice with each copy of the object code that the
-   Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the object code with a copy of the GNU GPL and this license
-   document.
-
-  4. Combined Works.
-
-  You may convey a Combined Work under terms of your choice that,
-taken together, effectively do not restrict modification of the
-portions of the Library contained in the Combined Work and reverse
-engineering for debugging such modifications, if you also do each of
-the following:
-
-   a) Give prominent notice with each copy of the Combined Work that
-   the Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the Combined Work with a copy of the GNU GPL and this license
-   document.
-
-   c) For a Combined Work that displays copyright notices during
-   execution, include the copyright notice for the Library among
-   these notices, as well as a reference directing the user to the
-   copies of the GNU GPL and this license document.
-
-   d) Do one of the following:
-
-       0) Convey the Minimal Corresponding Source under the terms of this
-       License, and the Corresponding Application Code in a form
-       suitable for, and under terms that permit, the user to
-       recombine or relink the Application with a modified version of
-       the Linked Version to produce a modified Combined Work, in the
-       manner specified by section 6 of the GNU GPL for conveying
-       Corresponding Source.
-
-       1) Use a suitable shared library mechanism for linking with the
-       Library.  A suitable mechanism is one that (a) uses at run time
-       a copy of the Library already present on the user's computer
-       system, and (b) will operate properly with a modified version
-       of the Library that is interface-compatible with the Linked
-       Version.
-
-   e) Provide Installation Information, but only if you would otherwise
-   be required to provide such information under section 6 of the
-   GNU GPL, and only to the extent that such information is
-   necessary to install and execute a modified version of the
-   Combined Work produced by recombining or relinking the
-   Application with a modified version of the Linked Version. (If
-   you use option 4d0, the Installation Information must accompany
-   the Minimal Corresponding Source and Corresponding Application
-   Code. If you use option 4d1, you must provide the Installation
-   Information in the manner specified by section 6 of the GNU GPL
-   for conveying Corresponding Source.)
-
-  5. Combined Libraries.
-
-  You may place library facilities that are a work based on the
-Library side by side in a single library together with other library
-facilities that are not Applications and are not covered by this
-License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
-   a) Accompany the combined library with a copy of the same work based
-   on the Library, uncombined with any other library facilities,
-   conveyed under the terms of this License.
-
-   b) Give prominent notice with the combined library that part of it
-   is a work based on the Library, and explaining where to find the
-   accompanying uncombined form of the same work.
-
-  6. Revised Versions of the GNU Lesser General Public License.
-
-  The Free Software Foundation may publish revised and/or new versions
-of the GNU Lesser General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-  Each version is given a distinguishing version number. If the
-Library as you received it specifies that a certain numbered version
-of the GNU Lesser General Public License "or any later version"
-applies to it, you have the option of following the terms and
-conditions either of that published version or of any later version
-published by the Free Software Foundation. If the Library as you
-received it does not specify a version number of the GNU Lesser
-General Public License, you may choose any version of the GNU Lesser
-General Public License ever published by the Free Software Foundation.
-
-  If the Library as you received it specifies that a proxy can decide
-whether future versions of the GNU Lesser General Public License shall
-apply, that proxy's public statement of acceptance of any version is
-permanent authorization for you to choose that version for the
-Library.
+                   GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+
+  This version of the GNU Lesser General Public License incorporates
+the terms and conditions of version 3 of the GNU General Public
+License, supplemented by the additional permissions listed below.
+
+  0. Additional Definitions.
+
+  As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the GNU
+General Public License.
+
+  "The Library" refers to a covered work governed by this License,
+other than an Application or a Combined Work as defined below.
+
+  An "Application" is any work that makes use of an interface provided
+by the Library, but which is not otherwise based on the Library.
+Defining a subclass of a class defined by the Library is deemed a mode
+of using an interface provided by the Library.
+
+  A "Combined Work" is a work produced by combining or linking an
+Application with the Library.  The particular version of the Library
+with which the Combined Work was made is also called the "Linked
+Version".
+
+  The "Minimal Corresponding Source" for a Combined Work means the
+Corresponding Source for the Combined Work, excluding any source code
+for portions of the Combined Work that, considered in isolation, are
+based on the Application, and not on the Linked Version.
+
+  The "Corresponding Application Code" for a Combined Work means the
+object code and/or source code for the Application, including any data
+and utility programs needed for reproducing the Combined Work from the
+Application, but excluding the System Libraries of the Combined Work.
+
+  1. Exception to Section 3 of the GNU GPL.
+
+  You may convey a covered work under sections 3 and 4 of this License
+without being bound by section 3 of the GNU GPL.
+
+  2. Conveying Modified Versions.
+
+  If you modify a copy of the Library, and, in your modifications, a
+facility refers to a function or data to be supplied by an Application
+that uses the facility (other than as an argument passed when the
+facility is invoked), then you may convey a copy of the modified
+version:
+
+   a) under this License, provided that you make a good faith effort to
+   ensure that, in the event an Application does not supply the
+   function or data, the facility still operates, and performs
+   whatever part of its purpose remains meaningful, or
+
+   b) under the GNU GPL, with none of the additional permissions of
+   this License applicable to that copy.
+
+  3. Object Code Incorporating Material from Library Header Files.
+
+  The object code form of an Application may incorporate material from
+a header file that is part of the Library.  You may convey such object
+code under terms of your choice, provided that, if the incorporated
+material is not limited to numerical parameters, data structure
+layouts and accessors, or small macros, inline functions and templates
+(ten or fewer lines in length), you do both of the following:
+
+   a) Give prominent notice with each copy of the object code that the
+   Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the object code with a copy of the GNU GPL and this license
+   document.
+
+  4. Combined Works.
+
+  You may convey a Combined Work under terms of your choice that,
+taken together, effectively do not restrict modification of the
+portions of the Library contained in the Combined Work and reverse
+engineering for debugging such modifications, if you also do each of
+the following:
+
+   a) Give prominent notice with each copy of the Combined Work that
+   the Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the Combined Work with a copy of the GNU GPL and this license
+   document.
+
+   c) For a Combined Work that displays copyright notices during
+   execution, include the copyright notice for the Library among
+   these notices, as well as a reference directing the user to the
+   copies of the GNU GPL and this license document.
+
+   d) Do one of the following:
+
+       0) Convey the Minimal Corresponding Source under the terms of this
+       License, and the Corresponding Application Code in a form
+       suitable for, and under terms that permit, the user to
+       recombine or relink the Application with a modified version of
+       the Linked Version to produce a modified Combined Work, in the
+       manner specified by section 6 of the GNU GPL for conveying
+       Corresponding Source.
+
+       1) Use a suitable shared library mechanism for linking with the
+       Library.  A suitable mechanism is one that (a) uses at run time
+       a copy of the Library already present on the user's computer
+       system, and (b) will operate properly with a modified version
+       of the Library that is interface-compatible with the Linked
+       Version.
+
+   e) Provide Installation Information, but only if you would otherwise
+   be required to provide such information under section 6 of the
+   GNU GPL, and only to the extent that such information is
+   necessary to install and execute a modified version of the
+   Combined Work produced by recombining or relinking the
+   Application with a modified version of the Linked Version. (If
+   you use option 4d0, the Installation Information must accompany
+   the Minimal Corresponding Source and Corresponding Application
+   Code. If you use option 4d1, you must provide the Installation
+   Information in the manner specified by section 6 of the GNU GPL
+   for conveying Corresponding Source.)
+
+  5. Combined Libraries.
+
+  You may place library facilities that are a work based on the
+Library side by side in a single library together with other library
+facilities that are not Applications and are not covered by this
+License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+   a) Accompany the combined library with a copy of the same work based
+   on the Library, uncombined with any other library facilities,
+   conveyed under the terms of this License.
+
+   b) Give prominent notice with the combined library that part of it
+   is a work based on the Library, and explaining where to find the
+   accompanying uncombined form of the same work.
+
+  6. Revised Versions of the GNU Lesser General Public License.
+
+  The Free Software Foundation may publish revised and/or new versions
+of the GNU Lesser General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+  Each version is given a distinguishing version number. If the
+Library as you received it specifies that a certain numbered version
+of the GNU Lesser General Public License "or any later version"
+applies to it, you have the option of following the terms and
+conditions either of that published version or of any later version
+published by the Free Software Foundation. If the Library as you
+received it does not specify a version number of the GNU Lesser
+General Public License, you may choose any version of the GNU Lesser
+General Public License ever published by the Free Software Foundation.
+
+  If the Library as you received it specifies that a proxy can decide
+whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is
+permanent authorization for you to choose that version for the
+Library.
```

### Comparing `dafne-dl-1.3a3/PKG-INFO` & `dafne-dl-1.3a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: dafne-dl
-Version: 1.3a3
-Summary: Deep Learning module for Dafne
-Home-page: https://github.com/dafne-imaging/dafne-dl
-Author: Francesco Santini
-Author-email: francesco.santini@unibas.ch
-Project-URL: Bug Tracker, https://github.com/dafne-imaging/dafne-dl/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: COPYING
-License-File: COPYING.LESSER
-
-Sets of classes and interfaces for the definition of deep learning models.
-The framework is conceived to be extensible and serializable, in order to provide models that can be stored and/or sent through the network.
-## Interfaces.py
-Set of abstract classes that describe models and model providers. 
-### DeepLearningClass
-The rationale behind this is that an algorithm not only depends on the model, but might require some preprocessing steps (reformatting, normalization) before the application of the model itself. The interface is also "incremental-learning-oriented" as it provides abstract methods for the calculation and integration of deltas. The class provides operator override for the calculation of deltas (D = A-B) and call override for the apply method.
-An instance of DeepLearningClass should be able to simply provide the expected result when called with the appropriate input data (in form of dict). The most common data for our case will be:
-
- - Input: `{'image': 2D image, 'resolution': Sequence with pixel sizes}`
- - Output: for Classifiers: `str`, for Segmenters: `dict[str: image]` where str is the label and the image is a 2D numpy array containing the mask corresponding to the string.
-
-### ModelProvider
-This is an abstract class that is intended to encapsulate the logic of model load/transfer. It will have two subclasses, LocalModelProvider and RemoteModelProvider. In both cases, the method load_model of this class accepts a description of the requested model and will return an instance of DeepLearningClass. In principle, LocalModelProvider will be used on the server, and RemoteModelProvider on the client.
-
-## DynamicDLModel
-Concrete implementation of a DeepLearningClass which provides flexibility and serialization. This class delegates the important methods of the model implementation to top-level functions that are passed at the construction time. These functions can be easily serialized with the dill library.
-Constructor:
-
-        def __init__(self, model_id, # a unique ID to avoid mixing different models
-                 init_model_function, # inits the model. Accepts no parameters and returns the model
-                 apply_model_function, # function that applies the model. Has the object, and image, and a sequence containing resolutions as parameters
-                 weights_to_model_function = default_keras_weights_to_model_function, # put model weights inside the model.
-                 model_to_weights_function = default_keras_model_to_weights_function, # get the weights from the model in a pickable format
-                 calc_delta_function = default_keras_delta_function, # calculate the weight delta
-                 apply_delta_function = default_keras_apply_delta_function, # apply a weight delta
-                 incremental_learn_function = None, # function to perform an incremental learning step
-                 weights = None): # initial weights
-This allows the implementation of a very generic deep learning algorithm which includes the preprocessing steps in a way that can be serialized and defined at runtime, so if we want to change the model, we don't need to change the code of the client or server, as the implementation is self-contained within the model.
-The class provides the methods `dump(file_descriptor)` and `str = dumps()` to serialize and the static methods `Load(file_descriptor)` and `Loads(str)` to deserialize.
-Default functions for loading/setting keras weights and calculating deltas from keras models (which provide a get_weights(), set_weights() interface with lists of numpy arrays) are currently provided.
-**Important note when defining the functions**: in order for them to be serializable, they must be completely self-contained. That is, all imports should happen inside the functions and all the external function call should be implemented as nested functions. Common algorithms (such as padorcut.py which pads or cuts an image to fit it to a specific matrix size) should be placed in the repository.
+Metadata-Version: 2.1
+Name: dafne-dl
+Version: 1.3a4
+Summary: Deep Learning module for Dafne
+Home-page: https://github.com/dafne-imaging/dafne-dl
+Author: Francesco Santini
+Author-email: francesco.santini@unibas.ch
+Project-URL: Bug Tracker, https://github.com/dafne-imaging/dafne-dl/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: COPYING.LESSER
+
+Sets of classes and interfaces for the definition of deep learning models.
+The framework is conceived to be extensible and serializable, in order to provide models that can be stored and/or sent through the network.
+## Interfaces.py
+Set of abstract classes that describe models and model providers. 
+### DeepLearningClass
+The rationale behind this is that an algorithm not only depends on the model, but might require some preprocessing steps (reformatting, normalization) before the application of the model itself. The interface is also "incremental-learning-oriented" as it provides abstract methods for the calculation and integration of deltas. The class provides operator override for the calculation of deltas (D = A-B) and call override for the apply method.
+An instance of DeepLearningClass should be able to simply provide the expected result when called with the appropriate input data (in form of dict). The most common data for our case will be:
+
+ - Input: `{'image': 2D image, 'resolution': Sequence with pixel sizes}`
+ - Output: for Classifiers: `str`, for Segmenters: `dict[str: image]` where str is the label and the image is a 2D numpy array containing the mask corresponding to the string.
+
+### ModelProvider
+This is an abstract class that is intended to encapsulate the logic of model load/transfer. It will have two subclasses, LocalModelProvider and RemoteModelProvider. In both cases, the method load_model of this class accepts a description of the requested model and will return an instance of DeepLearningClass. In principle, LocalModelProvider will be used on the server, and RemoteModelProvider on the client.
+
+## DynamicDLModel
+Concrete implementation of a DeepLearningClass which provides flexibility and serialization. This class delegates the important methods of the model implementation to top-level functions that are passed at the construction time. These functions can be easily serialized with the dill library.
+Constructor:
+
+        def __init__(self, model_id, # a unique ID to avoid mixing different models
+                 init_model_function, # inits the model. Accepts no parameters and returns the model
+                 apply_model_function, # function that applies the model. Has the object, and image, and a sequence containing resolutions as parameters
+                 weights_to_model_function = default_keras_weights_to_model_function, # put model weights inside the model.
+                 model_to_weights_function = default_keras_model_to_weights_function, # get the weights from the model in a pickable format
+                 calc_delta_function = default_keras_delta_function, # calculate the weight delta
+                 apply_delta_function = default_keras_apply_delta_function, # apply a weight delta
+                 incremental_learn_function = None, # function to perform an incremental learning step
+                 weights = None): # initial weights
+This allows the implementation of a very generic deep learning algorithm which includes the preprocessing steps in a way that can be serialized and defined at runtime, so if we want to change the model, we don't need to change the code of the client or server, as the implementation is self-contained within the model.
+The class provides the methods `dump(file_descriptor)` and `str = dumps()` to serialize and the static methods `Load(file_descriptor)` and `Loads(str)` to deserialize.
+Default functions for loading/setting keras weights and calculating deltas from keras models (which provide a get_weights(), set_weights() interface with lists of numpy arrays) are currently provided.
+**Important note when defining the functions**: in order for them to be serializable, they must be completely self-contained. That is, all imports should happen inside the functions and all the external function call should be implemented as nested functions. Common algorithms (such as padorcut.py which pads or cuts an image to fit it to a specific matrix size) should be placed in the repository.
```

### Comparing `dafne-dl-1.3a3/README.md` & `dafne-dl-1.3a4/README.md`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Sets of classes and interfaces for the definition of deep learning models.
-The framework is conceived to be extensible and serializable, in order to provide models that can be stored and/or sent through the network.
-## Interfaces.py
-Set of abstract classes that describe models and model providers. 
-### DeepLearningClass
-The rationale behind this is that an algorithm not only depends on the model, but might require some preprocessing steps (reformatting, normalization) before the application of the model itself. The interface is also "incremental-learning-oriented" as it provides abstract methods for the calculation and integration of deltas. The class provides operator override for the calculation of deltas (D = A-B) and call override for the apply method.
-An instance of DeepLearningClass should be able to simply provide the expected result when called with the appropriate input data (in form of dict). The most common data for our case will be:
-
- - Input: `{'image': 2D image, 'resolution': Sequence with pixel sizes}`
- - Output: for Classifiers: `str`, for Segmenters: `dict[str: image]` where str is the label and the image is a 2D numpy array containing the mask corresponding to the string.
-
-### ModelProvider
-This is an abstract class that is intended to encapsulate the logic of model load/transfer. It will have two subclasses, LocalModelProvider and RemoteModelProvider. In both cases, the method load_model of this class accepts a description of the requested model and will return an instance of DeepLearningClass. In principle, LocalModelProvider will be used on the server, and RemoteModelProvider on the client.
-
-## DynamicDLModel
-Concrete implementation of a DeepLearningClass which provides flexibility and serialization. This class delegates the important methods of the model implementation to top-level functions that are passed at the construction time. These functions can be easily serialized with the dill library.
-Constructor:
-
-        def __init__(self, model_id, # a unique ID to avoid mixing different models
-                 init_model_function, # inits the model. Accepts no parameters and returns the model
-                 apply_model_function, # function that applies the model. Has the object, and image, and a sequence containing resolutions as parameters
-                 weights_to_model_function = default_keras_weights_to_model_function, # put model weights inside the model.
-                 model_to_weights_function = default_keras_model_to_weights_function, # get the weights from the model in a pickable format
-                 calc_delta_function = default_keras_delta_function, # calculate the weight delta
-                 apply_delta_function = default_keras_apply_delta_function, # apply a weight delta
-                 incremental_learn_function = None, # function to perform an incremental learning step
-                 weights = None): # initial weights
-This allows the implementation of a very generic deep learning algorithm which includes the preprocessing steps in a way that can be serialized and defined at runtime, so if we want to change the model, we don't need to change the code of the client or server, as the implementation is self-contained within the model.
-The class provides the methods `dump(file_descriptor)` and `str = dumps()` to serialize and the static methods `Load(file_descriptor)` and `Loads(str)` to deserialize.
-Default functions for loading/setting keras weights and calculating deltas from keras models (which provide a get_weights(), set_weights() interface with lists of numpy arrays) are currently provided.
-**Important note when defining the functions**: in order for them to be serializable, they must be completely self-contained. That is, all imports should happen inside the functions and all the external function call should be implemented as nested functions. Common algorithms (such as padorcut.py which pads or cuts an image to fit it to a specific matrix size) should be placed in the repository.
+Sets of classes and interfaces for the definition of deep learning models.
+The framework is conceived to be extensible and serializable, in order to provide models that can be stored and/or sent through the network.
+## Interfaces.py
+Set of abstract classes that describe models and model providers. 
+### DeepLearningClass
+The rationale behind this is that an algorithm not only depends on the model, but might require some preprocessing steps (reformatting, normalization) before the application of the model itself. The interface is also "incremental-learning-oriented" as it provides abstract methods for the calculation and integration of deltas. The class provides operator override for the calculation of deltas (D = A-B) and call override for the apply method.
+An instance of DeepLearningClass should be able to simply provide the expected result when called with the appropriate input data (in form of dict). The most common data for our case will be:
+
+ - Input: `{'image': 2D image, 'resolution': Sequence with pixel sizes}`
+ - Output: for Classifiers: `str`, for Segmenters: `dict[str: image]` where str is the label and the image is a 2D numpy array containing the mask corresponding to the string.
+
+### ModelProvider
+This is an abstract class that is intended to encapsulate the logic of model load/transfer. It will have two subclasses, LocalModelProvider and RemoteModelProvider. In both cases, the method load_model of this class accepts a description of the requested model and will return an instance of DeepLearningClass. In principle, LocalModelProvider will be used on the server, and RemoteModelProvider on the client.
+
+## DynamicDLModel
+Concrete implementation of a DeepLearningClass which provides flexibility and serialization. This class delegates the important methods of the model implementation to top-level functions that are passed at the construction time. These functions can be easily serialized with the dill library.
+Constructor:
+
+        def __init__(self, model_id, # a unique ID to avoid mixing different models
+                 init_model_function, # inits the model. Accepts no parameters and returns the model
+                 apply_model_function, # function that applies the model. Has the object, and image, and a sequence containing resolutions as parameters
+                 weights_to_model_function = default_keras_weights_to_model_function, # put model weights inside the model.
+                 model_to_weights_function = default_keras_model_to_weights_function, # get the weights from the model in a pickable format
+                 calc_delta_function = default_keras_delta_function, # calculate the weight delta
+                 apply_delta_function = default_keras_apply_delta_function, # apply a weight delta
+                 incremental_learn_function = None, # function to perform an incremental learning step
+                 weights = None): # initial weights
+This allows the implementation of a very generic deep learning algorithm which includes the preprocessing steps in a way that can be serialized and defined at runtime, so if we want to change the model, we don't need to change the code of the client or server, as the implementation is self-contained within the model.
+The class provides the methods `dump(file_descriptor)` and `str = dumps()` to serialize and the static methods `Load(file_descriptor)` and `Loads(str)` to deserialize.
+Default functions for loading/setting keras weights and calculating deltas from keras models (which provide a get_weights(), set_weights() interface with lists of numpy arrays) are currently provided.
+**Important note when defining the functions**: in order for them to be serializable, they must be completely self-contained. That is, all imports should happen inside the functions and all the external function call should be implemented as nested functions. Common algorithms (such as padorcut.py which pads or cuts an image to fit it to a specific matrix size) should be placed in the repository.
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/DynamicDLModel.py` & `dafne-dl-1.3a4/src/dafne_dl/DynamicDLModel.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,350 +1,350 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Implementation of a deep learning module that can be serialized and deserialized, and dynamically changed.
-Functions for the operation of the class are provided as references to top-level functions.
-Such top level functions should define all the imports within themselves (i.e. don't put the imports at the top of the file).
-"""
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-from __future__ import annotations
-
-import re
-
-from .interfaces import IncompatibleModelError, DeepLearningClass
-import dill
-from io import BytesIO
-import numpy as np
-import inspect
-import time
-
-def fn_to_source(function):
-    """
-    Given a function, returns it source. If the source cannot be retrieved, return the object itself
-    """
-    #print('Converting fn to source')
-    if function is None: return None
-    try:
-        return inspect.getsource(function)
-    except OSError:
-        #print('Conversion failed!')
-        try:
-            src = function.source
-            #print('Returning embedded source')
-            return src
-        except:
-            pass
-    print('Getting source failed - Returning bytecode')
-    return function # the source cannot be retrieved, return the object itself
-
-
-def source_to_fn(source, patches: dict = {}):
-    """
-    Given a source, return the (first) defined function. If the source is not a string, return the object itself
-    """
-    if type(source) is not str:
-        print("source to fn: source is not a string")
-        return source
-    #print("source to fn: source is string")
-    for search, replace in patches.items():
-        source = re.sub(search, replace, source)
-
-    locs = {}
-    globs = {}
-    try:
-        exec(source, globs, locs)
-    except:
-        return source # the string was just a string apparently, not valid code
-    for k,v in locs.items():
-        if callable(v):
-            #print('source_to_fn. Found function', k)
-            v.source = source
-            return v
-    return source
-
-
-def default_keras_weights_to_model_function(modelObj: DynamicDLModel, weights):
-    modelObj.model.set_weights(weights)
-
-
-def default_keras_model_to_weights_function(modelObj: DynamicDLModel):
-    return modelObj.model.get_weights()
-
-
-def default_keras_delta_function(lhs: DynamicDLModel, rhs: DynamicDLModel, threshold=None):
-    from dafne_dl.interfaces import IncompatibleModelError
-    if lhs.model_id != rhs.model_id: raise IncompatibleModelError
-    lhs_weights = lhs.get_weights()
-    rhs_weights = rhs.get_weights()
-    newWeights = []
-    for depth in range(len(lhs_weights)):
-        delta = lhs_weights[depth] - rhs_weights[depth]
-        if threshold is not None:
-            delta[np.abs(delta) < threshold] = 0
-        newWeights.append(delta)
-    outputObj = lhs.get_empty_copy()
-    outputObj.set_weights(newWeights)
-    outputObj.is_delta = True
-    outputObj.timestamp_id = rhs.timestamp_id # set the timestamp of the original model to identify the base
-    return outputObj
-
-
-def default_keras_add_weights_function(lhs: DynamicDLModel, rhs: DynamicDLModel):
-    from dafne_dl.interfaces import IncompatibleModelError
-    if lhs.model_id != rhs.model_id: raise IncompatibleModelError
-    lhs_weights = lhs.get_weights()
-    rhs_weights = rhs.get_weights()
-    newWeights = []
-    for depth in range(len(lhs_weights)):
-        newWeights.append(lhs_weights[depth] + rhs_weights[depth])
-    outputObj = lhs.get_empty_copy()
-    outputObj.set_weights(newWeights)
-    return outputObj
-
-
-def default_keras_multiply_function(lhs: DynamicDLModel, rhs: float):
-    if not isinstance(rhs, (int, float)):
-        raise NotImplementedError('Incompatible types for multiplication (only multiplication by numeric factor is allowed)')
-    lhs_weights = lhs.get_weights()
-    newWeights = []
-    for depth in range(len(lhs_weights)):
-        newWeights.append(lhs_weights[depth] * rhs)
-    outputObj = lhs.get_empty_copy()
-    outputObj.set_weights(newWeights)
-    return outputObj
-
-
-def default_keras_weight_copy_function(weights_in):
-    weights_out = []
-    for layer in weights_in:
-        weights_out.append(layer.copy())
-    return weights_out
-
-
-class DynamicDLModel(DeepLearningClass):
-
-    """
-    Class to represent a deep learning model that can be serialized/deserialized
-    """
-    def __init__(self, model_id,  # a unique ID to avoid mixing different models
-                 init_model_function,  # inits the model. Accepts no parameters and returns the model
-                 apply_model_function,  # function that applies the model. Has the object, and image
-                 weights_to_model_function = default_keras_weights_to_model_function,  # put model weights inside the model.
-                 model_to_weights_function = default_keras_model_to_weights_function,  # get the weights from the model in a pickable format
-                 calc_delta_function = default_keras_delta_function,  # calculate the weight delta
-                 apply_delta_function = default_keras_add_weights_function,  # apply a weight delta
-                 weight_copy_function = default_keras_weight_copy_function,  # create a deep copy of weights
-                 factor_multiply_function = default_keras_multiply_function,
-                 incremental_learn_function = None,  # function to perform an incremental learning step
-                 weights = None,  # initial weights
-                 timestamp_id = None,
-                 is_delta = False):
-        self.model = None
-        self.model_id = model_id
-        self.is_delta = is_delta
-
-        # lsit identifying the external functions that need to be saved with source and serialized
-        self.function_mappings = [
-            'init_model_function',
-            'apply_model_function',
-            'weights_to_model_function',
-            'model_to_weights_function',
-            'calc_delta_function',
-            'apply_delta_function',
-            'weight_copy_function',
-            'factor_multiply_function',
-            'incremental_learn_function',
-        ]
-
-        # the following sets the internal attributes self.fn = fn, with additionally adding the source to the function
-        for fn_name in self.function_mappings:
-            self.set_internal_fn(fn_name, locals()[fn_name])
-
-
-        self.init_model() # initializes the model
-        if timestamp_id is None:
-            self.reset_timestamp()
-        else:
-            self.timestamp_id = timestamp_id  # unique timestamp id; used to identify model versions during federated learning
-
-        if weights: self.set_weights(weights)
-
-    def set_internal_fn(self, internal_name, obj):
-        #print('Setting', internal_name)
-        if callable(obj):
-            src = fn_to_source(obj)
-            if type(src) == str:
-                obj.source = src
-
-        setattr(self, internal_name, obj)
-
-    def init_model(self):
-        """
-        Initializes the internal model
-
-        Returns
-        -------
-        None.
-
-        """
-        self.model = self.init_model_function()
-        
-    def set_weights(self, weights):
-        """
-        Loads the weights in the internal model
-
-        Parameters
-        ----------
-        weights : whatever is accepted by the model_to_weights_function
-            Weights to be loaded into the model
-
-        Returns
-        -------
-        None.
-
-        """
-        self.weights_to_model_function(self, weights)
-        
-    def get_weights(self):
-        return self.model_to_weights_function(self)
-        
-    def apply_delta(self, other):
-        return self.apply_delta_function(self, other)
-    
-    def calc_delta(self, other, threshold=None):
-        return self.calc_delta_function(self, other, threshold)
-    
-    def apply(self, data):
-        return self.apply_model_function(self, data)
-
-    def factor_multiply(self, factor: float):
-        return self.factor_multiply_function(self, factor)
-    
-    def incremental_learn(self, trainingData, trainingOutputs, bs=5, minTrainImages=5):
-        self.incremental_learn_function(self, trainingData, trainingOutputs, bs, minTrainImages)
-        
-    def dump(self, file):
-        """
-        Dumps the current status of the object, including functions and weights
-        
-        Parameters
-        ----------
-        file:
-            a file descriptor (open in writable mode)
-
-        Returns
-        -------
-        Nothing
-
-        """
-        outputDict = {
-            'model_id': self.model_id,
-            'weights': self.get_weights(),
-            'timestamp_id': self.timestamp_id,
-            'is_delta': self.is_delta
-            }
-
-        # add the internal functions to the dictionary
-        for fn_name in self.function_mappings:
-            outputDict[fn_name] = fn_to_source(getattr(self, fn_name))
-
-        dill.dump(outputDict, file)
-    
-    def dumps(self) -> bytes:
-        file = BytesIO()
-        self.dump(file)
-        return file.getvalue()
-    
-    def get_empty_copy(self) -> DynamicDLModel:
-        """
-        Gets an empty copy (i.e. without weights) of the current object
-
-        Returns
-        -------
-        DynamicDLModel
-            Output copy
-
-        """
-        new_model = DynamicDLModel(self.model_id, self.init_model_function, self.apply_model_function,
-                                   weights=None, timestamp_id=self.timestamp_id, is_delta=self.is_delta)
-        for fn_name in self.function_mappings:
-            new_model.set_internal_fn(fn_name, getattr(self, fn_name))
-        return new_model
-
-    def copy(self) -> DynamicDLModel:
-        """
-        Gets a copy (i.e. with weights) of the current object
-
-        Returns
-        -------
-        DynamicDLModel
-            Output copy
-
-        """
-        model_out = self.get_empty_copy()
-        model_out.set_weights( self.weight_copy_function(self.get_weights()) )
-        return model_out
-
-    @staticmethod
-    def Load(file) -> DynamicDLModel:
-        """
-        Creates an object from a file
-
-        Parameters
-        ----------
-        file : file descriptor
-            A file descriptor.
-
-        Returns
-        -------
-        DynamicDLModel
-            A new instance of a dynamic model
-
-        """
-
-        # code patches for on-the-fly conversion of old models to new format
-        patches = {
-            'from dl': 'from dafne_dl',
-            'import dl': 'import dafne_dl'
-        }
-
-        inputDict = dill.load(file)
-        for k,v in inputDict.items():
-            if '_function' in k:
-                inputDict[k] = source_to_fn(v, patches) # convert the functions from source
-
-        #print(inputDict)
-        outputObj = DynamicDLModel(**inputDict)
-        return outputObj
-        
-    @staticmethod
-    def Loads(b: bytes) -> DynamicDLModel:
-        """
-        Creates an object from a binary dump
-
-        Parameters
-        ----------
-        file : bytes
-            A sequence of bytes
-
-        Returns
-        -------
-        DynamicDLModel
-            A new instance of a dynamic model
-
-        """
-        file = BytesIO(b)
-        return DynamicDLModel.Load(file)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Implementation of a deep learning module that can be serialized and deserialized, and dynamically changed.
+Functions for the operation of the class are provided as references to top-level functions.
+Such top level functions should define all the imports within themselves (i.e. don't put the imports at the top of the file).
+"""
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from __future__ import annotations
+
+import re
+
+from .interfaces import IncompatibleModelError, DeepLearningClass
+import dill
+from io import BytesIO
+import numpy as np
+import inspect
+import time
+
+def fn_to_source(function):
+    """
+    Given a function, returns it source. If the source cannot be retrieved, return the object itself
+    """
+    #print('Converting fn to source')
+    if function is None: return None
+    try:
+        return inspect.getsource(function)
+    except OSError:
+        #print('Conversion failed!')
+        try:
+            src = function.source
+            #print('Returning embedded source')
+            return src
+        except:
+            pass
+    print('Getting source failed - Returning bytecode')
+    return function # the source cannot be retrieved, return the object itself
+
+
+def source_to_fn(source, patches: dict = {}):
+    """
+    Given a source, return the (first) defined function. If the source is not a string, return the object itself
+    """
+    if type(source) is not str:
+        print("source to fn: source is not a string")
+        return source
+    #print("source to fn: source is string")
+    for search, replace in patches.items():
+        source = re.sub(search, replace, source)
+
+    locs = {}
+    globs = {}
+    try:
+        exec(source, globs, locs)
+    except:
+        return source # the string was just a string apparently, not valid code
+    for k,v in locs.items():
+        if callable(v):
+            #print('source_to_fn. Found function', k)
+            v.source = source
+            return v
+    return source
+
+
+def default_keras_weights_to_model_function(modelObj: DynamicDLModel, weights):
+    modelObj.model.set_weights(weights)
+
+
+def default_keras_model_to_weights_function(modelObj: DynamicDLModel):
+    return modelObj.model.get_weights()
+
+
+def default_keras_delta_function(lhs: DynamicDLModel, rhs: DynamicDLModel, threshold=None):
+    from dafne_dl.interfaces import IncompatibleModelError
+    if lhs.model_id != rhs.model_id: raise IncompatibleModelError
+    lhs_weights = lhs.get_weights()
+    rhs_weights = rhs.get_weights()
+    newWeights = []
+    for depth in range(len(lhs_weights)):
+        delta = lhs_weights[depth] - rhs_weights[depth]
+        if threshold is not None:
+            delta[np.abs(delta) < threshold] = 0
+        newWeights.append(delta)
+    outputObj = lhs.get_empty_copy()
+    outputObj.set_weights(newWeights)
+    outputObj.is_delta = True
+    outputObj.timestamp_id = rhs.timestamp_id # set the timestamp of the original model to identify the base
+    return outputObj
+
+
+def default_keras_add_weights_function(lhs: DynamicDLModel, rhs: DynamicDLModel):
+    from dafne_dl.interfaces import IncompatibleModelError
+    if lhs.model_id != rhs.model_id: raise IncompatibleModelError
+    lhs_weights = lhs.get_weights()
+    rhs_weights = rhs.get_weights()
+    newWeights = []
+    for depth in range(len(lhs_weights)):
+        newWeights.append(lhs_weights[depth] + rhs_weights[depth])
+    outputObj = lhs.get_empty_copy()
+    outputObj.set_weights(newWeights)
+    return outputObj
+
+
+def default_keras_multiply_function(lhs: DynamicDLModel, rhs: float):
+    if not isinstance(rhs, (int, float)):
+        raise NotImplementedError('Incompatible types for multiplication (only multiplication by numeric factor is allowed)')
+    lhs_weights = lhs.get_weights()
+    newWeights = []
+    for depth in range(len(lhs_weights)):
+        newWeights.append(lhs_weights[depth] * rhs)
+    outputObj = lhs.get_empty_copy()
+    outputObj.set_weights(newWeights)
+    return outputObj
+
+
+def default_keras_weight_copy_function(weights_in):
+    weights_out = []
+    for layer in weights_in:
+        weights_out.append(layer.copy())
+    return weights_out
+
+
+class DynamicDLModel(DeepLearningClass):
+
+    """
+    Class to represent a deep learning model that can be serialized/deserialized
+    """
+    def __init__(self, model_id,  # a unique ID to avoid mixing different models
+                 init_model_function,  # inits the model. Accepts no parameters and returns the model
+                 apply_model_function,  # function that applies the model. Has the object, and image
+                 weights_to_model_function = default_keras_weights_to_model_function,  # put model weights inside the model.
+                 model_to_weights_function = default_keras_model_to_weights_function,  # get the weights from the model in a pickable format
+                 calc_delta_function = default_keras_delta_function,  # calculate the weight delta
+                 apply_delta_function = default_keras_add_weights_function,  # apply a weight delta
+                 weight_copy_function = default_keras_weight_copy_function,  # create a deep copy of weights
+                 factor_multiply_function = default_keras_multiply_function,
+                 incremental_learn_function = None,  # function to perform an incremental learning step
+                 weights = None,  # initial weights
+                 timestamp_id = None,
+                 is_delta = False):
+        self.model = None
+        self.model_id = model_id
+        self.is_delta = is_delta
+
+        # lsit identifying the external functions that need to be saved with source and serialized
+        self.function_mappings = [
+            'init_model_function',
+            'apply_model_function',
+            'weights_to_model_function',
+            'model_to_weights_function',
+            'calc_delta_function',
+            'apply_delta_function',
+            'weight_copy_function',
+            'factor_multiply_function',
+            'incremental_learn_function',
+        ]
+
+        # the following sets the internal attributes self.fn = fn, with additionally adding the source to the function
+        for fn_name in self.function_mappings:
+            self.set_internal_fn(fn_name, locals()[fn_name])
+
+
+        self.init_model() # initializes the model
+        if timestamp_id is None:
+            self.reset_timestamp()
+        else:
+            self.timestamp_id = timestamp_id  # unique timestamp id; used to identify model versions during federated learning
+
+        if weights: self.set_weights(weights)
+
+    def set_internal_fn(self, internal_name, obj):
+        #print('Setting', internal_name)
+        if callable(obj):
+            src = fn_to_source(obj)
+            if type(src) == str:
+                obj.source = src
+
+        setattr(self, internal_name, obj)
+
+    def init_model(self):
+        """
+        Initializes the internal model
+
+        Returns
+        -------
+        None.
+
+        """
+        self.model = self.init_model_function()
+        
+    def set_weights(self, weights):
+        """
+        Loads the weights in the internal model
+
+        Parameters
+        ----------
+        weights : whatever is accepted by the model_to_weights_function
+            Weights to be loaded into the model
+
+        Returns
+        -------
+        None.
+
+        """
+        self.weights_to_model_function(self, weights)
+        
+    def get_weights(self):
+        return self.model_to_weights_function(self)
+        
+    def apply_delta(self, other):
+        return self.apply_delta_function(self, other)
+    
+    def calc_delta(self, other, threshold=None):
+        return self.calc_delta_function(self, other, threshold)
+    
+    def apply(self, data):
+        return self.apply_model_function(self, data)
+
+    def factor_multiply(self, factor: float):
+        return self.factor_multiply_function(self, factor)
+    
+    def incremental_learn(self, trainingData, trainingOutputs, bs=5, minTrainImages=5):
+        self.incremental_learn_function(self, trainingData, trainingOutputs, bs, minTrainImages)
+        
+    def dump(self, file):
+        """
+        Dumps the current status of the object, including functions and weights
+        
+        Parameters
+        ----------
+        file:
+            a file descriptor (open in writable mode)
+
+        Returns
+        -------
+        Nothing
+
+        """
+        outputDict = {
+            'model_id': self.model_id,
+            'weights': self.get_weights(),
+            'timestamp_id': self.timestamp_id,
+            'is_delta': self.is_delta
+            }
+
+        # add the internal functions to the dictionary
+        for fn_name in self.function_mappings:
+            outputDict[fn_name] = fn_to_source(getattr(self, fn_name))
+
+        dill.dump(outputDict, file)
+    
+    def dumps(self) -> bytes:
+        file = BytesIO()
+        self.dump(file)
+        return file.getvalue()
+    
+    def get_empty_copy(self) -> DynamicDLModel:
+        """
+        Gets an empty copy (i.e. without weights) of the current object
+
+        Returns
+        -------
+        DynamicDLModel
+            Output copy
+
+        """
+        new_model = DynamicDLModel(self.model_id, self.init_model_function, self.apply_model_function,
+                                   weights=None, timestamp_id=self.timestamp_id, is_delta=self.is_delta)
+        for fn_name in self.function_mappings:
+            new_model.set_internal_fn(fn_name, getattr(self, fn_name))
+        return new_model
+
+    def copy(self) -> DynamicDLModel:
+        """
+        Gets a copy (i.e. with weights) of the current object
+
+        Returns
+        -------
+        DynamicDLModel
+            Output copy
+
+        """
+        model_out = self.get_empty_copy()
+        model_out.set_weights( self.weight_copy_function(self.get_weights()) )
+        return model_out
+
+    @staticmethod
+    def Load(file) -> DynamicDLModel:
+        """
+        Creates an object from a file
+
+        Parameters
+        ----------
+        file : file descriptor
+            A file descriptor.
+
+        Returns
+        -------
+        DynamicDLModel
+            A new instance of a dynamic model
+
+        """
+
+        # code patches for on-the-fly conversion of old models to new format
+        patches = {
+            'from dl': 'from dafne_dl',
+            'import dl': 'import dafne_dl'
+        }
+
+        inputDict = dill.load(file)
+        for k,v in inputDict.items():
+            if '_function' in k:
+                inputDict[k] = source_to_fn(v, patches) # convert the functions from source
+
+        #print(inputDict)
+        outputObj = DynamicDLModel(**inputDict)
+        return outputObj
+        
+    @staticmethod
+    def Loads(b: bytes) -> DynamicDLModel:
+        """
+        Creates an object from a binary dump
+
+        Parameters
+        ----------
+        file : bytes
+            A sequence of bytes
+
+        Returns
+        -------
+        DynamicDLModel
+            A new instance of a dynamic model
+
+        """
+        file = BytesIO(b)
+        return DynamicDLModel.Load(file)
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/RemoteModelProvider.py` & `dafne-dl-1.3a4/src/dafne_dl/RemoteModelProvider.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-import json
-import os
-from copy import copy
-from pathlib import Path
-import requests
-
-from .interfaces import ModelProvider
-from .DynamicDLModel import DynamicDLModel
-from typing import IO, Callable, List, Union, Optional
-import threading
-import time
-import datetime
-from .misc import calculate_file_hash
-
-UPLOAD_RETRIES = 3
-TIME_BETWEEN_RETRIES = 10
-
-
-def upload_model(url_base, filename, model_name, api_key, dice):
-    print('Calculating hash...')
-    file_hash = calculate_file_hash(filename)
-    print(file_hash)
-    for retries in range(UPLOAD_RETRIES):
-        print(f"Sending {filename}")
-        with open(filename, 'rb') as f:
-            files = {'model_binary': f}
-            r = requests.post(url_base + "upload_model",
-                              files=files,
-                              data={"model_type": model_name,
-                                    "api_key": api_key,
-                                    "dice": dice,
-                                    "hash": file_hash})
-        print(f"status code: {r.status_code}")
-        try:
-            print(f"message: {r.json()['message']}")
-        except:
-            pass
-
-        if r.status_code == 200:
-            print("upload successful") # success
-            break
-        print('Upload error')
-        time.sleep(TIME_BETWEEN_RETRIES)
-    os.remove(filename)
-
-
-def upload_data(url_base, filename, api_key):
-    for retries in range(UPLOAD_RETRIES):
-        print(f"Sending {filename}")
-        with open(filename, 'rb') as f:
-            files = {'data_binary': f}
-            r = requests.post(url_base + "upload_data",
-                              files=files,
-                              data={"api_key": api_key})
-        print(f"status code: {r.status_code}")
-        try:
-            print(f"message: {r.json()['message']}")
-        except:
-            pass
-
-        if r.status_code == 200:
-            print("upload successful") # success
-            break
-        print('Upload error')
-        time.sleep(TIME_BETWEEN_RETRIES)
-    os.remove(filename)
-
-
-class RemoteModelProvider(ModelProvider):
-    
-    def __init__(self, models_path, url_base, api_key, temp_upload_dir, delete_old_models = True):
-        self.models_path = Path(models_path)
-        self.url_base = url_base
-        self.api_key = api_key
-        self.temp_upload_dir = temp_upload_dir
-        self.delete_old_models = delete_old_models
-        os.makedirs(self.models_path, exist_ok=True)
-        print(f"Config: {self.url_base}, {self.api_key}")
-
-    def load_model(self, model_name: str, progress_callback: Optional[Callable[[int, int], None]] = None,
-                   force_download: bool = False,
-                   timestamp: Optional[Union[int,str]] = None) -> DynamicDLModel:
-        """
-        Load latest model from remote server if it does not already exist locally.
-
-        Parameters
-        ----------
-        model_name : str
-            The name of the model to load.
-        progress_callback: Callable[[int, int], None] (optional)
-            Callback function for progress
-        force_download: bool
-            Sets the forced redownload of models
-        timestamp: int or None
-            Return a specific model version (default: latest)
-
-        Returns
-        -------
-        The model object.
-        """
-        print(f"Loading model: {model_name}")
-
-        json_content = self.model_details(model_name)
-
-        if json_content is None:
-            return None
-
-        # Get the name of the latest model
-        r = requests.post(self.url_base + "info_model",
-                          json={"model_type": model_name,
-                                "api_key": self.api_key})
-
-        if timestamp is None:
-            timestamp = json_content['latest_timestamp']
-
-        timestamp = str(timestamp)
-
-        try:
-            hash_dict = json_content['hashes']
-            file_hash_remote = hash_dict[timestamp]
-        except:
-            file_hash_remote = json_content['hash'] # fallback to latest hash
-
-        # Check if model already exists locally
-        local_model_path = self.models_path / f"{model_name}_{timestamp}.model"
-        if os.path.exists(local_model_path) and not force_download:
-            print("Model already downloaded. Checking hash...")
-            file_hash_local = calculate_file_hash(local_model_path)
-            if file_hash_local == file_hash_remote:
-                print('Model exists, skipping download')
-                model = DynamicDLModel.Load(open(local_model_path, 'rb'))
-                return model
-            else:
-                print('Local model is corrupt')
-                os.remove(local_model_path)
-
-        print("Downloading new model...")
-
-        # Receive model
-        r = requests.post(self.url_base + "get_model",
-                          json={"model_type": model_name,
-                                "timestamp": timestamp,
-                                "api_key": self.api_key},
-                          stream=True)
-        success = False
-        if r.ok:
-            success = True
-            total_size_in_bytes = int(r.headers.get('content-length', 0))
-            print("Size to download:", total_size_in_bytes)
-            block_size = 1024*1024  # 1 MB
-            current_size = 0
-            with open(local_model_path, 'wb') as file:
-                for data in r.iter_content(block_size):
-                    current_size += len(data)
-                    #print(current_size)
-                    if progress_callback is not None:
-                        progress_callback(current_size, total_size_in_bytes)
-                    file.write(data)
-
-            print("Downloaded size", current_size)
-            file_hash_local = calculate_file_hash(local_model_path)
-
-            if current_size != total_size_in_bytes or file_hash_local != file_hash_remote:
-                print("Download failed!")
-                os.remove(local_model_path)
-                success = False
-
-        if success:
-            print('Model check OK')
-            model = DynamicDLModel.Load(open(local_model_path, "rb"))
-
-            if self.delete_old_models:
-                # Deleting older models
-                old_models = self.models_path.glob(f"{model_name}_*.model")
-                print("Deleting old models: ")
-                for old_model in old_models:
-                    if old_model != local_model_path:
-                        print(f"  Deleting: {str(old_model)}")
-                        os.remove(old_model)
-            return model
-        else:
-            print("ERROR: Request to server failed")
-            print(f"status code: {r.status_code}")
-            try:
-                print(f"message: {r.json()['message']}")
-            except:
-                pass
-            return None
-
-    def model_details(self, model_name: str) -> dict:
-        # get model versions
-        # Get the name of the latest model
-        r = requests.post(self.url_base + "info_model",
-                          json={"model_type": model_name,
-                                "api_key": self.api_key})
-        if r.ok:
-            json_content = r.json()
-        else:
-            print("ERROR: Request to server failed")
-            print(f"status code: {r.status_code}")
-            try:
-                print(f"message: {r.json()['message']}")
-            except:
-                pass
-            return None
-
-        # store json data in cache without the model-specific parts
-        json_out = copy(json_content)
-        keys_to_delete = ['hash', 'hashes', 'latest_timestamp', 'timestamps']
-        for k in keys_to_delete:
-            try:
-                del json_out[k]
-            except KeyError:
-                pass
-
-        json.dump(json_out, open(self.models_path / f'{model_name}.json', 'w'))
-
-        print("Model details:", json_content)
-
-        return json_content
-
-    def available_models(self) -> Union[None, List[str]]:
-        r = requests.post(self.url_base + "get_available_models",
-                          json={"api_key": self.api_key})
-        if r.ok:
-            models = r.json()['models']
-            return models
-        else:
-            print(f"status code: {r.status_code}")
-            try:
-                print(f"message: {r.json()['message']}")
-            except:
-                pass
-            if r.status_code == 401:
-                raise PermissionError("Your api_key is invalid.")
-            return None
-
-    def upload_model(self, model_name: str, model: DynamicDLModel, dice_score: float = 0.0):
-        """
-        Upload model to server
-        
-        Args:
-            model_name: classifier | thigh | leg
-            model: DynamicDLModel
-        """
-        print("Uploading model...")
-        filename_out = os.path.join(self.temp_upload_dir, f'{model_name}_{model.timestamp_id}.model')
-        model.dump(open(filename_out, 'wb'))
-        upload_thread = threading.Thread(target=upload_model, args=(self.url_base, filename_out, model_name,
-                                                                    self.api_key, dice_score))
-        upload_thread.start()
-
-    def _upload_bytes(self, data: IO):
-        # Note: the don't pass data directly to requests because the byte stream is not at the start.
-        # Use getbuffer or getvalue instead. See https://github.com/psf/requests/issues/2589
-        print("Uploading data")
-        filename = datetime.datetime.now().strftime("data_%Y%m%d_%H%M%S.npz")
-        filename_out = os.path.join(self.temp_upload_dir, filename)
-        with open(filename_out, 'wb') as f:
-            f.write(data.getbuffer())
-        upload_thread = threading.Thread(target=upload_data, args=(self.url_base, filename_out, self.api_key))
-        upload_thread.start()
-
-    def log(self, msg: str):
-        r = requests.post(self.url_base + "log",
-                        json={"api_key": self.api_key,
-                              "message": str(msg)})
-
-        if not r.ok:
-            if r.status_code == 401:
-                raise PermissionError("Your api_key is invalid.")
-            else:
-                raise OSError("Error communicating with server")
-
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+import json
+import os
+from copy import copy
+from pathlib import Path
+import requests
+
+from .interfaces import ModelProvider
+from .DynamicDLModel import DynamicDLModel
+from typing import IO, Callable, List, Union, Optional
+import threading
+import time
+import datetime
+from .misc import calculate_file_hash
+
+UPLOAD_RETRIES = 3
+TIME_BETWEEN_RETRIES = 10
+
+
+def upload_model(url_base, filename, model_name, api_key, dice):
+    print('Calculating hash...')
+    file_hash = calculate_file_hash(filename)
+    print(file_hash)
+    for retries in range(UPLOAD_RETRIES):
+        print(f"Sending {filename}")
+        with open(filename, 'rb') as f:
+            files = {'model_binary': f}
+            r = requests.post(url_base + "upload_model",
+                              files=files,
+                              data={"model_type": model_name,
+                                    "api_key": api_key,
+                                    "dice": dice,
+                                    "hash": file_hash})
+        print(f"status code: {r.status_code}")
+        try:
+            print(f"message: {r.json()['message']}")
+        except:
+            pass
+
+        if r.status_code == 200:
+            print("upload successful") # success
+            break
+        print('Upload error')
+        time.sleep(TIME_BETWEEN_RETRIES)
+    os.remove(filename)
+
+
+def upload_data(url_base, filename, api_key):
+    for retries in range(UPLOAD_RETRIES):
+        print(f"Sending {filename}")
+        with open(filename, 'rb') as f:
+            files = {'data_binary': f}
+            r = requests.post(url_base + "upload_data",
+                              files=files,
+                              data={"api_key": api_key})
+        print(f"status code: {r.status_code}")
+        try:
+            print(f"message: {r.json()['message']}")
+        except:
+            pass
+
+        if r.status_code == 200:
+            print("upload successful") # success
+            break
+        print('Upload error')
+        time.sleep(TIME_BETWEEN_RETRIES)
+    os.remove(filename)
+
+
+class RemoteModelProvider(ModelProvider):
+    
+    def __init__(self, models_path, url_base, api_key, temp_upload_dir, delete_old_models = True):
+        self.models_path = Path(models_path)
+        self.url_base = url_base
+        self.api_key = api_key
+        self.temp_upload_dir = temp_upload_dir
+        self.delete_old_models = delete_old_models
+        os.makedirs(self.models_path, exist_ok=True)
+        print(f"Config: {self.url_base}, {self.api_key}")
+
+    def load_model(self, model_name: str, progress_callback: Optional[Callable[[int, int], None]] = None,
+                   force_download: bool = False,
+                   timestamp: Optional[Union[int,str]] = None) -> DynamicDLModel:
+        """
+        Load latest model from remote server if it does not already exist locally.
+
+        Parameters
+        ----------
+        model_name : str
+            The name of the model to load.
+        progress_callback: Callable[[int, int], None] (optional)
+            Callback function for progress
+        force_download: bool
+            Sets the forced redownload of models
+        timestamp: int or None
+            Return a specific model version (default: latest)
+
+        Returns
+        -------
+        The model object.
+        """
+        print(f"Loading model: {model_name}")
+
+        json_content = self.model_details(model_name)
+
+        if json_content is None:
+            return None
+
+        # Get the name of the latest model
+        r = requests.post(self.url_base + "info_model",
+                          json={"model_type": model_name,
+                                "api_key": self.api_key})
+
+        if timestamp is None:
+            timestamp = json_content['latest_timestamp']
+
+        timestamp = str(timestamp)
+
+        try:
+            hash_dict = json_content['hashes']
+            file_hash_remote = hash_dict[timestamp]
+        except:
+            file_hash_remote = json_content['hash'] # fallback to latest hash
+
+        # Check if model already exists locally
+        local_model_path = self.models_path / f"{model_name}_{timestamp}.model"
+        if os.path.exists(local_model_path) and not force_download:
+            print("Model already downloaded. Checking hash...")
+            file_hash_local = calculate_file_hash(local_model_path)
+            if file_hash_local == file_hash_remote:
+                print('Model exists, skipping download')
+                model = DynamicDLModel.Load(open(local_model_path, 'rb'))
+                return model
+            else:
+                print('Local model is corrupt')
+                os.remove(local_model_path)
+
+        print("Downloading new model...")
+
+        # Receive model
+        r = requests.post(self.url_base + "get_model",
+                          json={"model_type": model_name,
+                                "timestamp": timestamp,
+                                "api_key": self.api_key},
+                          stream=True)
+        success = False
+        if r.ok:
+            success = True
+            total_size_in_bytes = int(r.headers.get('content-length', 0))
+            print("Size to download:", total_size_in_bytes)
+            block_size = 1024*1024  # 1 MB
+            current_size = 0
+            with open(local_model_path, 'wb') as file:
+                for data in r.iter_content(block_size):
+                    current_size += len(data)
+                    #print(current_size)
+                    if progress_callback is not None:
+                        progress_callback(current_size, total_size_in_bytes)
+                    file.write(data)
+
+            print("Downloaded size", current_size)
+            file_hash_local = calculate_file_hash(local_model_path)
+
+            if current_size != total_size_in_bytes or file_hash_local != file_hash_remote:
+                print("Download failed!")
+                os.remove(local_model_path)
+                success = False
+
+        if success:
+            print('Model check OK')
+            model = DynamicDLModel.Load(open(local_model_path, "rb"))
+
+            if self.delete_old_models:
+                # Deleting older models
+                old_models = self.models_path.glob(f"{model_name}_*.model")
+                print("Deleting old models: ")
+                for old_model in old_models:
+                    if old_model != local_model_path:
+                        print(f"  Deleting: {str(old_model)}")
+                        os.remove(old_model)
+            return model
+        else:
+            print("ERROR: Request to server failed")
+            print(f"status code: {r.status_code}")
+            try:
+                print(f"message: {r.json()['message']}")
+            except:
+                pass
+            return None
+
+    def model_details(self, model_name: str) -> dict:
+        # get model versions
+        # Get the name of the latest model
+        r = requests.post(self.url_base + "info_model",
+                          json={"model_type": model_name,
+                                "api_key": self.api_key})
+        if r.ok:
+            json_content = r.json()
+        else:
+            print("ERROR: Request to server failed")
+            print(f"status code: {r.status_code}")
+            try:
+                print(f"message: {r.json()['message']}")
+            except:
+                pass
+            return None
+
+        # store json data in cache without the model-specific parts
+        json_out = copy(json_content)
+        keys_to_delete = ['hash', 'hashes', 'latest_timestamp', 'timestamps']
+        for k in keys_to_delete:
+            try:
+                del json_out[k]
+            except KeyError:
+                pass
+
+        json.dump(json_out, open(self.models_path / f'{model_name}.json', 'w'))
+
+        print("Model details:", json_content)
+
+        return json_content
+
+    def available_models(self) -> Union[None, List[str]]:
+        r = requests.post(self.url_base + "get_available_models",
+                          json={"api_key": self.api_key})
+        if r.ok:
+            models = r.json()['models']
+            return models
+        else:
+            print(f"status code: {r.status_code}")
+            try:
+                print(f"message: {r.json()['message']}")
+            except:
+                pass
+            if r.status_code == 401:
+                raise PermissionError("Your api_key is invalid.")
+            return None
+
+    def upload_model(self, model_name: str, model: DynamicDLModel, dice_score: float = 0.0):
+        """
+        Upload model to server
+        
+        Args:
+            model_name: classifier | thigh | leg
+            model: DynamicDLModel
+        """
+        print("Uploading model...")
+        filename_out = os.path.join(self.temp_upload_dir, f'{model_name}_{model.timestamp_id}.model')
+        model.dump(open(filename_out, 'wb'))
+        upload_thread = threading.Thread(target=upload_model, args=(self.url_base, filename_out, model_name,
+                                                                    self.api_key, dice_score))
+        upload_thread.start()
+
+    def _upload_bytes(self, data: IO):
+        # Note: the don't pass data directly to requests because the byte stream is not at the start.
+        # Use getbuffer or getvalue instead. See https://github.com/psf/requests/issues/2589
+        print("Uploading data")
+        filename = datetime.datetime.now().strftime("data_%Y%m%d_%H%M%S.npz")
+        filename_out = os.path.join(self.temp_upload_dir, filename)
+        with open(filename_out, 'wb') as f:
+            f.write(data.getbuffer())
+        upload_thread = threading.Thread(target=upload_data, args=(self.url_base, filename_out, self.api_key))
+        upload_thread.start()
+
+    def log(self, msg: str):
+        r = requests.post(self.url_base + "log",
+                        json={"api_key": self.api_key,
+                              "message": str(msg)})
+
+        if not r.ok:
+            if r.status_code == 401:
+                raise PermissionError("Your api_key is invalid.")
+            else:
+                raise OSError("Error communicating with server")
+
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/__init__.py` & `dafne-dl-1.3a4/src/dafne_dl/labels/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,21 @@
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-# -*- coding: utf-8 -*-
-
-VERSION='1.3-alpha3'
-
-from . import resources
-
-import sys
-import flexidep
-
-assert sys.version_info.major == 3, "This software is only compatible with Python 3.x"
-
-if sys.version_info.minor < 10:
-    import importlib_resources as pkg_resources
-else:
-    import importlib.resources as pkg_resources
-
-# install the required resources
-if not flexidep.is_frozen():
-    with pkg_resources.files(resources).joinpath('runtime_dependencies.cfg').open() as f:
-        dm = flexidep.DependencyManager(config_file=f)
-    dm.install_auto()
-
-from .DynamicDLModel import DynamicDLModel
-from .LocalModelProvider import LocalModelProvider
-from .RemoteModelProvider import RemoteModelProvider
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+def invert_dict(d):
+    return { v:k for k,v in d.items() }
+
+# the nice union operator was introduced in python 3.9. Let's be compatible with older versions too
+def merge_dict(a,b):
+    return { **a, **b }
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/common/DataGenerators.py` & `dafne-dl-1.3a4/src/dafne_dl/common/DataGenerators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-# Data generator classes - from directory or from memory
-#from collections import Sequence
-from tensorflow.keras.utils import Sequence
-import numpy as np
-import os
-
-# This is NOT a general implementation! See the number of masks below
-class DataGeneratorDir(Sequence):
-    def __init__(self, path, list_X=list(range(1, 4501)), batch_size=20, dim=(432, 432), shuffle=True):
-        'Initialization'
-        self.dim = dim
-        self.batch_size = batch_size
-        self.list_X = list_X
-        self.path = path
-        self.shuffle = shuffle
-        self.on_epoch_end()
-
-    def __len__(self):
-        'Denotes the number of batches per epoch'
-        return int(np.floor(len(self.list_X) / self.batch_size))
-
-    def __getitem__(self, index):
-        'Generate one batch of data'
-        # Generate indexes of the batch
-        indexes = self.indexes[index * self.batch_size:(index + 1) * self.batch_size]
-
-        # Find list of IDs
-        list_X_temp = [self.list_X[k] for k in indexes]
-
-        # Generate data
-        X, y = self.__data_generation(list_X_temp, self.path)
-
-        return X, y
-
-    def on_epoch_end(self):
-        'Updates indexes after each epoch'
-        self.indexes = np.arange(len(self.list_X))
-        if self.shuffle == True:
-            np.random.shuffle(self.indexes)
-
-    def __data_generation(self, list_X_temp, path):
-        'Generates data containing batch_size samples'
-        # Initialization
-        X = np.empty((self.batch_size, *self.dim, 2))
-        y = np.empty((self.batch_size, *self.dim, 13)) # chenge this to be generic!
-
-        # Generate data
-        for i, j in enumerate(list_X_temp):
-            # Store sample
-            arr = np.load(os.path.join(path, 'train_' + str(j) + '.npy'))
-
-            X[i,] = np.stack([arr[:, :, 0], arr[:, :, -1]], axis=-1)
-
-            # Store class
-            y[i,] = arr[:, :, 1:-1]
-
-        return X, y
-
-class DataGeneratorMem(Sequence):
-    def __init__(self, training_data_list, list_X=list(range(1, 4501)), batch_size=20, dim=(432, 432), shuffle=True):
-        print('Data Generator Initialization. Data list len:', len(training_data_list))
-        print('list_X', list_X)
-        self.dim = dim
-        self.batch_size = batch_size
-        self.list_X = list_X
-        self.training_data_list = training_data_list
-        self.shuffle = shuffle
-        self.on_epoch_end()
-        self.n_labels = training_data_list[0].shape[2]-2
-
-    def __len__(self):
-        'Denotes the number of batches per epoch'
-        return int(np.floor(len(self.list_X) / self.batch_size))
-
-    def __getitem__(self, index):
-        'Generate one batch of data'
-        # Generate indexes of the batch
-        indexes = self.indexes[index * self.batch_size:(index + 1) * self.batch_size]
-
-        # Find list of IDs
-        list_X_temp = [self.list_X[k] for k in indexes]
-        print("list_X_temp", list_X_temp)
-
-        # Generate data
-        X, y = self.__data_generation(list_X_temp)
-
-        return X, y
-
-    def on_epoch_end(self):
-        'Updates indexes after each epoch'
-        self.indexes = np.arange(len(self.list_X))
-        if self.shuffle == True:
-            np.random.shuffle(self.indexes)
-
-    def __data_generation(self, list_X_temp):
-        'Generates data containing batch_size samples'
-        # Initialization
-        X = np.empty((self.batch_size, *self.dim, 2))
-        y = np.empty((self.batch_size, *self.dim, self.n_labels))
-
-        # Generate data
-        for i, j in enumerate(list_X_temp):
-            # Store sample
-            arr = self.training_data_list[j]
-
-            #X[i,] = np.stack([arr[:, :, 0], arr[:, :, -1]], axis=-1)
-            X[i, :, :, 0] = arr[:, :, 0]
-            X[i, :, :, 1] = arr[:, :, -1]
-
-            # Store class
-            y[i,] = arr[:, :, 1:-1]
-
-        return X, y
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+# Data generator classes - from directory or from memory
+#from collections import Sequence
+from tensorflow.keras.utils import Sequence
+import numpy as np
+import os
+
+# This is NOT a general implementation! See the number of masks below
+class DataGeneratorDir(Sequence):
+    def __init__(self, path, list_X=list(range(1, 4501)), batch_size=20, dim=(432, 432), shuffle=True):
+        'Initialization'
+        self.dim = dim
+        self.batch_size = batch_size
+        self.list_X = list_X
+        self.path = path
+        self.shuffle = shuffle
+        self.on_epoch_end()
+
+    def __len__(self):
+        'Denotes the number of batches per epoch'
+        return int(np.floor(len(self.list_X) / self.batch_size))
+
+    def __getitem__(self, index):
+        'Generate one batch of data'
+        # Generate indexes of the batch
+        indexes = self.indexes[index * self.batch_size:(index + 1) * self.batch_size]
+
+        # Find list of IDs
+        list_X_temp = [self.list_X[k] for k in indexes]
+
+        # Generate data
+        X, y = self.__data_generation(list_X_temp, self.path)
+
+        return X, y
+
+    def on_epoch_end(self):
+        'Updates indexes after each epoch'
+        self.indexes = np.arange(len(self.list_X))
+        if self.shuffle == True:
+            np.random.shuffle(self.indexes)
+
+    def __data_generation(self, list_X_temp, path):
+        'Generates data containing batch_size samples'
+        # Initialization
+        X = np.empty((self.batch_size, *self.dim, 2))
+        y = np.empty((self.batch_size, *self.dim, 13)) # chenge this to be generic!
+
+        # Generate data
+        for i, j in enumerate(list_X_temp):
+            # Store sample
+            arr = np.load(os.path.join(path, 'train_' + str(j) + '.npy'))
+
+            X[i,] = np.stack([arr[:, :, 0], arr[:, :, -1]], axis=-1)
+
+            # Store class
+            y[i,] = arr[:, :, 1:-1]
+
+        return X, y
+
+class DataGeneratorMem(Sequence):
+    def __init__(self, training_data_list, list_X=list(range(1, 4501)), batch_size=20, dim=(432, 432), shuffle=True):
+        #print('Data Generator Initialization. Data list len:', len(training_data_list))
+        #print('list_X', list_X)
+        self.dim = dim
+        self.batch_size = batch_size
+        self.list_X = list_X
+        self.training_data_list = training_data_list
+        self.shuffle = shuffle
+        self.on_epoch_end()
+        self.n_labels = training_data_list[0].shape[2]-2
+
+    def __len__(self):
+        'Denotes the number of batches per epoch'
+        return int(np.floor(len(self.list_X) / self.batch_size))
+
+    def __getitem__(self, index):
+        'Generate one batch of data'
+        # Generate indexes of the batch
+        indexes = self.indexes[index * self.batch_size:(index + 1) * self.batch_size]
+
+        # Find list of IDs
+        list_X_temp = [self.list_X[k] for k in indexes]
+        #print("list_X_temp", list_X_temp)
+
+        # Generate data
+        X, y = self.__data_generation(list_X_temp)
+
+        return X, y
+
+    def on_epoch_end(self):
+        'Updates indexes after each epoch'
+        self.indexes = np.arange(len(self.list_X))
+        if self.shuffle == True:
+            np.random.shuffle(self.indexes)
+
+    def __data_generation(self, list_X_temp):
+        'Generates data containing batch_size samples'
+        # Initialization
+        X = np.empty((self.batch_size, *self.dim, 2))
+        y = np.empty((self.batch_size, *self.dim, self.n_labels))
+
+        # Generate data
+        for i, j in enumerate(list_X_temp):
+            # Store sample
+            arr = self.training_data_list[j]
+
+            #X[i,] = np.stack([arr[:, :, 0], arr[:, :, -1]], axis=-1)
+            X[i, :, :, 0] = arr[:, :, 0]
+            X[i, :, :, 1] = arr[:, :, -1]
+
+            # Store class
+            y[i,] = arr[:, :, 1:-1]
+
+        return X, y
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/common/__init__.py` & `dafne-dl-1.3a4/src/dafne_dl/labels/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/common/biascorrection.py` & `dafne-dl-1.3a4/src/dafne_dl/common/biascorrection.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-# -*- coding: utf-8 -*-
-
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-import SimpleITK as sitk
-
-DEFAULT_BIAS_CORRECTION_LEVELS = 8
-
-
-def biascorrection(file_or_image, levels=DEFAULT_BIAS_CORRECTION_LEVELS):
-    if type(file_or_image) == str:
-        return biascorrection_file(file_or_image, levels)
-    else:
-        return biascorrection_image(file_or_image, levels)
-
-
-def biascorrection_image(image, levels=DEFAULT_BIAS_CORRECTION_LEVELS):
-    MAX_GRAY_VALUE = 600
-    if not type(image) == sitk.SimpleITK.Image:
-        # normalize values
-        image = image*MAX_GRAY_VALUE/image.max()
-        image = sitk.GetImageFromArray(image)
-        image = sitk.Cast(image, sitk.sitkFloat32)
-    else:
-        image = sitk.GetArrayFromImage(image)
-        image = image * MAX_GRAY_VALUE / image.max()
-        image = sitk.GetImageFromArray(image)
-        image = sitk.Cast(image, sitk.sitkFloat32)
-
-    maskImage = sitk.OtsuThreshold(image, 0, 1, 200)
-    corrector = sitk.N4BiasFieldCorrectionImageFilter()
-    numberFittingLevels = levels
-    numberOfIteration = [50]
-    corrector.SetMaximumNumberOfIterations(numberOfIteration * numberFittingLevels)
-    output = corrector.Execute(image, maskImage)
-    img2 = sitk.GetArrayFromImage(output)
-    return img2
-
-
-def biascorrection_file(nifti_file, levels=DEFAULT_BIAS_CORRECTION_LEVELS):
-    inputImage = sitk.ReadImage(nifti_file,sitk.sitkFloat32) 
-    return biascorrection_image(inputImage, levels)
+# -*- coding: utf-8 -*-
+
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+import SimpleITK as sitk
+
+DEFAULT_BIAS_CORRECTION_LEVELS = 8
+
+
+def biascorrection(file_or_image, levels=DEFAULT_BIAS_CORRECTION_LEVELS):
+    if type(file_or_image) == str:
+        return biascorrection_file(file_or_image, levels)
+    else:
+        return biascorrection_image(file_or_image, levels)
+
+
+def biascorrection_image(image, levels=DEFAULT_BIAS_CORRECTION_LEVELS):
+    MAX_GRAY_VALUE = 600
+    if not type(image) == sitk.SimpleITK.Image:
+        # normalize values
+        image = image*MAX_GRAY_VALUE/image.max()
+        image = sitk.GetImageFromArray(image)
+        image = sitk.Cast(image, sitk.sitkFloat32)
+    else:
+        image = sitk.GetArrayFromImage(image)
+        image = image * MAX_GRAY_VALUE / image.max()
+        image = sitk.GetImageFromArray(image)
+        image = sitk.Cast(image, sitk.sitkFloat32)
+
+    maskImage = sitk.OtsuThreshold(image, 0, 1, 200)
+    corrector = sitk.N4BiasFieldCorrectionImageFilter()
+    numberFittingLevels = levels
+    numberOfIteration = [50]
+    corrector.SetMaximumNumberOfIterations(numberOfIteration * numberFittingLevels)
+    output = corrector.Execute(image, maskImage)
+    img2 = sitk.GetArrayFromImage(output)
+    return img2
+
+
+def biascorrection_file(nifti_file, levels=DEFAULT_BIAS_CORRECTION_LEVELS):
+    inputImage = sitk.ReadImage(nifti_file,sitk.sitkFloat32) 
+    return biascorrection_image(inputImage, levels)
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/common/padorcut.py` & `dafne-dl-1.3a4/src/dafne_dl/common/padorcut.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-# -*- coding: utf-8 -*-
-
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-import math
-import numpy as np
-
-# new implementation, working on a generic number of axes
-def padorcut(arrayin, newSize, axis = None):
-    nDims = arrayin.ndim
-    
-    # extend dimensions
-    while nDims < len(newSize):
-        arrayin = np.expand_dims(arrayin, nDims)
-        nDims = arrayin.ndim
-        
-    if type(axis) is int:
-        # check if newsz is iterable, otherwise assume it's a number
-        try:
-            newSz = newSize[axis]
-        except:
-            newSz = int(newSize)
-        oldSz = arrayin.shape[axis]
-        if oldSz < newSz:
-            padBefore = int(math.floor(float(newSz - oldSz)/2))
-            padAfter = int(math.ceil(float(newSz - oldSz)/2))
-            padding = []
-            for i in range(nDims):
-                if i == axis:
-                    padding.append( (padBefore, padAfter) )
-                else:
-                    padding.append( (0,0) )
-            return np.pad(arrayin, padding, 'constant')
-        elif oldSz > newSz:
-            cutBefore = int(math.floor(float(oldSz - newSz)/2))
-            cutAfter = int(math.ceil(float(oldSz - newSz)/2))
-            slc = [slice(None)]*nDims
-            slc[axis] = slice(cutBefore, -cutAfter)
-            return arrayin[tuple(slc)]
-        else:
-            return arrayin
-    else:
-        for ax in range(nDims):
-            arrayin = padorcut(arrayin, newSize, ax)
-        return arrayin
-
-def translate(arrayin, translation):
-    padBeforeX = translation[0] if translation[0] > 0 else 0
-    padAfterX = -translation[0] if translation[0] < 0 else 0
-    padBeforeY = translation[1] if translation[1] > 0 else 0
-    padAfterY = -translation[1] if translation[1] < 0 else 0
-    
-    cutBeforeX = padAfterX
-    cutAfterX = padBeforeX
-    cutBeforeY = padAfterY
-    cutAfterY = padBeforeY
-    
-    nx, ny = arrayin.shape    
-    
-    cutArray = arrayin[cutBeforeX:(nx-cutAfterX), cutBeforeY:(ny-cutAfterY)]
-    arrayout = arrayout=np.pad(cutArray, ( (padBeforeX,padAfterX), (padBeforeY, padAfterY) ), 'constant')
-    return arrayout
-    
+# -*- coding: utf-8 -*-
+
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+import math
+import numpy as np
+
+# new implementation, working on a generic number of axes
+def padorcut(arrayin, newSize, axis = None):
+    nDims = arrayin.ndim
+    
+    # extend dimensions
+    while nDims < len(newSize):
+        arrayin = np.expand_dims(arrayin, nDims)
+        nDims = arrayin.ndim
+        
+    if type(axis) is int:
+        # check if newsz is iterable, otherwise assume it's a number
+        try:
+            newSz = newSize[axis]
+        except:
+            newSz = int(newSize)
+        oldSz = arrayin.shape[axis]
+        if oldSz < newSz:
+            padBefore = int(math.floor(float(newSz - oldSz)/2))
+            padAfter = int(math.ceil(float(newSz - oldSz)/2))
+            padding = []
+            for i in range(nDims):
+                if i == axis:
+                    padding.append( (padBefore, padAfter) )
+                else:
+                    padding.append( (0,0) )
+            return np.pad(arrayin, padding, 'constant')
+        elif oldSz > newSz:
+            cutBefore = int(math.floor(float(oldSz - newSz)/2))
+            cutAfter = int(math.ceil(float(oldSz - newSz)/2))
+            slc = [slice(None)]*nDims
+            slc[axis] = slice(cutBefore, -cutAfter)
+            return arrayin[tuple(slc)]
+        else:
+            return arrayin
+    else:
+        for ax in range(nDims):
+            arrayin = padorcut(arrayin, newSize, ax)
+        return arrayin
+
+def translate(arrayin, translation):
+    padBeforeX = translation[0] if translation[0] > 0 else 0
+    padAfterX = -translation[0] if translation[0] < 0 else 0
+    padBeforeY = translation[1] if translation[1] > 0 else 0
+    padAfterY = -translation[1] if translation[1] < 0 else 0
+    
+    cutBeforeX = padAfterX
+    cutAfterX = padBeforeX
+    cutBeforeY = padAfterY
+    cutAfterY = padBeforeY
+    
+    nx, ny = arrayin.shape    
+    
+    cutArray = arrayin[cutBeforeX:(nx-cutAfterX), cutBeforeY:(ny-cutAfterY)]
+    arrayout = arrayout=np.pad(cutArray, ( (padBeforeX,padAfterX), (padBeforeY, padAfterY) ), 'constant')
+    return arrayout
+
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/interfaces.py` & `dafne-dl-1.3a4/src/dafne_dl/interfaces.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-from __future__ import annotations
-from abc import ABC, abstractmethod
-from io import BytesIO
-from typing import IO, Callable, List, Union, Optional, Dict
-import numpy as np
-import time
-
-
-class IncompatibleModelError(Exception):
-    pass
-
-class DeepLearningClass(ABC):   
-    
-    @abstractmethod
-    def init_model(self):
-        """
-        Initializes the model when needed
-
-        Returns
-        -------
-        None.
-
-        """
-        pass
-    
-    @abstractmethod
-    def calc_delta(self, baseModel: DeepLearningClass) -> DeepLearningClass:
-        """
-        Calculate a delta with another model, Returns a new instance
-
-        Parameters
-        ----------
-        baseModel : DeepLearningClass
-            Base model to calculate the delta from
-
-        Returns
-        -------
-        DeepLearningClass
-            A deep learning class representing the delta of the two models
-
-        """
-        pass
-    
-    def __sub__(self, rhs):
-        return self.calc_delta(rhs)
-    
-    @abstractmethod
-    def apply_delta(self, delta_model: DeepLearningClass) -> DeepLearningClass:
-        """
-        Applies a delta to this class and returns a new model with the delta applied
-        
-
-        Parameters
-        ----------
-        delta_model : DeepLearningClass
-            Applies a delta to the current model
-
-        Returns
-        -------
-        DeepLearningClass
-            The model that is the current model plus the delta
-
-        """
-        pass
-
-    def sum(self, other):
-        """
-        Note: this defaults to apply_delta. Redefine to change behavior
-        """
-        return self.apply_delta(other)
-
-    def __add__(self, rhs):
-        return self.sum(rhs)
-    
-    @abstractmethod
-    def incremental_learn(self, training_data: dict, training_outputs: str):
-        """
-        Perform an incremental learning step on the given training data/outputs
-
-        Parameters
-        ----------
-        training_data : Dictionary
-            Contains the path to the training data and resolution.
-        training_outputs : String
-            Contains the path to the training labels.
-
-        Returns
-        -------
-        None.
-
-        """
-        pass
-    
-    @abstractmethod
-    def apply(self, data: dict):
-        """
-        Applies the deep learning model to the image
-
-        Parameters
-        ----------
-        data : Dictionary
-            Contains the data and the extra information (for example image and resolution)
-
-        Returns
-        -------
-        Depends on the operation performed:
-            For classifiers: str - Containing the label of the image
-            For segmenters: dict[str, mask] - Containing the labels and the corresponding 2D masks
-
-        """
-        pass
-
-    @abstractmethod
-    def factor_multiply(self, factor: float):
-        """
-        Multiplies all the weights by a float factor
-        
-        """
-        pass
-
-    def __mul__(self, factor: float):
-        if not isinstance(factor, (int, float)):
-            raise NotImplementedError('Incompatible types for multiplication (only multiplication by numeric factor is allowed)')
-        return self.factor_multiply(factor)
-
-    def __rmul__(self, factor: float):
-        if not isinstance(factor, (int, float)):
-            raise NotImplementedError('Incompatible types for multiplication (only multiplication by numeric factor is allowed)')
-        return self.factor_multiply(factor)
-
-    def __call__(self, data: dict):
-        return self.apply(data)
-
-    def reset_timestamp(self):
-        self.timestamp_id = int(time.time())
-
-class ModelProvider(ABC):
-    """
-        Abstract class that is the base for loading (and, in the future, storing?) models.
-        Has to be subclassed to support local and remote loading.
-    """
-    
-    @abstractmethod
-    def load_model(self, model_name: str, progress_callback: Optional[Callable[[int, int], None]] = None,
-                   force_download: bool = False,
-                   timestamp: Optional[Union[int,str]] = None) -> DeepLearningClass:
-        """
-        Loads a deep learning model.
-
-        Parameters
-        ----------
-        model_name : str
-            The name of the model to load.
-        progress_callback: Callable[[int, int], None] (optional)
-            Callback function for progress
-        force_download: bool
-            Sets the forced redownload of models
-        timestamp: int or None
-            Return a specific model version (default: latest)
-
-        Returns
-        -------
-        The model object.
-
-        """
-        pass
-
-    @abstractmethod
-    def model_details(self, model_name: str) -> dict:
-        pass
-
-    @abstractmethod
-    def available_models(self) -> Optional[list[str]]:
-        """
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        List of available models
-        """
-        pass
-
-    @abstractmethod
-    def upload_model(self, model_name: str, model: DeepLearningClass, dice_score: float=0.0) -> None:
-        """
-        Parameters
-        ----------
-        model_name : str
-            The name of the model to upload.
-        model:
-            The model to be uploaded
-        dice_score:
-            The average dice score of the client
-        """
-        pass
-
-    def upload_data(self, data: dict) -> None:
-        """
-        Uploads data to the server. Converts the data into a stream before calling _upload_bytes
-
-        Parameters
-        ----------
-        data: dict
-            Dictionary of objects that can be saved by Numpy and loaded without using pickle (which is unsafe)
-        """
-        bytes_io = BytesIO()
-        np.savez_compressed(bytes_io, **data)
-        self._upload_bytes(bytes_io)
-        bytes_io.close()
-
-
-    @abstractmethod
-    def _upload_bytes(self, data: IO):
-        """
-        Uploads generic data to the server. This is an internal function that implements the server communication.
-        The actual function to be called by the client is upload_data with a dict
-
-        Parameters
-        ----------
-        data: IO
-            byte stream that is sent to the server.
-        """
-        pass
-
-    @abstractmethod
-    def log(self, msg: str):
-        """
-        Sends a message to the server to be logged
-
-        Parameters
-        ----------
-        msg: str
-            the message.
-        """
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from __future__ import annotations
+from abc import ABC, abstractmethod
+from io import BytesIO
+from typing import IO, Callable, List, Union, Optional, Dict
+import numpy as np
+import time
+
+
+class IncompatibleModelError(Exception):
+    pass
+
+class DeepLearningClass(ABC):   
+    
+    @abstractmethod
+    def init_model(self):
+        """
+        Initializes the model when needed
+
+        Returns
+        -------
+        None.
+
+        """
+        pass
+    
+    @abstractmethod
+    def calc_delta(self, baseModel: DeepLearningClass) -> DeepLearningClass:
+        """
+        Calculate a delta with another model, Returns a new instance
+
+        Parameters
+        ----------
+        baseModel : DeepLearningClass
+            Base model to calculate the delta from
+
+        Returns
+        -------
+        DeepLearningClass
+            A deep learning class representing the delta of the two models
+
+        """
+        pass
+    
+    def __sub__(self, rhs):
+        return self.calc_delta(rhs)
+    
+    @abstractmethod
+    def apply_delta(self, delta_model: DeepLearningClass) -> DeepLearningClass:
+        """
+        Applies a delta to this class and returns a new model with the delta applied
+        
+
+        Parameters
+        ----------
+        delta_model : DeepLearningClass
+            Applies a delta to the current model
+
+        Returns
+        -------
+        DeepLearningClass
+            The model that is the current model plus the delta
+
+        """
+        pass
+
+    def sum(self, other):
+        """
+        Note: this defaults to apply_delta. Redefine to change behavior
+        """
+        return self.apply_delta(other)
+
+    def __add__(self, rhs):
+        return self.sum(rhs)
+    
+    @abstractmethod
+    def incremental_learn(self, training_data: dict, training_outputs: str):
+        """
+        Perform an incremental learning step on the given training data/outputs
+
+        Parameters
+        ----------
+        training_data : Dictionary
+            Contains the path to the training data and resolution.
+        training_outputs : String
+            Contains the path to the training labels.
+
+        Returns
+        -------
+        None.
+
+        """
+        pass
+    
+    @abstractmethod
+    def apply(self, data: dict):
+        """
+        Applies the deep learning model to the image
+
+        Parameters
+        ----------
+        data : Dictionary
+            Contains the data and the extra information (for example image and resolution)
+
+        Returns
+        -------
+        Depends on the operation performed:
+            For classifiers: str - Containing the label of the image
+            For segmenters: dict[str, mask] - Containing the labels and the corresponding 2D masks
+
+        """
+        pass
+
+    @abstractmethod
+    def factor_multiply(self, factor: float):
+        """
+        Multiplies all the weights by a float factor
+        
+        """
+        pass
+
+    def __mul__(self, factor: float):
+        if not isinstance(factor, (int, float)):
+            raise NotImplementedError('Incompatible types for multiplication (only multiplication by numeric factor is allowed)')
+        return self.factor_multiply(factor)
+
+    def __rmul__(self, factor: float):
+        if not isinstance(factor, (int, float)):
+            raise NotImplementedError('Incompatible types for multiplication (only multiplication by numeric factor is allowed)')
+        return self.factor_multiply(factor)
+
+    def __call__(self, data: dict):
+        return self.apply(data)
+
+    def reset_timestamp(self):
+        self.timestamp_id = int(time.time())
+
+class ModelProvider(ABC):
+    """
+        Abstract class that is the base for loading (and, in the future, storing?) models.
+        Has to be subclassed to support local and remote loading.
+    """
+    
+    @abstractmethod
+    def load_model(self, model_name: str, progress_callback: Optional[Callable[[int, int], None]] = None,
+                   force_download: bool = False,
+                   timestamp: Optional[Union[int,str]] = None) -> DeepLearningClass:
+        """
+        Loads a deep learning model.
+
+        Parameters
+        ----------
+        model_name : str
+            The name of the model to load.
+        progress_callback: Callable[[int, int], None] (optional)
+            Callback function for progress
+        force_download: bool
+            Sets the forced redownload of models
+        timestamp: int or None
+            Return a specific model version (default: latest)
+
+        Returns
+        -------
+        The model object.
+
+        """
+        pass
+
+    @abstractmethod
+    def model_details(self, model_name: str) -> dict:
+        pass
+
+    @abstractmethod
+    def available_models(self) -> Optional[list[str]]:
+        """
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        List of available models
+        """
+        pass
+
+    @abstractmethod
+    def upload_model(self, model_name: str, model: DeepLearningClass, dice_score: float=0.0) -> None:
+        """
+        Parameters
+        ----------
+        model_name : str
+            The name of the model to upload.
+        model:
+            The model to be uploaded
+        dice_score:
+            The average dice score of the client
+        """
+        pass
+
+    def upload_data(self, data: dict) -> None:
+        """
+        Uploads data to the server. Converts the data into a stream before calling _upload_bytes
+
+        Parameters
+        ----------
+        data: dict
+            Dictionary of objects that can be saved by Numpy and loaded without using pickle (which is unsafe)
+        """
+        bytes_io = BytesIO()
+        np.savez_compressed(bytes_io, **data)
+        self._upload_bytes(bytes_io)
+        bytes_io.close()
+
+
+    @abstractmethod
+    def _upload_bytes(self, data: IO):
+        """
+        Uploads generic data to the server. This is an internal function that implements the server communication.
+        The actual function to be called by the client is upload_data with a dict
+
+        Parameters
+        ----------
+        data: IO
+            byte stream that is sent to the server.
+        """
+        pass
+
+    @abstractmethod
+    def log(self, msg: str):
+        """
+        Sends a message to the server to be logged
+
+        Parameters
+        ----------
+        msg: str
+            the message.
+        """
         pass
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/labels/__init__.py` & `dafne-dl-1.3a4/src/dafne_dl/common/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/labels/leg.py` & `dafne-dl-1.3a4/src/dafne_dl/labels/leg.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-from .utils import invert_dict, merge_dict
-
-short_labels = {
-    1: 'SOL',
-    2: 'GM',
-    3: 'GL',
-    4: 'TA',
-    5: 'ELD',
-    6: 'PE',
-}
-
-long_labels = {
-    1: 'Soleus',
-    2: 'Gastrocnemius Medialis',
-    3: 'Gastrocnemius Lateralis',
-    4: 'Tibialis Anterior',
-    5: 'Extensor Longus Digitorum',
-    6: 'Peroneus'
-}
-
-long_labels_split = {}
-ctr = 1
-for key, val in long_labels.items():
-    long_labels_split[ctr] = val + "_R"
-    long_labels_split[ctr+1] = val + "_L"
-    ctr += 2
-
-inverse_labels = merge_dict(invert_dict(short_labels), invert_dict(long_labels))
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from .utils import invert_dict, merge_dict
+
+short_labels = {
+    1: 'SOL',
+    2: 'GM',
+    3: 'GL',
+    4: 'TA',
+    5: 'ELD',
+    6: 'PE',
+}
+
+long_labels = {
+    1: 'Soleus',
+    2: 'Gastrocnemius Medialis',
+    3: 'Gastrocnemius Lateralis',
+    4: 'Tibialis Anterior',
+    5: 'Extensor Longus Digitorum',
+    6: 'Peroneus'
+}
+
+long_labels_split = {}
+ctr = 1
+for key, val in long_labels.items():
+    long_labels_split[ctr] = val + "_R"
+    long_labels_split[ctr+1] = val + "_L"
+    ctr += 2
+
+inverse_labels = merge_dict(invert_dict(short_labels), invert_dict(long_labels))
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/labels/thigh.py` & `dafne-dl-1.3a4/src/dafne_dl/labels/thigh.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-from .utils import invert_dict, merge_dict
-
-short_labels = {
-    1: 'VL',
-    2: 'VM',
-    3: 'VI',
-    4: 'RF',
-    5: 'SAR',
-    6: 'GRA',
-    7: 'AM',
-    8: 'SM',
-    9: 'ST',
-    10: 'BFL',
-    11: 'BFS',
-    12: 'AL'
-}
-
-long_labels = {
-    1: 'Vastus Lateralis',
-    2: 'Vastus Medialis',
-    3: 'Vastus Intermedius',
-    4: 'Rectus Femoris',
-    5: 'Sartorius',
-    6: 'Gracilis',
-    7: 'Adductor Magnus',
-    8: 'Semimembranosus',
-    9: 'Semitendinosus',
-    10: 'Biceps Femoris Long',
-    11: 'Biceps Femoris Short',
-    12: 'Adductor Longus'
-}
-
-long_labels_split = {}
-ctr = 1
-for key, val in long_labels.items():
-    long_labels_split[ctr] = val + "_R"
-    long_labels_split[ctr+1] = val + "_L"
-    ctr += 2
-
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from .utils import invert_dict, merge_dict
+
+short_labels = {
+    1: 'VL',
+    2: 'VM',
+    3: 'VI',
+    4: 'RF',
+    5: 'SAR',
+    6: 'GRA',
+    7: 'AM',
+    8: 'SM',
+    9: 'ST',
+    10: 'BFL',
+    11: 'BFS',
+    12: 'AL'
+}
+
+long_labels = {
+    1: 'Vastus Lateralis',
+    2: 'Vastus Medialis',
+    3: 'Vastus Intermedius',
+    4: 'Rectus Femoris',
+    5: 'Sartorius',
+    6: 'Gracilis',
+    7: 'Adductor Magnus',
+    8: 'Semimembranosus',
+    9: 'Semitendinosus',
+    10: 'Biceps Femoris Long',
+    11: 'Biceps Femoris Short',
+    12: 'Adductor Longus'
+}
+
+long_labels_split = {}
+ctr = 1
+for key, val in long_labels.items():
+    long_labels_split[ctr] = val + "_R"
+    long_labels_split[ctr+1] = val + "_L"
+    ctr += 2
+
 inverse_labels = merge_dict(invert_dict(short_labels), invert_dict(long_labels))
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl/misc.py` & `dafne-dl-1.3a4/src/dafne_dl/misc.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-#  Copyright (c) 2021 Dafne-Imaging Team
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-import hashlib
-import os
-
-import numpy as np
-
-
-def calculate_file_hash(file_path, cache_results=False, force_rewrite_cache=False):
-    if not cache_results:
-        return hashlib.sha256(open(file_path, 'rb').read()).hexdigest()
-    
-    # check if the hash exists on disk
-    hash_file = file_path + '.sha256'
-    if not force_rewrite_cache:
-        try:
-            with open(hash_file, 'r') as f:
-                output_hash = f.readline().strip()
-        except OSError:
-            print('Error while reading from hash file')
-        else:
-            if len(output_hash) == 64:
-                #print('Using cached hash')
-                return output_hash
-            else:
-                print('Invalid stored hash')
-
-    # file does not exist, or stored hash is invalid
-    output_hash = calculate_file_hash(file_path, False)  # fallback to calculating hash
-    try:
-        with open(hash_file, 'w') as f:
-            f.write(output_hash)
-    except OSError:
-        print('Error writing hash to file')
-    return output_hash
-
-
-def calc_dice_score(y_true, y_pred):
-    """
-    Binary f1. Same results as sklearn f1 binary.
-
-    y_true: 1D / 2D / 3D array
-    y_pred: 1D / 2D / 3D array
-    """
-    intersect = np.sum(y_true * y_pred)  # works because all multiplied by 0 gets 0
-    denominator = np.sum(y_true) + np.sum(y_pred)  # works because all multiplied by 0 gets 0
-    return (2 * intersect) / (denominator + 1e-6)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+#  Copyright (c) 2021 Dafne-Imaging Team
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+import hashlib
+import os
+
+import numpy as np
+
+
+def calculate_file_hash(file_path, cache_results=False, force_rewrite_cache=False):
+    if not cache_results:
+        return hashlib.sha256(open(file_path, 'rb').read()).hexdigest()
+    
+    # check if the hash exists on disk
+    hash_file = file_path + '.sha256'
+    if not force_rewrite_cache:
+        try:
+            with open(hash_file, 'r') as f:
+                output_hash = f.readline().strip()
+        except OSError:
+            print('Error while reading from hash file')
+        else:
+            if len(output_hash) == 64:
+                #print('Using cached hash')
+                return output_hash
+            else:
+                print('Invalid stored hash')
+
+    # file does not exist, or stored hash is invalid
+    output_hash = calculate_file_hash(file_path, False)  # fallback to calculating hash
+    try:
+        with open(hash_file, 'w') as f:
+            f.write(output_hash)
+    except OSError:
+        print('Error writing hash to file')
+    return output_hash
+
+
+def calc_dice_score(y_true, y_pred):
+    """
+    Binary f1. Same results as sklearn f1 binary.
+
+    y_true: 1D / 2D / 3D array
+    y_pred: 1D / 2D / 3D array
+    """
+    intersect = np.sum(y_true * y_pred)  # works because all multiplied by 0 gets 0
+    denominator = np.sum(y_true) + np.sum(y_pred)  # works because all multiplied by 0 gets 0
+    return (2 * intersect) / (denominator + 1e-6)
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl.egg-info/PKG-INFO` & `dafne-dl-1.3a4/src/dafne_dl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: dafne-dl
-Version: 1.3a3
-Summary: Deep Learning module for Dafne
-Home-page: https://github.com/dafne-imaging/dafne-dl
-Author: Francesco Santini
-Author-email: francesco.santini@unibas.ch
-Project-URL: Bug Tracker, https://github.com/dafne-imaging/dafne-dl/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: COPYING
-License-File: COPYING.LESSER
-
-Sets of classes and interfaces for the definition of deep learning models.
-The framework is conceived to be extensible and serializable, in order to provide models that can be stored and/or sent through the network.
-## Interfaces.py
-Set of abstract classes that describe models and model providers. 
-### DeepLearningClass
-The rationale behind this is that an algorithm not only depends on the model, but might require some preprocessing steps (reformatting, normalization) before the application of the model itself. The interface is also "incremental-learning-oriented" as it provides abstract methods for the calculation and integration of deltas. The class provides operator override for the calculation of deltas (D = A-B) and call override for the apply method.
-An instance of DeepLearningClass should be able to simply provide the expected result when called with the appropriate input data (in form of dict). The most common data for our case will be:
-
- - Input: `{'image': 2D image, 'resolution': Sequence with pixel sizes}`
- - Output: for Classifiers: `str`, for Segmenters: `dict[str: image]` where str is the label and the image is a 2D numpy array containing the mask corresponding to the string.
-
-### ModelProvider
-This is an abstract class that is intended to encapsulate the logic of model load/transfer. It will have two subclasses, LocalModelProvider and RemoteModelProvider. In both cases, the method load_model of this class accepts a description of the requested model and will return an instance of DeepLearningClass. In principle, LocalModelProvider will be used on the server, and RemoteModelProvider on the client.
-
-## DynamicDLModel
-Concrete implementation of a DeepLearningClass which provides flexibility and serialization. This class delegates the important methods of the model implementation to top-level functions that are passed at the construction time. These functions can be easily serialized with the dill library.
-Constructor:
-
-        def __init__(self, model_id, # a unique ID to avoid mixing different models
-                 init_model_function, # inits the model. Accepts no parameters and returns the model
-                 apply_model_function, # function that applies the model. Has the object, and image, and a sequence containing resolutions as parameters
-                 weights_to_model_function = default_keras_weights_to_model_function, # put model weights inside the model.
-                 model_to_weights_function = default_keras_model_to_weights_function, # get the weights from the model in a pickable format
-                 calc_delta_function = default_keras_delta_function, # calculate the weight delta
-                 apply_delta_function = default_keras_apply_delta_function, # apply a weight delta
-                 incremental_learn_function = None, # function to perform an incremental learning step
-                 weights = None): # initial weights
-This allows the implementation of a very generic deep learning algorithm which includes the preprocessing steps in a way that can be serialized and defined at runtime, so if we want to change the model, we don't need to change the code of the client or server, as the implementation is self-contained within the model.
-The class provides the methods `dump(file_descriptor)` and `str = dumps()` to serialize and the static methods `Load(file_descriptor)` and `Loads(str)` to deserialize.
-Default functions for loading/setting keras weights and calculating deltas from keras models (which provide a get_weights(), set_weights() interface with lists of numpy arrays) are currently provided.
-**Important note when defining the functions**: in order for them to be serializable, they must be completely self-contained. That is, all imports should happen inside the functions and all the external function call should be implemented as nested functions. Common algorithms (such as padorcut.py which pads or cuts an image to fit it to a specific matrix size) should be placed in the repository.
+Metadata-Version: 2.1
+Name: dafne-dl
+Version: 1.3a4
+Summary: Deep Learning module for Dafne
+Home-page: https://github.com/dafne-imaging/dafne-dl
+Author: Francesco Santini
+Author-email: francesco.santini@unibas.ch
+Project-URL: Bug Tracker, https://github.com/dafne-imaging/dafne-dl/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: COPYING.LESSER
+
+Sets of classes and interfaces for the definition of deep learning models.
+The framework is conceived to be extensible and serializable, in order to provide models that can be stored and/or sent through the network.
+## Interfaces.py
+Set of abstract classes that describe models and model providers. 
+### DeepLearningClass
+The rationale behind this is that an algorithm not only depends on the model, but might require some preprocessing steps (reformatting, normalization) before the application of the model itself. The interface is also "incremental-learning-oriented" as it provides abstract methods for the calculation and integration of deltas. The class provides operator override for the calculation of deltas (D = A-B) and call override for the apply method.
+An instance of DeepLearningClass should be able to simply provide the expected result when called with the appropriate input data (in form of dict). The most common data for our case will be:
+
+ - Input: `{'image': 2D image, 'resolution': Sequence with pixel sizes}`
+ - Output: for Classifiers: `str`, for Segmenters: `dict[str: image]` where str is the label and the image is a 2D numpy array containing the mask corresponding to the string.
+
+### ModelProvider
+This is an abstract class that is intended to encapsulate the logic of model load/transfer. It will have two subclasses, LocalModelProvider and RemoteModelProvider. In both cases, the method load_model of this class accepts a description of the requested model and will return an instance of DeepLearningClass. In principle, LocalModelProvider will be used on the server, and RemoteModelProvider on the client.
+
+## DynamicDLModel
+Concrete implementation of a DeepLearningClass which provides flexibility and serialization. This class delegates the important methods of the model implementation to top-level functions that are passed at the construction time. These functions can be easily serialized with the dill library.
+Constructor:
+
+        def __init__(self, model_id, # a unique ID to avoid mixing different models
+                 init_model_function, # inits the model. Accepts no parameters and returns the model
+                 apply_model_function, # function that applies the model. Has the object, and image, and a sequence containing resolutions as parameters
+                 weights_to_model_function = default_keras_weights_to_model_function, # put model weights inside the model.
+                 model_to_weights_function = default_keras_model_to_weights_function, # get the weights from the model in a pickable format
+                 calc_delta_function = default_keras_delta_function, # calculate the weight delta
+                 apply_delta_function = default_keras_apply_delta_function, # apply a weight delta
+                 incremental_learn_function = None, # function to perform an incremental learning step
+                 weights = None): # initial weights
+This allows the implementation of a very generic deep learning algorithm which includes the preprocessing steps in a way that can be serialized and defined at runtime, so if we want to change the model, we don't need to change the code of the client or server, as the implementation is self-contained within the model.
+The class provides the methods `dump(file_descriptor)` and `str = dumps()` to serialize and the static methods `Load(file_descriptor)` and `Loads(str)` to deserialize.
+Default functions for loading/setting keras weights and calculating deltas from keras models (which provide a get_weights(), set_weights() interface with lists of numpy arrays) are currently provided.
+**Important note when defining the functions**: in order for them to be serializable, they must be completely self-contained. That is, all imports should happen inside the functions and all the external function call should be implemented as nested functions. Common algorithms (such as padorcut.py which pads or cuts an image to fit it to a specific matrix size) should be placed in the repository.
```

### Comparing `dafne-dl-1.3a3/src/dafne_dl.egg-info/SOURCES.txt` & `dafne-dl-1.3a4/src/dafne_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

