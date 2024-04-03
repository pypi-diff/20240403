# Comparing `tmp/psy-view-0.2.0.tar.gz` & `tmp/psy-view-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psy-view-0.2.0.tar", last modified: Sat Oct  9 05:32:15 2021, max compression
+gzip compressed data, was "psy-view-0.3.0.tar", last modified: Wed Apr  3 18:22:57 2024, max compression
```

## Comparing `psy-view-0.2.0.tar` & `psy-view-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 05:32:15.172681 psy-view-0.2.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2021-10-09 05:30:42.000000 psy-view-0.2.0/COPYING
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7652 2021-10-09 05:30:42.000000 psy-view-0.2.0/COPYING.LESSER
--rw-r--r--   0 circleci  (3434) circleci  (3434)      115 2021-10-09 05:30:42.000000 psy-view-0.2.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8530 2021-10-09 05:32:15.172681 psy-view-0.2.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7211 2021-10-09 05:30:42.000000 psy-view-0.2.0/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 05:32:15.180681 psy-view-0.2.0/psy_view/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5177 2021-10-09 05:30:42.000000 psy-view-0.2.0/psy_view/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1663 2021-10-09 05:30:42.000000 psy-view-0.2.0/psy_view/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      497 2021-10-09 05:32:15.180681 psy-view-0.2.0/psy_view/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    38690 2021-10-09 05:30:42.000000 psy-view-0.2.0/psy_view/dialogs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    63480 2021-10-09 05:30:42.000000 psy-view-0.2.0/psy_view/ds_widget.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 05:32:15.172681 psy-view-0.2.0/psy_view/icons/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21233 2021-10-09 05:30:42.000000 psy-view-0.2.0/psy_view/icons/color_settings.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20549 2021-10-09 05:30:42.000000 psy-view-0.2.0/psy_view/icons/proj_settings.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    47334 2021-10-09 05:30:42.000000 psy-view-0.2.0/psy_view/plotmethods.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2721 2021-10-09 05:30:42.000000 psy-view-0.2.0/psy_view/rcsetup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2706 2021-10-09 05:30:42.000000 psy-view-0.2.0/psy_view/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 05:32:15.172681 psy-view-0.2.0/psy_view.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8530 2021-10-09 05:32:14.000000 psy-view-0.2.0/psy_view.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2021-10-09 05:32:14.000000 psy-view-0.2.0/psy_view.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-10-09 05:32:14.000000 psy-view-0.2.0/psy_view.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      109 2021-10-09 05:32:14.000000 psy-view-0.2.0/psy_view.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-10-09 05:32:14.000000 psy-view-0.2.0/psy_view.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       79 2021-10-09 05:32:14.000000 psy-view-0.2.0/psy_view.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2021-10-09 05:32:14.000000 psy-view-0.2.0/psy_view.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      204 2021-10-09 05:32:15.180681 psy-view-0.2.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4217 2021-10-09 05:30:42.000000 psy-view-0.2.0/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    69678 2021-10-09 05:30:42.000000 psy-view-0.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:22:57.277659 psy-view-0.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:22:57.269659 psy-view-0.3.0/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    17023 2024-04-03 18:22:24.000000 psy-view-0.3.0/LICENSES/CC-BY-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-03 18:22:24.000000 psy-view-0.3.0/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    42098 2024-04-03 18:22:24.000000 psy-view-0.3.0/LICENSES/LGPL-3.0-only.txt
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-04-03 18:22:24.000000 psy-view-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2730 2024-04-03 18:22:57.273659 psy-view-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6067 2024-04-03 18:22:24.000000 psy-view-0.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:22:57.269659 psy-view-0.3.0/psy_view/
+-rw-rw-rw-   0 root         (0) root         (0)     4430 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-03 18:22:57.277659 psy-view-0.3.0/psy_view/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    40699 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/dialogs.py
+-rw-rw-rw-   0 root         (0) root         (0)    64320 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/ds_widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:22:57.273659 psy-view-0.3.0/psy_view/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     2198 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/icons/color_settings.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/icons/color_settings.png.license
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/icons/proj_settings.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/icons/proj_settings.png.license
+-rw-rw-rw-   0 root         (0) root         (0)    50193 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/plotmethods.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/rcsetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1995 2024-04-03 18:22:24.000000 psy-view-0.3.0/psy_view/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:22:57.273659 psy-view-0.3.0/psy_view.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2730 2024-04-03 18:22:57.000000 psy-view-0.3.0/psy_view.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      723 2024-04-03 18:22:57.000000 psy-view-0.3.0/psy_view.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 18:22:57.000000 psy-view-0.3.0/psy_view.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-03 18:22:57.000000 psy-view-0.3.0/psy_view.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 18:22:56.000000 psy-view-0.3.0/psy_view.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      356 2024-04-03 18:22:57.000000 psy-view-0.3.0/psy_view.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-03 18:22:57.000000 psy-view-0.3.0/psy_view.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3261 2024-04-03 18:22:24.000000 psy-view-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 18:22:57.277659 psy-view-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      284 2024-04-03 18:22:24.000000 psy-view-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:22:57.273659 psy-view-0.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4111 2024-04-03 18:22:24.000000 psy-view-0.3.0/tests/test_dialogs.py
+-rw-rw-rw-   0 root         (0) root         (0)    17913 2024-04-03 18:22:24.000000 psy-view-0.3.0/tests/test_ds_widget.py
```

### Comparing `psy-view-0.2.0/COPYING` & `psy-view-0.3.0/LICENSES/LGPL-3.0-only.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,674 +1,304 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+GNU LESSER GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007
 
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
+Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+
+This version of the GNU Lesser General Public License incorporates the terms and conditions of version 3 of the GNU General Public License, supplemented by the additional permissions listed below.
+
+0. Additional Definitions.
+
+As used herein, "this License" refers to version 3 of the GNU Lesser General Public License, and the "GNU GPL" refers to version 3 of the GNU General Public License.
+
+"The Library" refers to a covered work governed by this License, other than an Application or a Combined Work as defined below.
+
+An "Application" is any work that makes use of an interface provided by the Library, but which is not otherwise based on the Library. Defining a subclass of a class defined by the Library is deemed a mode of using an interface provided by the Library.
+
+A "Combined Work" is a work produced by combining or linking an Application with the Library.  The particular version of the Library with which the Combined Work was made is also called the "Linked Version".
+
+The "Minimal Corresponding Source" for a Combined Work means the Corresponding Source for the Combined Work, excluding any source code for portions of the Combined Work that, considered in isolation, are based on the Application, and not on the Linked Version.
+
+The "Corresponding Application Code" for a Combined Work means the object code and/or source code for the Application, including any data and utility programs needed for reproducing the Combined Work from the Application, but excluding the System Libraries of the Combined Work.
+
+1. Exception to Section 3 of the GNU GPL.
+You may convey a covered work under sections 3 and 4 of this License without being bound by section 3 of the GNU GPL.
+
+2. Conveying Modified Versions.
+If you modify a copy of the Library, and, in your modifications, a facility refers to a function or data to be supplied by an Application that uses the facility (other than as an argument passed when the facility is invoked), then you may convey a copy of the modified version:
+
+     a) under this License, provided that you make a good faith effort to ensure that, in the event an Application does not supply the function or data, the facility still operates, and performs whatever part of its purpose remains meaningful, or
+
+     b) under the GNU GPL, with none of the additional permissions of this License applicable to that copy.
+
+3. Object Code Incorporating Material from Library Header Files.
+The object code form of an Application may incorporate material from a header file that is part of the Library.  You may convey such object code under terms of your choice, provided that, if the incorporated material is not limited to numerical parameters, data structure layouts and accessors, or small macros, inline functions and templates (ten or fewer lines in length), you do both of the following:
+
+     a) Give prominent notice with each copy of the object code that the Library is used in it and that the Library and its use are covered by this License.
+
+     b) Accompany the object code with a copy of the GNU GPL and this license document.
+
+4. Combined Works.
+You may convey a Combined Work under terms of your choice that, taken together, effectively do not restrict modification of the portions of the Library contained in the Combined Work and reverse engineering for debugging such modifications, if you also do each of the following:
+
+     a) Give prominent notice with each copy of the Combined Work that the Library is used in it and that the Library and its use are covered by this License.
+
+     b) Accompany the Combined Work with a copy of the GNU GPL and this license document.
+
+     c) For a Combined Work that displays copyright notices during execution, include the copyright notice for the Library among these notices, as well as a reference directing the user to the copies of the GNU GPL and this license document.
+
+     d) Do one of the following:
+
+           0) Convey the Minimal Corresponding Source under the terms of this License, and the Corresponding Application Code in a form suitable for, and under terms that permit, the user to recombine or relink the Application with a modified version of the Linked Version to produce a modified Combined Work, in the manner specified by section 6 of the GNU GPL for conveying Corresponding Source.
+
+          1) Use a suitable shared library mechanism for linking with the Library.  A suitable mechanism is one that (a) uses at run time a copy of the Library already present on the user's computer system, and (b) will operate properly with a modified version of the Library that is interface-compatible with the Linked Version.
+
+     e) Provide Installation Information, but only if you would otherwise be required to provide such information under section 6 of the GNU GPL, and only to the extent that such information is necessary to install and execute a modified version of the Combined Work produced by recombining or relinking the Application with a modified version of the Linked Version. (If you use option 4d0, the Installation Information must accompany the Minimal Corresponding Source and Corresponding Application Code. If you use option 4d1, you must provide the Installation Information in the manner specified by section 6 of the GNU GPL for conveying Corresponding Source.)
+
+5. Combined Libraries.
+You may place library facilities that are a work based on the Library side by side in a single library together with other library facilities that are not Applications and are not covered by this License, and convey such a combined library under terms of your choice, if you do both of the following:
+
+     a) Accompany the combined library with a copy of the same work based on the Library, uncombined with any other library facilities, conveyed under the terms of this License.
+
+     b) Give prominent notice with the combined library that part of it is a work based on the Library, and explaining where to find the accompanying uncombined form of the same work.
+
+6. Revised Versions of the GNU Lesser General Public License.
+The Free Software Foundation may publish revised and/or new versions of the GNU Lesser General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Library as you received it specifies that a certain numbered version of the GNU Lesser General Public License "or any later version" applies to it, you have the option of following the terms and conditions either of that published version or of any later version published by the Free Software Foundation. If the Library as you received it does not specify a version number of the GNU Lesser General Public License, you may choose any version of the GNU Lesser General Public License ever published by the Free Software Foundation.
+
+If the Library as you received it specifies that a proxy can decide whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is permanent authorization for you to choose that version for the Library.
+
+GNU GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007
+
+Copyright © 2007 Free Software Foundation, Inc. <http://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+
+Preamble
+
+The GNU General Public License is a free, copyleft license for software and other kinds of works.
+
+The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, the GNU General Public License is intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users. We, the Free Software Foundation, use the GNU General Public License for most of our software; it applies also to any other work released this way by its authors. You can apply it to your programs, too.
+
+When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
+
+To protect your rights, we need to prevent others from denying you these rights or asking you to surrender the rights. Therefore, you have certain responsibilities if you distribute copies of the software, or if you modify it: responsibilities to respect the freedom of others.
+
+For example, if you distribute copies of such a program, whether gratis or for a fee, you must pass on to the recipients the same freedoms that you received. You must make sure that they, too, receive or can get the source code. And you must show them these terms so they know their rights.
+
+Developers that use the GNU GPL protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License giving you legal permission to copy, distribute and/or modify it.
+
+For the developers' and authors' protection, the GPL clearly explains that there is no warranty for this free software. For both users' and authors' sake, the GPL requires that modified versions be marked as changed, so that their problems will not be attributed erroneously to authors of previous versions.
+
+Some devices are designed to deny users access to install or run modified versions of the software inside them, although the manufacturer can do so. This is fundamentally incompatible with the aim of protecting users' freedom to change the software. The systematic pattern of such abuse occurs in the area of products for individuals to use, which is precisely where it is most unacceptable. Therefore, we have designed this version of the GPL to prohibit the practice for those products. If such problems arise substantially in other domains, we stand ready to extend this provision to those domains in future versions of the GPL, as needed to protect the freedom of users.
+
+Finally, every program is threatened constantly by software patents. States should not allow patents to restrict development and use of software on general-purpose computers, but in those that do, we wish to avoid the special danger that patents applied to a free program could make it effectively proprietary. To prevent this, the GPL assures that patents cannot be used to render the program non-free.
+
+The precise terms and conditions for copying, distribution and modification follow.
+
+TERMS AND CONDITIONS
+
+0. Definitions.
+
+“This License” refers to version 3 of the GNU General Public License.
+
+“Copyright” also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
+
+“The Program” refers to any copyrightable work licensed under this License. Each licensee is addressed as “you”. “Licensees” and “recipients” may be individuals or organizations.
+
+To “modify” a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a “modified version” of the earlier work or a work “based on” the earlier work.
+
+A “covered work” means either the unmodified Program or a work based on the Program.
+
+To “propagate” a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
+
+To “convey” a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays “Appropriate Legal Notices” to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
+
+1. Source Code.
+The “source code” for a work means the preferred form of the work for making modifications to it. “Object code” means any non-source form of a work.
+
+A “Standard Interface” means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
+
+The “System Libraries” of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A “Major Component”, in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
+
+The “Corresponding Source” for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same work.
+
+2. Basic Permissions.
+All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
+
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
+
+When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
+
+4. Conveying Verbatim Copies.
+You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
+
+5. Conveying Modified Source Versions.
+You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
+
+     a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
+
+     b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to “keep intact all notices”.
+
+     c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
+
+     d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
+
+A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an “aggregate” if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
+
+6. Conveying Non-Source Forms.
+You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
+
+     a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
+
+     b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
+
+     c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
+
+     d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
+
+     e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
+
+A “User Product” is either (1) a “consumer product”, which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, “normally used” refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
+
+“Installation Information” for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
+
+The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
+
+7. Additional Terms.
+“Additional permissions” are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
+
+     a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
+
+     b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
+
+     c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
+
+     d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
+
+     e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
+
+     f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
+
+All other non-permissive additional terms are considered “further restrictions” within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
+
+8. Termination.
+You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
+
+However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
+
+Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
+
+9. Acceptance Not Required for Having Copies.
+You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
+
+10. Automatic Licensing of Downstream Recipients.
+Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
+
+An “entity transaction” is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
+
+11. Patents.
+A “contributor” is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's “contributor version”.
+
+A contributor's “essential patent claims” are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, “control” includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
+
+In the following three paragraphs, a “patent license” is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To “grant” such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. “Knowingly relying” means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
+
+A patent license is “discriminatory” if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
+
+12. No Surrender of Others' Freedom.
+If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
+
+13. Use with the GNU Affero General Public License.
+Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU Affero General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the special requirements of the GNU Affero General Public License, section 13, concerning interaction through a network will apply to the combination as such.
+
+14. Revised Versions of this License.
+The Free Software Foundation may publish revised and/or new versions of the GNU General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU General Public License, you may choose any version ever published by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions of the GNU General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
+
+Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
+
+15. Disclaimer of Warranty.
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+16. Limitation of Liability.
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+
+17. Interpretation of Sections 15 and 16.
+If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
+
+How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest possible use to the public, the best way to achieve this is to make it free software which everyone can redistribute and change under these terms.
+
+To do so, attach the following notices to the program. It is safest to attach them to the start of each source file to most effectively state the exclusion of warranty; and each file should have at least the “copyright” line and a pointer to where the full notice is found.
+
+     <one line to give the program's name and a brief idea of what it does.>
+     Copyright (C) <year>  <name of author>
+
+     This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
+If the program does terminal interaction, make it output a short notice like this when it starts in an interactive mode:
+
+     <program>  Copyright (C) <year>  <name of author>
+     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+     This is free software, and you are welcome to redistribute it under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate parts of the General Public License. Of course, your program's commands might be different; for a GUI interface, you would use an “about box”.
+
+You should also get your employer (if you work as a programmer) or school, if any, to sign a “copyright disclaimer” for the program, if necessary. For more information on this, and how to apply and follow the GNU GPL, see <http://www.gnu.org/licenses/>.
 
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
+The GNU General Public License does not permit incorporating your program into proprietary programs. If your program is a subroutine library, you may consider it more useful to permit linking proprietary applications with the library. If this is what you want to do, use the GNU Lesser General Public License instead of this License. But first, please read <http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `psy-view-0.2.0/README.rst` & `psy-view-0.3.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,26 @@
+.. SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 =========================================
 psy-view: An ncview-like GUI with psyplot
 =========================================
 
 .. start-badges
 
-.. list-table::
-    :stub-columns: 1
-    :widths: 10 90
-
-    * - docs
-      - |docs| |mybinder|
-    * - tests
-      - |circleci| |appveyor| |codecov|
-    * - package
-      - |version| |conda| |github| |zenodo|
-    * - implementations
-      - |supported-versions| |supported-implementations|
-    * - get in touch
-      - |gitter| |mailing-list| |issues|
-
-.. |docs| image:: https://img.shields.io/github/deployments/psyplot/psy-view/github-pages
-    :alt: Documentation
-    :target: http://psyplot.github.io/psy-view/
-
-.. |mybinder| image:: https://mybinder.org/badge_logo.svg
-    :target: https://mybinder.org/v2/gh/psyplot/psy-view/master?urlpath=%2Fdesktop
-    :alt: mybinder.org
-
-.. |circleci| image:: https://circleci.com/gh/psyplot/psy-view/tree/master.svg?style=svg
-    :alt: CircleCI
-    :target: https://circleci.com/gh/psyplot/psy-view/tree/master
-
-.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/a7qxvvwt0e41j32h/branch/master?svg=true
-    :alt: AppVeyor
-    :target: https://ci.appveyor.com/project/psyplot/psy-view/branch/master
-
-.. |codecov| image:: https://codecov.io/gh/psyplot/psy-view/branch/master/graph/badge.svg
-    :alt: Coverage
-    :target: https://codecov.io/gh/psyplot/psy-view
-
-.. |conda| image:: https://anaconda.org/conda-forge/psy-view/badges/version.svg
-    :alt: conda
-    :target: https://anaconda.org/conda-forge/psy-view
-
-.. |github| image:: https://img.shields.io/github/release/psyplot/psy-view.svg
-    :target: https://github.com/psyplot/psy-view/releases/latest
-    :alt: Latest github release
-
-.. |version| image:: https://img.shields.io/pypi/v/psy-view.svg?style=flat
-    :alt: PyPI Package latest release
-    :target: https://pypi.python.org/pypi/psy-view
-
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/psy-view.svg?style=flat
-    :alt: Supported versions
-    :target: https://pypi.python.org/pypi/psy-view
-
-.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/psy-view.svg?style=flat
-    :alt: Supported implementations
-    :target: https://pypi.python.org/pypi/psy-view
-
-.. |gitter| image:: https://img.shields.io/gitter/room/psyplot/community.svg?style=flat
-    :target: https://gitter.im/psyplot/community
-    :alt: Gitter
-
-.. |mailing-list| image:: https://img.shields.io/badge/join-mailing%20list-brightgreen.svg?style=flat
-    :target: https://www.listserv.dfn.de/sympa/subscribe/psyplot
-    :alt: DFN mailing list
-
-.. |issues| image:: https://img.shields.io/github/issues-raw/psyplot/psy-view.svg?style=flat
-    :target: https://github.com/psyplot/psy-view/issues
-    :alt: GitHub issues
-
-.. |zenodo| image:: https://zenodo.org/badge/249615633.svg
-    :alt: Zenodo
-    :target: https://zenodo.org/badge/latestdoi/249615633
+|CI|
+|Code coverage|
+|Latest Release|
+|PyPI version|
+|Code style: black|
+|Imports: isort|
+|PEP8|
+|Checked with mypy|
+|REUSE status|
 
 .. end-badges
 
 This package defines a viewer application for netCDF files, that is highly
 motivated by the ncview_ package but entirely built upon the psyplot framework.
 It supports strucutured and unstructured grids and provides an intuitive
 graphical user interface to quickly dive into the data inside a netCDF file.
@@ -102,15 +45,15 @@
   plot
 - automatically decodes CF-conventions and supports unstructured grid, such as
   ICON_ or UGRID_
 - animation interface
 - different projections
 - implemented in psyplot-gui_ for full flexibility (if desired)
 
-.. _ICON: https://mpimet.mpg.de/en/science/modeling-with-icon/icon-configurations
+.. _ICON: https://code.mpimet.mpg.de/projects/iconpublic
 .. _UGRID: http://ugrid-conventions.github.io/ugrid-conventions/
 .. _psyplot-gui: https://psyplot.github.io/psyplot-gui
 
 
 Test it without installation
 ----------------------------
 You can try the functionalities with some selected example files headless in
@@ -194,7 +137,27 @@
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see https://www.gnu.org/licenses/.
+
+
+.. |CI| image:: https://codebase.helmholtz.cloud/psyplot/psy-view/badges/master/pipeline.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psy-view/-/pipelines?page=1&scope=all&ref=master
+.. |Code coverage| image:: https://codebase.helmholtz.cloud/psyplot/psy-view/badges/master/coverage.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psy-view/-/graphs/master/charts
+.. |Latest Release| image:: https://codebase.helmholtz.cloud/psyplot/psy-view/-/badges/release.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psy-view
+.. |PyPI version| image:: https://img.shields.io/pypi/v/psy-view.svg
+   :target: https://pypi.python.org/pypi/psy-view/
+.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. |Imports: isort| image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+   :target: https://pycqa.github.io/isort/
+.. |PEP8| image:: https://img.shields.io/badge/code%20style-pep8-orange.svg
+   :target: https://www.python.org/dev/peps/pep-0008/
+.. |Checked with mypy| image:: http://www.mypy-lang.org/static/mypy_badge.svg
+   :target: http://mypy-lang.org/
+.. |REUSE status| image:: https://api.reuse.software/badge/codebase.helmholtz.cloud/psyplot/psy-view
+   :target: https://api.reuse.software/info/codebase.helmholtz.cloud/psyplot/psy-view
```

### Comparing `psy-view-0.2.0/psy_view/dialogs.py` & `psy-view-0.3.0/psy_view/dialogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,25 @@
 """Dialogs for manipulating formatoptions."""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-#
-# This file is part of psy-view and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
 from __future__ import annotations
-from typing import (
-    TYPE_CHECKING,
-    Dict,
-    Any,
-    Optional,
-    Tuple,
-    Union,
-    Type,
-)
+
+from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Type, Union
 
 import yaml
-from PyQt5 import QtWidgets, QtGui
 from matplotlib.backends.backend_qt5agg import (
-    FigureCanvasQTAgg as FigureCanvas)
+    FigureCanvasQTAgg as FigureCanvas,
+)
 from matplotlib.figure import Figure
-
-from psyplot.plotter import Plotter, Formatoption
+from psyplot.plotter import Formatoption, Plotter
+from PyQt5 import QtGui, QtWidgets
 
 if TYPE_CHECKING:
     from psyplot.project import Project
     from PyQt5.QtCore import QEvent  # pylint: disable=no-name-in-module
 
 
 #: TODO: Find a more appropriate description here
@@ -62,30 +38,32 @@
     def __init__(self, plotter: Plotter, *args, **kwargs) -> None:
         """
         Parameters
         ----------
         plotter: psy_maps.plotters.MapPlotter
             The psyplot plotter to configure
         """
-        import psy_simple.widgets.colors as pswc
         import pandas as pd
+        import psy_simple.widgets.colors as pswc
+
         super().__init__(*args, **kwargs)
         vbox = QtWidgets.QVBoxLayout(self)
 
         #: colors that affect the map background
-        self.colors = ['background', 'land', 'ocean', 'coast']
+        self.colors = ["background", "land", "ocean", "coast"]
 
         #: QGridLayout to display the various colors
         grid = QtWidgets.QGridLayout()
 
         defaults = self.default_colors
 
         #: :class:`pandas.DataFrame` of widgets to modifiy the :attr:`colors`
         self.widgets = widgets = pd.DataFrame(
-            index=['enable', 'color'], columns=self.colors, dtype=object)
+            index=["enable", "color"], columns=self.colors, dtype=object
+        )
 
         for i, col in enumerate(self.colors):
             widgets.iloc[0, i] = cb = QtWidgets.QCheckBox()
             cb.setChecked(False)
             widgets.iloc[1, i] = lbl = pswc.ColorLabel(defaults[col])
             lbl.setEnabled(False)
 
@@ -96,41 +74,42 @@
             grid.addWidget(lbl, 2, i)
 
         vbox.addLayout(grid)
 
         #: Button box to cancel the operator or update the plotter
         self.button_box = QtWidgets.QDialogButtonBox(
             QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel,
-            self)
+            self,
+        )
 
         self.button_box.accepted.connect(self.accept)
         self.button_box.rejected.connect(self.reject)
 
         proj_box = QtWidgets.QGroupBox("Projection settings")
         layout = QtWidgets.QFormLayout(proj_box)
 
         #: text box for the central longitude (clon formatoption)
         self.txt_clon = QtWidgets.QLineEdit()
-        self.txt_clon.setPlaceholderText('auto')
-        self.txt_clon.setToolTip('Central longitude in degrees East')
+        self.txt_clon.setPlaceholderText("auto")
+        self.txt_clon.setToolTip("Central longitude in degrees East")
         self.txt_clon.setValidator(QtGui.QDoubleValidator(-360, 360, 7))
-        layout.addRow('Central longitude: ', self.txt_clon)
+        layout.addRow("Central longitude: ", self.txt_clon)
 
         #: text box for the central latitude (clat formatoption)
         self.txt_clat = QtWidgets.QLineEdit()
-        self.txt_clat.setPlaceholderText('auto')
-        self.txt_clat.setToolTip('Central latitude in degrees North')
+        self.txt_clat.setPlaceholderText("auto")
+        self.txt_clat.setToolTip("Central latitude in degrees North")
         self.txt_clat.setValidator(QtGui.QDoubleValidator(-90, 90, 7))
-        layout.addRow('Central latitude: ', self.txt_clat)
+        layout.addRow("Central latitude: ", self.txt_clat)
 
         vbox.addWidget(proj_box)
 
         #: group box for modifying the resolution of the land-sea-mask, see
         #: :attr:`opt_110m`, :attr:`opt_50m`, :attr:`opt_10m`
-        self.lsm_box = QtWidgets.QGroupBox('Coastlines')
+        self.lsm_box = QtWidgets.QGroupBox("Coastlines")
         self.lsm_box.setCheckable(True)
         hbox = QtWidgets.QHBoxLayout(self.lsm_box)
         hbox.addWidget(QtWidgets.QLabel("Resolution:"))
 
         #: Radiobutton for 110m resolution of lsm
         self.opt_110m = QtWidgets.QRadioButton("110m")
 
@@ -142,31 +121,32 @@
         hbox.addWidget(self.opt_110m)
         hbox.addWidget(self.opt_50m)
         hbox.addWidget(self.opt_10m)
 
         vbox.addWidget(self.lsm_box)
 
         #: group box drawing grid lines and labels
-        self.grid_labels_box = QtWidgets.QGroupBox('Labels')
-        self.grid_labels_box.setToolTip("Draw labels of meridionals and "
-                                        "parallels")
+        self.grid_labels_box = QtWidgets.QGroupBox("Labels")
+        self.grid_labels_box.setToolTip(
+            "Draw labels of meridionals and " "parallels"
+        )
         self.grid_labels_box.setCheckable(True)
 
         #: text box for the fontsize of grid labels
         self.txt_grid_fontsize = QtWidgets.QLineEdit()
 
         form = QtWidgets.QFormLayout(self.grid_labels_box)
         form.addRow("Font size:", self.txt_grid_fontsize)
 
         vbox.addWidget(self.grid_labels_box)
 
         #: Group box for options specific to meridionals (see
         #: :attr:`opt_meri_auto`, :attr:`opt_meri_at` and
         #: :attr:`opt_meri_every`, :attr:`opt_meri_num`)
-        self.meridionals_box = QtWidgets.QGroupBox('Meridionals')
+        self.meridionals_box = QtWidgets.QGroupBox("Meridionals")
         self.meridionals_box.setCheckable(True)
 
         #: Radiobutton for automatic drawing of meridionals
         self.opt_meri_auto = QtWidgets.QRadioButton("auto")
 
         #: Radiobutton for giving the exact position of meridionals (see
         #: :attr:`txt_meri_at`)
@@ -205,15 +185,15 @@
         form.addRow(self.opt_meri_num, self.txt_meri_num)
 
         vbox.addWidget(self.meridionals_box)
 
         #: Group box for options specific to parallels (see
         #: :attr:`opt_para_auto`, :attr:`opt_para_at` and
         #: :attr:`opt_para_every`, :attr:`opt_para_num`)
-        self.parallels_box = QtWidgets.QGroupBox('Parallels')
+        self.parallels_box = QtWidgets.QGroupBox("Parallels")
         self.parallels_box.setCheckable(True)
 
         #: Radiobutton for automatic drawing of parallels
         self.opt_para_auto = QtWidgets.QRadioButton("auto")
 
         #: Radiobutton for giving the exact position of parallels (see
         #: :attr:`txt_para_at`)
@@ -249,35 +229,70 @@
         form.addRow(self.opt_para_auto)
         form.addRow(self.opt_para_at, self.txt_para_at)
         form.addRow(self.opt_para_every, self.txt_para_every)
         form.addRow(self.opt_para_num, self.txt_para_num)
 
         vbox.addWidget(self.parallels_box)
 
+        #: A box for selecting the background image
+        self.background_img_box = QtWidgets.QGroupBox("Background image")
+        self.background_img_box.setCheckable(True)
+
+        #: Radio button for using the ``stock_image`` formatoption
+        self.opt_stock_img = QtWidgets.QRadioButton("Stock image")
+
+        #: Radio button for using the ``google_map_detail`` formatoption
+        self.opt_google_image = QtWidgets.QRadioButton("Google maps")
+
+        #: Test box for specifying the detail
+        self.sb_google_image = QtWidgets.QSpinBox()
+        self.sb_google_image.setMinimum(0)
+        self.sb_google_image.setValue(4)
+        self.sb_google_image.setToolTip(
+            "The detail level for the Google image. The higher this "
+            "number, the more details you'll see (and the slower it is)"
+        )
+
+        form = QtWidgets.QFormLayout(self.background_img_box)
+
+        form.addRow(self.opt_stock_img)
+        form.addRow(self.opt_google_image, self.sb_google_image)
+
+        vbox.addWidget(self.background_img_box)
+
         vbox.addWidget(self.button_box)
 
         self.fill_from_plotter(plotter)
 
-        for button in [self.opt_meri_at, self.opt_meri_auto, self.opt_meri_num,
-                       self.opt_meri_every, self.opt_para_at,
-                       self.opt_para_auto, self.opt_para_num,
-                       self.opt_para_every]:
+        for button in [
+            self.opt_meri_at,
+            self.opt_meri_auto,
+            self.opt_meri_num,
+            self.opt_meri_every,
+            self.opt_para_at,
+            self.opt_para_auto,
+            self.opt_para_num,
+            self.opt_para_every,
+            self.opt_stock_img,
+            self.opt_google_image,
+        ]:
             button.clicked.connect(self.update_forms)
 
     @property
     def default_colors(self) -> Dict[str, Color]:
         """Get default colors for the color labels in :attr:`widgets`."""
         import cartopy.feature as cf
         import matplotlib as mpl
+
         return {
-            'background': mpl.rcParams['axes.facecolor'],
-            'land': cf.LAND._kwargs['facecolor'],
-            'ocean': cf.OCEAN._kwargs['facecolor'],
-            'coast': 'k',
-            }
+            "background": mpl.rcParams["axes.facecolor"],
+            "land": cf.LAND._kwargs["facecolor"],
+            "ocean": cf.OCEAN._kwargs["facecolor"],
+            "coast": "k",
+        }
 
     def get_colors(self, plotter: Plotter) -> Dict[str, Color]:
         """Get the colors for :attr:`widgets` from the plotter formatoptions.
 
         Parameters
         ----------
         plotter: psy_maps.plotters.MapPlotter
@@ -286,18 +301,18 @@
         Returns
         -------
         dict
             A mapping from formatoptions in :attr:`colors` to the corresponding
             color in the `plotter`.
         """
         ret = {}
-        if plotter.background.value != 'rc':
-            ret['background'] = plotter.background.value
+        if plotter.background.value != "rc":
+            ret["background"] = plotter.background.value
         lsm = plotter.lsm.value
-        for part in ['land', 'ocean', 'coast']:
+        for part in ["land", "ocean", "coast"]:
             if part in lsm:
                 ret[part] = lsm[part]
         return ret
 
     def fill_from_plotter(self, plotter: Plotter) -> None:
         """Fill the dialog from a given plotter.
 
@@ -322,16 +337,16 @@
             self.txt_clat.setText(str(plotter.clat.value))
 
         lsm = plotter.lsm.value
 
         if not lsm:
             self.lsm_box.setChecked(False)
         else:
-            res = lsm['res']
-            getattr(self, 'opt_' + res).setChecked(True)
+            res = lsm["res"]
+            getattr(self, "opt_" + res).setChecked(True)
 
         grid_labels = plotter.grid_labels.value
         if grid_labels is None:
             grid_labels = True
         self.grid_labels_box.setChecked(grid_labels)
         self.txt_grid_fontsize.setText(str(plotter.grid_labelsize.value))
 
@@ -348,15 +363,15 @@
         elif isinstance(value, tuple):
             self.xgrid_value: Tuple[Any, Any] = value[:2]  # type: ignore
             self.opt_meri_num.setChecked(True)
             steps = 11 if len(value) == 2 else value[3]
             self.txt_meri_num.setText(str(steps))
         else:
             self.opt_meri_at.setChecked(True)
-            self.txt_meri_at.setText(', '.join(map(str, value)))
+            self.txt_meri_at.setText(", ".join(map(str, value)))
 
         self.ygrid_value = None
         value = plotter.ygrid.value
         if not value:
             self.parallels_box.setChecked(False)
         elif value is True:
             self.opt_para_auto.setChecked(True)
@@ -367,113 +382,155 @@
         elif isinstance(value, tuple):
             self.ygrid_value: Tuple[Any, Any] = value[:2]  # type: ignore
             self.opt_para_num.setChecked(True)
             steps = 11 if len(value) == 2 else value[3]
             self.txt_para_num.setText(str(steps))
         else:
             self.opt_para_at.setChecked(True)
-            self.txt_para_at.setText(', '.join(map(str, value)))
+            self.txt_para_at.setText(", ".join(map(str, value)))
+
+        stock_img = plotter.stock_img.value
+        google_img_detail = plotter.google_map_detail.value
+
+        if not stock_img and google_img_detail is None:
+            self.background_img_box.setChecked(False)
+        else:
+            self.background_img_box.setChecked(True)
+            if stock_img:
+                self.opt_stock_img.setChecked(True)
+            elif google_img_detail is not None:
+                self.opt_google_image.setChecked(True)
+                self.sb_google_image.setValue(google_img_detail)
 
     def update_forms(self) -> None:
-        """Update text widgets for the options to draw merdionals and parallels.
-        """
+        """Update text widgets for the options to draw merdionals and parallels."""
         if self.meridionals_box.isChecked():
             self.txt_meri_at.setEnabled(self.opt_meri_at.isChecked())
             self.txt_meri_every.setEnabled(self.opt_meri_every.isChecked())
             self.txt_meri_num.setEnabled(self.opt_meri_num.isChecked())
         if self.parallels_box.isChecked():
             self.txt_para_at.setEnabled(self.opt_para_at.isChecked())
             self.txt_para_every.setEnabled(self.opt_para_every.isChecked())
             self.txt_para_num.setEnabled(self.opt_para_num.isChecked())
+        if self.background_img_box.isChecked():
+            self.sb_google_image.setEnabled(self.opt_google_image.isChecked())
 
     @property
     def value(self) -> Dict[str, Any]:
         """Get the formatoptions of this dialog to update a plotter."""
         import numpy as np
+
         ret: Dict[str, Any] = {}
-        ret['clon'] = None if not self.txt_clon.text().strip() else float(
-            self.txt_clon.text().strip())
-        ret['clat'] = None if not self.txt_clat.text().strip() else float(
-            self.txt_clat.text().strip())
+        ret["clon"] = (
+            None
+            if not self.txt_clon.text().strip()
+            else float(self.txt_clon.text().strip())
+        )
+        ret["clat"] = (
+            None
+            if not self.txt_clat.text().strip()
+            else float(self.txt_clat.text().strip())
+        )
 
         lsm: LSM_T = {}
 
-        for col in ['land', 'ocean', 'coast']:
-            lbl = self.widgets.loc['color', col]
+        for col in ["land", "ocean", "coast"]:
+            lbl = self.widgets.loc["color", col]
             if lbl.isEnabled():
                 lsm[col] = list(lbl.color.getRgbF())
 
         if lsm or self.lsm_box.isChecked():
             if self.opt_110m.isChecked():
-                lsm['res'] = '110m'
+                lsm["res"] = "110m"
             elif self.opt_50m.isChecked():
-                lsm['res'] = '50m'
+                lsm["res"] = "50m"
             elif self.opt_10m.isChecked():
-                lsm['res'] = '10m'
+                lsm["res"] = "10m"
             else:
-                lsm['res'] = '110m'
+                lsm["res"] = "110m"
         else:
-            lsm['res'] = False
+            lsm["res"] = False
         if lsm:
-            ret['lsm'] = lsm
+            ret["lsm"] = lsm
 
-        bc_lbl = self.widgets.loc['color', 'background']
+        bc_lbl = self.widgets.loc["color", "background"]
         if bc_lbl.isEnabled():
-            ret['background'] = list(bc_lbl.color.getRgbF())
+            ret["background"] = list(bc_lbl.color.getRgbF())
 
         ret["grid_labels"] = self.grid_labels_box.isChecked()
         if ret["grid_labels"]:
             ret["grid_labels"] = None
             labelsize = self.txt_grid_fontsize.text().strip()
             if labelsize:
                 try:
                     labelsize = float(labelsize)
                 except TypeError:
                     pass
                 ret["grid_labelsize"] = labelsize
 
         if not self.meridionals_box.isChecked():
-            ret['xgrid'] = False
+            ret["xgrid"] = False
         elif self.opt_meri_auto.isChecked():
-            ret['xgrid'] = True
+            ret["xgrid"] = True
         elif self.opt_meri_every.isChecked():
-            ret['xgrid'] = np.arange(
-                -180, 180, float(self.txt_meri_every.text().strip() or 30))
+            ret["xgrid"] = np.arange(
+                -180, 180, float(self.txt_meri_every.text().strip() or 30)
+            )
         elif self.opt_meri_at.isChecked():
-            ret['xgrid'] = list(map(
-                float, self.txt_meri_at.text().split(','))) or False
+            ret["xgrid"] = (
+                list(map(float, self.txt_meri_at.text().split(","))) or False
+            )
         elif self.opt_meri_num.isChecked():
             if self.xgrid_value is None:
-                ret['xgrid'] = ['rounded', int(self.txt_meri_num.text() or 5)]
+                ret["xgrid"] = ["rounded", int(self.txt_meri_num.text() or 5)]
             elif isinstance(self.xgrid_value, str):
-                ret['xgrid'] = [self.xgrid_value,
-                                int(self.txt_meri_num.text() or 5)]
+                ret["xgrid"] = [
+                    self.xgrid_value,
+                    int(self.txt_meri_num.text() or 5),
+                ]
             else:
-                ret['xgrid'] = tuple(self.xgrid_value) + (
-                    int(self.txt_meri_num.text() or 5), )
+                ret["xgrid"] = tuple(self.xgrid_value) + (
+                    int(self.txt_meri_num.text() or 5),
+                )
 
         if not self.parallels_box.isChecked():
-            ret['ygrid'] = False
+            ret["ygrid"] = False
         elif self.opt_para_auto.isChecked():
-            ret['ygrid'] = True
+            ret["ygrid"] = True
         elif self.opt_para_every.isChecked():
-            ret['ygrid'] = np.arange(
-                -180, 180, float(self.txt_para_every.text().strip() or 30))
+            ret["ygrid"] = np.arange(
+                -180, 180, float(self.txt_para_every.text().strip() or 30)
+            )
         elif self.opt_para_at.isChecked():
-            ret['ygrid'] = list(map(
-                float, self.txt_para_at.text().split(','))) or False
+            ret["ygrid"] = (
+                list(map(float, self.txt_para_at.text().split(","))) or False
+            )
         elif self.opt_para_num.isChecked():
             if self.ygrid_value is None:
-                ret['ygrid'] = ['rounded', int(self.txt_para_num.text() or 5)]
+                ret["ygrid"] = ["rounded", int(self.txt_para_num.text() or 5)]
             elif isinstance(self.ygrid_value, str):
-                ret['ygrid'] = [self.ygrid_value,
-                                int(self.txt_para_num.text() or 5)]
+                ret["ygrid"] = [
+                    self.ygrid_value,
+                    int(self.txt_para_num.text() or 5),
+                ]
             else:
-                ret['ygrid'] = tuple(self.ygrid_value) + (
-                    int(self.txt_para_num.text() or 5), )
+                ret["ygrid"] = tuple(self.ygrid_value) + (
+                    int(self.txt_para_num.text() or 5),
+                )
+
+        if self.background_img_box.isChecked():
+            if self.opt_stock_img.isChecked():
+                ret["stock_img"] = True
+                ret["google_map_detail"] = None
+            elif self.opt_google_image.isChecked():
+                ret["stock_img"] = False
+                ret["google_map_detail"] = self.sb_google_image.value() or 0
+        else:
+            ret["stock_img"] = False
+            ret["google_map_detail"] = None
         return ret
 
     @classmethod
     def update_plotter(cls, plotter: Plotter) -> None:
         """Open a :class:`BasemapDialog` to update a plotter.
 
         Parameters
@@ -483,70 +540,83 @@
         """
         dialog = cls(plotter)
         dialog.show()
         dialog.raise_()
         dialog.activateWindow()
         dialog.exec_()
         if dialog.result() == QtWidgets.QDialog.Accepted:
-            plotter.update(
-                **dialog.value)
+            plotter.update(**dialog.value)
 
 
 class CmapDialog(QtWidgets.QDialog):
     """A dialog to modify color bounds and colormaps."""
 
     def __init__(self, project: Project, *args, **kwargs) -> None:
         """
         Parameters
         ----------
         project: psyplot.project.Project
             The psyplot project to update. Note that we will only use the
             very first plotter in this project
         """
         import psy_simple.widgets.colors as pswc
+
         super().__init__(*args, **kwargs)
 
         #: Button box to accept or cancel this dialog
         self.button_box = QtWidgets.QDialogButtonBox(
             QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel,
-            self)
+            self,
+        )
         self.button_box.accepted.connect(self.accept)
         self.button_box.rejected.connect(self.reject)
 
         #: Mapping from formatoption key to :class:`LabelWidgetLine` widgets to
         #: controlling the formatoption
         self.fmt_widgets = {}
-        plotter = project(fmts=['cmap', 'bounds']).plotters[0]
+        plotter = project(fmts=["cmap", "bounds"]).plotters[0]
 
         #: Widget for manipulating the color map
-        self.cmap_widget = self.fmt_widgets['cmap'] = LabelWidgetLine(
-            plotter.cmap, project, pswc.CMapFmtWidget,
-            widget_kws=dict(properties=False))
+        self.cmap_widget = self.fmt_widgets["cmap"] = LabelWidgetLine(
+            plotter.cmap,
+            project,
+            pswc.CMapFmtWidget,
+            widget_kws=dict(properties=False),
+        )
         self.cmap_widget.editor.setVisible(False)
         self.cmap_widget.editor.line_edit.textChanged.connect(
-            self.update_preview)
+            self.update_preview
+        )
 
         #: tabs for switching between bounds (:attr:`bounds_widget`) and
         #: colorbar ticks (:attr:`cticks_widget`)
         self.tabs = QtWidgets.QTabWidget()
 
         #: :class:`LabelWidgetLine` to controll the colorbar bounds
-        self.bounds_widget = self.fmt_widgets['bounds'] = LabelWidgetLine(
-            plotter.bounds, project, pswc.BoundsFmtWidget,
-            widget_kws=dict(properties=False))
+        self.bounds_widget = self.fmt_widgets["bounds"] = LabelWidgetLine(
+            plotter.bounds,
+            project,
+            pswc.BoundsFmtWidget,
+            widget_kws=dict(properties=False),
+        )
         self.bounds_widget.editor.line_edit.textChanged.connect(
-            self.update_preview)
+            self.update_preview
+        )
         self.tabs.addTab(self.bounds_widget, "Colormap boundaries")
 
         #: :class:`LabelWidgetLine` to controll the ctick positions
-        self.cticks_widget = self.fmt_widgets['cticks'] = LabelWidgetLine(
-            plotter.cticks, project, pswc.CTicksFmtWidget,
-            widget_kws=dict(properties=False))
+        self.cticks_widget = self.fmt_widgets["cticks"] = LabelWidgetLine(
+            plotter.cticks,
+            project,
+            pswc.CTicksFmtWidget,
+            widget_kws=dict(properties=False),
+        )
         self.cticks_widget.editor.line_edit.textChanged.connect(
-            self.update_preview)
+            self.update_preview
+        )
         self.tabs.addTab(self.cticks_widget, "Colorbar ticks")
 
         #: :class:`ColorbarPreview` to show a preview of the colorbar with
         #: the selected formatoption in :attr:`fmt_widgets`
         self.cbar_preview = ColorbarPreview(plotter)
         self.cbar_preview.setMaximumHeight(self.tabs.sizeHint().height() // 3)
 
@@ -558,42 +628,44 @@
 
     @property
     def plotter(self) -> Plotter:
         """Get the plotter with the formatoptions we use to fill this dialog."""
         return self.bounds_widget.editor.fmto.plotter
 
     def update_preview(self) -> None:
-        """Update the :attr:`cbar_preview` from the various :attr:`fmt_widgets`.
-        """
+        """Update the :attr:`cbar_preview` from the various :attr:`fmt_widgets`."""
         try:
             bounds = self.bounds_widget.editor.value
         except Exception:
             bounds = self.plotter.bounds.value
         try:
             cticks = self.cticks_widget.editor.value
         except Exception:
             cticks = self.plotter.cticks.value
         try:
             cmap = self.cmap_widget.editor.value
         except Exception:
             cmap = self.plotter.cmap.value
         self.cbar_preview.update_colorbar(
-            bounds=bounds, cticks=cticks, cmap=cmap)
+            bounds=bounds, cticks=cticks, cmap=cmap
+        )
 
     @property
     def fmts(self) -> Dict[str, Any]:
         """Map from formatoption in :attr:`fmt_widgets` to values."""
         ret = {}
         for fmt, widget in self.fmt_widgets.items():
             if widget.editor.changed:
                 try:
                     value = widget.editor.value
-                except:
-                    raise IOError(f"{fmt}-value {widget.editor.text} could "
-                                  "not be parsed to python!")
+                except Exception:
+                    raise IOError(
+                        f"{fmt}-value {widget.editor.text} could "
+                        "not be parsed to python!"
+                    )
                 else:
                     ret[fmt] = value
         return ret
 
     @classmethod
     def update_project(cls, project: Project) -> None:
         """Create a :class:`CmapDialog` to update a `project`
@@ -619,55 +691,61 @@
 class _DummyFormatOption(Formatoption):
     """Dummy formatoption for static type checking.
 
     This is just a workaround for the static type checker to be able to tell
     what the :class:`FakePlotter` formatoptions are, used in
     :attr:`ColorbarPreview.fake_plotter`
     """
-    def update(self,):
+
+    def update(
+        self,
+    ):
         pass
 
 
 class FakePlotter(Plotter):
     """A dummy plotter for the colorbar preview."""
 
-    bounds: Formatoption = _DummyFormatOption('bounds')
-    cmap: Formatoption = _DummyFormatOption('cmap')
-    cticks: Formatoption = _DummyFormatOption('cticks')
-    cbar: Formatoption = _DummyFormatOption('cbar')
+    bounds: Formatoption = _DummyFormatOption("bounds")
+    cmap: Formatoption = _DummyFormatOption("cmap")
+    cticks: Formatoption = _DummyFormatOption("cticks")
+    cbar: Formatoption = _DummyFormatOption("cbar")
 
 
 class ColorbarPreview(FigureCanvas):
     """A preview widget of a colorbar.
 
     This matplotlib figure contains one single axes to display the colorbar
     filled by the formatoptions of a given `plotter`."""
 
     def __init__(
-            self,
-            plotter: Plotter,
-            parent: Optional[QtWidgets.QWidget] = None,
-            *args, **kwargs
-        ) -> None:
+        self,
+        plotter: Plotter,
+        parent: Optional[QtWidgets.QWidget] = None,
+        *args,
+        **kwargs,
+    ) -> None:
         """
         Parameters
         ----------
         plotter: psy_simple.plotters.Base2D
             The plotter to use to draw the colorbar from
         parent: QtWidget.QWidget
             The parent widget
         """
         fig = Figure(*args, **kwargs)
 
         FigureCanvas.__init__(self, fig)
         self.setParent(parent)
 
-        FigureCanvas.setSizePolicy(self,
-                                   QtWidgets.QSizePolicy.Expanding,
-                                   QtWidgets.QSizePolicy.Expanding)
+        FigureCanvas.setSizePolicy(
+            self,
+            QtWidgets.QSizePolicy.Expanding,
+            QtWidgets.QSizePolicy.Expanding,
+        )
         FigureCanvas.updateGeometry(self)
         self.axes_counter = 0
 
         #: The plotter to use for displaying the colorbar
         self.plotter = plotter
         self.init_colorbar(plotter)
 
@@ -681,49 +759,57 @@
     def init_colorbar(self, plotter: Plotter) -> None:
         """Initialize the colorbar.
 
         This method extracts the formatoptions of the given `plotter` and draws
         the colorbar.
         """
         from matplotlib.cm import ScalarMappable
+
         norm = plotter.bounds.norm
         cmap = plotter.cmap.get_cmap(self.plotter.plot.array)
 
         self.mappable = sm = ScalarMappable(cmap=cmap, norm=norm)
         sm.set_array([])
 
-        self.cax = self.figure.add_axes([0.1, 0.5, 0.8, 0.5],
-                                        label=self.axes_counter)
+        self.cax = self.figure.add_axes(
+            [0.1, 0.5, 0.8, 0.5], label=self.axes_counter
+        )
 
         self.cbar = self.figure.colorbar(
-            sm, norm=norm, cmap=cmap, cax=self.cax, orientation='horizontal')
+            sm, norm=norm, cmap=cmap, cax=self.cax, orientation="horizontal"
+        )
 
     @property
     def fake_plotter(self) -> FakePlotter:
         """Create a plotter with the formatoptions of the real :attr:`plotter`.
 
         We can update this plotter without impacting the origin :attr:`plotter`
         """
-        from psyplot.plotter import Plotter
 
         class _FakePlotter(FakePlotter):
-            bounds = self.plotter.bounds.__class__('bounds')
-            cmap = self.plotter.cmap.__class__('cmap')
-            cticks = self.plotter.cticks.__class__('cticks')
-            cbar = self.plotter.cbar.__class__('cbar')
+            bounds = self.plotter.bounds.__class__("bounds")
+            cmap = self.plotter.cmap.__class__("cmap")
+            cticks = self.plotter.cticks.__class__("cticks")
+            cbar = self.plotter.cbar.__class__("cbar")
 
             _rcparams_string = self.plotter._get_rc_strings()
 
         ref = self.plotter
         fig = Figure()
         ax = fig.add_subplot()
 
         plotter = _FakePlotter(
-            ref.data.copy(), make_plot=False, bounds=ref['bounds'],
-            cmap=ref['cmap'], cticks=ref['cticks'], cbar='', ax=ax)
+            ref.data.copy(),
+            make_plot=False,
+            bounds=ref["bounds"],
+            cmap=ref["cmap"],
+            cticks=ref["cticks"],
+            cbar="",
+            ax=ax,
+        )
 
         plotter.cticks._colorbar = self.cbar
 
         plotter.plot_data = ref.plot_data
         return plotter
 
     def update_colorbar(self, **kwargs) -> None:
@@ -762,19 +848,21 @@
             except (AttributeError, TypeError):
                 pass
             try:
                 plotter.bounds.norm.autoscale_None(plotter.bounds.array)
             except AttributeError:
                 pass
             self.mappable.set_norm(plotter.bounds.norm)
-            self.mappable.set_cmap(plotter.cmap.get_cmap(
-                self.plotter.plot.array))
+            self.mappable.set_cmap(
+                plotter.cmap.get_cmap(self.plotter.plot.array)
+            )
             plotter.cticks.colorbar = self.cbar
-            plotter.cticks.default_locator = \
+            plotter.cticks.default_locator = (
                 self.plotter.cticks.default_locator
+            )
             plotter.cticks.update_axis(plotter.cticks.value)
             self.draw()
 
         except Exception:
             self.mappable.set_norm(current_norm)
             self.mappable.set_cmap(current_cmap)
             self.cbar.locator = current_locator
@@ -812,31 +900,30 @@
         self.text_edit = QtWidgets.QTextEdit()
         self.text_edit.setVisible(False)
         layout.addWidget(self.text_edit)
 
         #: A tool button to switch from the single line editor :attr:`line_edit`
         #: to the multi-line editor :attr:`text_edit`
         self.btn_multiline = QtWidgets.QToolButton()
-        self.btn_multiline.setText('⌵')
+        self.btn_multiline.setText("⌵")
         self.btn_multiline.setCheckable(True)
         self.btn_multiline.setToolTip("Toggle multiline editor")
         self.btn_multiline.clicked.connect(self.toggle_multiline)
         layout.addWidget(self.btn_multiline)
 
         self.insert_obj(fmto.value)
 
         #: Value of the :attr:`fmto` at the initialization of this widget
         self.initial_value = self.line_edit.text()
 
         self.setLayout(layout)
 
     @property
     def changed(self) -> bool:
-        """Check if the value in this editor differs from the original `fmto`.
-        """
+        """Check if the value in this editor differs from the original `fmto`."""
         return self.fmto.diff(self.fmto.validate(self.get_obj()))
 
     def toggle_multiline(self) -> None:
         """Switch from :attr:`line_edit` and :attr:`text_edit` or back."""
         multiline = self.multiline
         self.text_edit.setVisible(multiline)
         self.line_edit.setVisible(not multiline)
@@ -849,16 +936,19 @@
     def multiline(self) -> bool:
         """True if the :attr:`text_edit` should be visible."""
         return self.btn_multiline.isChecked()
 
     @property
     def text(self) -> str:
         """Text of the :attr:`text_edit` (or :attr:`line_edit`)."""
-        return (self.text_edit.toPlainText() if self.multiline else
-                self.line_edit.text())
+        return (
+            self.text_edit.toPlainText()
+            if self.multiline
+            else self.line_edit.text()
+        )
 
     @text.setter
     def text(self, s: str) -> None:
         self.clear_text()
         if self.multiline:
             self.text_edit.insertPlainText(s)
         else:
@@ -911,20 +1001,20 @@
                 if current[0] in ['"', "'"]:
                     current = current[1:-1]
                 self.clear_text()
                 if pos == 0:
                     s = '"' + obj + current + '"'
                 else:
                     s = '"' + current + obj + '"'
-                current = ''
+                current = ""
         elif isinstance(obj, str):  # add quotation marks
             s = '"' + obj + '"'
         else:
             s = yaml.dump(obj, default_flow_style=True).strip()
-            if s.endswith('\n...'):
+            if s.endswith("\n..."):
                 s = s[:-4]
         if use_line_edit:
             self.line_edit.insert(s)
         else:
             self.text_edit.insertPlainText(s)
 
 
@@ -933,17 +1023,23 @@
 
     This class holds a :class:`FormatoptionsEditor` to control the
     appearance of a specific formatoption. Additionally it displays the
     formatoption specific line widget (see
     :meth:`psyplot.plotter.Formatoption.get_fmt_widget`) to contol it.
     """
 
-    def __init__(self, fmto: Formatoption, project: Project,
-                 fmto_widget: Type[QtWidgets.QWidget],
-                 widget_kws: Dict[str, Any] = {}, *args, **kwargs) -> None:
+    def __init__(
+        self,
+        fmto: Formatoption,
+        project: Project,
+        fmto_widget: Type[QtWidgets.QWidget],
+        widget_kws: Dict[str, Any] = {},
+        *args,
+        **kwargs,
+    ) -> None:
         """
         Parameters
         ----------
         fmto: psyplot.plotter.Formatoption
             The formatoption to manipulate
         project: psyplot.project.Project
             The project to use to fill this formatoption
@@ -952,19 +1048,18 @@
             the formatoption. This class is commonly used in the
             :meth:`psyplot.plotter.Formatoption.get_fmt_widget` of the given
             `fmto`
         widget_kws: dict
             Further keywords that are passed to the creation of the
             `fmto_widget` instance.
         """
-        super().__init__(f'{fmto.name} ({fmto.key})', *args, **kwargs)
+        super().__init__(f"{fmto.name} ({fmto.key})", *args, **kwargs)
         self.editor = FormatoptionsEditor(fmto)
         vbox = QtWidgets.QVBoxLayout()
-        vbox.addWidget(
-            fmto_widget(self.editor, fmto, project, **widget_kws))
+        vbox.addWidget(fmto_widget(self.editor, fmto, project, **widget_kws))
         vbox.addWidget(self.editor)
         self.setLayout(vbox)
 
 
 class LabelDialog(QtWidgets.QDialog):
     """A dialog to change labels.
 
@@ -978,45 +1073,50 @@
             The psyplot project to update. Note that we will only use the
             very first plotter in this project
         ``*fmts``
             The formatoption keys to display. Each formatoption should be a
             subclass of :class:`psy_simple.base.TextBase`
         """
         from psy_simple.widgets.texts import LabelWidget
+
         super().__init__()
         self.project = project
         layout = QtWidgets.QVBoxLayout()
         plotter = project.plotters[0]
         self.fmt_widgets = {}
         for fmt in fmts:
             fmto = getattr(plotter, fmt)
             fmt_widget = LabelWidgetLine(
-                fmto, project, LabelWidget, widget_kws=dict(properties=False))
+                fmto, project, LabelWidget, widget_kws=dict(properties=False)
+            )
             self.fmt_widgets[fmt] = fmt_widget
             layout.addWidget(fmt_widget)
 
         self.button_box = QtWidgets.QDialogButtonBox(
             QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel,
-            self)
+            self,
+        )
         self.button_box.accepted.connect(self.accept)
         self.button_box.rejected.connect(self.reject)
         layout.addWidget(self.button_box)
         self.setLayout(layout)
 
     @property
     def fmts(self) -> Dict[str, Any]:
         """Mapping from formatoption key to value in this dialog."""
         ret = {}
         for fmt, widget in self.fmt_widgets.items():
             if widget.editor.changed:
                 try:
                     value = widget.editor.value
                 except Exception:
-                    raise IOError(f"{fmt}-value {widget.editor.text} could "
-                                  "not be parsed to python!")
+                    raise IOError(
+                        f"{fmt}-value {widget.editor.text} could "
+                        "not be parsed to python!"
+                    )
                 else:
                     ret[fmt] = value
         return ret
 
     @classmethod
     def update_project(cls, project: Project, *fmts: str) -> None:
         """Create a :class:`LabelDialog` to update the labels in a `project`.
@@ -1036,9 +1136,8 @@
         """
         dialog = cls(project, *fmts)
         dialog.show()
         dialog.raise_()
         dialog.activateWindow()
         dialog.exec_()
         if dialog.result() == QtWidgets.QDialog.Accepted:
-            project.update(
-                **dialog.fmts)
+            project.update(**dialog.fmts)
```

### Comparing `psy-view-0.2.0/psy_view/ds_widget.py` & `psy-view-0.3.0/psy_view/ds_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,80 +1,63 @@
 # -*- coding: utf-8 -*-
 """Dataset widget to display the contents of a dataset."""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-#
-# This file is part of psy-view and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
 from __future__ import annotations
 
-import os.path as osp
+import contextlib
 import os
-
+import os.path as osp
 from typing import (
-    List,
     TYPE_CHECKING,
-    Optional,
-    Union,
-    Dict,
-    Iterator,
-    Type,
     Any,
     Callable,
+    Dict,
     Hashable,
+    Iterator,
+    List,
+    Optional,
     Tuple,
+    Union,
 )
 
-import contextlib
-
+import psyplot.data as psyd
 import yaml
-from PyQt5 import QtWidgets, QtGui
+from matplotlib.animation import FuncAnimation
+from psyplot.config.rcsetup import get_configdir
+from psyplot_gui.common import DockMixin, PyErrorMessage
+from psyplot_gui.common import get_icon as get_psy_icon
+from psyplot_gui.content_widget import (
+    DatasetTree,
+    DatasetTreeItem,
+    escape_html,
+)
+from PyQt5 import QtGui, QtWidgets
 from PyQt5.QtCore import Qt  # pylint: disable=no-name-in-module
+
 import psy_view.utils as utils
-from psyplot_gui.content_widget import (
-    DatasetTree, DatasetTreeItem, escape_html)
-from psyplot_gui.common import (
-    DockMixin, get_icon as get_psy_icon, PyErrorMessage)
-import psyplot.data as psyd
-from psy_view.rcsetup import rcParams
 from psy_view.plotmethods import (
-    PlotMethodWidget,
+    LinePlotWidget,
     MapPlotWidget,
     Plot2DWidget,
-    LinePlotWidget,
+    PlotMethodWidget,
 )
-from psyplot.config.rcsetup import get_configdir
-
-from matplotlib.animation import FuncAnimation
+from psy_view.rcsetup import rcParams
 
 if TYPE_CHECKING:
-    from xarray import DataArray, Dataset
-    from psyplot.project import PlotterInterface, Project
-    from psyplot.plotter import Plotter
-    from matplotlib.figure import Figure
     from matplotlib.backend_bases import MouseEvent
+    from matplotlib.figure import Figure
+    from psyplot.plotter import Plotter
+    from psyplot.project import PlotterInterface, Project
     from psyplot_gui.main import MainWindow
+    from xarray import DataArray, Dataset
 
 
 NOTSET = "__NOVARIABLEAVAILABLE"
 
 
 def get_dims_to_iterate(arr: DataArray) -> List[str]:
     """Get the dimensions of an array to iterate over
@@ -89,16 +72,20 @@
 
     Returns
     -------
     list of strings
         The dimension strings
     """
     base_var = next(arr.psy.iter_base_variables)
-    return [dim for dim, size in zip(base_var.dims, base_var.shape)
-            if size > 1 and arr[dim].ndim == 0]
+    return [
+        dim
+        for dim, size in zip(base_var.dims, base_var.shape)
+        if size > 1 and arr[dim].ndim == 0
+    ]
+
 
 TOO_MANY_FIGURES_WARNING = """
 Multiple figures are open but you specified only {} filenames: {}.<br>
 
 Saving the figures will cause that not all images are saved! We recommend to
 export to a single PDF (that then includes multiple pages), or modify your
 filename with strings like
@@ -115,15 +102,15 @@
 """
 
 
 class DatasetWidget(QtWidgets.QSplitter):
     """A widget to control the visualization of the variables in a dataset"""
 
     #: The title of the widget
-    title: str = 'psy-view Plot Control'
+    title: str = "psy-view Plot Control"
 
     #: Display the dock widget at the right side of the GUI
     dock_position = Qt.RightDockWidgetArea
 
     _animating: bool = False
 
     _ani: Optional[FuncAnimation] = None
@@ -137,15 +124,15 @@
     variable_buttons: Dict[str, QtWidgets.QPushButton]
 
     _new_plot: bool = False
 
     _preset: Optional[Union[str, Dict]] = None
 
     #: Attributes to use in the dataset tree
-    ds_attr_columns: List[str] = ['long_name', 'dims', 'shape']
+    ds_attr_columns: List[str] = ["long_name", "dims", "shape"]
 
     def __init__(self, ds: Optional[Dataset] = None, *args, **kwargs) -> None:
         """
         Parameters
         ----------
         ds: xarray.Dataset
             A dataset to visualize with this widget
@@ -163,21 +150,24 @@
         self.error_msg = PyErrorMessage(self)
 
         # first row: dataset name
         self.open_box = QtWidgets.QHBoxLayout()
         self.lbl_ds = QtWidgets.QLineEdit()
         self.open_box.addWidget(self.lbl_ds)
         self.btn_open = utils.add_pushbutton(
-            get_psy_icon('run_arrow.png'), lambda: self.set_dataset(),
-            "Select and open a netCDF dataset", self.open_box, icon=True)
+            get_psy_icon("run_arrow.png"),
+            lambda: self.set_dataset(),
+            "Select and open a netCDF dataset",
+            self.open_box,
+            icon=True,
+        )
         self.open_widget = QtWidgets.QWidget()
         self.open_widget.setLayout(self.open_box)
         self.addWidget(self.open_widget)
 
-
         # second row: dataset representation
         self.setup_ds_tree()
         if ds is not None:
             self.add_ds_item()
 
         self.ds_tree.itemExpanded.connect(self.change_ds)
         self.ds_tree.itemExpanded.connect(self.load_variable_desc)
@@ -185,119 +175,145 @@
         self.addWidget(self.ds_tree)
 
         # third row, navigation
         self.navigation_box = QtWidgets.QHBoxLayout()
 
         # -- animate backwards button
         self.btn_animate_backward = utils.add_pushbutton(
-            "◀◀", lambda: self.animate_backward(),
-            "Animate the time dimension backwards", self.navigation_box)
+            "◀◀",
+            lambda: self.animate_backward(),
+            "Animate the time dimension backwards",
+            self.navigation_box,
+        )
         self.btn_animate_backward.setCheckable(True)
 
         # -- go to previous button
         self.btn_prev = utils.add_pushbutton(
-            '◀', self.go_to_previous_step,
-            "Go to previous time step", self.navigation_box)
+            "◀",
+            self.go_to_previous_step,
+            "Go to previous time step",
+            self.navigation_box,
+        )
 
         # -- dimension menu for animation
         self.combo_dims = QtWidgets.QComboBox()
         self.navigation_box.addWidget(self.combo_dims)
 
         # -- go to next button
         self.btn_next = utils.add_pushbutton(
-            '▶', self.go_to_next_step,
-            "Go to next time step", self.navigation_box)
+            "▶",
+            self.go_to_next_step,
+            "Go to next time step",
+            self.navigation_box,
+        )
 
         # -- animate forward button
         self.btn_animate_forward = utils.add_pushbutton(
-            "▶▶", lambda: self.animate_forward(),
-            "Animate the time dimension", self.navigation_box)
+            "▶▶",
+            lambda: self.animate_forward(),
+            "Animate the time dimension",
+            self.navigation_box,
+        )
         self.btn_animate_forward.setCheckable(True)
 
         # -- interval slider
         self.sl_interval = QtWidgets.QSlider(Qt.Horizontal)
         self.sl_interval.setMinimum(40)  # 24 fps
         self.sl_interval.setMaximum(10000)
         self.sl_interval.setSingleStep(50)
         self.sl_interval.setPageStep(500)
         self.sl_interval.setValue(500)
         self.sl_interval.valueChanged.connect(self.reset_timer_interval)
         self.navigation_box.addWidget(self.sl_interval)
 
         # -- interval label
-        self.lbl_interval = QtWidgets.QLabel('500 ms')
+        self.lbl_interval = QtWidgets.QLabel("500 ms")
         self.navigation_box.addWidget(self.lbl_interval)
 
         # --- export/import menus
         self.export_box = QtWidgets.QHBoxLayout()
 
         # -- Export button
         self.btn_export = QtWidgets.QToolButton()
-        self.btn_export.setText('Export')
+        self.btn_export.setText("Export")
         self.btn_export.setPopupMode(QtWidgets.QToolButton.InstantPopup)
         self.btn_export.setMenu(self.setup_export_menu())
         self.btn_export.setEnabled(False)
         self.export_box.addWidget(self.btn_export)
 
         # --- Presets button
         self.frm_preset = QtWidgets.QFrame()
         self.frm_preset.setFrameStyle(QtWidgets.QFrame.StyledPanel)
         hbox = QtWidgets.QHBoxLayout(self.frm_preset)
 
         self.btn_preset = QtWidgets.QToolButton()
-        self.btn_preset.setText('Preset')
+        self.btn_preset.setText("Preset")
         self.btn_preset.setPopupMode(QtWidgets.QToolButton.InstantPopup)
         self.btn_preset.setMenu(self.setup_preset_menu())
         hbox.addWidget(self.btn_preset)
 
         # --- presets label
-        self.lbl_preset = QtWidgets.QLabel('')
+        self.lbl_preset = QtWidgets.QLabel("")
         self.lbl_preset.setVisible(False)
         hbox.addWidget(self.lbl_preset)
 
         # --- unset preset button
         self.btn_unset_preset = utils.add_pushbutton(
-            get_psy_icon('invalid.png'), self.unset_preset,
-            "Unset the current preset", hbox, icon=True)
+            get_psy_icon("invalid.png"),
+            self.unset_preset,
+            "Unset the current preset",
+            hbox,
+            icon=True,
+        )
         self.btn_unset_preset.setVisible(False)
 
         self.export_box.addWidget(self.frm_preset)
 
         self.btn_reload = utils.add_pushbutton(
-            get_psy_icon("refresh.png"), self.reload,
+            get_psy_icon("refresh.png"),
+            self.reload,
             "Close all open datasets and recreate the plots",
-            self.export_box, icon=True
+            self.export_box,
+            icon=True,
         )
 
         self.export_box.addStretch(0)
 
         vbox = QtWidgets.QVBoxLayout()
         vbox.addLayout(self.navigation_box)
         vbox.addLayout(self.export_box)
 
         self.addLayout(vbox)
 
         # fourth row: array selector
 
-        self.array_frame = QtWidgets.QGroupBox('Current plot')
+        self.array_frame = QtWidgets.QGroupBox("Current plot")
         hbox = QtWidgets.QHBoxLayout()
 
         self.combo_array = QtWidgets.QComboBox()
         self.combo_array.setEditable(False)
         self.combo_array.currentIndexChanged.connect(lambda: self.refresh())
         self.combo_array.currentIndexChanged.connect(self.show_current_figure)
         hbox.addWidget(self.combo_array)
 
         self.btn_add = utils.add_pushbutton(
-            QtGui.QIcon(get_psy_icon('plus')), self.new_plot,
-            "Create a new plot", hbox, icon=True)
+            QtGui.QIcon(get_psy_icon("plus")),
+            self.new_plot,
+            "Create a new plot",
+            hbox,
+            icon=True,
+        )
         self.btn_add.setEnabled(ds is not None)
         self.btn_del = utils.add_pushbutton(
-            QtGui.QIcon(get_psy_icon('minus')), self.close_current_plot,
-            "Remove the current plot", hbox, icon=True)
+            QtGui.QIcon(get_psy_icon("minus")),
+            self.close_current_plot,
+            "Remove the current plot",
+            hbox,
+            icon=True,
+        )
         self.btn_del.setEnabled(False)
 
         hbox.addWidget(self.btn_add)
         hbox.addWidget(self.btn_del)
         self.array_frame.setLayout(hbox)
         self.addWidget(self.array_frame)
 
@@ -326,14 +342,16 @@
         self.cids: Dict[str, int] = {}
 
     def reload(self) -> None:
         """Close the plot and recreate it."""
         import psyplot.project as psy
 
         sp = self._sp
+        if sp is None:
+            return
         fname = sp.dsnames_map[self.ds.psy.num]  # type: ignore
         project = sp.save_project()
         sp.close(True, True, True)
         self.ds_tree.clear()
         self._ds_nums.clear()
         self.refresh()
         self._sp = sp = psy.Project.load_project(project)
@@ -345,15 +363,15 @@
         sp.show()
         self.refresh()
 
     def setup_ds_tree(self) -> None:
         """Setup the number of columns and the header of the dataset tree."""
         self.ds_tree = tree = QtWidgets.QTreeWidget()
         tree.setColumnCount(len(self.ds_attr_columns) + 1)
-        tree.setHeaderLabels([''] + self.ds_attr_columns)
+        tree.setHeaderLabels([""] + self.ds_attr_columns)
 
     def showEvent(self, event):
         ret = super().showEvent(event)
         current_size = self.size()
         current_sizes = self.sizes()
 
         itree = self.indexOf(self.ds_tree)
@@ -380,15 +398,15 @@
 
     @property
     def arr_name(self) -> Optional[str]:
         """Get the name of the array of the current plot (if there is one)."""
         if not self.combo_array.count():
             return None
         else:
-            return self.combo_array.currentText().split(':')[0]
+            return self.combo_array.currentText().split(":")[0]
 
     def change_ds(self, ds_item: DatasetTreeItem) -> None:
         """Change the current dataset to another one.
 
         Parameters
         ----------
         ds_item: psyplot_gui.content_widget.DatasetTreeItem
@@ -434,19 +452,21 @@
             The :class:`xarray.Dataset` of the selected file, or None if the
             user aborted the dialog.
         """
         current = self.lbl_ds.text()
         if not current or not osp.exists(current):
             current = os.getcwd()
         fname, ok = QtWidgets.QFileDialog.getOpenFileName(
-            self, 'Open dataset', current,
-            'NetCDF files (*.nc *.nc4);;'
-            'Shape files (*.shp);;'
-            'All files (*)'
-            )
+            self,
+            "Open dataset",
+            current,
+            "NetCDF files (*.nc *.nc4);;"
+            "Shape files (*.shp);;"
+            "All files (*)",
+        )
         if not ok:
             return None
         ds = psyd.open_dataset(fname)
         return ds
 
     @contextlib.contextmanager
     def block_tree(self) -> Iterator[None]:
@@ -483,28 +503,27 @@
         tree = self.ds_tree
         ds_item = DatasetTreeItem(ds, self.ds_attr_columns, 0)
         fname = psyd.get_filename_ds(ds, False)[0]
         if fname is not None:
             self.lbl_ds.setText(fname)
             fname = osp.basename(fname)
         else:
-            self.lbl_ds.setText('')
-            fname = ''
+            self.lbl_ds.setText("")
+            fname = ""
         ds_item.setText(0, fname)
         tree.addTopLevelItem(ds_item)
 
         self.expand_ds_item(ds_item)
 
         tree.resizeColumnToContents(0)
 
         if ds.psy.num not in self.open_datasets:
             # make sure we do not loose track of open datasets
             self._ds_nums[ds.psy.num] = ds
 
-
     @property
     def open_datasets(self) -> Dict[int, Dataset]:
         """Get a mapping from path to dataset number of the open datasets."""
         return self._ds_nums
 
     @property
     def ds_items(self) -> List[DatasetTreeItem]:
@@ -518,98 +537,107 @@
         ds = self.ds
         for item in self.ds_items:
             if item.ds() is ds:
                 return item
         return None
 
     def expand_current_variable(
-            self, variable: Optional[Union[Any, Hashable]] = None) -> None:
+        self, variable: Optional[Union[Any, Hashable]] = None
+    ) -> None:
         """Expand the item in the dataset tree of variable.
 
         Parameters
         ----------
         variable: str
             The name of the variable to expand. If None, the current variable is
             used.
         """
         tree = self.ds_tree
         top: DatasetTreeItem = self.ds_item  # type: ignore
         tree.expandItem(top)
         tree.expandItem(top.child(0))
         if variable is None:
             variable: str = self.variable  # type: ignore
-        for var_item in map(top.child(0).child,
-                            range(top.child(0).childCount())):
+        for var_item in map(
+            top.child(0).child, range(top.child(0).childCount())
+        ):
             if var_item.text(0) == variable:
                 tree.expandItem(var_item)
             else:
                 tree.collapseItem(var_item)
 
     def setup_variable_buttons(self, ncols: int = 4) -> None:
         """Setup the variable buttons for the current dataset."""
-        variable_frame = QtWidgets.QGroupBox('Variables')
+        variable_frame = QtWidgets.QGroupBox("Variables")
 
         self.variable_scroll.setWidget(variable_frame)
         self.variable_frame = variable_frame
         self.variable_layout = QtWidgets.QGridLayout(self.variable_frame)
         self.variable_buttons = {}
 
         ds = self.ds
 
         if ds is not None:
-
             for i, v in enumerate(ds):
                 btn = utils.add_pushbutton(
-                    v, self._draw_variable(v), f"Visualize variable {v}")
+                    v, self._draw_variable(v), f"Visualize variable {v}"
+                )
                 btn.setCheckable(True)
                 self.variable_buttons[v] = btn
                 self.variable_layout.addWidget(btn, i // ncols, i % ncols)
 
             if len(ds):
                 rows = len(ds) // ncols
                 minrows = max(1, min(3, rows))
                 self.variable_scroll.setMinimumHeight(
-                        (minrows + 2) * btn.sizeHint().height())
+                    (minrows + 2) * btn.sizeHint().height()
+                )
 
     def load_variable_desc(self, item: QtWidgets.QTreeWidgetItem) -> None:
         """Load the description of the variable of a given tree item.
 
         Parameters
         ----------
         item: PyQt5.QtWidget.QTreeWidgetItem
             The item of the variable in the :attr:`ds_tree`. If this is not an
             item of a variable, nothing is done.
         """
         parent = item.parent()
 
         tree = self.ds_tree
 
-        if parent is tree or parent is None or not (
-                DatasetTree.is_variable(item) or DatasetTree.is_coord(item)):
+        if (
+            parent is tree
+            or parent is None
+            or not (
+                DatasetTree.is_variable(item) or DatasetTree.is_coord(item)
+            )
+        ):
             return
 
         if tree.isColumnHidden(1):
             tree.showColumn(1)
             tree.resizeColumnToContents(0)
 
         top = item
         while top.parent() and top.parent() is not self:
             top = top.parent()
         ds = top.ds()
         if ds is None:
             return
         desc = escape_html(str(ds.variables[item.text(0)]))
-        item.setToolTip(0, '<pre>' + desc + '</pre>')
+        item.setToolTip(0, "<pre>" + desc + "</pre>")
 
     def clear_table(self) -> None:
         """Clear the table that shows the available dimensions."""
         self.dimension_table.clear()
         self.dimension_table.setColumnCount(5)
         self.dimension_table.setHorizontalHeaderLabels(
-            ['Type', 'First', 'Current', 'Last', 'Units'])
+            ["Type", "First", "Current", "Last", "Units"]
+        )
         self.dimension_table.setRowCount(0)
 
     def addLayout(self, layout: QtWidgets.QLayout) -> QtWidgets.QWidget:
         """Add a layout to the splitter.
 
         This convenience function creates a new QWidget that wraps the given
         layout and returns it.
@@ -639,42 +667,40 @@
         dim = self.combo_dims.currentText()
         self.increase_dim(dim)()
 
     def animate_backward(self) -> None:
         """Start the current animation in backward direction, or stop it."""
         if self._animating:
             self.stop_animation()
-            self.btn_animate_backward.setText('◀◀')
+            self.btn_animate_backward.setText("◀◀")
             self.enable_navigation()
         else:
             self._animate_forward = False
-            self.btn_animate_backward.setText('■')
+            self.btn_animate_backward.setText("■")
             self.disable_navigation(self.btn_animate_backward)
             self.start_animation()
 
     def animate_forward(self, nframes=None):
         """Start the current animation in forward direction, or stop it."""
         if self._animating:
             self.stop_animation()
-            self.btn_animate_forward.setText('▶▶')
+            self.btn_animate_forward.setText("▶▶")
             self.enable_navigation()
         else:
             self._animate_forward = True
-            self.btn_animate_forward.setText('■')
+            self.btn_animate_forward.setText("■")
             self.disable_navigation(self.btn_animate_forward)
             self.start_animation(nframes)
 
     def setup_plot_tabs(self) -> None:
         """Setup the tabs of the various plot methods."""
-        self.plot_tabs.addTab(MapPlotWidget(self.get_sp, self.ds),
-                              'mapplot')
-        self.plot_tabs.addTab(Plot2DWidget(self.get_sp, self.ds),
-                              'plot2d')
+        self.plot_tabs.addTab(MapPlotWidget(self.get_sp, self.ds), "mapplot")
+        self.plot_tabs.addTab(Plot2DWidget(self.get_sp, self.ds), "plot2d")
         lineplot_widget = LinePlotWidget(self.get_sp, self.ds)
-        self.plot_tabs.addTab(lineplot_widget, 'lineplot')
+        self.plot_tabs.addTab(lineplot_widget, "lineplot")
 
         for w in map(self.plot_tabs.widget, range(self.plot_tabs.count())):
             w.replot.connect(self.replot)
             w.reset.connect(self.reset)
             w.changed.connect(lambda: self.refresh())
 
     def replot(self, plotmethod: str) -> None:
@@ -709,35 +735,37 @@
         """
         self.plotmethod = plotmethod
         self.close_sp()
         self.make_plot()
         self.refresh()
 
     def disable_navigation(
-            self, but: Optional[QtWidgets.QPushButton] = None
-        ) -> None:
+        self, but: Optional[QtWidgets.QPushButton] = None
+    ) -> None:
         """Disable the navigation buttons.
 
         This function disables all navigation buttons but the one you specify.
 
         Parameters
         ----------
         but: PyQt5.QtWidgets.QPushButton
             If not None, this button is not disabled.
         """
-        for item in map(self.navigation_box.itemAt,
-                        range(self.navigation_box.count())):
+        for item in map(
+            self.navigation_box.itemAt, range(self.navigation_box.count())
+        ):
             w = item.widget()
             if w is not but and w is not self.sl_interval:
                 w.setEnabled(False)
 
     def enable_navigation(self) -> None:
         """Enable all navigation buttons again."""
-        for item in map(self.navigation_box.itemAt,
-                        range(self.navigation_box.count())):
+        for item in map(
+            self.navigation_box.itemAt, range(self.navigation_box.count())
+        ):
             w = item.widget()
             w.setEnabled(True)
 
     def disable_variables(self):
         """Disable all variable selection buttons."""
         for btn in self.variable_buttons.values():
             btn.setEnabled(False)
@@ -764,48 +792,57 @@
         self._animation_frames = nframes
         self._starting_step = 1
         self.disable_variables()
         self.plot_tabs.setEnabled(False)
         if self.sp is not None:
             if self.animation is None or self.animation.event_source is None:
                 self.animation = FuncAnimation(
-                    self.fig, self.update_dims, frames=self.animation_frames(),
-                    init_func=self.sp.draw, interval=self.sl_interval.value(),
-                    repeat=False)
+                    self.fig,
+                    self.update_dims,
+                    frames=self.animation_frames(),
+                    init_func=self.sp.draw,
+                    interval=self.sl_interval.value(),
+                    repeat=False,
+                )
                 # HACK: Make sure that the animation starts although the figure
                 # is already shown
                 self.animation._draw_frame(next(self.animation_frames()))
             else:
                 self.animation.event_source.start()
 
     def reset_timer_interval(self, value: int) -> None:
         """Change the interval of the timer."""
-        self.lbl_interval.setText('%i ms' % value)
+        self.lbl_interval.setText("%i ms" % value)
         if self.animation is None or self.animation.event_source is None:
             pass
         else:
             self.animation.event_source.stop()
             self.animation._interval = value
             self.animation.event_source.interval = value
             self.animation.event_source.start()
 
     def stop_animation(self) -> None:
         """Stop the current animation."""
         self._animating = False
-        if (self.animation is not None and
-                self.animation.event_source is not None):
+        if (
+            self.animation is not None
+            and self.animation.event_source is not None
+        ):
             self.animation.event_source.stop()
         self.plot_tabs.setEnabled(True)
         self.enable_variables()
         self.refresh()
 
     def animation_frames(self) -> Iterator[Dict[str, int]]:
         """Get the animation frames for the :attr:`combo_dims` dimension."""
-        while self._animating and self._animation_frames is None or \
-                self._animation_frames:
+        while (
+            self._animating
+            and self._animation_frames is None
+            or self._animation_frames
+        ):
             if self._animation_frames is not None and not self._init_step:
                 self._animation_frames -= 1
             dim = self.combo_dims.currentText()
             i = self.data.psy.idims[dim]
             imax = self.ds.dims[dim] - 1  # type: ignore
             if self._init_step:
                 self._init_step -= 1
@@ -820,17 +857,19 @@
     def update_dims(self, dims: Dict[str, Any]):
         if self.sp is not None:
             self.sp.update(dims=dims)
 
     def _load_preset(self) -> None:
         """Open a file dialog and load the selected preset."""
         fname, ok = QtWidgets.QFileDialog.getOpenFileName(
-            self, 'Load preset', osp.join(get_configdir(), 'presets'),
-            'YAML files (*.yml *.yaml);;'
-            'All files (*)')
+            self,
+            "Load preset",
+            osp.join(get_configdir(), "presets"),
+            "YAML files (*.yml *.yaml);;" "All files (*)",
+        )
         if ok:
             self.load_preset(fname)
 
     def load_preset(self, preset: Optional[Union[str, Dict[str, Any]]]):
         """Load a given preset from disk.
 
         Parameters
@@ -848,49 +887,53 @@
 
     @property
     def preset(self) -> Dict[str, Any]:
         """Get the currently loaded preset."""
         if self._preset is None:
             return {}
         import psyplot.project as psy
+
         preset = self._preset
         try:
             preset = psy.Project._load_preset(preset)
         except yaml.constructor.ConstructorError:
             answer = QtWidgets.QMessageBox.question(
-                self, "Can I trust this?",
+                self,
+                "Can I trust this?",
                 f"Failed to load the preset at <i>{preset}</i> in safe mode. Can we "
-                "trust this preset and load it in unsafe mode?")
+                "trust this preset and load it in unsafe mode?",
+            )
             if answer == QtWidgets.QMessageBox.Yes:
-                psyd.rcParams['presets.trusted'].append(
-                    psy.Project._resolve_preset_path(preset))
+                psyd.rcParams["presets.trusted"].append(
+                    psy.Project._resolve_preset_path(preset)
+                )
                 preset = psy.Project._load_preset(preset)
             else:
                 preset = {}
         return preset  # type: ignore
 
     @preset.setter
     def preset(self, value: Optional[Union[str, Dict[str, Any]]]):
         self._preset = value
 
-
     def unset_preset(self) -> None:
         """Unset the current preset and do not use it anymore."""
         self.preset = None  # type: ignore
         self.maybe_show_preset()
 
     def maybe_show_preset(self) -> None:
         """Show the name of the current preset if one is selected."""
         if self._preset is not None and isinstance(self._preset, str):
-            self.lbl_preset.setText('<i>' +
-                osp.basename(osp.splitext(self._preset)[0]) + '</i>')
+            self.lbl_preset.setText(
+                "<i>" + osp.basename(osp.splitext(self._preset)[0]) + "</i>"
+            )
             self.lbl_preset.setVisible(True)
             self.btn_unset_preset.setVisible(True)
         elif self._preset is not None:
-            self.lbl_preset.setText('<i>custom</i>')
+            self.lbl_preset.setText("<i>custom</i>")
             self.lbl_preset.setVisible(True)
             self.btn_unset_preset.setVisible(True)
         else:
             self.lbl_preset.setVisible(False)
             self.btn_unset_preset.setVisible(False)
 
     def save_current_preset(self) -> None:
@@ -912,123 +955,145 @@
         Parameters
         ----------
         save_func: function
             The function that is called to save the preset. Must accept the
             path as an argument
         """
         fname, ok = QtWidgets.QFileDialog.getSaveFileName(
-            self, 'Save preset', osp.join(get_configdir(), 'presets'),
-            'YAML files (*.yml *.yaml);;'
-            'All files (*)')
+            self,
+            "Save preset",
+            osp.join(get_configdir(), "presets"),
+            "YAML files (*.yml *.yaml);;" "All files (*)",
+        )
         if not ok:
             return None
         save_func(fname)
 
     def setup_preset_menu(self) -> QtWidgets.QMenu:
         """Set up the menu to select/load presets."""
         self.preset_menu = menu = QtWidgets.QMenu()
         self._save_preset_actions = []
 
         self._load_preset_action = menu.addAction(
-            "Load preset", self._load_preset)
+            "Load preset", self._load_preset
+        )
         self._unset_preset_action = menu.addAction(
-            "Unset preset", self.unset_preset)
+            "Unset preset", self.unset_preset
+        )
 
         menu.addSeparator()
 
         self._save_preset_actions.append(
-            menu.addAction('Save format of current plot as preset',
-                           self.save_current_preset))
+            menu.addAction(
+                "Save format of current plot as preset",
+                self.save_current_preset,
+            )
+        )
         self._save_preset_actions.append(
-            menu.addAction('Save format of all plots as preset',
-                           self.save_full_preset))
+            menu.addAction(
+                "Save format of all plots as preset", self.save_full_preset
+            )
+        )
 
         for action in self._save_preset_actions:
             action.setEnabled(False)
 
         return menu
 
     def setup_export_menu(self) -> QtWidgets.QMenu:
         """Set up the menu to export the current plot."""
         self.export_menu = menu = QtWidgets.QMenu()
-        menu.addAction('image (PDF, PNG, etc.)', self.export_image)
-        menu.addAction('all images (PDF, PNG, etc.)', self.export_all_images)
-        menu.addAction('animation (GIF, MP4, etc.', self.export_animation)
-        menu.addAction('psyplot project (.pkl file)', self.export_project)
-        menu.addAction('psyplot project with data',
-                       self.export_project_with_data)
-        py_action = menu.addAction('python script (.py)', self.export_python)
+        menu.addAction("image (PDF, PNG, etc.)", self.export_image)
+        menu.addAction("all images (PDF, PNG, etc.)", self.export_all_images)
+        menu.addAction("animation (GIF, MP4, etc.", self.export_animation)
+        menu.addAction("psyplot project (.pkl file)", self.export_project)
+        menu.addAction(
+            "psyplot project with data", self.export_project_with_data
+        )
+        py_action = menu.addAction("python script (.py)", self.export_python)
         py_action.setEnabled(False)  # psyplot does not yet export to python
         return menu
 
     def export_image(self) -> None:
         """Ask for a filename and export the current plot to a file."""
         if self.sp is not None:
             fname, ok = QtWidgets.QFileDialog.getSaveFileName(
-                self, "Export image", os.getcwd(),
-                "Images (*.png *.pdf *.jpg *.svg)")
+                self,
+                "Export image",
+                os.getcwd(),
+                "Images (*.png *.pdf *.jpg *.svg)",
+            )
             if ok:
-                self.sp.export(fname, **rcParams['savefig_kws'])
+                self.sp.export(fname, **rcParams["savefig_kws"])
 
     def export_all_images(self) -> None:
         """Ask for a filename and export all plots to one (or more) files."""
         fname, ok = QtWidgets.QFileDialog.getSaveFileName(
-            self, "Export image", os.getcwd(),
-            "Images (*.png *.pdf *.jpg *.svg)")
+            self,
+            "Export image",
+            os.getcwd(),
+            "Images (*.png *.pdf *.jpg *.svg)",
+        )
         if ok and self._sp:
             # test filenames
-            if not osp.splitext(fname)[-1].lower() == '.pdf':
+            if not osp.splitext(fname)[-1].lower() == ".pdf":
                 fnames = [
                     sp.format_string(fname, False, i)
-                    for i, sp in enumerate(self._sp.figs.values())]
+                    for i, sp in enumerate(self._sp.figs.values())
+                ]
                 if len(fnames) != len(set(fnames)):
                     answer = QtWidgets.QMessageBox.question(
-                        self, "Too many figures",
+                        self,
+                        "Too many figures",
                         TOO_MANY_FIGURES_WARNING.format(
-                            len(set(fnames)), ', '.join(set(fnames))))
+                            len(set(fnames)), ", ".join(set(fnames))
+                        ),
+                    )
                     if answer == QtWidgets.QMessageBox.No:
                         return
-            self._sp.export(fname, **rcParams['savefig_kws'])
+            self._sp.export(fname, **rcParams["savefig_kws"])
 
     def export_animation(self) -> None:
         """Ask for a filename and export the animation."""
         fname, ok = QtWidgets.QFileDialog.getSaveFileName(
-            self, "Export animation", os.getcwd(),
-            "Movie (*.mp4 *.mov *.gif)")
+            self, "Export animation", os.getcwd(), "Movie (*.mp4 *.mov *.gif)"
+        )
         if ok:
             dim = self.combo_dims.currentText()
             nframes: int = self.ds.dims[dim]  # type: ignore
 
             self._init_step = 1
             self.animate_forward(nframes)
             if self.animation is not None:
                 self.animation.save(
-                    fname, **rcParams['animations.export_kws'],
-                    fps=round(1000. / self.sl_interval.value()))
+                    fname,
+                    **rcParams["animations.export_kws"],
+                    fps=round(1000.0 / self.sl_interval.value()),
+                )
             self.animate_forward()
             self.animation = None
 
     def export_project(self) -> None:
         """Ask for a filename and export the psyplot project as .pkl file."""
         if self.sp is not None:
             fname, ok = QtWidgets.QFileDialog.getSaveFileName(
-                self, "Export project", os.getcwd(),
-                "Psyplot projects (*.pkl)")
+                self, "Export project", os.getcwd(), "Psyplot projects (*.pkl)"
+            )
             if ok:
                 self.sp.save_project(fname)
 
     def export_project_with_data(self) -> None:
         """Ask for a filename export project (incl. data) as .pkl file.
 
         Same as :meth:`export_project`, but adds the data to the pickle dump.
         """
         if self.sp is not None:
             fname, ok = QtWidgets.QFileDialog.getSaveFileName(
-                self, "Export project", os.getcwd(),
-                "Psyplot projects (*.pkl)")
+                self, "Export project", os.getcwd(), "Psyplot projects (*.pkl)"
+            )
             if ok:
                 self.sp.save_project(fname, ds_description={"ds"})
 
     def export_python(self):
         """Export the project as python file.
 
         This method is not yet implemented as the functionality is missing in
@@ -1101,82 +1166,101 @@
     @property
     def plot(self) -> PlotterInterface:
         """Get the plotting function of the currently selected plotmethod."""
         if self.ds is not None:
             return getattr(self.ds.psy.plot, self.plotmethod)
         else:
             raise ValueError(
-                "No dataset has yet been selected, so no plot method!")
+                "No dataset has yet been selected, so no plot method!"
+            )
 
     @property
     def plot_options(self) -> Dict[str, Any]:
         """Get further keyword arguments for the :attr:`plot` function."""
         if self.ds is not None:
             ret: Dict[str, Any] = self.plotmethod_widget.get_fmts(  # type: ignore
-                self.ds.psy[self.variable], True)
+                self.ds.psy[self.variable], True
+            )
             preset = self.preset
             if preset:
                 import psyplot.project as psy
+
                 preset = psy.Project.extract_fmts_from_preset(
-                    preset, self.plotmethod)
+                    preset, self.plotmethod
+                )
                 ret.update(dict(preset))
             return ret
         return {}
 
     @property
     def plotmethod(self) -> str:
         """Get the name of the current plotmethod."""
         return self.plot_tabs.tabText(self.plot_tabs.currentIndex())
 
     @plotmethod.setter
     def plotmethod(self, label: str):
-        i = next((i for i in range(self.plot_tabs.count())
-                  if self.plot_tabs.tabText(i) == label), None)
+        i = next(
+            (
+                i
+                for i in range(self.plot_tabs.count())
+                if self.plot_tabs.tabText(i) == label
+            ),
+            None,
+        )
         if i is not None:
             self.plot_tabs.setCurrentIndex(i)
 
     @property
     def plotmethods(self) -> List[str]:
         """Get a list of available plotmethods."""
         return list(map(self.plot_tabs.tabText, range(self.plot_tabs.count())))
 
     @property
     def plotmethod_widget(self) -> PlotMethodWidget:
         """Get widget of the current plotmethod."""
         label = self.plotmethod
-        i = next((i for i in range(self.plot_tabs.count())
-                  if self.plot_tabs.tabText(i) == label), None)
+        i = next(
+            (
+                i
+                for i in range(self.plot_tabs.count())
+                if self.plot_tabs.tabText(i) == label
+            ),
+            None,
+        )
         return self.plot_tabs.widget(i)
 
     @property
     def plotmethod_widgets(self) -> Dict[str, PlotMethodWidget]:
         """Get a list of available plotmethod widgets."""
-        return dict(zip(self.plotmethods, map(self.plot_tabs.widget,
-                                              range(self.plot_tabs.count()))))
+        return dict(
+            zip(
+                self.plotmethods,
+                map(self.plot_tabs.widget, range(self.plot_tabs.count())),
+            )
+        )
 
     _sp = None
 
     def get_sp(self) -> Optional[Project]:
         sp = self._sp
         if sp is None:
             return sp
         return self.filter_sp(sp)
 
     def filter_sp(self, sp: Project, ds_only: bool = False) -> Project:
-        """Filter the psyplot project to only include the arrays of :attr:`ds`
-        """
+        """Filter the psyplot project to only include the arrays of :attr:`ds`"""
         if self._new_plot:
             return None
         if self.ds is None:
             return sp
         num = self.ds.psy.num
         ret = sp[:0]
         for i in range(len(sp)):
-            if list(sp[i:i+1].datasets) == [num]:
-                ret += sp[i:i+1]
+            if list(sp[i : i + 1].datasets) == [num]:
+                ret += sp[i : i + 1]
         if ds_only:
             return ret
         arr_name = self.arr_name
         if arr_name is None:
             return ret
         return ret(arr_name=arr_name)
 
@@ -1188,16 +1272,19 @@
 
         See Also
         --------
         make_plot: plot the currently selected variable without asking
         """
         if self.ds is not None:
             name, ok = QtWidgets.QInputDialog.getItem(
-                self, 'New plot', 'Select a variable',
-                self.plotmethod_widget.valid_variables(self.ds))
+                self,
+                "New plot",
+                "Select a variable",
+                self.plotmethod_widget.valid_variables(self.ds),
+            )
             if not ok:
                 return
             with self.silence_variable_buttons():
                 for v, btn in self.variable_buttons.items():
                     btn.setChecked(v == name)
             with self.creating_new_plot():
                 self.make_plot()
@@ -1214,16 +1301,17 @@
     @property
     def sp(self) -> Optional[Project]:
         """Get the psyplot project of the current plotmethod."""
         return self.plotmethod_widget.sp or None
 
     @sp.setter
     def sp(self, sp: Optional[Project]):
-        if sp is None and (not self._sp or not getattr(
-                self._sp, self.plotmethod)):
+        if sp is None and (
+            not self._sp or not getattr(self._sp, self.plotmethod)
+        ):
             pass
         else:
             # first remove the current arrays
             if self.get_sp() and getattr(self.get_sp(), self.plotmethod):
                 to_remove = getattr(self.get_sp(), self.plotmethod).arr_names
                 _sp: Project = self._sp  # type: ignore
                 for i in list(reversed(range(len(_sp)))):
@@ -1274,19 +1362,22 @@
         new_plot: A function to select the variable first
         """
         plotmethods = self.available_plotmethods
         plotmethod = self.plotmethod
         if plotmethod not in plotmethods:
             if not plotmethods:
                 QtWidgets.QMessageBox.critical(
-                    self, "Visualization impossible",
-                    f"Found no plotmethod for variable {self.variable}")
+                    self,
+                    "Visualization impossible",
+                    f"Found no plotmethod for variable {self.variable}",
+                )
                 return
             plotmethod, ok = QtWidgets.QInputDialog.getItem(
-                self, "Choose a plot method", "Plot method:", plotmethods)
+                self, "Choose a plot method", "Plot method:", plotmethods
+            )
             if not ok:
                 return
             self.plotmethod = plotmethod
         new_v = self.variable
         fmts: Dict[str, Any] = {}
         dims: Dict[Hashable, int] = {}
         if self.sp:
@@ -1307,15 +1398,16 @@
                 self.data.psy.update(name=self.variable, dims=dims, **fmts)
             self.show_fig(self.sp)
         else:
             self.ani = None
             self.sp = sp = self.plot(name=self.variable, **self.plot_options)
             self._preset = None
             cid = sp.plotters[0].ax.figure.canvas.mpl_connect(
-                'button_press_event', self.display_line)
+                "button_press_event", self.display_line
+            )
             self.cids[self.plotmethod] = cid
             self.show_fig(sp)
             descr = sp[0].psy._short_info()
             with self.block_widgets(self.combo_array):
                 self.combo_array.addItem(descr)
                 self.combo_array.setCurrentText(descr)
         self.expand_current_variable()
@@ -1332,50 +1424,55 @@
 
     def display_line(self, event: MouseEvent) -> None:
         """Display the line when clicked on a 2D-plot."""
         if not event.inaxes:
             return
         else:
             sl = None
-            for widget in map(self.plot_tabs.widget,
-                              range(self.plot_tabs.count())):
+            for widget in map(
+                self.plot_tabs.widget, range(self.plot_tabs.count())
+            ):
                 if widget.sp and event.inaxes == widget.plotter.ax:
                     sl = widget.get_slice(event.xdata, event.ydata)
                     break
             variable = widget.data.name
             raw_data = widget.data.psy.base.psy[variable]
-            if (sl is None or widget.plotmethod not in ['mapplot', 'plot2d'] or
-                raw_data.ndim == 2 or
-                widget.plotter.ax.figure.canvas.manager.toolbar.mode != ''):
+            if (
+                sl is None
+                or widget.plotmethod not in ["mapplot", "plot2d"]
+                or raw_data.ndim == 2
+                or widget.plotter.ax.figure.canvas.manager.toolbar.mode != ""
+            ):
                 return
             # check if the mappable contains the event
             if not self.plotter.plot.mappable.contains(event)[0] and (
-                    not hasattr(self.plotter.plot, '_wrapped_plot') or
-                    not self.plotter.plot._wrapped_plot.contains(event)[0]):
+                not hasattr(self.plotter.plot, "_wrapped_plot")
+                or not self.plotter.plot._wrapped_plot.contains(event)[0]
+            ):
                 return
             current_pm = self.plotmethod
-            self.plotmethod = 'lineplot'
+            self.plotmethod = "lineplot"
             linewidget = self.plotmethod_widget
             xdim = linewidget.xdim
             if xdim is None:
                 xdim = self.combo_dims.currentText()
 
-            if not linewidget.sp or (linewidget.xdim and
-                                     linewidget.xdim not in raw_data.dims):
+            if not linewidget.sp or (
+                linewidget.xdim and linewidget.xdim not in raw_data.dims
+            ):
                 with self.silence_variable_buttons():
                     for v, btn in self.variable_buttons.items():
                         btn.setChecked(v == variable)
                 self.make_plot()
                 linewidget.xdim = xdim
             else:
                 linewidget.xdim = xdim
                 linewidget.add_line(variable, **sl)
             self.plotmethod = current_pm
 
-
     def close_sp(self) -> None:
         """Close the current subproject."""
         sp = self.sp
         self.sp = None
         if sp is not None:
             sp.close(figs=True, data=True, ds=False)
 
@@ -1438,15 +1535,16 @@
                         self.combo_array.addItem(arr.psy._short_info())
                     if curr_arr_name in all_arrays.arr_names:
                         idx_arr = all_arrays.arr_names.index(curr_arr_name)
                         self.combo_array.setCurrentIndex(idx_arr)
                     else:
                         idx_arr = 0
                     self.ds = list(
-                        all_arrays[idx_arr:idx_arr+1].datasets.values())[0]
+                        all_arrays[idx_arr : idx_arr + 1].datasets.values()
+                    )[0]
                     if self.ds is not current_ds:
                         with self.block_tree():
                             self.expand_ds_item(self.ds_item)
                             self.expand_current_variable(self.data.name)
 
     def refresh(self, reset_combo: bool = True) -> None:
         """Refresh the state of this widget.
@@ -1473,15 +1571,14 @@
         else:
             variable = self.variable
             for action in self._save_preset_actions:
                 action.setEnabled(False)
             self.btn_del.setEnabled(False)
             self.btn_export.setEnabled(False)
 
-
         # refresh variable buttons
         with self.silence_variable_buttons():
             for v, btn in self.variable_buttons.items():
                 btn.setChecked(v == variable)
 
         # refresh tabs
         for i in range(self.plot_tabs.count()):
@@ -1494,86 +1591,92 @@
         elif self.ds is None or variable == NOTSET or not self.sp:
             return
 
         table = self.dimension_table
 
         if self.sp:
             data = self.data
-            ds_data = self.ds[self.variable]
+            ds_data = self.ds.psy[self.variable]
 
             with self.silence_variable_buttons():
                 self.variable_buttons[self.variable].setChecked(True)
 
             dims: Tuple[Hashable, ...] = ds_data.dims  # type: ignore
             table.setRowCount(ds_data.ndim)
             table.setVerticalHeaderLabels(ds_data.dims)
 
             # set time, z, x, y info
-            for c in 'XYTZ':
+            for c in "XYTZ":
                 cname = ds_data.psy.get_dim(c)
                 if cname and cname in dims:
                     table.setItem(
-                        dims.index(cname), 0, QtWidgets.QTableWidgetItem(c))
+                        dims.index(cname), 0, QtWidgets.QTableWidgetItem(c)
+                    )
 
             for i, dim in enumerate(dims):
                 coord = self.ds[dim]
-                if 'units' in coord.attrs:
+                if "units" in coord.attrs:
                     table.setItem(
-                        i, 4, QtWidgets.QTableWidgetItem(
-                            str(coord.attrs['units'])))
+                        i,
+                        4,
+                        QtWidgets.QTableWidgetItem(str(coord.attrs["units"])),
+                    )
                 try:
                     coord = list(map("{:1.4f}".format, coord.values))  # type: ignore
                 except (ValueError, TypeError):
                     try:
                         coord = coord.to_pandas().dt.to_pydatetime()  # type: ignore
                     except AttributeError:
                         coord = list(map(str, coord.values))  # type: ignore
                     else:
                         coord = [t.isoformat() for t in coord]  # type: ignore
                 first = coord[0]
                 last = coord[-1]
-                table.setItem(
-                    i, 1, QtWidgets.QTableWidgetItem(first))
-                table.setItem(
-                    i, 3, QtWidgets.QTableWidgetItem(last))
+                table.setItem(i, 1, QtWidgets.QTableWidgetItem(first))
+                table.setItem(i, 3, QtWidgets.QTableWidgetItem(last))
 
                 current = data.psy.idims.get(dim)
                 if current is not None and isinstance(current, int):
                     table.setCellWidget(
-                        i, 2, self.new_dimension_button(dim, coord[current]))
+                        i, 2, self.new_dimension_button(dim, coord[current])
+                    )
 
             # update animation checkbox
             dims_to_animate = get_dims_to_iterate(data)
 
-            current_dims_to_animate = list(map(
-                self.combo_dims.itemText,
-                range(self.combo_dims.count())))
+            current_dims_to_animate = list(
+                map(self.combo_dims.itemText, range(self.combo_dims.count()))
+            )
             if dims_to_animate != current_dims_to_animate:
                 self.combo_dims.clear()
                 self.combo_dims.addItems(dims_to_animate)
 
         table.resizeColumnsToContents()
 
         # update plots items
         for ds_item in self.ds_items:
             for item in map(ds_item.child, range(ds_item.childCount())):
                 for child in map(item.child, range(item.childCount())):
                     if DatasetTree.is_variable(child):
                         plots_item = ds_item.get_plots_item(child)
                         ds_item.refresh_plots_item(
-                            plots_item, child.text(0), self._sp, self.sp)
+                            plots_item, child.text(0), self._sp, self.sp
+                        )
 
     def new_dimension_button(
-            self, dim: Hashable, label: Any) -> utils.QRightPushButton:
+        self, dim: Hashable, label: Any
+    ) -> utils.QRightPushButton:
         """Generate a new button to increase of decrease a dimension."""
         btn = utils.QRightPushButton(label)
         btn.clicked.connect(self.increase_dim(str(dim)))
         btn.rightclicked.connect(self.increase_dim(str(dim), -1))
-        btn.setToolTip(f"Increase dimension {dim} with left-click, and "
-                       "decrease with right-click.")
+        btn.setToolTip(
+            f"Increase dimension {dim} with left-click, and "
+            "decrease with right-click."
+        )
         return btn
 
     def update_project(self, *args, **kwargs) -> None:
         """Update the correct project :attr:`sp` and refresh the widget."""
         sp = self.sp
         if sp is not None:
             sp.update(*args, **kwargs)
@@ -1585,20 +1688,24 @@
         Parameters
         ----------
         dim: str
             The dimension name
         increase: int
             The number of steps to increase (or decrease) the given `dim`.
         """
+
         def update():
             i = self.data.psy.idims[dim]
-            self.data.psy.update(dims={dim: (i+increase) % self.ds.dims[dim]})
+            self.data.psy.update(
+                dims={dim: (i + increase) % self.ds.dims[dim]}
+            )
             if self.data.psy.plotter is None:
                 self.sp.update(replot=True)
             self.refresh()
+
         return update
 
 
 class DatasetWidgetStandAlone(DatasetWidget):
     """A :class:`DatasetWidget` that is supposed to work as a standalone GUI"""
 
     def closeEvent(self, event: Any):
@@ -1613,27 +1720,29 @@
 
     This widget can be embeded in the psyplot GUI. Different from the standalone
     :class:`DatasetWidget` class, this one here uses the current psyplot project
     (:func:`psyplot.project.gcp`)
     """
 
     #: The title of the widget
-    title = 'psy-view Dataset viewer'
+    title = "psy-view Dataset viewer"
 
     #: Display the dock widget at the right side of the GUI
     dock_position = Qt.RightDockWidgetArea
 
     def __init__(self, *args, **kwargs):
         import psyplot.project as psy
+
         super().__init__(*args, **kwargs)
         psy.Project.oncpchange.connect(self.oncpchange)
 
     @property  # type: ignore
     def _sp(self) -> Project:  # type: ignore
         import psyplot.project as psy
+
         return psy.gcp(True)
 
     @_sp.setter
     def _sp(self, value):
         pass
 
     @property
@@ -1643,15 +1752,14 @@
 
     @sp.setter
     def sp(self, sp: Optional[Project]):
         current = self.get_sp()
         if sp is None or not current:
             return
         elif getattr(current, self.plotmethod, []):
-
             if len(current) == 1 and len(sp) == 1:
                 pass
             # first remove the current arrays
             if current and getattr(current, self.plotmethod):
                 to_remove = getattr(self.get_sp(), self.plotmethod).arr_names
                 for i in list(reversed(range(len(current)))):
                     if current[i].psy.arr_name in to_remove:
@@ -1681,18 +1789,20 @@
     def reload(self) -> None:
         """Close the plot and recreate it."""
         import psyplot.project as psy
 
         if not all(self._sp.dsnames_map.values()):
             # we have datasets that only exist in memory, so better ask
             answer = QtWidgets.QMessageBox.question(
-                self, "Shall I close this?",
+                self,
+                "Shall I close this?",
                 "Reloading the data closes all open plots. Any data in the memory "
                 "is lost and open files are reloaded from disk! "
-                "Shall I really continue?")
+                "Shall I really continue?",
+            )
             if answer != QtWidgets.QMessageBox.Yes:
                 return
 
         sp = self._sp
         fname = sp.dsnames_map[self.ds.psy.num]  # type: ignore
         project = sp.save_project()
         sp.close(True, True, True)
@@ -1718,14 +1828,15 @@
             self.set_dataset(next(iter(self._sp.datasets.values())))
         elif self.ds is not None and self._sp:
             self.enable_navigation()
 
     def show_fig(self, sp: Optional[Project]) -> None:
         """Show the figure of the the current subproject."""
         from psyplot_gui.main import mainwindow
+
         super().show_fig(sp)
         if mainwindow.figures and sp:
             try:
                 dock = sp.plotters[0].ax.figure.canvas.manager.window
                 dock.widget().show_plugin()
                 dock.raise_()
             except AttributeError:
@@ -1734,15 +1845,18 @@
     def setup_ds_tree(self) -> None:
         """Setup the number of columns and the header of the dataset tree.
 
         Reimplemented to use the :class:`psyplot_gui.content_widget.DatasetTree`
         """
         self.ds_tree = tree = DatasetTree()
         tree.setColumnCount(len(self.ds_attr_columns) + 1)
-        tree.setHeaderLabels([''] + self.ds_attr_columns)
+        tree.setHeaderLabels([""] + self.ds_attr_columns)
 
     def position_dock(self, main: MainWindow, *args, **kwargs) -> None:
         height = main.help_explorer.dock.size().height()
         main.splitDockWidget(main.help_explorer.dock, self.dock, Qt.Vertical)
-        if hasattr(main, 'resizeDocks'):  # qt >= 5.6
-            main.resizeDocks([main.help_explorer.dock, self.dock],
-                             [height // 2, height // 2], Qt.Vertical)
+        if hasattr(main, "resizeDocks"):  # qt >= 5.6
+            main.resizeDocks(
+                [main.help_explorer.dock, self.dock],
+                [height // 2, height // 2],
+                Qt.Vertical,
+            )
```

### Comparing `psy-view-0.2.0/psy_view/plotmethods.py` & `psy-view-0.3.0/psy_view/plotmethods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,79 +1,59 @@
 """Plotmethod widgets.
 
 This module defines the widgets to interface with the mapplot, plot2d and
 lineplot plotmethods.
 """
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-#
-# This file is part of psy-view and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
 from __future__ import annotations
-import os.path as osp
 
+import contextlib
+import dataclasses
+import textwrap
+from enum import Enum
+from functools import partial
+from itertools import chain, cycle
 from typing import (
     TYPE_CHECKING,
-    ClassVar,
+    Any,
     Callable,
-    Optional,
-    Union,
-    List,
-    Hashable,
+    ClassVar,
     Dict,
-    Any,
-    Tuple,
+    Hashable,
     Iterator,
-    TypeVar,
+    List,
+    Optional,
+    Tuple,
     Type,
+    TypeVar,
+    Union,
 )
-from enum import Enum
-
-from functools import partial
-from itertools import chain, cycle
-import contextlib
-import textwrap
-
-import dataclasses
 
+import matplotlib.colors as mcol
+import psy_simple.widgets.colors as pswc
+import psyplot.data as psyd
 import xarray as xr
 from psyplot.utils import unique_everseen
+from psyplot_gui.common import get_icon as get_psy_icon
+from PyQt5 import QtCore, QtGui, QtWidgets
 
-from PyQt5 import QtWidgets, QtCore, QtGui
 import psy_view.dialogs as dialogs
 import psy_view.utils as utils
 from psy_view.rcsetup import rcParams
 
-from psyplot_gui.common import get_icon as get_psy_icon
-import psy_simple.widgets.colors as pswc
-import matplotlib.colors as mcol
-
 if TYPE_CHECKING:
-    from xarray import DataArray, Dataset, Variable
-    from psyplot.project import PlotterInterface, Project
     from psyplot.data import InteractiveList
     from psyplot.plotter import Plotter
+    from psyplot.project import Project
+    from xarray import DataArray, Dataset
 
 
 T = TypeVar("T", bound="GridCell")
 
 
 class PlotType(str, Enum):
     """A value for the 2D ``plot`` formatoption.
@@ -122,15 +102,15 @@
 
     @classmethod
     def from_alias(
         cls: Type[T],
         o: Union[QtWidgets.QWidget, QtWidgets.QLayout],
         c: Optional[int] = None,
         cs: int = 1,
-        s: bool = False
+        s: bool = False,
     ) -> T:
         """Create a :class:`GridCell` from shorter kws.
 
         Parameters
         ----------
         o: QWidget or QLayout
             The alias for :attr:`qobject`
@@ -155,15 +135,15 @@
     This method serves as a base class for interfacing any of the psyplot
     plot methods registered via :func:`psyplot.project.register_plotter`.
 
     The name of the plotmethod should be implemented as the :attr:`plotmethod`
     attribute.
     """
 
-    plotmethod: ClassVar[str] = ''
+    plotmethod: ClassVar[str] = ""
 
     #: trigger a replot of this widget. This can be emitted with the
     #: :meth:`trigger_replot` method
     replot = QtCore.pyqtSignal(str)
 
     #: trigger a replot of this widget. This can be emitted with the
     #: :meth:`trigger_reset` method
@@ -174,16 +154,16 @@
     changed = QtCore.pyqtSignal(str)
 
     array_info = None
 
     layout: QtWidgets.QGridLayout = None
 
     def __init__(
-            self, get_sp: Callable[[], Optional[Project]],
-            ds: Optional[Dataset]):
+        self, get_sp: Callable[[], Optional[Project]], ds: Optional[Dataset]
+    ):
         super().__init__()
         self._get_sp = get_sp
 
         self.setup()
 
         if hasattr(self, "layout"):
             self.setLayout(self.layout)
@@ -200,15 +180,14 @@
     def formatoption_rows(self) -> List[List[GridCell]]:
         """Get a mapping from row name to a row of :class:`GridCells`."""
         rows: List[List[GridCell]] = []
         for func in self.fmt_setup_functions:
             rows.extend(self.get_rows(func))
         return rows
 
-
     def get_rows(self, func: Callable) -> List[List[GridCell]]:
         """Get the rows of the formatoption widgets.
 
         This method should take callable from the :attr:`fmt_setup_functions`
         list and return the rows corresponding to :attr:`formatoption_rows`.
         """
         return [[]]
@@ -245,14 +224,15 @@
                 col = gc.column if gc.column is not None else col
                 if isinstance(gc.qobject, QtWidgets.QLayout):
                     layout.addLayout(gc.qobject, i, col, 1, gc.colspan)
                 else:
                     layout.addWidget(gc.qobject, i, col, 1, gc.colspan)
                 col += gc.colspan
         layout.setRowStretch(len(rows), 1)
+
     @property
     def sp(self) -> Optional[Project]:
         """Get the subproject of this plotmethod interface."""
         return getattr(self._get_sp(), self.plotmethod, None)
 
     @property
     def data(self) -> Union[DataArray, InteractiveList]:
@@ -273,19 +253,20 @@
     @property
     def formatoptions(self) -> List[str]:
         """Get the formatoption keys of this plotmethod."""
         if self.plotter is not None:
             return list(self.plotter)
         else:
             import psyplot.project as psy
+
             return list(getattr(psy.plot, self.plotmethod).plotter_cls())
 
     def get_fmts(
-            self, var: DataArray, init: bool = False
-        ) -> Dict[Union[Hashable, str, Any], Any]:
+        self, var: DataArray, init: bool = False
+    ) -> Dict[Union[Hashable, str, Any], Any]:
         """Get the formatoptions for a new plot.
 
         Parameters
         ----------
         var: xarray.Variable
             The variable in the base dataset
         init: bool
@@ -300,16 +281,16 @@
         """
         ret = {}
         if init:
             ret.update(self.init_dims(var))
         return ret
 
     def init_dims(
-            self, var: DataArray
-        ) -> Dict[Union[Hashable, str, Any], Any]:
+        self, var: DataArray
+    ) -> Dict[Union[Hashable, str, Any], Any]:
         """Get the formatoptions for a new plot.
 
         Parameters
         ----------
         var: xarray.Variable
             The variable in the base dataset
 
@@ -328,25 +309,26 @@
 
     def trigger_replot(self) -> None:
         """Emit the :attr:`replot` signal to replot the project."""
         self.replot.emit(self.plotmethod)
 
     def trigger_reset(self):
         """Emit the :attr:`reset` signal to reinitialize the project."""
-        self.array_info = self.sp.array_info(
-            standardize_dims=False)[self.sp[0].psy.arr_name]
+        self.array_info = self.sp.array_info(standardize_dims=False)[
+            self.sp[0].psy.arr_name
+        ]
         self.reset.emit(self.plotmethod)
 
     def trigger_refresh(self):
         """Emit the :attr:`changed` signal to notify changes in the plot."""
         self.changed.emit(self.plotmethod)
 
     def get_slice(
-            self, x: float, y: float
-        ) -> Optional[Dict[Hashable, Union[int, slice]]]:
+        self, x: float, y: float
+    ) -> Optional[Dict[Hashable, Union[int, slice]]]:
         """Get the slice for the selected coordinates.
 
         This method is called when the user clicks on the coordinates in the
         plot.
 
         See Also
         --------
@@ -371,39 +353,51 @@
         list of str
             List of variable names to plot
         """
         ret = []
         plotmethod = getattr(ds.psy.plot, self.plotmethod)
         for v in list(ds):
             init_kws = self.init_dims(ds[v])  # type: ignore
-            dims = init_kws.get('dims', {})
-            decoder = init_kws.get('decoder')
+            dims = init_kws.get("dims", {})
+            decoder = init_kws.get("decoder")
             if plotmethod.check_data(ds, v, dims, decoder)[0][0]:
                 ret.append(v)
         return ret
 
 
 class QHLine(QtWidgets.QFrame):
     """A horizontal seperation line."""
+
     def __init__(self):
         super().__init__()
         self.setMinimumWidth(1)
         self.setFixedHeight(20)
         self.setFrameShape(QtWidgets.QFrame.HLine)
         self.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.setSizePolicy(
-            QtWidgets.QSizePolicy.Preferred,
-            QtWidgets.QSizePolicy.Minimum
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Minimum
         )
 
 
 class MapPlotWidget(PlotMethodWidget):
     """A widget to control the mapplot plotmethod."""
 
-    plotmethod = 'mapplot'
+    plotmethod = "mapplot"
+
+    @property
+    def sp(self) -> Optional[Project]:
+        sp = super().sp
+        if sp:
+            arrays: List[str] = [
+                data.psy.arr_name
+                for data in sp
+                if not isinstance(data, psyd.InteractiveList)
+            ]
+            return sp(arr_name=arrays)
+        return sp
 
     def get_rows(self, func: Callable) -> List[List[GridCell]]:
         """Get the rows of the formatoption widgets.
 
         This method should take callable from the :attr:`fmt_setup_functions`
         list and return the rows corresponding to :attr:`formatoption_rows`.
         """
@@ -427,58 +421,130 @@
             ]
         elif func == self.setup_labels_button:
             row = [GridCell(self.btn_labels, colspan=3)]
         elif func == self.setup_separation_line:
             row = [GridCell(QHLine(), colspan=3)]
         elif func == self.setup_dimension_box:
             row = [GridCell(self.dimension_box, colspan=3)]
+        elif func == self.setup_fix_extent_buttons:
+            hbox = QtWidgets.QHBoxLayout()
+            hbox.addWidget(self.btn_fix_extent)
+            hbox.addWidget(self.btn_fix_lonlatbox)
+            hbox.addWidget(self.btn_reset_extent)
+            row = [
+                GridCell(QtWidgets.QLabel("Viewport")),
+                GridCell(hbox, colspan=3),
+            ]
         else:
             raise ValueError(f"Unknown function {func}")
         return [row]
 
     @property
     def fmt_setup_functions(self) -> List[Callable]:
         """Get a list of rows for formatoptions.
 
         This property returns a list of callable. Each callable should setup
         a horizonal (or widget) that is added to the :attr:`layout` vbox.
         """
         return [
-            self.setup_color_buttons, self.setup_plot_buttons,
-            self.setup_projection_buttons, self.setup_labels_button,
+            self.setup_color_buttons,
+            self.setup_plot_buttons,
+            self.setup_projection_buttons,
+            self.setup_labels_button,
+            self.setup_separation_line,
+            self.setup_fix_extent_buttons,
             self.setup_separation_line,
             self.setup_dimension_box,
         ]
 
     def setup_labels_button(self) -> None:
         """Add a button to modify the text labels."""
         self.btn_labels = utils.add_pushbutton(
-            "Edit labels", self.edit_labels, "Edit title, colorbar labels, etc."
+            "Edit labels",
+            self.edit_labels,
+            "Edit title, colorbar labels, etc.",
         )
 
+    def setup_fix_extent_buttons(self):
+        """Setup the buttons for fixing the extent or data"""
+        self.btn_fix_extent = utils.add_pushbutton(
+            "Fix view",
+            self.fix_extent,
+            (
+                "Fix the current view such that it is not update on redrawing "
+                "the plot."
+            ),
+        )
+
+        self.btn_fix_lonlatbox = utils.add_pushbutton(
+            "Restrict data",
+            self.fix_data,
+            (
+                "Extract the data for the plot, such that it matches the "
+                "current view."
+            ),
+        )
+
+        self.btn_reset_extent = utils.add_pushbutton(
+            "Reset",
+            self.reset_extent_and_lonlatbox,
+            (
+                "Reset the view and the data selection to the default "
+                "(i.e. to the full data)."
+            ),
+        )
+
+    def fix_extent(self):
+        """Call the fix_map_extent method of all map plotters."""
+        for plotter in self.sp.plotters:
+            if hasattr(plotter, "fix_map_extent"):
+                plotter.fix_map_extent()
+
+    def fix_data(self):
+        """Call the fix_lonlatbox method of all map plotters."""
+        for plotter in self.sp.plotters:
+            if hasattr(plotter, "fix_lonlatbox"):
+                plotter.fix_lonlatbox()
+
+    def reset_extent_and_lonlatbox(self):
+        """Reset the extent and the lonlatbox to the defaults."""
+        for plotter in self.sp.plotters:
+            plotter.update(
+                lonlatbox=plotter.lonlatbox.default,
+                map_extent=plotter.map_extent.default,
+                force=True,
+            )
+
     def setup_plot_buttons(self) -> None:
         """Setup the second row of formatoption widgets."""
         self.combo_plot = QtWidgets.QComboBox()
         self.plot_types: List[Optional[PlotType]] = [
             PlotType.mesh,
             PlotType.contourf,
             PlotType.contour,
             PlotType.poly,
-            None
+            None,
         ]
         self.combo_plot.setEditable(False)
-        self.combo_plot.addItems([
-            "Default", "Filled contours", "Contours", "Gridcell polygons",
-            "Disable"
-        ])
+        self.combo_plot.addItems(
+            [
+                "Default",
+                "Filled contours",
+                "Contours",
+                "Gridcell polygons",
+                "Disable",
+            ]
+        )
         self.combo_plot.currentIndexChanged.connect(self._set_plot_type)
 
         self.btn_datagrid = utils.add_pushbutton(
-            "Gridcell boundaries", self.toggle_datagrid,
-            "Toggle the visibility of grid cell boundaries")
+            "Gridcell boundaries",
+            self.toggle_datagrid,
+            "Toggle the visibility of grid cell boundaries",
+        )
         self.btn_datagrid.setCheckable(True)
 
         return
 
     def setup_color_buttons(self) -> None:
         """Set up the buttons to change the colormap, etc."""
         self.btn_cmap = pswc.CmapButton()
@@ -488,29 +554,34 @@
         self.btn_cmap.setToolTip("Select a different colormap")
 
         self.btn_cmap.colormap_changed.connect(self.set_cmap)
         self.btn_cmap.colormap_changed[mcol.Colormap].connect(self.set_cmap)
         self.setup_cmap_menu()
 
         self.btn_cmap_settings = utils.add_pushbutton(
-            utils.get_icon('color_settings'), self.edit_color_settings,
+            utils.get_icon("color_settings"),
+            self.edit_color_settings,
             "Edit color settings",
-            icon=True)
+            icon=True,
+        )
 
     def setup_cmap_menu(self) -> QtWidgets.QMenu:
         """Set up the menu to change the colormaps."""
         menu = self.btn_cmap.cmap_menu
 
         menu.addSeparator()
         self.select_cmap_action = menu.addAction(
-            'More colormaps', self.open_cmap_dialog)
+            "More colormaps", self.open_cmap_dialog
+        )
 
         self.color_settings_action = menu.addAction(
-            QtGui.QIcon(utils.get_icon('color_settings')), 'More options',
-            self.edit_color_settings)
+            QtGui.QIcon(utils.get_icon("color_settings")),
+            "More options",
+            self.edit_color_settings,
+        )
 
         return menu
 
     def open_cmap_dialog(self, N: int = 10) -> None:
         """Open the dialog to change the colormap.
 
         Parameters
@@ -527,23 +598,25 @@
         else:
             N = 10
         self.btn_cmap.open_cmap_dialog(N)
 
     def setup_projection_menu(self) -> QtWidgets.QMenu:
         """Set up the menu to modify the basemap."""
         menu = QtWidgets.QMenu()
-        for projection in rcParams['projections']:
+        for projection in rcParams["projections"]:
             menu.addAction(
                 projection_map.get(projection, projection),
                 partial(self.set_projection, projection),
             )
         menu.addSeparator()
         self.proj_settings_action = menu.addAction(
-            QtGui.QIcon(utils.get_icon('proj_settings')),
-            "Customize basemap...", self.edit_basemap_settings)
+            QtGui.QIcon(utils.get_icon("proj_settings")),
+            "Customize basemap...",
+            self.edit_basemap_settings,
+        )
         return menu
 
     def get_projection_label(self, proj: str) -> str:
         """Get the label for a projection in the GUI.
 
         Parameters
         ----------
@@ -589,45 +662,49 @@
         inv_map = {lbl: proj for proj, lbl in projection_map.items()}
         return inv_map.get(label, rcParams["projections"][0])
 
     def setup_projection_buttons(self) -> None:
         """Set up the buttons to modify the basemap."""
         self.btn_proj = utils.add_pushbutton(
             self.get_projection_label(rcParams["projections"][0]),
-            self.choose_next_projection, "Change the basemap projection",
-            toolbutton=True)
+            self.choose_next_projection,
+            "Change the basemap projection",
+            toolbutton=True,
+        )
         self.btn_proj.setMenu(self.setup_projection_menu())
 
         self.btn_proj.setSizePolicy(
             QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding
         )
         self.btn_proj.setPopupMode(QtWidgets.QToolButton.MenuButtonPopup)
 
         self.btn_proj_settings = utils.add_pushbutton(
-            utils.get_icon('proj_settings'), self.edit_basemap_settings,
+            utils.get_icon("proj_settings"),
+            self.edit_basemap_settings,
             "Edit basemap settings",
-            icon=True)
+            icon=True,
+        )
 
     def setup_dimension_box(self) -> None:
         """Set up a box to control, what is the x and y-dimension."""
         self.dimension_box = QtWidgets.QGridLayout()
 
-        self.dimension_box.addWidget(QtWidgets.QLabel('x-Dimension:'), 0, 0)
+        self.dimension_box.addWidget(QtWidgets.QLabel("x-Dimension:"), 0, 0)
         self.combo_xdim = QtWidgets.QComboBox()
         self.dimension_box.addWidget(self.combo_xdim, 0, 1)
 
-        self.dimension_box.addWidget(QtWidgets.QLabel('y-Dimension:'), 0, 2)
+        self.dimension_box.addWidget(QtWidgets.QLabel("y-Dimension:"), 0, 2)
         self.combo_ydim = QtWidgets.QComboBox()
         self.dimension_box.addWidget(self.combo_ydim, 0, 3)
 
-        self.dimension_box.addWidget(QtWidgets.QLabel('x-Coordinate:'), 1, 0)
+        self.dimension_box.addWidget(QtWidgets.QLabel("x-Coordinate:"), 1, 0)
         self.combo_xcoord = QtWidgets.QComboBox()
         self.dimension_box.addWidget(self.combo_xcoord, 1, 1)
 
-        self.dimension_box.addWidget(QtWidgets.QLabel('y-Coordinate:'), 1, 2)
+        self.dimension_box.addWidget(QtWidgets.QLabel("y-Coordinate:"), 1, 2)
         self.combo_ycoord = QtWidgets.QComboBox()
         self.dimension_box.addWidget(self.combo_ycoord, 1, 3)
 
         self.combo_xdim.currentTextChanged.connect(self.set_xcoord)
         self.combo_ydim.currentTextChanged.connect(self.set_ycoord)
 
         for combo in self.coord_combos:
@@ -651,16 +728,16 @@
         text: str
             The item to use"""
         items = list(map(combo.itemText, range(combo.count())))
         if text in items:
             combo.setCurrentIndex(items.index(text))
 
     def init_dims(
-            self, var: DataArray
-        ) -> Dict[Union[Hashable, str, Any], Any]:
+        self, var: DataArray
+    ) -> Dict[Union[Hashable, str, Any], Any]:
         """Get the formatoptions for a new plot.
 
         This method updates the coordinates combo boxes with the
         x- and y-coordinate of the variable.
 
         Parameters
         ----------
@@ -694,28 +771,31 @@
                 dims[dim] = 0
             if len(dims) == 1 and xdim != ydim:
                 if xdim is None:
                     xdim = missing[-1]
                 else:
                     ydim = missing[-1]
                 dims[missing[-1]] = slice(None)  # keep the last dimension
-            ret['dims'] = dims
-
+            ret["dims"] = dims
 
         if self.combo_xcoord.currentIndex():
             xcoord = self.combo_xcoord.currentText()
-            ret['decoder'] = {'x': {xcoord}}
+            ret["decoder"] = {"x": {xcoord}}
         if self.combo_ycoord.currentIndex():
             ycoord = self.combo_ycoord.currentText()
-            ret.setdefault('decoder', {})
-            ret['decoder']['y'] = {ycoord}
+            ret.setdefault("decoder", {})
+            ret["decoder"]["y"] = {ycoord}
 
-        if (xdim is not None and xdim in var.dims and
-                ydim is not None and ydim in var.dims):
-            ret['transpose'] = var.dims.index(xdim) < var.dims.index(ydim)
+        if (
+            xdim is not None
+            and xdim in var.dims
+            and ydim is not None
+            and ydim in var.dims
+        ):
+            ret["transpose"] = var.dims.index(xdim) < var.dims.index(ydim)
 
         return ret
 
     def valid_variables(self, ds: Dataset) -> List[Hashable]:
         """Get a list of variables that can be visualized with this plotmethod.
 
         Parameters
@@ -725,38 +805,41 @@
 
         Returns
         -------
         list of str
             List of variable names to plot
         """
         valid = super().valid_variables(ds)
-        if (not any(combo.count() for combo in self.coord_combos) or
-                not any(combo.currentIndex() for combo in self.coord_combos)):
+        if not any(combo.count() for combo in self.coord_combos) or not any(
+            combo.currentIndex() for combo in self.coord_combos
+        ):
             return valid
         if self.combo_xdim.currentIndex():
             xdim = self.combo_xdim.currentText()
             valid = [v for v in valid if xdim in ds[v].dims]
         if self.combo_ydim.currentIndex():
             ydim = self.combo_xdim.currentText()
             valid = [v for v in valid if ydim in ds[v].dims]
         if self.combo_xcoord.currentIndex():
             xc_dims = set(ds[self.combo_xcoord.currentText()].dims)
-            valid = [v for v in valid
-                     if xc_dims.intersection(ds[v].dims)]
+            valid = [v for v in valid if xc_dims.intersection(ds[v].dims)]
         if self.combo_ycoord.currentIndex():
             yc_dims = set(ds[self.combo_ycoord.currentText()].dims)
-            valid = [v for v in valid
-                     if yc_dims.intersection(ds[v].dims)]
+            valid = [v for v in valid if yc_dims.intersection(ds[v].dims)]
         return valid
 
     @property
     def coord_combos(self) -> List[QtWidgets.QComboBox]:
         """Get the combo boxes for x- and y-dimension and -coordinates."""
-        return [self.combo_xdim, self.combo_ydim, self.combo_xcoord,
-                self.combo_ycoord]
+        return [
+            self.combo_xdim,
+            self.combo_ydim,
+            self.combo_xcoord,
+            self.combo_ycoord,
+        ]
 
     @contextlib.contextmanager
     def block_combos(self) -> Iterator[None]:
         """Temporarilly block any signal of the :attr:`coord_combos`."""
         for combo in self.coord_combos:
             combo.blockSignals(True)
         yield
@@ -773,56 +856,60 @@
         """
         self.btn_proj_settings.setEnabled(b)
         self.proj_settings_action.setEnabled(b)
         self.btn_datagrid.setEnabled(b)
         self.color_settings_action.setEnabled(b)
         self.btn_cmap_settings.setEnabled(b)
         self.btn_labels.setEnabled(b)
+        self.btn_fix_extent.setEnabled(b)
+        self.btn_fix_lonlatbox.setEnabled(b)
+        self.btn_reset_extent.setEnabled(b)
 
     def set_cmap(self, cmap: str) -> None:
         """Update the plotter with the given colormap.
 
         Parameters
         ----------
         cmap: str
             The colormap name.
         """
         plotter = self.plotter
-        if plotter and 'cmap' in plotter:
+        if plotter and "cmap" in plotter:
             plotter.update(cmap=cmap)
 
     def toggle_datagrid(self) -> None:
         """Toggle the visibility of the grid cell boundaries."""
         if self.plotter:
             if self.btn_datagrid.isChecked():
-                self.plotter.update(datagrid='k-')
+                self.plotter.update(datagrid="k-")
             else:
                 self.plotter.update(datagrid=None)
 
     def edit_labels(self) -> None:
         """Open the dialog to edit the text labels in the plot."""
         dialogs.LabelDialog.update_project(
-            self.sp, 'figtitle', 'title', 'clabel')
+            self.sp, "figtitle", "title", "clabel"
+        )
 
     def edit_color_settings(self) -> None:
         """Open the dialog to edit the color settings."""
         if self.sp and self.plotter:
             dialogs.CmapDialog.update_project(self.sp)
             if isinstance(self.plotter.cmap.value, str):
                 self.btn_cmap.setText(self.plotter.cmap.value)
             else:
-                self.btn_cmap.setText('Custom')
+                self.btn_cmap.setText("Custom")
 
     def choose_next_projection(self) -> None:
         """Choose the next projection from the rcParams `projection` value."""
         select = False
-        nprojections = len(rcParams['projections'])
+        nprojections = len(rcParams["projections"])
         current = self.get_projection_value(self.btn_proj.text())
 
-        for i, proj in enumerate(cycle(rcParams['projections'])):
+        for i, proj in enumerate(cycle(rcParams["projections"])):
             if proj == current:
                 select = True
             elif select or i == nprojections:
                 break
         self.set_projection(proj)
 
     def set_projection(self, proj: str) -> None:
@@ -832,15 +919,15 @@
         ----------
         projection: str
             The projection name for the
             :attr:`~psy_maps.plotters.FieldPlotter.projection` formatoption.
         """
         self.btn_proj.setText(self.get_projection_label(proj))
         plotter = self.plotter
-        if plotter and 'projection' in plotter:
+        if plotter and "projection" in plotter:
             plotter.update(projection=proj)
 
     def _set_plot_type(self, i: int) -> None:
         """Set the plot type from the index in :attr:`combo_plot`."""
         self.set_plot_type(self.plot_types[i])
 
     def set_plot_type(self, plot_type: Optional[PlotType]) -> None:
@@ -858,17 +945,16 @@
 
     def edit_basemap_settings(self) -> None:
         """Open a dialog to edit the basemap and projection settings."""
         if self.plotter:
             dialogs.BasemapDialog.update_plotter(self.plotter)
 
     def get_fmts(
-            self, var: DataArray,
-            init: bool = False
-        ) -> Dict[Union[Hashable, str, Any], Any]:
+        self, var: DataArray, init: bool = False
+    ) -> Dict[Union[Hashable, str, Any], Any]:
         """Get the formatoptions for a new plot.
 
         Parameters
         ----------
         var: xarray.Variable
             The variable in the base dataset
         init: bool
@@ -879,117 +965,126 @@
         -------
         dict
             A mapping from formatoption or dimension to the corresponding value
             for the plotmethod.
         """
         fmts: Dict[Union[Hashable, str, Any], Any] = {}
 
-        fmts['cmap'] = self.btn_cmap.text()
+        fmts["cmap"] = self.btn_cmap.text()
 
-        if 'projection' in self.formatoptions:
-            fmts['projection'] = self.get_projection_value(
+        if "projection" in self.formatoptions:
+            fmts["projection"] = self.get_projection_value(
                 self.btn_proj.text()
             )
 
-        if 'time' in var.dims:
-            fmts['title'] = '%(time)s'
+        if "time" in var.dims:
+            fmts["title"] = "%(time)s"
 
-        if 'long_name' in var.attrs:
-            fmts['clabel'] = '%(long_name)s'
+        if "long_name" in var.attrs:
+            fmts["clabel"] = "%(long_name)s"
         else:
-            fmts['clabel'] = '%(name)s'
-        if 'units' in var.attrs:
-            fmts['clabel'] += ' %(units)s'
+            fmts["clabel"] = "%(name)s"
+        if "units" in var.attrs:
+            fmts["clabel"] += " %(units)s"
 
-        fmts['plot'] = self.plot_types[self.combo_plot.currentIndex()]
-        if fmts['plot'] == 'contour':
+        fmts["plot"] = self.plot_types[self.combo_plot.currentIndex()]
+        if fmts["plot"] == "contour":
             # we need to set a global map extend, see
             # https://github.com/SciTools/cartopy/issues/1673
-            fmts['map_extent'] = 'global'
+            fmts["map_extent"] = "global"
 
         if init:
             fmts.update(self.init_dims(var))
 
         return fmts
 
     def refresh(self, ds: Optional[Dataset]) -> None:
         """Refresh this widget from the given dataset."""
         self.setEnabled(bool(self.sp))
 
-        auto = 'Set automatically'
+        auto = "Set automatically"
 
         self.refresh_from_sp()
 
         with self.block_combos():
-
             if ds is None:
                 ds = xr.Dataset()
 
-            current_dims = set(map(
-                self.combo_xdim.itemText, range(1, self.combo_xdim.count())))
+            current_dims = set(
+                map(
+                    self.combo_xdim.itemText, range(1, self.combo_xdim.count())
+                )
+            )
             ds_dims = list(
-                map(str, (dim for dim, n in ds.dims.items() if n > 1)))
+                map(str, (dim for dim, n in ds.dims.items() if n > 1))
+            )
             if current_dims != set(ds_dims):
                 self.combo_xdim.clear()
                 self.combo_ydim.clear()
                 self.combo_xdim.addItems([auto] + ds_dims)
                 self.combo_ydim.addItems([auto] + ds_dims)
 
-            current_coords = set(map(
-                self.combo_xcoord.itemText, range(1, self.combo_xcoord.count())))
+            current_coords = set(
+                map(
+                    self.combo_xcoord.itemText,
+                    range(1, self.combo_xcoord.count()),
+                )
+            )
             ds_coords = list(
-                map(str, (c for c, arr in ds.coords.items() if arr.ndim)))
+                map(str, (c for c, arr in ds.coords.items() if arr.ndim))
+            )
             if current_coords != set(ds_coords):
                 self.combo_xcoord.clear()
                 self.combo_ycoord.clear()
                 self.combo_xcoord.addItems([auto] + ds_coords)
                 self.combo_ycoord.addItems([auto] + ds_coords)
 
             enable_combos = not bool(self.sp)
 
             if not enable_combos and self.combo_xdim.isEnabled():
-                self.reset_combos = [combo.currentIndex() == 0
-                                    for combo in self.coord_combos]
+                self.reset_combos = [
+                    combo.currentIndex() == 0 for combo in self.coord_combos
+                ]
             elif enable_combos and not self.combo_xdim.isEnabled():
                 for reset, combo in zip(self.reset_combos, self.coord_combos):
                     if reset:
                         combo.setCurrentIndex(0)
                 self.reset_combos = [False] * len(self.coord_combos)
 
             for combo in self.coord_combos:
                 combo.setEnabled(enable_combos)
 
             if not enable_combos:
                 data = self.data
-                xdim = str(data.psy.get_dim('x'))
-                ydim = str(data.psy.get_dim('y'))
+                xdim = str(data.psy.get_dim("x"))
+                ydim = str(data.psy.get_dim("y"))
                 self.combo_xdim.setCurrentText(xdim)
                 self.combo_ydim.setCurrentText(ydim)
-                xcoord = data.psy.get_coord('x')
+                xcoord = data.psy.get_coord("x")
                 xcoord = xcoord.name if xcoord is not None else xdim
-                ycoord = data.psy.get_coord('y')
+                ycoord = data.psy.get_coord("y")
                 ycoord = ycoord.name if ycoord is not None else ydim
 
                 self.combo_xcoord.setCurrentText(xcoord)
                 self.combo_ycoord.setCurrentText(ycoord)
 
     def refresh_from_sp(self) -> None:
         """Refresh this widget from the plotters project."""
         plotter = self.plotter
         if plotter:
             if isinstance(plotter.projection.value, str):
                 self.btn_proj.setText(
                     self.get_projection_label(plotter.projection.value)
                 )
             else:
-                self.btn_proj.setText('Custom')
+                self.btn_proj.setText("Custom")
             if isinstance(plotter.cmap.value, str):
                 self.btn_cmap.setText(plotter.cmap.value)
             else:
-                self.btn_cmap.setText('Custom')
+                self.btn_cmap.setText("Custom")
 
     def transform(self, x: float, y: float) -> Tuple[float, float]:
         """Transform coordinates of a point to the plots projection.
 
         Parameters
         ----------
         x: float
@@ -1002,93 +1097,101 @@
         float
             The transformed x-coordinate `x`
         float
             The transformed y-coordinate `y`
         """
         import cartopy.crs as ccrs
         import numpy as np
+
         plotter = self.plotter
         if not plotter:
             raise ValueError(
                 "Cannot transform the coordinates as no plot is shown "
-                "currently!")
+                "currently!"
+            )
         x, y = plotter.transform.projection.transform_point(
-            x, y, plotter.ax.projection)
+            x, y, plotter.ax.projection
+        )
         # shift if necessary
         if isinstance(plotter.transform.projection, ccrs.PlateCarree):
             coord = plotter.plot.xcoord
             if coord.min() >= 0 and x < 0:
                 x -= 360
             elif coord.max() <= 180 and x > 180:
                 x -= 360
-            if 'rad' in coord.attrs.get('units', '').lower():
+            if "rad" in coord.attrs.get("units", "").lower():
                 x = np.deg2rad(x)
                 y = np.deg2rad(y)
         return x, y
 
     def get_slice(
-            self, x: float, y: float
-        ) -> Optional[Dict[Hashable, Union[int, slice]]]:
+        self, x: float, y: float
+    ) -> Optional[Dict[Hashable, Union[int, slice]]]:
         """Get the slice for the selected coordinates.
 
         This method is called when the user clicks on the coordinates in the
         plot.
 
         See Also
         --------
         psy_view.ds_widget.DatasetWidget.display_line
 
         Notes
         -----
         This is reimplemented in the :class:`MapPlotWidget`.
         """
         import numpy as np
+
         data = self.data.psy.base.psy[self.data.name]
         x, y = self.transform(x, y)
         plotter = self.plotter
 
         if not plotter:
             raise ValueError(
                 "Cannot transform the coordinates as no plot is shown "
-                "currently!")
+                "currently!"
+            )
 
         fmto = plotter.plot
 
         xcoord = fmto.xcoord
         ycoord = fmto.ycoord
         if fmto.decoder.is_unstructured(fmto.raw_data) or xcoord.ndim == 2:
             xy = xcoord.values.ravel() + 1j * ycoord.values.ravel()
             dist = np.abs(xy - (x + 1j * y))
             imin = np.nanargmin(dist)
             if xcoord.ndim == 2:
                 ncols = data.shape[-2]
-                return dict(zip(data.dims[-2:],
-                                [imin // ncols, imin % ncols]))
+                return dict(zip(data.dims[-2:], [imin // ncols, imin % ncols]))
             else:
                 return {data.dims[-1]: imin}
         else:
-            ix: int = xcoord.indexes[xcoord.name].get_loc(x, method='nearest')
-            iy: int = ycoord.indexes[ycoord.name].get_loc(y, method='nearest')
+            ix: int = xcoord.indexes[xcoord.name].get_loc(x, method="nearest")
+            iy: int = ycoord.indexes[ycoord.name].get_loc(y, method="nearest")
             return dict(zip(data.dims[-2:], [iy, ix]))
 
 
 class Plot2DWidget(MapPlotWidget):
     """A widget to control the plot2d plotmethod."""
 
-    plotmethod = 'plot2d'
+    plotmethod = "plot2d"
 
     @property
     def fmt_setup_functions(self) -> List[Callable]:
         """Get a list of rows for formatoptions.
 
         This property returns a list of callable. Each callable should setup
         a horizonal (or widget) that is added to the :attr:`layout` vbox.
         """
         ret = super().fmt_setup_functions
         ret.remove(self.setup_projection_buttons)
+        idx_extent = ret.index(self.setup_fix_extent_buttons)
+        # remove the separator and the function
+        del ret[idx_extent - 1]
+        del ret[idx_extent - 1]
         return ret
 
     def setEnabled(self, b: bool) -> None:
         """Enable or disable the datagrid and color buttons.
 
         Parameters
         ----------
@@ -1098,15 +1201,16 @@
         self.btn_datagrid.setEnabled(b)
         self.btn_cmap_settings.setEnabled(b)
         self.btn_labels.setEnabled(b)
 
     def edit_labels(self) -> None:
         """Open the dialog to edit the text labels in the plot."""
         dialogs.LabelDialog.update_project(
-            self.sp, 'figtitle', 'title', 'clabel', 'xlabel', 'ylabel')
+            self.sp, "figtitle", "title", "clabel", "xlabel", "ylabel"
+        )
 
     def transform(self, x: float, y: float) -> Tuple[float, float]:
         """Reimplemented to not transform the coordinates."""
         return x, y
 
     def refresh_from_sp(self) -> None:
         """Refresh this widget from the plotters project."""
@@ -1115,15 +1219,15 @@
             if isinstance(plotter.cmap.value, str):
                 self.btn_cmap.setText(plotter.cmap.value)
 
 
 class LinePlotWidget(PlotMethodWidget):
     """A widget to control the lineplot plotmethod."""
 
-    plotmethod = 'lineplot'
+    plotmethod = "lineplot"
 
     @property
     def fmt_setup_functions(self) -> List[Callable]:
         return [
             self.setup_dimension_combo,
             self.setup_line_selection,
             self.setup_labels_button,
@@ -1133,23 +1237,23 @@
         """Get the rows of the formatoption widgets.
 
         This method should take callable from the :attr:`fmt_setup_functions`
         list and return the rows corresponding to :attr:`formatoption_rows`.
         """
         if func == self.setup_dimension_combo:
             row = [
-                GridCell(QtWidgets.QLabel('x-Dimension:')),
-                GridCell(self.combo_dims)
+                GridCell(QtWidgets.QLabel("x-Dimension:")),
+                GridCell(self.combo_dims),
             ]
         elif func == self.setup_line_selection:
             row = [
-                GridCell(QtWidgets.QLabel('Active line:')),
+                GridCell(QtWidgets.QLabel("Active line:")),
                 GridCell(self.combo_lines),
                 GridCell(self.btn_add),
-                GridCell(self.btn_del)
+                GridCell(self.btn_del),
             ]
         elif func == self.setup_labels_button:
             row = [GridCell(self.btn_labels, colspan=4)]
         else:
             raise ValueError(f"Unknown function {func}")
         return [row]
 
@@ -1169,25 +1273,33 @@
 
         self.combo_lines.setSizePolicy(
             QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding
         )
         self.combo_lines.currentIndexChanged.connect(self.trigger_refresh)
 
         self.btn_add = utils.add_pushbutton(
-            QtGui.QIcon(get_psy_icon('plus')), lambda: self.add_line(),
-            "Add a line to the plot", icon=True)
+            QtGui.QIcon(get_psy_icon("plus")),
+            lambda: self.add_line(),
+            "Add a line to the plot",
+            icon=True,
+        )
         self.btn_del = utils.add_pushbutton(
-            QtGui.QIcon(get_psy_icon('minus')), self.remove_line,
-            "Add a line to the plot", icon=True)
+            QtGui.QIcon(get_psy_icon("minus")),
+            self.remove_line,
+            "Add a line to the plot",
+            icon=True,
+        )
 
     def setup_labels_button(self) -> None:
         """Add a button to modify the text labels."""
         self.btn_labels = utils.add_pushbutton(
-            "Edit labels", self.edit_labels,
-            "Edit title, x-label, legendlabels, etc.")
+            "Edit labels",
+            self.edit_labels,
+            "Edit title, x-label, legendlabels, etc.",
+        )
 
     @property
     def xdim(self) -> str:
         """Get the x-dimension for the plot."""
         return self.combo_dims.currentText()
 
     @xdim.setter
@@ -1219,17 +1331,19 @@
         """
         if not self.sp:
             raise ValueError("No plot has yet been initialized!")
         ds = self.data.psy.base
         xdim = self.xdim
         if name is None:
             name, ok = QtWidgets.QInputDialog.getItem(
-                self, 'New line', 'Select a variable',
-                [key for key, var in ds.items()
-                 if xdim in var.dims])
+                self,
+                "New line",
+                "Select a variable",
+                [key for key, var in ds.items() if xdim in var.dims],
+            )
             if not ok:
                 return
         arr = ds.psy[name]
         for key, val in self.data.psy.idims.items():
             if key in arr.dims:
                 sl.setdefault(key, val)
         for dim in arr.dims:
@@ -1255,20 +1369,22 @@
         self.changed.emit(self.plotmethod)
 
     @property
     def item_texts(self) -> List[str]:
         """Get the labels for the individual lines."""
         if not self.sp:
             return []
-        return [f'Line {i}: {arr.psy._short_info()}'
-                for i, arr in enumerate(self.sp[0])]
+        return [
+            f"Line {i}: {arr.psy._short_info()}"
+            for i, arr in enumerate(self.sp[0])
+        ]
 
     def init_dims(
-            self, var: DataArray
-        ) -> Dict[Union[Hashable, str, Any], Any]:
+        self, var: DataArray
+    ) -> Dict[Union[Hashable, str, Any], Any]:
         """Get the formatoptions for a new plot.
 
         Parameters
         ----------
         var: xarray.Variable
             The variable in the base dataset
 
@@ -1282,42 +1398,44 @@
         ret: Dict[Union[Hashable, str, Any], Any] = {}
         xdim: Union[None, Hashable, str] = self.xdim or next(
             (d for d in var.dims if var[d].size > 1), None  # type: ignore
         )
         if self.array_info:
             arr_names = {}
             for arrname, d in self.array_info.items():
-                if arrname != 'attrs':
-                    dims = d['dims'].copy()
+                if arrname != "attrs":
+                    dims = d["dims"].copy()
                     if xdim in dims:
                         for dim, sl in dims.items():
                             if not isinstance(sl, int):
                                 dims[dim] = 0
                         dims[xdim] = slice(None)
-                    dims['name'] = d['name']
+                    dims["name"] = d["name"]
                     arr_names[arrname] = dims
-            ret['arr_names'] = arr_names
+            ret["arr_names"] = arr_names
             del self.array_info
         else:
             if xdim not in var.dims:
                 xdim = next((d for d in var.dims if var[d].size > 1), None)
             if xdim is None:
                 raise ValueError(
                     f"Cannot plot variable {var.name} with size smaller than "
-                    "2")
+                    "2"
+                )
             ret[xdim] = slice(None)
             for d in var.dims:
                 if d != xdim:
                     ret[d] = 0
         return ret
 
     def edit_labels(self) -> None:
         """Open the dialog to edit the text labels in the plot."""
         dialogs.LabelDialog.update_project(
-            self.sp, 'figtitle', 'title', 'xlabel', 'ylabel', 'legendlabels')
+            self.sp, "figtitle", "title", "xlabel", "ylabel", "legendlabels"
+        )
 
     @contextlib.contextmanager
     def block_combos(self) -> Iterator[None]:
         """Temporarilly block any signal of the combo boxes."""
         self.combo_dims.blockSignals(True)
         self.combo_lines.blockSignals(True)
         yield
@@ -1359,36 +1477,47 @@
     def refresh(self, ds) -> None:
         """Refresh this widget from the given dataset."""
         self.setEnabled(bool(self.sp))
 
         if self.sp:
             with self.block_combos():
                 self.combo_dims.clear()
-                all_dims = list(chain.from_iterable(
-                    [[d for i, d in enumerate(a.dims) if a.shape[i] > 1]
-                     for a in arr.psy.iter_base_variables]
-                    for arr in self.sp[0]))
+                all_dims = list(
+                    chain.from_iterable(
+                        [
+                            [d for i, d in enumerate(a.dims) if a.shape[i] > 1]
+                            for a in arr.psy.iter_base_variables
+                        ]
+                        for arr in self.sp[0]
+                    )
+                )
                 intersection = set(all_dims[0])
                 for dims in all_dims[1:]:
                     intersection.intersection_update(dims)
                 new_dims = list(
-                    filter(lambda d: d in intersection,
-                           unique_everseen(chain.from_iterable(all_dims))))
+                    filter(
+                        lambda d: d in intersection,
+                        unique_everseen(chain.from_iterable(all_dims)),
+                    )
+                )
 
                 self.combo_dims.addItems(new_dims)
                 self.combo_dims.setCurrentIndex(
-                    new_dims.index(self.data.dims[-1]))
+                    new_dims.index(self.data.dims[-1])
+                )
 
                 # fill lines combo
                 current = self.combo_lines.currentIndex()
                 self.combo_lines.clear()
                 descriptions = self.item_texts
                 short_descs = [textwrap.shorten(s, 50) for s in descriptions]
                 self.combo_lines.addItems(short_descs)
                 for i, desc in enumerate(descriptions):
-                    self.combo_lines.setItemData(i, desc, QtCore.Qt.ToolTipRole)
+                    self.combo_lines.setItemData(
+                        i, desc, QtCore.Qt.ToolTipRole
+                    )
                 if current < len(descriptions):
                     self.combo_lines.setCurrentText(short_descs[current])
         else:
             with self.block_combos():
                 self.combo_dims.clear()
                 self.combo_lines.clear()
```

### Comparing `psy-view-0.2.0/psy_view/rcsetup.py` & `psy-view-0.3.0/psy_view/rcsetup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,50 @@
 """Configuration parameters for psy-view."""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-#
-# This file is part of psy-view and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
 from __future__ import annotations
-from typing import (
-    Dict,
-    List,
-    Any,
-    Optional,
-)
 
-from psyplot_gui.config.rcsetup import (
-    RcParams, validate_stringlist, psyplot_fname)
-from psyplot.config.rcsetup import validate_dict
+from typing import Any, Dict, List, Optional
 
+from psyplot.config.rcsetup import validate_dict
+from psyplot_gui.config.rcsetup import (
+    RcParams,
+    psyplot_fname,
+    validate_stringlist,
+)
 
 defaultParams: Dict[str, List[Any]] = {
     "projections": [
         ["cf", "cyl", "robin", "ortho", "moll", "northpole", "southpole"],
-         validate_stringlist, "The names of available projections"],
+        validate_stringlist,
+        "The names of available projections",
+    ],
     "savefig_kws": [
-        dict(dpi=250), validate_dict,
-        "Options that are passed to plt.savefig when exporting images"],
+        dict(dpi=250),
+        validate_dict,
+        "Options that are passed to plt.savefig when exporting images",
+    ],
     "animations.export_kws": [
-        dict(writer="ffmpeg"), validate_dict,
-        "Options that are passed to FuncAnimation.save"],
-    }
+        dict(writer="ffmpeg"),
+        validate_dict,
+        "Options that are passed to FuncAnimation.save",
+    ],
+}
 
 
 class PsyViewRcParams(RcParams):
     """RcParams for the psyplot-gui package."""
 
     HEADER: str = RcParams.HEADER.replace(
-        'psyplotrc.yml', 'psyviewrc.yml').replace(
-            'PSYVIEWRC', 'psyviewrc.yml')
+        "psyplotrc.yml", "psyviewrc.yml"
+    ).replace("PSYVIEWRC", "psyviewrc.yml")
 
     def load_from_file(self, fname: Optional[str] = None):
         """
         Update rcParams from user-defined settings
 
         This function updates the instance with what is found in `fname`
 
@@ -67,16 +54,17 @@
             Path to the yaml configuration file. Possible keys of the
             dictionary are defined by :data:`config.rcsetup.defaultParams`.
             If None, the :func:`config.rcsetup.psyplot_fname` function is used.
 
         See Also
         --------
         dump_to_file, psyplot_fname"""
-        fname = fname or psyplot_fname(env_key='PSYVIEWRC',
-                                       fname='psyviewrc.yml')
+        fname = fname or psyplot_fname(
+            env_key="PSYVIEWRC", fname="psyviewrc.yml"
+        )
         if fname:
             super().load_from_file(fname)
 
 
 rcParams = PsyViewRcParams(defaultParams=defaultParams)
 rcParams.update_from_defaultParams()
 rcParams.load_from_file()
```

