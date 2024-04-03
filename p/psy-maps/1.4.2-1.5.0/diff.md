# Comparing `tmp/psy-maps-1.4.2.tar.gz` & `tmp/psy-maps-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psy-maps-1.4.2.tar", last modified: Fri Apr 15 16:45:40 2022, max compression
+gzip compressed data, was "psy-maps-1.5.0.tar", last modified: Wed Apr  3 17:48:29 2024, max compression
```

## Comparing `psy-maps-1.4.2.tar` & `psy-maps-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,40 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 16:45:40.618892 psy-maps-1.4.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2022-04-15 16:33:11.000000 psy-maps-1.4.2/COPYING
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7652 2022-04-15 16:33:11.000000 psy-maps-1.4.2/COPYING.LESSER
--rw-r--r--   0 circleci  (3434) circleci  (3434)      109 2022-04-15 16:33:11.000000 psy-maps-1.4.2/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5135 2022-04-15 16:45:40.618892 psy-maps-1.4.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3936 2022-04-15 16:33:11.000000 psy-maps-1.4.2/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 16:45:40.618892 psy-maps-1.4.2/psy_maps/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1634 2022-04-15 16:33:11.000000 psy-maps-1.4.2/psy_maps/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      497 2022-04-15 16:45:40.618892 psy-maps-1.4.2/psy_maps/_version.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13349 2022-04-15 16:33:11.000000 psy-maps-1.4.2/psy_maps/boxes.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    78290 2022-04-15 16:33:11.000000 psy-maps-1.4.2/psy_maps/plotters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11064 2022-04-15 16:33:11.000000 psy-maps-1.4.2/psy_maps/plugin.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 16:45:40.618892 psy-maps-1.4.2/psy_maps/widgets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6545 2022-04-15 16:33:11.000000 psy-maps-1.4.2/psy_maps/widgets/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 16:45:40.618892 psy-maps-1.4.2/psy_maps.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5135 2022-04-15 16:45:40.000000 psy-maps-1.4.2/psy_maps.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2022-04-15 16:45:40.000000 psy-maps-1.4.2/psy_maps.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-04-15 16:45:40.000000 psy-maps-1.4.2/psy_maps.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2022-04-15 16:45:40.000000 psy-maps-1.4.2/psy_maps.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-04-15 16:45:40.000000 psy-maps-1.4.2/psy_maps.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2022-04-15 16:45:40.000000 psy-maps-1.4.2/psy_maps.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2022-04-15 16:45:40.000000 psy-maps-1.4.2/psy_maps.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      204 2022-04-15 16:45:40.618892 psy-maps-1.4.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3404 2022-04-15 16:33:11.000000 psy-maps-1.4.2/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    69727 2022-04-15 16:33:11.000000 psy-maps-1.4.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:48:29.099556 psy-maps-1.5.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:48:29.083556 psy-maps-1.5.0/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    17023 2024-04-03 17:47:56.000000 psy-maps-1.5.0/LICENSES/CC-BY-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-03 17:47:56.000000 psy-maps-1.5.0/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    42098 2024-04-03 17:47:56.000000 psy-maps-1.5.0/LICENSES/LGPL-3.0-only.txt
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-03 17:47:56.000000 psy-maps-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5982 2024-04-03 17:48:29.099556 psy-maps-1.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3457 2024-04-03 17:47:56.000000 psy-maps-1.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:48:29.083556 psy-maps-1.5.0/psy_maps/
+-rw-rw-rw-   0 root         (0) root         (0)      749 2024-04-03 17:47:56.000000 psy-maps-1.5.0/psy_maps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-03 17:48:29.103556 psy-maps-1.5.0/psy_maps/_version.py
+-rwxrwxrwx   0 root         (0) root         (0)    12686 2024-04-03 17:47:56.000000 psy-maps-1.5.0/psy_maps/boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)    82105 2024-04-03 17:47:56.000000 psy-maps-1.5.0/psy_maps/plotters.py
+-rw-rw-rw-   0 root         (0) root         (0)    12382 2024-04-03 17:47:56.000000 psy-maps-1.5.0/psy_maps/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:48:29.095556 psy-maps-1.5.0/psy_maps/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     5884 2024-04-03 17:47:56.000000 psy-maps-1.5.0/psy_maps/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:48:29.095556 psy-maps-1.5.0/psy_maps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5982 2024-04-03 17:48:29.000000 psy-maps-1.5.0/psy_maps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      934 2024-04-03 17:48:29.000000 psy-maps-1.5.0/psy_maps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:48:29.000000 psy-maps-1.5.0/psy_maps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-03 17:48:29.000000 psy-maps-1.5.0/psy_maps.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:48:28.000000 psy-maps-1.5.0/psy_maps.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      357 2024-04-03 17:48:29.000000 psy-maps-1.5.0/psy_maps.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-03 17:48:29.000000 psy-maps-1.5.0/psy_maps.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2890 2024-04-03 17:47:56.000000 psy-maps-1.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 17:48:29.099556 psy-maps-1.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      284 2024-04-03 17:47:56.000000 psy-maps-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:48:29.095556 psy-maps-1.5.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     5754 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_base.py
+-rwxrwxrwx   0 root         (0) root         (0)    13043 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_plotters_combinedplotter.py
+-rwxrwxrwx   0 root         (0) root         (0)     6216 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_plotters_combinedplotter_icon.py
+-rwxrwxrwx   0 root         (0) root         (0)    24154 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_plotters_fieldplotter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1366 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_plotters_fieldplotter_contour.py
+-rwxrwxrwx   0 root         (0) root         (0)     1205 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_plotters_fieldplotter_contourf.py
+-rwxrwxrwx   0 root         (0) root         (0)     4828 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_plotters_fieldplotter_icon.py
+-rwxrwxrwx   0 root         (0) root         (0)     3445 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_plotters_fieldplotter_icon_edge.py
+-rwxrwxrwx   0 root         (0) root         (0)     6252 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_plotters_vectorplotter.py
+-rwxrwxrwx   0 root         (0) root         (0)     4432 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_plotters_vectorplotter_icon.py
+-rwxrwxrwx   0 root         (0) root         (0)     2624 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_plotters_vectorplotter_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     5262 2024-04-03 17:47:56.000000 psy-maps-1.5.0/tests/test_projections.py
```

### Comparing `psy-maps-1.4.2/COPYING` & `psy-maps-1.5.0/LICENSES/LGPL-3.0-only.txt`

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

### Comparing `psy-maps-1.4.2/README.rst` & `psy-maps-1.5.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,25 @@
+.. SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 ========================================================
 psy-maps: The psyplot plugin for visualizations on a map
 ========================================================
 
 .. start-badges
 
-.. list-table::
-    :stub-columns: 1
-    :widths: 10 90
-
-    * - docs
-      - |docs|
-    * - tests
-      - |circleci| |appveyor| |codecov|
-    * - package
-      - |version| |conda| |github| |zenodo|
-    * - implementations
-      - |supported-versions| |supported-implementations|
-
-.. |docs| image:: https://img.shields.io/github/deployments/psyplot/psy-maps/github-pages
-    :alt: Documentation
-    :target: http://psyplot.github.io/psy-maps/
-
-.. |circleci| image:: https://circleci.com/gh/psyplot/psy-maps/tree/master.svg?style=svg
-    :alt: CircleCI
-    :target: https://circleci.com/gh/psyplot/psy-maps/tree/master
-
-.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/rd733xj3tfrk4tot/branch/master?svg=true
-    :alt: AppVeyor
-    :target: https://ci.appveyor.com/project/psyplot/psy-maps
-
-.. |codecov| image:: https://codecov.io/gh/psyplot/psy-maps/branch/master/graph/badge.svg
-    :alt: Coverage
-    :target: https://codecov.io/gh/psyplot/psy-maps
-
-.. |version| image:: https://img.shields.io/pypi/v/psy-maps.svg?style=flat
-    :alt: PyPI Package latest release
-    :target: https://pypi.python.org/pypi/psy-maps
-
-.. |conda| image:: https://anaconda.org/conda-forge/psy-maps/badges/version.svg
-    :alt: conda
-    :target: https://anaconda.org/conda-forge/psy-maps
-
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/psy-maps.svg?style=flat
-    :alt: Supported versions
-    :target: https://pypi.python.org/pypi/psy-maps
-
-.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/psy-maps.svg?style=flat
-    :alt: Supported implementations
-    :target: https://pypi.python.org/pypi/psy-maps
-
-.. |zenodo| image:: https://zenodo.org/badge/83305582.svg
-    :alt: Zenodo
-    :target: https://zenodo.org/badge/latestdoi/83305582
-
-.. |github| image:: https://img.shields.io/github/release/psyplot/psy-simple.svg
-    :target: https://github.com/psyplot/psy-simple/releases/latest
-    :alt: Latest github release
-
+|CI|
+|Code coverage|
+|Latest Release|
+|PyPI version|
+|Code style: black|
+|Imports: isort|
+|PEP8|
+|REUSE status|
 
 .. end-badges
 
 Welcome to the psyplot plugin for visualizations on a map. This package uses the
 cartopy_ package to project the plots that are made with the psy-simple_ plugin
 to an earth-referenced grid. It's main plot methods are the
 mapplot_ and mapvector_ plot methods which can plot
@@ -95,7 +54,24 @@
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU LGPL-3.0 license for more details.
 
 You should have received a copy of the GNU LGPL-3.0 license
 along with this program.  If not, see https://www.gnu.org/licenses/.
+
+.. |CI| image:: https://codebase.helmholtz.cloud/psyplot/psy-maps/badges/master/pipeline.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psy-maps/-/pipelines?page=1&scope=all&ref=master
+.. |Code coverage| image:: https://codebase.helmholtz.cloud/psyplot/psy-maps/badges/master/coverage.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psy-maps/-/graphs/master/charts
+.. |Latest Release| image:: https://codebase.helmholtz.cloud/psyplot/psy-maps/-/badges/release.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psy-maps
+.. |PyPI version| image:: https://img.shields.io/pypi/v/psy-maps.svg
+   :target: https://pypi.python.org/pypi/psy-maps/
+.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. |Imports: isort| image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+   :target: https://pycqa.github.io/isort/
+.. |PEP8| image:: https://img.shields.io/badge/code%20style-pep8-orange.svg
+   :target: https://www.python.org/dev/peps/pep-0008/
+.. |REUSE status| image:: https://api.reuse.software/badge/codebase.helmholtz.cloud/psyplot/psy-maps
+   :target: https://api.reuse.software/info/codebase.helmholtz.cloud/psyplot/psy-maps
```

### Comparing `psy-maps-1.4.2/psy_maps/boxes.py` & `psy-maps-1.5.0/psy_maps/boxes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,300 +1,287 @@
 # -*- coding: utf-8 -*-
 """Module defining a dictionary containing longitude-latitude boundary boxes
 for all countries and continents covered by the Vmap0 dataset
 """
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psy-maps and is released under the GNU LGPL-3.O license.
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
 
 #: :class:`dict`. lonlatboxes for different countries and continents
 lonlatboxes = {
-    'Afghanistan': [60.0, 74.0, 29.0, 38.0],
-    'Africa': [-26.0, 63.0, -41.0, 37.0],
-    'Albania': [19.0, 21.0, 39.0, 42.0],
-    'Algeria': [-9.0, 11.0, 18.0, 37.0],
-    'American Samoa': [-172.0, -170.0, -15.0, -12.0],
-    'Andorra': [1.0, 1.0, 42.0, 42.0],
-    'Angola': [11.0, 24.0, -19.0, -5.0],
-    'Anguilla': [-64.0, -63.0, 18.0, 18.0],
-    'Antarctic Area': [-180.0, 180.0, -90.0, -38.0],
-    'Antarctica': [-180.0, 180.0, -90.0, -61.0],
-    'Antigua and Barbuda': [-63.0, -62.0, 16.0, 17.0],
-    'Argentina': [-74.0, -54.0, -56.0, -22.0],
-    'Armenia': [43.0, 46.0, 38.0, 41.0],
-    'Aruba': [-71.0, -70.0, 12.0, 12.0],
-    'Ashmore and Cartier Islands': [122.0, 123.0, -13.0, -13.0],
-    'Asia': [25.0, 190.0, -12.0, 81.0],
-    'Australia': [112.0, 159.0, -55.0, -10.0],
-    'Australian Area': [96.0, 236.0, -55.0, 16.0],
-    'Austria': [9.0, 17.0, 46.0, 49.0],
-    'Azerbaijan': [44.0, 50.0, 38.0, 41.0],
-    'Bahrain': [50.0, 50.0, 25.0, 26.0],
-    'Baker Island': [-177.0, -177.0, 0.0, 0.0],
-    'Bangladesh': [88.0, 92.0, 20.0, 26.0],
-    'Barbados': [-60.0, -60.0, 13.0, 13.0],
-    'Belarus': [23.0, 32.0, 51.0, 56.0],
-    'Belgium': [2.0, 6.0, 49.0, 51.0],
-    'Belize': [-90.0, -88.0, 15.0, 18.0],
-    'Benin': [0.0, 3.0, 6.0, 12.0],
-    'Bermuda': [-65.0, -65.0, 32.0, 32.0],
-    'Bhutan': [88.0, 92.0, 26.0, 28.0],
-    'Bolivia': [-70.0, -58.0, -23.0, -10.0],
-    'Bosnia and Herzegovina': [15.0, 19.0, 42.0, 45.0],
-    'Botswana': [19.0, 29.0, -27.0, -18.0],
-    'Bouvet Island': [3.0, 3.0, -55.0, -55.0],
-    'Brazil': [-74.0, -29.0, -34.0, 5.0],
-    'British Indian Ocean Territory': [71.0, 72.0, -8.0, -6.0],
-    'British Virgin Islands': [-65.0, -65.0, 18.0, 18.0],
-    'Brunei': [114.0, 115.0, 4.0, 5.0],
-    'Bulgaria': [22.0, 28.0, 41.0, 44.0],
-    'Burkina Faso': [-6.0, 2.0, 9.0, 15.0],
-    'Burma': [92.0, 101.0, 9.0, 28.0],
-    'Burundi': [28.0, 30.0, -5.0, -3.0],
-    'Cambodia': [102.0, 107.0, 9.0, 14.0],
-    'Cameroon': [8.0, 16.0, 1.0, 13.0],
-    'Canada': [-141.0, -53.0, 41.0, 83.0],
-    'Cape Verde': [-26.0, -23.0, 14.0, 17.0],
-    'Cayman Islands': [-82.0, -80.0, 19.0, 19.0],
-    'Central African Republic': [14.0, 27.0, 2.0, 11.0],
-    'Chad': [13.0, 24.0, 7.0, 23.0],
-    'Chile': [-110.0, -67.0, -56.0, -18.0],
-    'China': [73.0, 134.0, 18.0, 53.0],
-    'Christmas Island': [105.0, 105.0, -11.0, -11.0],
-    'Clipperton Island': [-110.0, -110.0, 10.0, 10.0],
-    'Cocos (Keeling) Islands': [96.0, 96.0, -13.0, -12.0],
-    'Colombia': [-82.0, -67.0, -5.0, 13.0],
-    'Comoros': [43.0, 44.0, -13.0, -12.0],
-    'Congo': [11.0, 18.0, -6.0, 3.0],
-    'Congo (Democratic Republic of the)': [12.0, 31.0, -14.0, 5.0],
-    'Cook Islands': [-166.0, -158.0, -22.0, -9.0],
-    'Coral Sea Islands': [149.0, 155.0, -18.0, -17.0],
-    'Costa Rica': [-88.0, -83.0, 5.0, 11.0],
+    "Afghanistan": [60.0, 74.0, 29.0, 38.0],
+    "Africa": [-26.0, 63.0, -41.0, 37.0],
+    "Albania": [19.0, 21.0, 39.0, 42.0],
+    "Algeria": [-9.0, 11.0, 18.0, 37.0],
+    "American Samoa": [-172.0, -170.0, -15.0, -12.0],
+    "Andorra": [1.0, 1.0, 42.0, 42.0],
+    "Angola": [11.0, 24.0, -19.0, -5.0],
+    "Anguilla": [-64.0, -63.0, 18.0, 18.0],
+    "Antarctic Area": [-180.0, 180.0, -90.0, -38.0],
+    "Antarctica": [-180.0, 180.0, -90.0, -61.0],
+    "Antigua and Barbuda": [-63.0, -62.0, 16.0, 17.0],
+    "Argentina": [-74.0, -54.0, -56.0, -22.0],
+    "Armenia": [43.0, 46.0, 38.0, 41.0],
+    "Aruba": [-71.0, -70.0, 12.0, 12.0],
+    "Ashmore and Cartier Islands": [122.0, 123.0, -13.0, -13.0],
+    "Asia": [25.0, 190.0, -12.0, 81.0],
+    "Australia": [112.0, 159.0, -55.0, -10.0],
+    "Australian Area": [96.0, 236.0, -55.0, 16.0],
+    "Austria": [9.0, 17.0, 46.0, 49.0],
+    "Azerbaijan": [44.0, 50.0, 38.0, 41.0],
+    "Bahrain": [50.0, 50.0, 25.0, 26.0],
+    "Baker Island": [-177.0, -177.0, 0.0, 0.0],
+    "Bangladesh": [88.0, 92.0, 20.0, 26.0],
+    "Barbados": [-60.0, -60.0, 13.0, 13.0],
+    "Belarus": [23.0, 32.0, 51.0, 56.0],
+    "Belgium": [2.0, 6.0, 49.0, 51.0],
+    "Belize": [-90.0, -88.0, 15.0, 18.0],
+    "Benin": [0.0, 3.0, 6.0, 12.0],
+    "Bermuda": [-65.0, -65.0, 32.0, 32.0],
+    "Bhutan": [88.0, 92.0, 26.0, 28.0],
+    "Bolivia": [-70.0, -58.0, -23.0, -10.0],
+    "Bosnia and Herzegovina": [15.0, 19.0, 42.0, 45.0],
+    "Botswana": [19.0, 29.0, -27.0, -18.0],
+    "Bouvet Island": [3.0, 3.0, -55.0, -55.0],
+    "Brazil": [-74.0, -29.0, -34.0, 5.0],
+    "British Indian Ocean Territory": [71.0, 72.0, -8.0, -6.0],
+    "British Virgin Islands": [-65.0, -65.0, 18.0, 18.0],
+    "Brunei": [114.0, 115.0, 4.0, 5.0],
+    "Bulgaria": [22.0, 28.0, 41.0, 44.0],
+    "Burkina Faso": [-6.0, 2.0, 9.0, 15.0],
+    "Burma": [92.0, 101.0, 9.0, 28.0],
+    "Burundi": [28.0, 30.0, -5.0, -3.0],
+    "Cambodia": [102.0, 107.0, 9.0, 14.0],
+    "Cameroon": [8.0, 16.0, 1.0, 13.0],
+    "Canada": [-141.0, -53.0, 41.0, 83.0],
+    "Cape Verde": [-26.0, -23.0, 14.0, 17.0],
+    "Cayman Islands": [-82.0, -80.0, 19.0, 19.0],
+    "Central African Republic": [14.0, 27.0, 2.0, 11.0],
+    "Chad": [13.0, 24.0, 7.0, 23.0],
+    "Chile": [-110.0, -67.0, -56.0, -18.0],
+    "China": [73.0, 134.0, 18.0, 53.0],
+    "Christmas Island": [105.0, 105.0, -11.0, -11.0],
+    "Clipperton Island": [-110.0, -110.0, 10.0, 10.0],
+    "Cocos (Keeling) Islands": [96.0, 96.0, -13.0, -12.0],
+    "Colombia": [-82.0, -67.0, -5.0, 13.0],
+    "Comoros": [43.0, 44.0, -13.0, -12.0],
+    "Congo": [11.0, 18.0, -6.0, 3.0],
+    "Congo (Democratic Republic of the)": [12.0, 31.0, -14.0, 5.0],
+    "Cook Islands": [-166.0, -158.0, -22.0, -9.0],
+    "Coral Sea Islands": [149.0, 155.0, -18.0, -17.0],
+    "Costa Rica": [-88.0, -83.0, 5.0, 11.0],
     "Cote D'Ivoire": [-9.0, -3.0, 4.0, 10.0],
-    'Croatia': [13.0, 19.0, 42.0, 46.0],
-    'Cuba': [-85.0, -75.0, 19.0, 23.0],
-    'Cyprus': [32.0, 34.0, 34.0, 35.0],
-    'Czech Republic': [12.0, 18.0, 48.0, 51.0],
-    'Denmark': [8.0, 15.0, 54.0, 57.0],
-    'Djibouti': [41.0, 43.0, 10.0, 12.0],
-    'Dominica': [-62.0, -62.0, 15.0, 15.0],
-    'Dominican Republic': [-73.0, -69.0, 17.0, 19.0],
-    'Ecuador': [-93.0, -76.0, -5.0, 1.0],
-    'Egypt': [24.0, 36.0, 21.0, 31.0],
-    'El Salvador': [-91.0, -88.0, 13.0, 14.0],
-    'Equatorial Guinea': [5.0, 11.0, -2.0, 3.0],
-    'Eritrea': [36.0, 43.0, 12.0, 18.0],
-    'Estonia': [21.0, 28.0, 57.0, 59.0],
-    'Ethiopia': [32.0, 47.0, 3.0, 14.0],
-    'Europa Island': [40.0, 40.0, -23.0, -23.0],
-    'Europe': [-32.0, 69.0, 34.0, 81.0],
-    'Falkland Islands (Islas Malvinas)': [-62.0, -58.0, -53.0, -52.0],
-    'Faroe Islands': [-8.0, -7.0, 61.0, 62.0],
-    'Federated States of Micronesia': [138.0, 163.0, 5.0, 11.0],
-    'Fiji': [175.0, 182.0, -21.0, -13.0],
-    'Finland': [19.0, 31.0, 59.0, 70.0],
-    'France': [-6.0, 9.0, 41.0, 51.0],
-    'French Guiana': [-55.0, -52.0, 2.0, 5.0],
-    'French Polynesia': [-155.0, -135.0, -28.0, -8.0],
-    'French Southern and Antarctic Lands': [50.0, 77.0, -51.0, -38.0],
-    'Gabon': [8.0, 14.0, -4.0, 2.0],
-    'Gaza Strip': [34.0, 34.0, 31.0, 31.0],
-    'Georgia': [40.0, 46.0, 41.0, 43.0],
-    'Germany': [5.0, 15.0, 47.0, 55.0],
-    'Ghana': [-4.0, 1.0, 4.0, 11.0],
-    'Gibraltar': [-6.0, -6.0, 36.0, 36.0],
-    'Glorioso Islands': [47.0, 47.0, -12.0, -12.0],
-    'Greece': [19.0, 29.0, 34.0, 41.0],
-    'Greenland': [-74.0, -12.0, 59.0, 83.0],
-    'Grenada': [-62.0, -62.0, 11.0, 12.0],
-    'Guadeloupe': [-64.0, -61.0, 15.0, 18.0],
-    'Guam': [144.0, 144.0, 13.0, 13.0],
-    'Guatemala': [-93.0, -89.0, 13.0, 17.0],
-    'Guernsey': [-3.0, -3.0, 49.0, 49.0],
-    'Guinea': [-16.0, -8.0, 7.0, 12.0],
-    'Guinea-Bissau': [-17.0, -14.0, 10.0, 12.0],
-    'Guyana': [-62.0, -57.0, 1.0, 8.0],
-    'Haiti': [-75.0, -72.0, 18.0, 20.0],
-    'Heard Island and McDonald Islands': [72.0, 73.0, -54.0, -53.0],
-    'Honduras': [-90.0, -84.0, 12.0, 17.0],
-    'Hong Kong': [113.0, 114.0, 22.0, 22.0],
-    'Howland Island': [-177.0, -177.0, 0.0, 0.0],
-    'Hungary': [16.0, 22.0, 45.0, 48.0],
-    'Iceland': [-25.0, -14.0, 63.0, 66.0],
-    'India': [68.0, 97.0, 6.0, 35.0],
-    'Indonesia': [95.0, 141.0, -12.0, 5.0],
-    'Iran': [44.0, 63.0, 25.0, 39.0],
-    'Iraq': [38.0, 48.0, 29.0, 37.0],
-    'Ireland': [-11.0, -7.0, 51.0, 55.0],
-    'Isle of Man': [-5.0, -5.0, 54.0, 54.0],
-    'Israel': [34.0, 35.0, 29.0, 33.0],
-    'Italy': [6.0, 18.0, 35.0, 47.0],
-    'Jamaica': [-79.0, -77.0, 17.0, 18.0],
-    'Jan Mayen': [-10.0, -8.0, 70.0, 71.0],
-    'Japan': [122.0, 153.0, 24.0, 45.0],
-    'Jarvis Island': [-161.0, -161.0, -1.0, -1.0],
-    'Jersey': [-3.0, -3.0, 49.0, 49.0],
-    'Johnston Atoll': [-170.0, -170.0, 16.0, 16.0],
-    'Jordan': [34.0, 39.0, 29.0, 33.0],
-    'Juan De Nova Island': [42.0, 42.0, -18.0, -18.0],
-    'Kazakhstan': [46.0, 87.0, 40.0, 55.0],
-    'Kenya': [33.0, 41.0, -5.0, 4.0],
-    'Kingman Reef': [-163.0, -163.0, 6.0, 6.0],
-    'Kiribati': [168.0, 210.0, -12.0, 4.0],
-    'Kuwait': [46.0, 48.0, 28.0, 30.0],
-    'Kyrgyzstan': [69.0, 80.0, 39.0, 43.0],
-    'Laos': [100.0, 107.0, 13.0, 22.0],
-    'Latvia': [20.0, 28.0, 55.0, 58.0],
-    'Lebanon': [35.0, 36.0, 33.0, 34.0],
-    'Lesotho': [27.0, 29.0, -31.0, -29.0],
-    'Liberia': [-12.0, -8.0, 4.0, 8.0],
-    'Libya': [9.0, 25.0, 19.0, 33.0],
-    'Liechtenstein': [9.0, 9.0, 47.0, 47.0],
-    'Lithuania': [20.0, 26.0, 53.0, 56.0],
-    'Luxembourg': [5.0, 6.0, 49.0, 50.0],
-    'Macau': [113.0, 113.0, 22.0, 22.0],
-    'Madagascar': [43.0, 50.0, -26.0, -12.0],
-    'Malawi': [32.0, 35.0, -18.0, -10.0],
-    'Malaysia': [98.0, 119.0, 0.0, 7.0],
-    'Maldives': [72.0, 73.0, -1.0, 7.0],
-    'Mali': [-13.0, 4.0, 10.0, 25.0],
-    'Malta': [14.0, 14.0, 35.0, 36.0],
-    'Marshall Islands': [165.0, 172.0, 4.0, 14.0],
-    'Martinique': [-62.0, -61.0, 14.0, 14.0],
-    'Mauritania': [-18.0, -5.0, 14.0, 27.0],
-    'Mauritius': [56.0, 63.0, -21.0, -11.0],
-    'Mayotte': [45.0, 45.0, -14.0, -13.0],
-    'Mexico': [-119.0, -87.0, 14.0, 32.0],
-    'Midway Islands': [-179.0, -178.0, 28.0, 28.0],
-    'Moldova': [26.0, 30.0, 45.0, 48.0],
-    'Monaco': [7.0, 7.0, 43.0, 43.0],
-    'Mongolia': [87.0, 119.0, 41.0, 52.0],
-    'Montenegro': [18.0, 20.0, 41.0, 43.0],
-    'Montserrat': [-63.0, -63.0, 16.0, 16.0],
-    'Morocco': [-14.0, -1.0, 27.0, 35.0],
-    'Mozambique': [30.0, 40.0, -27.0, -11.0],
-    'Namibia': [11.0, 25.0, -29.0, -17.0],
-    'Nauru': [166.0, 166.0, -1.0, -1.0],
-    'Navassa Island': [-76.0, -75.0, 18.0, 18.0],
-    'Nepal': [80.0, 88.0, 26.0, 30.0],
-    'Netherlands': [3.0, 7.0, 50.0, 53.0],
-    'Netherlands Antilles': [-70.0, -63.0, 11.0, 18.0],
-    'New Caledonia': [158.0, 172.0, -23.0, -20.0],
-    'New Zealand': [166.0, 185.0, -53.0, -30.0],
-    'Nicaragua': [-88.0, -83.0, 10.0, 15.0],
-    'Niger': [0.0, 15.0, 11.0, 23.0],
-    'Nigeria': [2.0, 14.0, 4.0, 13.0],
-    'Niue': [-170.0, -170.0, -20.0, -19.0],
-    'Norfolk Island': [167.0, 168.0, -30.0, -29.0],
-    'North America': [172.0, 349.0, 5.0, 83.0],
-    'North Korea': [124.0, 130.0, 37.0, 43.0],
-    'Northern Mariana Islands': [144.0, 146.0, 14.0, 20.0],
-    'Norway': [4.0, 31.0, 57.0, 79.0],
-    'Oman': [52.0, 59.0, 16.0, 26.0],
-    'Other': [34.0, 43.0, 17.0, 31.0],
-    'Pakistan': [60.0, 77.0, 23.0, 37.0],
-    'Palau': [131.0, 134.0, 3.0, 8.0],
-    'Palmyra Atoll': [-163.0, -163.0, 5.0, 5.0],
-    'Panama': [-84.0, -78.0, 7.0, 9.0],
-    'Papua New Guinea': [140.0, 159.0, -12.0, -1.0],
-    'Paracel Islands': [111.0, 112.0, 15.0, 16.0],
-    'Paraguay': [-63.0, -55.0, -28.0, -20.0],
-    'Peru': [-82.0, -69.0, -19.0, -1.0],
-    'Philippines': [116.0, 126.0, 4.0, 21.0],
-    'Pitcairn Islands': [-131.0, -125.0, -26.0, -24.0],
-    'Poland': [14.0, 24.0, 49.0, 54.0],
-    'Portugal': [-32.0, -7.0, 30.0, 42.0],
-    'Puerto Rico': [-68.0, -66.0, 17.0, 18.0],
-    'Qatar': [50.0, 52.0, 24.0, 26.0],
-    'Reunion': [55.0, 55.0, -22.0, -21.0],
-    'Romania': [20.0, 29.0, 43.0, 48.0],
-    'Russia': [18.0, 191.0, 41.0, 81.0],
-    'Rwanda': [28.0, 30.0, -3.0, -2.0],
-    'Saint Helena': [-15.0, -6.0, -41.0, -8.0],
-    'Saint Kitts and Nevis': [-63.0, -63.0, 17.0, 17.0],
-    'Saint Lucia': [-62.0, -61.0, 13.0, 14.0],
-    'Saint Pierre and Miquelon': [-57.0, -57.0, 46.0, 47.0],
-    'Saint Vincent and the Grenadines': [-62.0, -62.0, 12.0, 13.0],
-    'Samoa': [-173.0, -172.0, -15.0, -14.0],
-    'San Marino': [12.0, 12.0, 43.0, 43.0],
-    'Sao Tome and Principe': [6.0, 7.0, -1.0, 1.0],
-    'Saudi Arabia': [34.0, 55.0, 15.0, 32.0],
-    'Senegal': [-18.0, -12.0, 12.0, 16.0],
-    'Serbia': [18.0, 23.0, 41.0, 46.0],
-    'Seychelles': [46.0, 56.0, -11.0, -4.0],
-    'Sierra Leone': [-14.0, -11.0, 6.0, 10.0],
-    'Singapore': [103.0, 104.0, 1.0, 1.0],
-    'Slovakia': [16.0, 22.0, 47.0, 49.0],
-    'Slovenia': [13.0, 16.0, 45.0, 46.0],
-    'Solomon Islands': [155.0, 168.0, -13.0, -6.0],
-    'Somalia': [40.0, 51.0, -2.0, 11.0],
-    'South Africa': [16.0, 38.0, -47.0, -23.0],
-    'South America': [-110.0, -29.0, -56.0, 13.0],
-    'South Georgia and the South Sandwich Islands': [
-        -42.0, -27.0, -60.0, -54.0],
-    'South Korea': [124.0, 130.0, 33.0, 38.0],
-    'Spain': [-19.0, 4.0, 27.0, 43.0],
-    'Spratly Islands': [114.0, 115.0, 9.0, 11.0],
-    'Sri Lanka': [79.0, 81.0, 5.0, 9.0],
-    'Sudan': [21.0, 38.0, 3.0, 23.0],
-    'Suriname': [-59.0, -54.0, 1.0, 6.0],
-    'Svalbard': [10.0, 36.0, 74.0, 80.0],
-    'Swaziland': [30.0, 32.0, -28.0, -26.0],
-    'Sweden': [10.0, 24.0, 55.0, 69.0],
-    'Switzerland': [5.0, 10.0, 45.0, 47.0],
-    'Syria': [35.0, 42.0, 32.0, 37.0],
-    'Taiwan': [116.0, 122.0, 20.0, 26.0],
-    'Tajikistan': [67.0, 75.0, 36.0, 41.0],
-    'Tanzania': [29.0, 40.0, -12.0, -1.0],
-    'Thailand': [97.0, 105.0, 5.0, 20.0],
-    'The Bahamas': [-81.0, -73.0, 20.0, 27.0],
-    'The Former Yugoslav Republic of Macedonia': [20.0, 23.0, 40.0, 42.0],
-    'The Gambia': [-17.0, -14.0, 13.0, 13.0],
-    'Togo': [-1.0, 1.0, 6.0, 11.0],
-    'Tokelau': [-173.0, -172.0, -10.0, -9.0],
-    'Tonga': [-177.0, -174.0, -23.0, -16.0],
-    'Trinidad and Tobago': [-62.0, -61.0, 10.0, 11.0],
-    'Tromelin Island': [54.0, 54.0, -16.0, -16.0],
-    'Tunisia': [7.0, 11.0, 30.0, 37.0],
-    'Turkey': [25.0, 44.0, 35.0, 42.0],
-    'Turkmenistan': [52.0, 66.0, 35.0, 42.0],
-    'Turks and Caicas Islands': [-73.0, -72.0, 21.0, 21.0],
-    'Tuvalu': [176.0, 179.0, -10.0, -6.0],
-    'Uganda': [29.0, 35.0, -2.0, 4.0],
-    'Ukraine': [22.0, 40.0, 44.0, 52.0],
-    'United Arab Emirates': [51.0, 56.0, 22.0, 26.0],
-    'United Kingdom': [-9.0, 33.0, 34.0, 60.0],
-    'United States': [172.0, 294.0, 18.0, 71.0],
-    'Uruguay': [-59.0, -54.0, -36.0, -31.0],
-    'Uzbekistan': [55.0, 73.0, 37.0, 45.0],
-    'Vanuatu': [166.0, 170.0, -21.0, -14.0],
-    'Vatican City': [12.0, 12.0, 41.0, 41.0],
-    'Venezuela': [-74.0, -60.0, 0.0, 12.0],
-    'Vietnam': [102.0, 109.0, 8.0, 23.0],
-    'Virgin Islands': [-66.0, -65.0, 17.0, 18.0],
-    'Wake Island': [166.0, 166.0, 19.0, 19.0],
-    'Wallis and Futuna': [-179.0, -177.0, -15.0, -14.0],
-    'Western Sahara': [-18.0, -9.0, 20.0, 27.0],
-    'Yemen': [41.0, 54.0, 12.0, 19.0],
-    'Zambia': [21.0, 33.0, -19.0, -9.0],
-    'Zimbabwe': [25.0, 33.0, -23.0, -16.0]
-    }
+    "Croatia": [13.0, 19.0, 42.0, 46.0],
+    "Cuba": [-85.0, -75.0, 19.0, 23.0],
+    "Cyprus": [32.0, 34.0, 34.0, 35.0],
+    "Czech Republic": [12.0, 18.0, 48.0, 51.0],
+    "Denmark": [8.0, 15.0, 54.0, 57.0],
+    "Djibouti": [41.0, 43.0, 10.0, 12.0],
+    "Dominica": [-62.0, -62.0, 15.0, 15.0],
+    "Dominican Republic": [-73.0, -69.0, 17.0, 19.0],
+    "Ecuador": [-93.0, -76.0, -5.0, 1.0],
+    "Egypt": [24.0, 36.0, 21.0, 31.0],
+    "El Salvador": [-91.0, -88.0, 13.0, 14.0],
+    "Equatorial Guinea": [5.0, 11.0, -2.0, 3.0],
+    "Eritrea": [36.0, 43.0, 12.0, 18.0],
+    "Estonia": [21.0, 28.0, 57.0, 59.0],
+    "Ethiopia": [32.0, 47.0, 3.0, 14.0],
+    "Europa Island": [40.0, 40.0, -23.0, -23.0],
+    "Europe": [-32.0, 69.0, 34.0, 81.0],
+    "Falkland Islands (Islas Malvinas)": [-62.0, -58.0, -53.0, -52.0],
+    "Faroe Islands": [-8.0, -7.0, 61.0, 62.0],
+    "Federated States of Micronesia": [138.0, 163.0, 5.0, 11.0],
+    "Fiji": [175.0, 182.0, -21.0, -13.0],
+    "Finland": [19.0, 31.0, 59.0, 70.0],
+    "France": [-6.0, 9.0, 41.0, 51.0],
+    "French Guiana": [-55.0, -52.0, 2.0, 5.0],
+    "French Polynesia": [-155.0, -135.0, -28.0, -8.0],
+    "French Southern and Antarctic Lands": [50.0, 77.0, -51.0, -38.0],
+    "Gabon": [8.0, 14.0, -4.0, 2.0],
+    "Gaza Strip": [34.0, 34.0, 31.0, 31.0],
+    "Georgia": [40.0, 46.0, 41.0, 43.0],
+    "Germany": [5.0, 15.0, 47.0, 55.0],
+    "Ghana": [-4.0, 1.0, 4.0, 11.0],
+    "Gibraltar": [-6.0, -6.0, 36.0, 36.0],
+    "Glorioso Islands": [47.0, 47.0, -12.0, -12.0],
+    "Greece": [19.0, 29.0, 34.0, 41.0],
+    "Greenland": [-74.0, -12.0, 59.0, 83.0],
+    "Grenada": [-62.0, -62.0, 11.0, 12.0],
+    "Guadeloupe": [-64.0, -61.0, 15.0, 18.0],
+    "Guam": [144.0, 144.0, 13.0, 13.0],
+    "Guatemala": [-93.0, -89.0, 13.0, 17.0],
+    "Guernsey": [-3.0, -3.0, 49.0, 49.0],
+    "Guinea": [-16.0, -8.0, 7.0, 12.0],
+    "Guinea-Bissau": [-17.0, -14.0, 10.0, 12.0],
+    "Guyana": [-62.0, -57.0, 1.0, 8.0],
+    "Haiti": [-75.0, -72.0, 18.0, 20.0],
+    "Heard Island and McDonald Islands": [72.0, 73.0, -54.0, -53.0],
+    "Honduras": [-90.0, -84.0, 12.0, 17.0],
+    "Hong Kong": [113.0, 114.0, 22.0, 22.0],
+    "Howland Island": [-177.0, -177.0, 0.0, 0.0],
+    "Hungary": [16.0, 22.0, 45.0, 48.0],
+    "Iceland": [-25.0, -14.0, 63.0, 66.0],
+    "India": [68.0, 97.0, 6.0, 35.0],
+    "Indonesia": [95.0, 141.0, -12.0, 5.0],
+    "Iran": [44.0, 63.0, 25.0, 39.0],
+    "Iraq": [38.0, 48.0, 29.0, 37.0],
+    "Ireland": [-11.0, -7.0, 51.0, 55.0],
+    "Isle of Man": [-5.0, -5.0, 54.0, 54.0],
+    "Israel": [34.0, 35.0, 29.0, 33.0],
+    "Italy": [6.0, 18.0, 35.0, 47.0],
+    "Jamaica": [-79.0, -77.0, 17.0, 18.0],
+    "Jan Mayen": [-10.0, -8.0, 70.0, 71.0],
+    "Japan": [122.0, 153.0, 24.0, 45.0],
+    "Jarvis Island": [-161.0, -161.0, -1.0, -1.0],
+    "Jersey": [-3.0, -3.0, 49.0, 49.0],
+    "Johnston Atoll": [-170.0, -170.0, 16.0, 16.0],
+    "Jordan": [34.0, 39.0, 29.0, 33.0],
+    "Juan De Nova Island": [42.0, 42.0, -18.0, -18.0],
+    "Kazakhstan": [46.0, 87.0, 40.0, 55.0],
+    "Kenya": [33.0, 41.0, -5.0, 4.0],
+    "Kingman Reef": [-163.0, -163.0, 6.0, 6.0],
+    "Kiribati": [168.0, 210.0, -12.0, 4.0],
+    "Kuwait": [46.0, 48.0, 28.0, 30.0],
+    "Kyrgyzstan": [69.0, 80.0, 39.0, 43.0],
+    "Laos": [100.0, 107.0, 13.0, 22.0],
+    "Latvia": [20.0, 28.0, 55.0, 58.0],
+    "Lebanon": [35.0, 36.0, 33.0, 34.0],
+    "Lesotho": [27.0, 29.0, -31.0, -29.0],
+    "Liberia": [-12.0, -8.0, 4.0, 8.0],
+    "Libya": [9.0, 25.0, 19.0, 33.0],
+    "Liechtenstein": [9.0, 9.0, 47.0, 47.0],
+    "Lithuania": [20.0, 26.0, 53.0, 56.0],
+    "Luxembourg": [5.0, 6.0, 49.0, 50.0],
+    "Macau": [113.0, 113.0, 22.0, 22.0],
+    "Madagascar": [43.0, 50.0, -26.0, -12.0],
+    "Malawi": [32.0, 35.0, -18.0, -10.0],
+    "Malaysia": [98.0, 119.0, 0.0, 7.0],
+    "Maldives": [72.0, 73.0, -1.0, 7.0],
+    "Mali": [-13.0, 4.0, 10.0, 25.0],
+    "Malta": [14.0, 14.0, 35.0, 36.0],
+    "Marshall Islands": [165.0, 172.0, 4.0, 14.0],
+    "Martinique": [-62.0, -61.0, 14.0, 14.0],
+    "Mauritania": [-18.0, -5.0, 14.0, 27.0],
+    "Mauritius": [56.0, 63.0, -21.0, -11.0],
+    "Mayotte": [45.0, 45.0, -14.0, -13.0],
+    "Mexico": [-119.0, -87.0, 14.0, 32.0],
+    "Midway Islands": [-179.0, -178.0, 28.0, 28.0],
+    "Moldova": [26.0, 30.0, 45.0, 48.0],
+    "Monaco": [7.0, 7.0, 43.0, 43.0],
+    "Mongolia": [87.0, 119.0, 41.0, 52.0],
+    "Montenegro": [18.0, 20.0, 41.0, 43.0],
+    "Montserrat": [-63.0, -63.0, 16.0, 16.0],
+    "Morocco": [-14.0, -1.0, 27.0, 35.0],
+    "Mozambique": [30.0, 40.0, -27.0, -11.0],
+    "Namibia": [11.0, 25.0, -29.0, -17.0],
+    "Nauru": [166.0, 166.0, -1.0, -1.0],
+    "Navassa Island": [-76.0, -75.0, 18.0, 18.0],
+    "Nepal": [80.0, 88.0, 26.0, 30.0],
+    "Netherlands": [3.0, 7.0, 50.0, 53.0],
+    "Netherlands Antilles": [-70.0, -63.0, 11.0, 18.0],
+    "New Caledonia": [158.0, 172.0, -23.0, -20.0],
+    "New Zealand": [166.0, 185.0, -53.0, -30.0],
+    "Nicaragua": [-88.0, -83.0, 10.0, 15.0],
+    "Niger": [0.0, 15.0, 11.0, 23.0],
+    "Nigeria": [2.0, 14.0, 4.0, 13.0],
+    "Niue": [-170.0, -170.0, -20.0, -19.0],
+    "Norfolk Island": [167.0, 168.0, -30.0, -29.0],
+    "North America": [172.0, 349.0, 5.0, 83.0],
+    "North Korea": [124.0, 130.0, 37.0, 43.0],
+    "Northern Mariana Islands": [144.0, 146.0, 14.0, 20.0],
+    "Norway": [4.0, 31.0, 57.0, 79.0],
+    "Oman": [52.0, 59.0, 16.0, 26.0],
+    "Other": [34.0, 43.0, 17.0, 31.0],
+    "Pakistan": [60.0, 77.0, 23.0, 37.0],
+    "Palau": [131.0, 134.0, 3.0, 8.0],
+    "Palmyra Atoll": [-163.0, -163.0, 5.0, 5.0],
+    "Panama": [-84.0, -78.0, 7.0, 9.0],
+    "Papua New Guinea": [140.0, 159.0, -12.0, -1.0],
+    "Paracel Islands": [111.0, 112.0, 15.0, 16.0],
+    "Paraguay": [-63.0, -55.0, -28.0, -20.0],
+    "Peru": [-82.0, -69.0, -19.0, -1.0],
+    "Philippines": [116.0, 126.0, 4.0, 21.0],
+    "Pitcairn Islands": [-131.0, -125.0, -26.0, -24.0],
+    "Poland": [14.0, 24.0, 49.0, 54.0],
+    "Portugal": [-32.0, -7.0, 30.0, 42.0],
+    "Puerto Rico": [-68.0, -66.0, 17.0, 18.0],
+    "Qatar": [50.0, 52.0, 24.0, 26.0],
+    "Reunion": [55.0, 55.0, -22.0, -21.0],
+    "Romania": [20.0, 29.0, 43.0, 48.0],
+    "Russia": [18.0, 191.0, 41.0, 81.0],
+    "Rwanda": [28.0, 30.0, -3.0, -2.0],
+    "Saint Helena": [-15.0, -6.0, -41.0, -8.0],
+    "Saint Kitts and Nevis": [-63.0, -63.0, 17.0, 17.0],
+    "Saint Lucia": [-62.0, -61.0, 13.0, 14.0],
+    "Saint Pierre and Miquelon": [-57.0, -57.0, 46.0, 47.0],
+    "Saint Vincent and the Grenadines": [-62.0, -62.0, 12.0, 13.0],
+    "Samoa": [-173.0, -172.0, -15.0, -14.0],
+    "San Marino": [12.0, 12.0, 43.0, 43.0],
+    "Sao Tome and Principe": [6.0, 7.0, -1.0, 1.0],
+    "Saudi Arabia": [34.0, 55.0, 15.0, 32.0],
+    "Senegal": [-18.0, -12.0, 12.0, 16.0],
+    "Serbia": [18.0, 23.0, 41.0, 46.0],
+    "Seychelles": [46.0, 56.0, -11.0, -4.0],
+    "Sierra Leone": [-14.0, -11.0, 6.0, 10.0],
+    "Singapore": [103.0, 104.0, 1.0, 1.0],
+    "Slovakia": [16.0, 22.0, 47.0, 49.0],
+    "Slovenia": [13.0, 16.0, 45.0, 46.0],
+    "Solomon Islands": [155.0, 168.0, -13.0, -6.0],
+    "Somalia": [40.0, 51.0, -2.0, 11.0],
+    "South Africa": [16.0, 38.0, -47.0, -23.0],
+    "South America": [-110.0, -29.0, -56.0, 13.0],
+    "South Georgia and the South Sandwich Islands": [
+        -42.0,
+        -27.0,
+        -60.0,
+        -54.0,
+    ],
+    "South Korea": [124.0, 130.0, 33.0, 38.0],
+    "Spain": [-19.0, 4.0, 27.0, 43.0],
+    "Spratly Islands": [114.0, 115.0, 9.0, 11.0],
+    "Sri Lanka": [79.0, 81.0, 5.0, 9.0],
+    "Sudan": [21.0, 38.0, 3.0, 23.0],
+    "Suriname": [-59.0, -54.0, 1.0, 6.0],
+    "Svalbard": [10.0, 36.0, 74.0, 80.0],
+    "Swaziland": [30.0, 32.0, -28.0, -26.0],
+    "Sweden": [10.0, 24.0, 55.0, 69.0],
+    "Switzerland": [5.0, 10.0, 45.0, 47.0],
+    "Syria": [35.0, 42.0, 32.0, 37.0],
+    "Taiwan": [116.0, 122.0, 20.0, 26.0],
+    "Tajikistan": [67.0, 75.0, 36.0, 41.0],
+    "Tanzania": [29.0, 40.0, -12.0, -1.0],
+    "Thailand": [97.0, 105.0, 5.0, 20.0],
+    "The Bahamas": [-81.0, -73.0, 20.0, 27.0],
+    "The Former Yugoslav Republic of Macedonia": [20.0, 23.0, 40.0, 42.0],
+    "The Gambia": [-17.0, -14.0, 13.0, 13.0],
+    "Togo": [-1.0, 1.0, 6.0, 11.0],
+    "Tokelau": [-173.0, -172.0, -10.0, -9.0],
+    "Tonga": [-177.0, -174.0, -23.0, -16.0],
+    "Trinidad and Tobago": [-62.0, -61.0, 10.0, 11.0],
+    "Tromelin Island": [54.0, 54.0, -16.0, -16.0],
+    "Tunisia": [7.0, 11.0, 30.0, 37.0],
+    "Turkey": [25.0, 44.0, 35.0, 42.0],
+    "Turkmenistan": [52.0, 66.0, 35.0, 42.0],
+    "Turks and Caicas Islands": [-73.0, -72.0, 21.0, 21.0],
+    "Tuvalu": [176.0, 179.0, -10.0, -6.0],
+    "Uganda": [29.0, 35.0, -2.0, 4.0],
+    "Ukraine": [22.0, 40.0, 44.0, 52.0],
+    "United Arab Emirates": [51.0, 56.0, 22.0, 26.0],
+    "United Kingdom": [-9.0, 33.0, 34.0, 60.0],
+    "United States": [172.0, 294.0, 18.0, 71.0],
+    "Uruguay": [-59.0, -54.0, -36.0, -31.0],
+    "Uzbekistan": [55.0, 73.0, 37.0, 45.0],
+    "Vanuatu": [166.0, 170.0, -21.0, -14.0],
+    "Vatican City": [12.0, 12.0, 41.0, 41.0],
+    "Venezuela": [-74.0, -60.0, 0.0, 12.0],
+    "Vietnam": [102.0, 109.0, 8.0, 23.0],
+    "Virgin Islands": [-66.0, -65.0, 17.0, 18.0],
+    "Wake Island": [166.0, 166.0, 19.0, 19.0],
+    "Wallis and Futuna": [-179.0, -177.0, -15.0, -14.0],
+    "Western Sahara": [-18.0, -9.0, 20.0, 27.0],
+    "Yemen": [41.0, 54.0, 12.0, 19.0],
+    "Zambia": [21.0, 33.0, -19.0, -9.0],
+    "Zimbabwe": [25.0, 33.0, -23.0, -16.0],
+}
```

### Comparing `psy-maps-1.4.2/psy_maps/plotters.py` & `psy-maps-1.5.0/psy_maps/plotters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,59 @@
 """Plotters and formatoption of the psy-maps psyplot plugin."""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psy-maps and is released under the GNU LGPL-3.O license.
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
 
-import six
+import copy
 import re
 import warnings
 from abc import abstractproperty
 from difflib import get_close_matches
-import copy
-from itertools import starmap, chain, repeat
+from itertools import chain, repeat, starmap
+
 import cartopy
 import cartopy.crs as ccrs
 import cartopy.feature as cf
-from cartopy.mpl.gridliner import Gridliner
 import matplotlib as mpl
 import matplotlib.ticker as ticker
-from matplotlib.colors import BoundaryNorm
 import numpy as np
+import psy_simple.base
+import psy_simple.plotters as psyps
+import six
+from cartopy.mpl.gridliner import Gridliner
+from matplotlib.colors import BoundaryNorm
+from psy_simple.colors import FixedBoundaryNorm
 from psyplot import rcParams
-from psyplot.compat.pycompat import map
-from psyplot.docstring import docstrings
 from psyplot.data import InteractiveList, _infer_interval_breaks
+from psyplot.docstring import docstrings
 from psyplot.plotter import (
-    Formatoption, START, DictFormatoption, END, BEFOREPLOTTING)
-import psy_simple.plotters as psyps
-import psy_simple.base
-from psy_maps.boxes import lonlatboxes
-from psy_simple.colors import FixedBoundaryNorm
+    BEFOREPLOTTING,
+    END,
+    START,
+    DictFormatoption,
+    Formatoption,
+)
 
+from psy_maps.boxes import lonlatboxes
 
-wrap_proj_types = (ccrs._RectangularProjection,
-                   ccrs._WarpedRectangularProjection,
-                   ccrs.InterruptedGoodeHomolosine,
-                   ccrs.Mercator)
+wrap_proj_types = (
+    ccrs._RectangularProjection,
+    ccrs._WarpedRectangularProjection,
+    ccrs.InterruptedGoodeHomolosine,
+    ccrs.Mercator,
+)
 
 
 cartopy_version = list(map(int, cartopy.__version__.split(".")[:2]))
 
 
-@docstrings.get_sections(base='shiftdata')
+@docstrings.get_sections(base="shiftdata")
 def shiftdata(lonsin, datain, lon_0):
     """
     Shift longitudes (and optionally data) so that they match map projection
     region.
     Only valid for cylindrical/pseudo-cylindrical global projections and data
     on regular lat/lon grids. longitudes and data can be 1-d or 2-d, if 2-d
     it is assumed longitudes are 2nd (rightmost) dimension.
@@ -81,106 +71,108 @@
     ----------
     This function is copied and taken from the
     :class:`mpl_toolkits.basemap.Basemap` class. The only difference is that
     we do not mask values outside the map projection region
     """
     lonsin = np.asarray(lonsin)
     if lonsin.ndim not in [1, 2]:
-        raise ValueError('1-d or 2-d longitudes required')
+        raise ValueError("1-d or 2-d longitudes required")
     if datain is not None:
         # if it's a masked array, leave it alone.
         if not np.ma.isMA(datain):
             datain = np.asarray(datain)
         if datain.ndim not in [1, 2]:
-            raise ValueError('1-d or 2-d data required')
+            raise ValueError("1-d or 2-d data required")
     # 2-d data.
     if lonsin.ndim == 2:
         raise NotImplementedError(
-            "Shifting of 2D-data is currently not supported")
+            "Shifting of 2D-data is currently not supported"
+        )
     # 1-d data.
     elif lonsin.ndim == 1:
-        lonsin = np.where(lonsin > lon_0+180, lonsin-360, lonsin)
-        lonsin = np.where(lonsin < lon_0-180, lonsin+360, lonsin)
-        londiff = np.abs(lonsin[0:-1]-lonsin[1:])
+        lonsin = np.where(lonsin > lon_0 + 180, lonsin - 360, lonsin)
+        lonsin = np.where(lonsin < lon_0 - 180, lonsin + 360, lonsin)
+        londiff = np.abs(lonsin[0:-1] - lonsin[1:])
         londiff_sort = np.sort(londiff)
-        thresh = 360.-londiff_sort[-2]
+        thresh = 360.0 - londiff_sort[-2]
         itemindex = len(lonsin) - np.where(londiff >= thresh)[0]
         if itemindex:
             # check to see if cyclic (wraparound) point included
             # if so, remove it.
-            if np.abs(lonsin[0]-lonsin[-1]) < 1.e-4:
+            if np.abs(lonsin[0] - lonsin[-1]) < 1.0e-4:
                 hascyclic = True
                 lonsin_save = lonsin.copy()
                 lonsin = lonsin[1:]
                 if datain is not None:
                     datain_save = datain.copy()
                     datain = datain[1:]
             else:
                 hascyclic = False
-            lonsin = np.roll(lonsin, itemindex-1)
+            lonsin = np.roll(lonsin, itemindex - 1)
             if datain is not None:
-                datain = np.roll(datain, itemindex-1)
+                datain = np.roll(datain, itemindex - 1)
             # add cyclic point back at beginning.
             if hascyclic:
                 lonsin_save[1:] = lonsin
-                lonsin_save[0] = lonsin[-1]-360.
+                lonsin_save[0] = lonsin[-1] - 360.0
                 lonsin = lonsin_save
                 if datain is not None:
                     datain_save[1:] = datain
                     datain_save[0] = datain[-1]
                     datain = datain_save
     if datain is not None:
         return lonsin, datain
     else:
         return lonsin
 
 
 def degree_format():
-    if mpl.rcParams['text.usetex']:
-        return r'${%g\/^{\circ}\/%s}$'
+    if mpl.rcParams["text.usetex"]:
+        return r"${%g\/^{\circ}\/%s}$"
     else:
-        return u'%g\N{DEGREE SIGN}%s'
+        return "%g\N{DEGREE SIGN}%s"
 
 
 def format_lons(x, pos):
     fmt_string = degree_format()
     x = x - 360 if x > 180 else x
     if x == 0:
-        return fmt_string % (x, '')
-    return fmt_string % (abs(x), 'W' if x < 0 else 'E')
+        return fmt_string % (x, "")
+    return fmt_string % (abs(x), "W" if x < 0 else "E")
 
 
 def format_lats(x, pos):
     fmt_string = degree_format()
     if x == 0:
-        return fmt_string % (abs(x), '')
-    return fmt_string % (abs(x), 'S' if x < 0 else 'N')
+        return fmt_string % (abs(x), "")
+    return fmt_string % (abs(x), "S" if x < 0 else "N")
 
 
 class Transpose(Formatoption):
     """Transpose the data before plotting
 
     This formatoption can be used in case the data order of the variable
     dimensions is (x, y) instead of (y, x)"""
 
     priority = START
 
-    group = 'axes'
+    group = "axes"
 
-    name = 'Transpose (switch) x- and y-dimensions'
+    name = "Transpose (switch) x- and y-dimensions"
 
     def update(self, value):
-        for i, (raw, data) in enumerate(zip(
-                self.iter_raw_data, self.iter_data)):
+        for i, (raw, data) in enumerate(
+            zip(self.iter_raw_data, self.iter_data)
+        ):
             base_var = next(raw.psy.iter_base_variables)
             is_unstructured = raw.psy.decoder.is_unstructured(base_var)
             if is_unstructured and value:
                 decoder = copy.copy(data.psy.decoder)
-                xcoord = data.psy.get_coord('x').name
-                ycoord = data.psy.get_coord('y').name
+                xcoord = data.psy.get_coord("x").name
+                ycoord = data.psy.get_coord("y").name
                 decoder.x.add(ycoord)
                 decoder.y.add(xcoord)
                 self.set_decoder(decoder, i)
             elif is_unstructured:
                 self.set_decoder(raw.psy.decoder, i)
             elif value:
                 if data.ndim > 2:
@@ -190,16 +182,17 @@
                 self.set_data(data.transpose(*new_dims), i)
 
 
 lon_formatter = ticker.FuncFormatter(format_lons)
 lat_formatter = ticker.FuncFormatter(format_lats)
 
 
-@docstrings.get_sections(base=
-    'ProjectionBase', sections=['Possible types', 'See Also'])
+@docstrings.get_sections(
+    base="ProjectionBase", sections=["Possible types", "See Also"]
+)
 class ProjectionBase(Formatoption):
     """
     Base class for formatoptions that uses cartopy.crs.CRS instances
 
     Possible types
     --------------
     cartopy.crs.CRS
@@ -230,275 +223,282 @@
 
     See Also
     --------
     `Grid-mappings of cf-conventions <http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html#appendix-grid-mappings>`__
     """
 
     projections = {
-        'cyl': ccrs.PlateCarree,
-        'robin': ccrs.Robinson,
-        'moll': ccrs.Mollweide,
-        'geo': ccrs.Geostationary,
-        'northpole': ccrs.NorthPolarStereo,
-        'southpole': ccrs.SouthPolarStereo,
-        'ortho': ccrs.Orthographic,
-        'stereo': ccrs.Stereographic,
-        'near': ccrs.NearsidePerspective,
-        'rotated': ccrs.RotatedPole,
-        }
+        "cyl": ccrs.PlateCarree,
+        "robin": ccrs.Robinson,
+        "moll": ccrs.Mollweide,
+        "geo": ccrs.Geostationary,
+        "northpole": ccrs.NorthPolarStereo,
+        "southpole": ccrs.SouthPolarStereo,
+        "ortho": ccrs.Orthographic,
+        "stereo": ccrs.Stereographic,
+        "near": ccrs.NearsidePerspective,
+        "rotated": ccrs.RotatedPole,
+    }
 
     projection_kwargs = dict(
-        chain(zip(projections.keys(), repeat(['central_longitude']))))
-    projection_kwargs['ortho'] = ['central_longitude', 'central_latitude']
-    projection_kwargs['stereo'] = ['central_longitude', 'central_latitude']
-    projection_kwargs['near'] = ['central_longitude', 'central_latitude']
-    projection_kwargs['rotated'] = ['pole_longitude', 'pole_latitude']
+        chain(zip(projections.keys(), repeat(["central_longitude"])))
+    )
+    projection_kwargs["ortho"] = ["central_longitude", "central_latitude"]
+    projection_kwargs["stereo"] = ["central_longitude", "central_latitude"]
+    projection_kwargs["near"] = ["central_longitude", "central_latitude"]
+    projection_kwargs["rotated"] = ["pole_longitude", "pole_latitude"]
 
     # CRS that are supported to be interpreted by CF-conventions
     supported_crs = [
-        'albers_conical_equal_area',
-        'azimuthal_equidistant',
-        'geostationary',
-        'lambert_azimuthal_equal_area',
-        'lambert_conformal_conic',
-        'lambert_cylindrical_equal_area',
-        'latitude_longitude',
-        'mercator',
-        #'oblique_mercator',  # not available for cartopy
-        'orthographic',
-        'polar_stereographic',
-        'rotated_latitude_longitude',
-        'sinusoidal',
-        'stereographic',
-        'transverse_mercator',
-        #'vertical_perspective',  # not available for cartopy
-        ]
+        "albers_conical_equal_area",
+        "azimuthal_equidistant",
+        "geostationary",
+        "lambert_azimuthal_equal_area",
+        "lambert_conformal_conic",
+        "lambert_cylindrical_equal_area",
+        "latitude_longitude",
+        "mercator",
+        # 'oblique_mercator',  # not available for cartopy
+        "orthographic",
+        "polar_stereographic",
+        "rotated_latitude_longitude",
+        "sinusoidal",
+        "stereographic",
+        "transverse_mercator",
+        # 'vertical_perspective',  # not available for cartopy
+    ]
 
     def transform_lonlatbox(self, value):
         """Transform a lon-lat-box to the specific projection"""
         value = np.asarray(value)
         transformed = self.projection.transform_points(
             ccrs.PlateCarree(), value[:2], value[2:]
         )[..., :2]
         value[:2] = transformed[..., 0]
         value[2:] = transformed[..., 1]
         if value[0] == value[1] and isinstance(
-                self.projection, ccrs.PlateCarree
-            ):
+            self.projection, ccrs.PlateCarree
+        ):
             value[1] += 360
         return value
 
     @property
     def cf_projection(self):
         data = next(self.iter_data)
-        if 'grid_mapping' in data.attrs:
+        if "grid_mapping" in data.attrs:
             try:
-                crs = data[data.attrs['grid_mapping']]
+                crs = data[data.attrs["grid_mapping"]]
             except KeyError:
                 try:
-                    crs = data.psy.base[data.attrs['grid_mapping']]
+                    crs = data.psy.base[data.attrs["grid_mapping"]]
                 except KeyError:
                     warnings.warn(
                         "Grid mapping variable %(grid_mapping)s specified but "
-                        "impossible to find!" % data.attrs)
+                        "impossible to find!" % data.attrs
+                    )
                     return
-            if 'grid_mapping_name' not in crs.attrs:
+            if "grid_mapping_name" not in crs.attrs:
                 warnings.warn(
                     "Grid mapping variable %(grid_mapping)s specified but "
-                    "without 'grid_mapping_name' attribute!" % data.attrs)
+                    "without 'grid_mapping_name' attribute!" % data.attrs
+                )
                 return
-            elif crs.attrs['grid_mapping_name'] not in self.supported_crs:
+            elif crs.attrs["grid_mapping_name"] not in self.supported_crs:
                 warnings.warn(
-                    "Grid mapping %(grid_mapping_name)s not supported!" %
-                    crs.attrs)
+                    "Grid mapping %(grid_mapping_name)s not supported!"
+                    % crs.attrs
+                )
                 return
             else:
                 func = getattr(
-                    self, crs.attrs['grid_mapping_name'] + '_from_cf')
+                    self, crs.attrs["grid_mapping_name"] + "_from_cf"
+                )
                 try:
                     return func(crs)
                 except Exception:
                     self.logger.debug(
                         "Failed to get CRS from crs variable %s",
-                        crs.name, exc_info=True)
+                        crs.name,
+                        exc_info=True,
+                    )
                     warnings.warn(
-                        f"Failed to get CRS from crs variable {crs.name}")
+                        f"Failed to get CRS from crs variable {crs.name}"
+                    )
 
     def albers_conical_equal_area_from_cf(self, crs):
         kwargs = dict(
             central_longitude=crs.longitude_of_central_meridian,
             central_latitude=crs.latitude_of_projection_origin,
-            standard_parallels=crs.standard_parallel
-            )
+            standard_parallels=crs.standard_parallel,
+        )
         try:
-            iter(kwargs['standard_parallels'])
+            iter(kwargs["standard_parallels"])
         except TypeError:
-            kwargs['standard_parallels'] = [kwargs['standard_parallels']]
-        if getattr(crs, 'false_easting', None):
-            kwargs['false_easting'] = crs.false_easting
-        if getattr(crs, 'false_northing', None):
-            kwargs['false_northing'] = crs.false_northing
+            kwargs["standard_parallels"] = [kwargs["standard_parallels"]]
+        if getattr(crs, "false_easting", None):
+            kwargs["false_easting"] = crs.false_easting
+        if getattr(crs, "false_northing", None):
+            kwargs["false_northing"] = crs.false_northing
         return ccrs.AlbersEqualArea(**kwargs)
 
     def azimuthal_equidistant_from_cf(self, crs):
         kwargs = dict(
             central_longitude=crs.longitude_of_projection_origin,
             central_latitude=crs.latitude_of_projection_origin,
-            )
-        if getattr(crs, 'false_easting', None):
-            kwargs['false_easting'] = crs.false_easting
-        if getattr(crs, 'false_northing', None):
-            kwargs['false_northing'] = crs.false_northing
+        )
+        if getattr(crs, "false_easting", None):
+            kwargs["false_easting"] = crs.false_easting
+        if getattr(crs, "false_northing", None):
+            kwargs["false_northing"] = crs.false_northing
         return ccrs.AzimuthalEquidistant(**kwargs)
 
     def geostationary_from_cf(self, crs):
         kwargs = dict(
             central_longitude=crs.longitude_of_projection_origin,
             satellite_height=crs.perspective_point_height,
             sweep_axis=crs.sweep_angle_axis,
-            )
-        if getattr(crs, 'false_easting', None):
-            kwargs['false_easting'] = crs.false_easting
-        if getattr(crs, 'false_northing', None):
-            kwargs['false_northing'] = crs.false_northing
+        )
+        if getattr(crs, "false_easting", None):
+            kwargs["false_easting"] = crs.false_easting
+        if getattr(crs, "false_northing", None):
+            kwargs["false_northing"] = crs.false_northing
         return ccrs.Geostationary(**kwargs)
 
     def lambert_azimuthal_equal_area_from_cf(self, crs):
         kwargs = dict(
             central_longitude=crs.longitude_of_projection_origin,
             central_latitude=crs.latitude_of_projection_origin,
-            )
-        if getattr(crs, 'false_easting', None):
-            kwargs['false_easting'] = crs.false_easting
-        if getattr(crs, 'false_northing', None):
-            kwargs['false_northing'] = crs.false_northing
+        )
+        if getattr(crs, "false_easting", None):
+            kwargs["false_easting"] = crs.false_easting
+        if getattr(crs, "false_northing", None):
+            kwargs["false_northing"] = crs.false_northing
         return ccrs.LambertAzimuthalEqualArea(**kwargs)
 
     def lambert_conformal_conic_from_cf(self, crs):
         kwargs = dict(
             central_longitude=crs.longitude_of_central_meridian,
             central_latitude=crs.latitude_of_projection_origin,
             standard_parallels=crs.standard_parallel,
-            )
+        )
         try:
-            iter(kwargs['standard_parallels'])
+            iter(kwargs["standard_parallels"])
         except TypeError:
-            kwargs['standard_parallels'] = [kwargs['standard_parallels']]
-        if getattr(crs, 'false_easting', None):
-            kwargs['false_easting'] = crs.false_easting
-        if getattr(crs, 'false_northing', None):
-            kwargs['false_northing'] = crs.false_northing
+            kwargs["standard_parallels"] = [kwargs["standard_parallels"]]
+        if getattr(crs, "false_easting", None):
+            kwargs["false_easting"] = crs.false_easting
+        if getattr(crs, "false_northing", None):
+            kwargs["false_northing"] = crs.false_northing
         return ccrs.LambertConformal(**kwargs)
 
     def lambert_cylindrical_equal_area_from_cf(self, crs):
-        kwargs = dict(
-            central_longitude=crs.longitude_of_central_meridian
-            )
+        kwargs = dict(central_longitude=crs.longitude_of_central_meridian)
         return ccrs.LambertCylindrical(**kwargs)
 
     def latitude_longitude_from_cf(self, crs):
         return ccrs.PlateCarree()
 
     def mercator_from_cf(self, crs):
         kwargs = dict(
             central_longitude=crs.longitude_of_projection_origin,
-            )
-        if hasattr(crs, 'scale_factor_at_projection_origin'):
-            kwargs['scale_factor'] = crs.scale_factor_at_projection_origin
-        if getattr(crs, 'false_easting', None):
-            kwargs['false_easting'] = crs.false_easting
-        if getattr(crs, 'false_northing', None):
-            kwargs['false_northing'] = crs.false_northing
+        )
+        if hasattr(crs, "scale_factor_at_projection_origin"):
+            kwargs["scale_factor"] = crs.scale_factor_at_projection_origin
+        if getattr(crs, "false_easting", None):
+            kwargs["false_easting"] = crs.false_easting
+        if getattr(crs, "false_northing", None):
+            kwargs["false_northing"] = crs.false_northing
         return ccrs.Mercator(**kwargs)
 
     def orthographic_from_cf(self, crs):
         kwargs = dict(
             central_longitude=crs.longitude_of_projection_origin,
             central_latitude=crs.latitude_of_projection_origin,
-            )
+        )
         return ccrs.Orthographic(**kwargs)
 
     def polar_stereographic_from_cf(self, crs):
         kwargs = dict(
-            central_longitude=crs.straight_vertical_longitude_from_pole)
+            central_longitude=crs.straight_vertical_longitude_from_pole
+        )
         if crs.latitude_of_projection_origin == -90:
             return ccrs.SouthPolarStereo(**kwargs)
         else:
             return ccrs.NorthPolarStereo(**kwargs)
 
     def rotated_latitude_longitude_from_cf(self, crs):
-        args = [crs.grid_north_pole_longitude,
-                crs.grid_north_pole_latitude]
-        if hasattr(crs, 'north_pole_grid_longitude'):
+        args = [crs.grid_north_pole_longitude, crs.grid_north_pole_latitude]
+        if hasattr(crs, "north_pole_grid_longitude"):
             args.append(crs.north_pole_grid_longitude)
         return ccrs.RotatedPole(*args)
 
     def sinusoidal_from_cf(self, crs):
         try:
             kwargs = dict(
                 central_longitude=crs.longitude_of_projection_origin,
-                )
+            )
         except AttributeError:
             kwargs = dict(
                 central_longitude=crs.longitude_of_central_meridian,
-                )
-        if getattr(crs, 'false_easting', None):
-            kwargs['false_easting'] = crs.false_easting
-        if getattr(crs, 'false_northing', None):
-            kwargs['false_northing'] = crs.false_northing
+            )
+        if getattr(crs, "false_easting", None):
+            kwargs["false_easting"] = crs.false_easting
+        if getattr(crs, "false_northing", None):
+            kwargs["false_northing"] = crs.false_northing
         return ccrs.Sinusoidal(**kwargs)
 
     def stereographic_from_cf(self, crs):
         kwargs = dict(
             central_latitude=crs.latitude_of_projection_origin,
             central_longitude=crs.longitude_of_projection_origin,
-            scale_factor=crs.scale_factor_at_projection_origin
-            )
-        if getattr(crs, 'false_easting', None):
-            kwargs['false_easting'] = crs.false_easting
-        if getattr(crs, 'false_northing', None):
-            kwargs['false_northing'] = crs.false_northing
+            scale_factor=crs.scale_factor_at_projection_origin,
+        )
+        if getattr(crs, "false_easting", None):
+            kwargs["false_easting"] = crs.false_easting
+        if getattr(crs, "false_northing", None):
+            kwargs["false_northing"] = crs.false_northing
         return ccrs.Stereographic(**kwargs)
 
     def transverse_mercator_from_cf(self, crs):
         kwargs = dict(
             central_longitude=crs.longitude_of_central_meridian,
             central_latitude=crs.latitude_of_projection_origin,
             scale_factor=crs.scale_factor_at_central_meridian,
-            )
-        if getattr(crs, 'false_easting', None):
-            kwargs['false_easting'] = crs.false_easting
-        if getattr(crs, 'false_northing', None):
-            kwargs['false_northing'] = crs.false_northing
+        )
+        if getattr(crs, "false_easting", None):
+            kwargs["false_easting"] = crs.false_easting
+        if getattr(crs, "false_northing", None):
+            kwargs["false_northing"] = crs.false_northing
         return ccrs.TransverseMercator(**kwargs)
 
     def set_projection(self, value, *args, **kwargs):
-        if value == 'cf':
+        if value == "cf":
             ret = self.cf_projection
             if ret is not None:
                 return ret
         if isinstance(value, ccrs.CRS):
             return value
         else:
-            value = 'cyl' if value == 'cf' else value
-            return self.projections[value](**self.get_kwargs(
-                value, *args, **kwargs))
+            value = "cyl" if value == "cf" else value
+            return self.projections[value](
+                **self.get_kwargs(value, *args, **kwargs)
+            )
 
     def get_kwargs(self, value, clon=None, clat=None):
         ret = {}
         keys = self.projection_kwargs[value]
-        if 'central_longitude' in keys:
-            ret['central_longitude'] = self.clon.clon if clon is None else clon
-        if 'central_latitude' in keys:
-            ret['central_latitude'] = self.clat.clat if clat is None else clat
-        if 'pole_longitude' in keys:  # rotated pole
-            ret['pole_longitude'] = self.clon.clon if clon is None else clon
-            ret['pole_longitude'] -= 180
-        if 'pole_latitude' in keys:  # rotated pole
-            ret['pole_latitude'] = self.clat.clat if clat is None else clat
+        if "central_longitude" in keys:
+            ret["central_longitude"] = self.clon.clon if clon is None else clon
+        if "central_latitude" in keys:
+            ret["central_latitude"] = self.clat.clat if clat is None else clat
+        if "pole_longitude" in keys:  # rotated pole
+            ret["pole_longitude"] = self.clon.clon if clon is None else clon
+            ret["pole_longitude"] -= 180
+        if "pole_latitude" in keys:  # rotated pole
+            ret["pole_latitude"] = self.clat.clat if clat is None else clat
         self.logger.debug("Setting projection with %s", ret)
         return ret
 
 
 class Projection(ProjectionBase):
     """
     Specify the projection for the plot
@@ -520,47 +520,46 @@
 
     # the axes has to be cleared completly if the projection is updated
     priority = START
 
     #: an update of this formatoption requires that the axes is cleared
     requires_clearing = True
 
-    name = 'Projection of the plot'
+    name = "Projection of the plot"
 
-    dependencies = ['clon', 'clat']
+    dependencies = ["clon", "clat"]
 
-    connections = ['transform', 'lonlatbox']
+    connections = ["transform", "lonlatbox"]
 
     def __init__(self, *args, **kwargs):
         super(Projection, self).__init__(*args, **kwargs)
         self.projection = None
 
     @property
     def lonlatbox_transformed(self):
         """Transform the lonlatbox according to the projection"""
         return self.transform_lonlatbox(self.lonlatbox.lonlatbox)
 
     def initialize_plot(self, value, clear=True):
-        """Initialize the plot and set the projection for the axes
-        """
+        """Initialize the plot and set the projection for the axes"""
         self.projection = self.set_projection(value)
         if self.plotter.cleared:
             self.ax.projection = self.projection
             self.ax.clear()
 
     def update(self, value):
         """Update the formatoption
 
         Since this formatoption requires clearing, this method does nothing.
         Everything is done in the :meth:`initialize_plot` method.
         """
         pass
 
 
-@docstrings.get_sections(base='BoxBase')
+@docstrings.get_sections(base="BoxBase")
 class BoxBase(Formatoption):
     """
     Abstract base class for specifying a longitude-latitude box
 
     Possible types
     --------------
     str
@@ -596,31 +595,42 @@
         -------
         float: lonmin, lonmax, latmin, latmax or None
             The surrounding longitude-latitude box of all items in
             ``psyplot.rcParams['extents.boxes']`` whose key match `s` if there
             was any match. Otherwise None is returned
         """
         patt = re.compile(s)
-        boxes = np.array([
-            box for key, box in chain(*map(
-                six.iteritems, [lonlatboxes, rcParams['lonlatbox.boxes']]))
-            if patt.search(key)])
+        boxes = np.array(
+            [
+                box
+                for key, box in chain(
+                    *map(
+                        six.iteritems,
+                        [lonlatboxes, rcParams["lonlatbox.boxes"]],
+                    )
+                )
+                if patt.search(key)
+            ]
+        )
         if len(boxes) == 0:
-            similar_keys = get_close_matches(s, rcParams['lonlatbox.boxes'])
+            similar_keys = get_close_matches(s, rcParams["lonlatbox.boxes"])
             message = "Did not find any matches for %s!" % s
             if similar_keys:
-                message += " Maybe you mean on of " + ', '.join(
-                    similar_keys)
+                message += " Maybe you mean on of " + ", ".join(similar_keys)
             warnings.warn(message, RuntimeWarning)
             return
-        return [boxes[:, 0].min(), boxes[:, 1].max(),
-                boxes[:, 2].min(), boxes[:, 3].max()]
+        return [
+            boxes[:, 0].min(),
+            boxes[:, 1].max(),
+            boxes[:, 2].min(),
+            boxes[:, 3].max(),
+        ]
 
 
-docstrings.keep_types('BoxBase.possible_types', 'str', 'str')
+docstrings.keep_types("BoxBase.possible_types", "str", "str")
 
 
 class CenterLon(BoxBase):
     """
     Set the center longitude of the plot
 
     Parameters
@@ -630,19 +640,19 @@
     float
         Specifiy the center manually
     %(BoxBase.possible_types.str)s
     """
 
     priority = START
 
-    name = 'Longitude of the center of the plot'
+    name = "Longitude of the center of the plot"
 
     requires_clearing = True
 
-    dependencies = ['lonlatbox']
+    dependencies = ["lonlatbox"]
 
     def update(self, value):
         self.lon_mean = float(np.mean(self.lonlatbox.lonlatbox[:2]))
         if value is not None:
             if isinstance(value, six.string_types):
                 box = self.lola_from_pattern(value)
                 if box is not None:
@@ -670,19 +680,19 @@
     float
         Specifiy the center manually
     %(BoxBase.possible_types.str)s
     """
 
     priority = START
 
-    name = 'Latitude of the center of the plot'
+    name = "Latitude of the center of the plot"
 
     requires_clearing = True
 
-    dependencies = ['lonlatbox']
+    dependencies = ["lonlatbox"]
 
     def update(self, value):
         self.lat_mean = float(np.mean(self.lonlatbox.lonlatbox[2:]))
         if value is not None:
             if isinstance(value, six.string_types):
                 box = self.lola_from_pattern(value)
                 if box is not None:
@@ -695,15 +705,15 @@
             latmin, latmax = self.lonlatbox.lonlatbox[2:]
             if latmax - latmin > 170:
                 self.clat = 0
             else:
                 self.clat = self.lat_mean
 
 
-@docstrings.get_sections(base='LonLatBox')
+@docstrings.get_sections(base="LonLatBox")
 class LonLatBox(BoxBase):
     """
     Set the longitude-latitude box of the data shown
 
     This formatoption extracts the data that matches the specified box.
 
     Possible types
@@ -722,124 +732,158 @@
 
     See Also
     --------
     map_extent"""
 
     priority = START
 
-    name = 'Longitude-Latitude box of the data'
+    name = "Longitude-Latitude box of the data"
 
     requires_clearing = True
 
-    dependencies = ['transform', 'transpose']
+    dependencies = ["transform", "transpose"]
 
     @property
     def lonlatbox_transformed(self):
         return self.transform.transform_lonlatbox(self.lonlatbox)
 
     def data_dependent(self, data, set_data=True):
         if isinstance(data, InteractiveList):
             data = data[0]
         decoder = data.psy.decoder
         lon, lat = self._get_lola(data, decoder)
         new_lonlatbox = self.calc_lonlatbox(
-            lon, lat, decoder.is_unstructured(data))
+            lon, lat, decoder.is_unstructured(data)
+        )
         update = self.data_lonlatbox != new_lonlatbox
         if not update and set_data and self.value is not None:
             self.update(self.value)
         elif update:
             self.logger.debug(
                 "Reinitializing because lonlatbox of new data %s does not "
-                "match the old one %s", new_lonlatbox, self.data_lonlatbox)
+                "match the old one %s",
+                new_lonlatbox,
+                self.data_lonlatbox,
+            )
         return update
 
     def update(self, value):
         if isinstance(self.data, InteractiveList):
             for i, arr in enumerate(self.data):
                 decoder = self.get_decoder(i)
                 self.data[i] = self.update_array(
-                    value, arr, decoder, next(six.itervalues(
-                        self.raw_data[i].psy.base_variables)))
+                    value,
+                    arr,
+                    decoder,
+                    next(six.itervalues(self.raw_data[i].psy.base_variables)),
+                )
         else:
             arr = self.data
             arr = self.update_array(
-                    value, arr, self.decoder, next(six.itervalues(
-                        self.raw_data.psy.base_variables)))
+                value,
+                arr,
+                self.decoder,
+                next(six.itervalues(self.raw_data.psy.base_variables)),
+            )
             self.data = arr
 
     def _get_lola(self, data, decoder):
         """Get longitude and latitde informations from the given data array"""
         lon_da = decoder.get_x(data, data.coords)
         lat_da = decoder.get_y(data, data.coords)
-        lon, lat = self.to_degree(lon_da.attrs.get('units'), lon_da.values,
-                                  lat_da.values)
-        data_shape = data.shape[-2:] if not decoder.is_unstructured(data) \
-            else (data.shape[-1], )
+        lon, lat = self.to_degree(
+            lon_da.attrs.get("units"), lon_da.values, lat_da.values
+        )
+        data_shape = (
+            data.shape[-2:]
+            if not decoder.is_unstructured(data)
+            else (data.shape[-1],)
+        )
         is_combined = data_shape != data.shape
         if lon.shape == data_shape and lat.shape == data_shape:
             vals = data.values[0 if is_combined else slice(None)]
             lon = np.where(np.isnan(vals), np.nan, lon)
             lat = np.where(np.isnan(vals), np.nan, lat)
         return lon, lat
 
     def update_array(self, value, data, decoder, base_var=None):
         """Update the given `data` array"""
         lon, lat = self._get_lola(data, decoder)
         self.data_lonlatbox = self.calc_lonlatbox(
-            lon, lat, decoder.is_unstructured(data))
+            lon, lat, decoder.is_unstructured(data)
+        )
         if value is None:
             self.lonlatbox = self.data_lonlatbox
             return data
         else:
             if isinstance(value, six.string_types):
                 value = self.lola_from_pattern(value)
                 if value is None:
                     self.lonlatbox = self.data_lonlatbox
                     return data
             value = list(value)
             for i, v in enumerate(value):
                 if isinstance(v, six.string_types):
                     value[i] = self.lola_from_pattern(v)[i]
             is_unstructured = decoder.is_unstructured(
-                base_var if base_var is not None else data)
+                base_var if base_var is not None else data
+            )
             is_rectilinear = lon.ndim == 1 and not is_unstructured
             shift = isinstance(self.transform.projection, ccrs.PlateCarree)
             if is_rectilinear and shift:
                 data = data.copy(True)
                 lon, data.values = self.shiftdata(
-                    lon, data.values, np.mean(value[:2]))
+                    lon, data.values, np.mean(value[:2])
+                )
                 lon_name = decoder.get_x(data, data.coords).name
-                data[lon_name] = (data[lon_name].dims, lon,
-                                  data[lon_name].attrs)
+                data[lon_name] = (
+                    data[lon_name].dims,
+                    lon,
+                    data[lon_name].attrs,
+                )
             elif is_unstructured and shift:
                 # make sure that we are inside the map extent
                 ret = self.transform.projection.transform_points(
-                    self.transform.projection, lon, lat)
+                    self.transform.projection, lon, lat
+                )
                 lon = ret[..., 0]
                 lat = ret[..., 1]
             self.lonlatbox = value
             value = self.lonlatbox_transformed
             with warnings.catch_warnings():
-                warnings.filterwarnings('ignore', 'invalid value encountered',
-                                        RuntimeWarning)
+                warnings.filterwarnings(
+                    "ignore", "invalid value encountered", RuntimeWarning
+                )
                 if is_rectilinear and (lat[1:] < lat[:-1]).all():
                     lat_values = value[3:1:-1]
                 else:
                     lat_values = value[2:]
                 if is_rectilinear:
-                    kwargs = dict(zip(
-                        data.dims[-2:], starmap(
-                            slice, [lat_values, value[:2]])))
+                    kwargs = dict(
+                        zip(
+                            data.dims[-2:],
+                            starmap(slice, [lat_values, value[:2]]),
+                        )
+                    )
                     ret = data.sel(**kwargs)
                 else:
-                    ret = self.mask_outside(data.copy(True), lon, lat, *value,
-                                            is_unstructured=is_unstructured)
+                    ret = self.mask_outside(
+                        data.copy(True),
+                        lon,
+                        lat,
+                        *value,
+                        is_unstructured=is_unstructured,
+                        decoder=decoder,
+                    )
             lon, lat = self._get_lola(ret, decoder)
             self.data_lonlatbox = self.calc_lonlatbox(
-                lon, lat, is_unstructured)
+                lon, lat, is_unstructured
+            )
+            ret.psy.decoder = decoder
+            decoder.clear_cache()
             return ret
 
     def to_degree(self, units=None, *args):
         """Converts arrays with radian units to degree
 
         Parameters
         ----------
@@ -853,59 +897,74 @@
         list of np.ndarray
             returns the arrays provided with ``*args``
 
         Notes
         -----
         if `units` is ``'radian'``, a copy of the array will be returned"""
         args = list(args)
-        if units == 'radian' and isinstance(self.transform.projection,
-                                            ccrs.PlateCarree):
+        if units == "radian" and isinstance(
+            self.transform.projection, ccrs.PlateCarree
+        ):
             for i, array in enumerate(args):
-                args[i] = array * 180. / np.pi
+                args[i] = array * 180.0 / np.pi
         return args
 
-    def mask_outside(self, data, lon, lat, lonmin, lonmax, latmin, latmax,
-                     is_unstructured=False):
+    def mask_outside(
+        self,
+        data,
+        lon,
+        lat,
+        lonmin,
+        lonmax,
+        latmin,
+        latmax,
+        is_unstructured=False,
+        decoder=None,
+    ):
         data.values = data.values.copy()
         ndim = 2 if not is_unstructured else 1
         if lonmax < lonmin:
             lonmax += 360
             lon[lon < 0] += 360
-        mask = np.any([lon < lonmin, lon > lonmax, lat < latmin,
-                       lat > latmax], axis=0)
+        mask = np.any(
+            [lon < lonmin, lon > lonmax, lat < latmin, lat > latmax], axis=0
+        )
+        decoder = decoder or data.psy.decoder
         if data.ndim > ndim:
-            if is_unstructured:
+            if is_unstructured and decoder.supports_spatial_slicing:
                 data = data.psy[:, np.where(~mask)[0]]
             else:
                 for i, arr in enumerate(data.values):
                     arr[mask] = np.nan
                     data.values[i, :] = arr
         else:
-            if is_unstructured:
+            if is_unstructured and decoder.supports_spatial_slicing:
                 data = data.psy[np.where(~mask)[0]]
             else:
                 data.values[mask] = np.nan
         return data
 
     def calc_lonlatbox(self, lon, lat, is_unstructured=False):
         if isinstance(self.transform.projection, ccrs.PlateCarree):
             with warnings.catch_warnings():
-                warnings.filterwarnings('ignore', 'invalid value encountered',
-                                        RuntimeWarning)
+                warnings.filterwarnings(
+                    "ignore", "invalid value encountered", RuntimeWarning
+                )
                 lon = lon[np.all([lon >= -180, lon <= 360], axis=0)]
                 lat = lat[np.all([lat >= -90, lat <= 90], axis=0)]
                 return [lon.min(), lon.max(), lat.min(), lat.max()]
         else:
             if lon.ndim == 1 and not is_unstructured:
                 lon, lat = np.meshgrid(lon, lat)
             points = ccrs.PlateCarree().transform_points(
-                self.transform.projection, lon, lat)
+                self.transform.projection, lon, lat
+            )
             lon = points[..., 0]
             lat = points[..., 1]
-            lon_0 = self.transform.projection.proj4_params.get('lon_0')
+            lon_0 = self.transform.projection.proj4_params.get("lon_0")
             if lon_0 is not None:
                 lon = np.where(lon > lon_0 + 180, lon - 360, lon)
                 lon = np.where(lon < lon_0 - 180, lon + 360, lon)
             return [lon.min(), lon.max(), lat.min(), lat.max()]
 
     def shiftdata(self, lonsin, datain, lon_0):
         """
@@ -935,14 +994,61 @@
             for i, a in enumerate(datain):
                 lonsin, datain[i] = shiftdata(lon_save, a, lon_0)
         if get_centers:
             lonsin = np.mean([lonsin[1:], lonsin[:-1]], axis=0)
         return lonsin, datain
 
 
+class GoogleMap(Formatoption):
+    """Show a map of google on the plot.
+
+    Possible types
+    --------------
+    None
+        Do not show anything
+    int
+        The level of detail to show (usually between 6 and 9, must be greater
+        than or equal to 0).
+    """
+
+    data_dependent = True
+
+    _image = None
+
+    _factory = None
+
+    dependencies = ["map_extent"]
+
+    def update(self, value):
+        """Draw or remove the image from the plot."""
+        from cartopy.io.img_tiles import GoogleTiles
+
+        if value is None and self._image is not None:
+            self.remove()
+        elif value is not None:
+            self._factory = factory = self._factory or GoogleTiles()
+            if self._image is not None:
+                self.remove()
+            img, extent, origin = factory.image_for_domain(
+                self.ax._get_extent_geom(factory.crs), value
+            )
+            self._image = self.ax.imshow(
+                img, extent=extent, origin=origin, transform=factory.crs
+            )
+
+    def remove(self):
+        if self._image is not None:
+            try:
+                self._image.remove()
+            except ValueError:
+                # image has already been removed
+                pass
+        self._image = None
+
+
 class MapExtent(BoxBase):
     """
     Set the extent of the map
 
     Possible types
     --------------
     None
@@ -960,34 +1066,33 @@
     This formatoption sets the extent of the plot. For choosing the region for
     the data, see the :attr:`lonlatbox` formatoption
 
     See Also
     --------
     lonlatbox"""
 
-    dependencies = ['lonlatbox', 'plot', 'vplot']
+    dependencies = ["lonlatbox", "plot", "vplot"]
 
-    name = 'Longitude-Latitude box of the plot'
+    name = "Longitude-Latitude box of the plot"
 
     priority = END
 
     update_after_plot = True
 
     @property
     def coords(self):
         arr = next(self.iter_data)
-        return [arr.psy.get_coord('x'),
-                arr.psy.get_coord('y')]
+        return [arr.psy.get_coord("x"), arr.psy.get_coord("y")]
 
     def update(self, value):
         set_global = False
         if isinstance(value, six.string_types):
-            if value == 'global':
+            if value == "global":
                 set_global = True
-            elif value == 'data':
+            elif value == "data":
                 value = self.lonlatbox.lonlatbox
             else:
                 value = self.lola_from_pattern(value)
         elif value is None:
             # use autoscale
             self.ax.autoscale()
             return
@@ -1006,46 +1111,52 @@
                 try:
                     x1, x2, y1, y2 = self.ax.get_extent(ccrs.PlateCarree())
                 except ValueError:
                     # extent could not be guessed, we let cartopy do everything
                     x_rng = 360
                     y_rng = 180
                 else:
-                    x_rng = 360. if x1 == x2 else x2 - x1
+                    x_rng = 360.0 if x1 == x2 else x2 - x1
                     y_rng = y2 - y1
             proj = self.ax.projection
-        if set_global or ((value[1] - value[0]) / x_rng > 0.95 and
-                          (value[3] - value[2]) / y_rng > 0.95):
+        if set_global or (
+            (value[1] - value[0]) / x_rng > 0.95
+            and (value[3] - value[2]) / y_rng > 0.95
+        ):
             self.logger.debug("Setting to global extent...")
             self.ax.set_global()
             return
-        elif (isinstance(proj,
-                         (ccrs.Orthographic, ccrs.Stereographic)) and
-              np.abs(np.diff(value[:2])) > 350):
+        elif (
+            isinstance(proj, (ccrs.Orthographic, ccrs.Stereographic))
+            and np.abs(np.diff(value[:2])) > 350
+        ):
             # HACK: to make sure, that we don't get troubles with the
             # transformation, we don't go until 360
             value[:2] = 0, 359.9999
             self.ax.set_extent(value, crs=ccrs.PlateCarree())
         else:
             try:
                 self.ax.set_extent(value, crs=ccrs.PlateCarree())
             except ValueError:
                 self.logger.debug(
-                    "Failed to set_extent with lonlatbox %s", value,
-                    exc_info=True)
+                    "Failed to set_extent with lonlatbox %s",
+                    value,
+                    exc_info=True,
+                )
 
 
 class MapBackground(psy_simple.base.BackgroundColor):
-
     __doc__ = psy_simple.base.BackgroundColor.__doc__
 
     def update(self, value):
         super().update(value)
         if cartopy.__version__ < "0.18":
-            self.ax.background_patch.set_facecolor(self.ax.patch.get_facecolor())
+            self.ax.background_patch.set_facecolor(
+                self.ax.patch.get_facecolor()
+            )
         else:
             self.ax.patch.set_facecolor(self.ax.patch.get_facecolor())
 
 
 class ClipAxes(Formatoption):
     """
     Clip the part outside the latitudes of the map extent
@@ -1063,46 +1174,51 @@
     If the plot is clipped. You might need to update with `replot=True`!
     """
 
     _orig_path = None
 
     priority = BEFOREPLOTTING
 
-    connections = ['lonlatbox', 'map_extent']
+    connections = ["lonlatbox", "map_extent"]
 
     def draw_circle(self):
         import matplotlib.path as mpath
+
         self._orig_path = self._orig_path or self.ax.patch.get_path()
-        theta = np.linspace(0, 2*np.pi, 100)
+        theta = np.linspace(0, 2 * np.pi, 100)
         center, radius = [0.5, 0.5], 0.5
         verts = np.vstack([np.sin(theta), np.cos(theta)]).T
         circle = mpath.Path(verts * radius + center)
         self.ax.set_boundary(circle, transform=self.ax.transAxes)
 
     def update(self, value):
         if value:
             self.draw_circle()
         elif value is None:
             proj = self.ax.projection
             extent = self.map_extent.value or self.lonlatbox.lonlatbox
-            if extent == 'data':
+            if extent == "data":
                 extent = self.lonlatbox.lonlatbox
-            if (isinstance(proj, (ccrs.Orthographic, ccrs.Stereographic)) and
-                    extent != 'global' and np.abs(np.diff(extent[:2])) > 350):
+            if (
+                isinstance(proj, (ccrs.Orthographic, ccrs.Stereographic))
+                and extent != "global"
+                and np.abs(np.diff(extent[:2])) > 350
+            ):
                 self.draw_circle()
             else:
                 self.remove()
         else:
             self.remove()
 
     def remove(self):
         if self._orig_path is not None:
             try:
-                self.ax.set_boundary(self._orig_path,
-                                     transform=self.ax.transAxes)
+                self.ax.set_boundary(
+                    self._orig_path, transform=self.ax.transAxes
+                )
             except Exception:
                 pass
             del self._orig_path
 
 
 class Transform(ProjectionBase):
     """
@@ -1118,38 +1234,38 @@
     See Also
     --------
     %(ProjectionBase.see_also)s
     """
 
     priority = START
 
-    name = 'Coordinate system of the data'
+    name = "Coordinate system of the data"
 
-    connections = ['plot', 'vplot']
+    connections = ["plot", "vplot"]
 
     @property
     def cf_projection(self):
         data = next(self.iter_data)
-        xcoord = data.psy.get_coord('x')
-        if xcoord.attrs.get('standard_name') == 'longitude':
+        xcoord = data.psy.get_coord("x")
+        if xcoord.attrs.get("standard_name") == "longitude":
             return ccrs.PlateCarree()
         return super().cf_projection
 
     def update(self, value):
-        if value == 'cf':
+        if value == "cf":
             self.projection = self.cf_projection
             if self.projection is None:
                 self.projection = ccrs.PlateCarree()
-        elif value == 'cyl':
+        elif value == "cyl":
             self.projection = ccrs.PlateCarree()
         else:
             self.projection = self.set_projection(value, 0, 0)
         for key in self.connections:
             try:
-                getattr(self, key)._kwargs['transform'] = self.projection
+                getattr(self, key)._kwargs["transform"] = self.projection
             except AttributeError:
                 pass
 
 
 class LSM(Formatoption):
     """
     Draw the continents
@@ -1177,103 +1293,115 @@
         ocean
             The fill color for the oceans
         res
             The resolution (see above)
         linewidth
             The linewidth of the coastlines (see above)"""
 
-    name = 'Land-Sea mask'
+    name = "Land-Sea mask"
 
     lsm = None
 
-    dependencies = ['background']
+    dependencies = ["background"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.draw_funcs = {
-            ('coast', ): self.draw_coast,
-            ('coast', 'land'): self.draw_land_coast,
-            ('land', ): self.draw_land,
-            ('ocean', ): self.draw_ocean,
-            ('coast', 'land', 'ocean'): self.draw_all,
-            ('land', 'ocean'): self.draw_land_ocean,
-            ('coast', 'ocean'): self.draw_ocean_coast,
-            }
+            ("coast",): self.draw_coast,
+            ("coast", "land"): self.draw_land_coast,
+            ("land",): self.draw_land,
+            ("ocean",): self.draw_ocean,
+            ("coast", "land", "ocean"): self.draw_all,
+            ("land", "ocean"): self.draw_land_ocean,
+            ("coast", "ocean"): self.draw_ocean_coast,
+        }
         self.artists = []
 
     @property
     def lsm(self):
         try:
             return self.artists[0]
         except ValueError:
             return None
 
     @lsm.setter
     def lsm(self, val):
         self.artists.append(val)
 
-    def draw_all(self, land, ocean, coast, res='110m', linewidth=1):
+    def draw_all(self, land, ocean, coast, res="110m", linewidth=1):
         land_feature = cf.LAND.with_scale(res)
         if land is None:
-            land = land_feature._kwargs.get('facecolor')
+            land = land_feature._kwargs.get("facecolor")
         if ocean is None:
-            ocean = cf.OCEAN._kwargs.get('facecolor')
+            ocean = cf.OCEAN._kwargs.get("facecolor")
         self.lsm = self.ax.add_feature(
-            land_feature, facecolor=land, edgecolor=coast, linewidth=linewidth)
+            land_feature, facecolor=land, edgecolor=coast, linewidth=linewidth
+        )
         # draw the coast above the plot
         self.lsm = self.ax.add_feature(
-            land_feature, facecolor='none', edgecolor=coast,
-            linewidth=linewidth, zorder=1)
+            land_feature,
+            facecolor="none",
+            edgecolor=coast,
+            linewidth=linewidth,
+            zorder=1,
+        )
         if cartopy.__version__ < "0.18":
             self.ax.background_patch.set_facecolor(ocean)
         else:
             self.ax.patch.set_facecolor(ocean)
 
-    def draw_land(self, land, res='110m'):
+    def draw_land(self, land, res="110m"):
         if cartopy.__version__ < "0.18":
             ocean = self.ax.background_patch.get_facecolor()
         else:
             ocean = self.ax.patch.get_facecolor()
-        self.draw_all(land, ocean, 'face', res, 0.0)
+        self.draw_all(land, ocean, "face", res, 0.0)
 
-    def draw_coast(self, coast, res='110m', linewidth=1.0):
+    def draw_coast(self, coast, res="110m", linewidth=1.0):
         if coast is None:
-            coast = 'k'
+            coast = "k"
         self.lsm = self.ax.coastlines(res, color=coast, linewidth=linewidth)
 
-    def draw_ocean(self, ocean, res='110m'):
+    def draw_ocean(self, ocean, res="110m"):
         self.draw_ocean_coast(ocean, None, res, 0.0)
 
-    def draw_land_coast(self, land, coast, res='110m', linewidth=1.0):
+    def draw_land_coast(self, land, coast, res="110m", linewidth=1.0):
         if cartopy.__version__ < "0.18":
             ocean = self.ax.background_patch.get_facecolor()
         else:
             ocean = self.ax.patch.get_facecolor()
         self.draw_all(land, ocean, coast, res, linewidth)
 
-    def draw_ocean_coast(self, ocean, coast, res='110m', linewidth=1.0):
+    def draw_ocean_coast(self, ocean, coast, res="110m", linewidth=1.0):
         ocean_feature = cf.OCEAN.with_scale(res)
         if ocean is None:
-            ocean = cf.OCEAN._kwargs.get('facecolor')
+            ocean = cf.OCEAN._kwargs.get("facecolor")
         self.lsm = self.ax.add_feature(
-            ocean_feature, facecolor=ocean, edgecolor=coast,
-            linewidth=linewidth)
+            ocean_feature,
+            facecolor=ocean,
+            edgecolor=coast,
+            linewidth=linewidth,
+        )
         # draw the coast above the plot
         self.lsm = self.ax.add_feature(
-            ocean_feature, facecolor='none', edgecolor=coast,
-            linewidth=linewidth, zorder=1)
+            ocean_feature,
+            facecolor="none",
+            edgecolor=coast,
+            linewidth=linewidth,
+            zorder=1,
+        )
 
-    def draw_land_ocean(self, land, ocean, res='110m'):
+    def draw_land_ocean(self, land, ocean, res="110m"):
         self.draw_all(land, ocean, None, res, 0.0)
 
     def update(self, value):
         self.remove()
         # to make sure, we have a dictionary
         value = self.validate(value)
-        keys = tuple(sorted({'land', 'ocean', 'coast'}.intersection(value)))
+        keys = tuple(sorted({"land", "ocean", "coast"}.intersection(value)))
         if keys:
             self.draw_funcs[keys](**value)
 
     def remove(self):
         for artist in self.artists:
             try:
                 artist.remove()
@@ -1283,14 +1411,15 @@
         try:
             self.background.update(self.background.value)
         except Exception:
             pass
 
     def get_fmt_widget(self, parent, project):
         from psy_maps.widgets import LSMFmtWidget
+
         return LSMFmtWidget(parent, self, project)
 
 
 class StockImage(Formatoption):
     """
     Display a stock image on the map
 
@@ -1304,32 +1433,31 @@
         If True, the image is displayed
     """
 
     image = None
 
     priority = END
 
-    name = 'Display Natural Earth shaded relief raster'
+    name = "Display Natural Earth shaded relief raster"
 
-    connections = ['plot']
+    connections = ["plot"]
 
     def update(self, value):
         if value and self.image is None:
             self.image = self.ax.stock_img()
             # display below the plot
             try:
                 mappable = self.plot.mappable
             except AttributeError:
                 pass
             else:
                 try:
                     self.image.zorder = mappable.zorder - 0.1
                 except AttributeError:
-                    self.image.zorder = (
-                        mappable.collections[0].zorder - 0.1)
+                    self.image.zorder = mappable.collections[0].zorder - 0.1
         elif not value and self.image is not None:
             self.remove()
 
     def remove(self):
         if self.image is None:
             return
         self.image.remove()
@@ -1348,25 +1476,25 @@
         Any valid color for matplotlib (see the :func:`matplotlib.pyplot.plot`
         documentation)
 
     See Also
     --------
     grid_settings, grid_labels, grid_labelsize, xgrid, ygrid"""
 
-    name = 'Color of the latitude-longitude grid'
+    name = "Color of the latitude-longitude grid"
 
-    connections = ['xgrid', 'ygrid']
+    connections = ["xgrid", "ygrid"]
 
     def update(self, value):
         if value is not None:
             for connection in self.connections:
-                getattr(self, connection)._kwargs['color'] = value
+                getattr(self, connection)._kwargs["color"] = value
         else:
             for connection in self.connections:
-                getattr(self, connection)._kwargs.pop('color', None)
+                getattr(self, connection)._kwargs.pop("color", None)
 
 
 class GridLabels(Formatoption):
     """
     Display the labels of the grid
 
     Possible types
@@ -1377,35 +1505,34 @@
         If True, labels are drawn and if this is not possible, a warning is
         raised
 
     See Also
     --------
     grid_color, grid_settings, grid_labelsize, xgrid, ygrid"""
 
-    name = 'Labels of the latitude-longitude grid'
+    name = "Labels of the latitude-longitude grid"
 
-    dependencies = ['projection', 'transform']
+    dependencies = ["projection", "transform"]
 
-    connections = ['xgrid', 'ygrid']
+    connections = ["xgrid", "ygrid"]
 
     def update(self, value):
         if value is None or value:
             # initialize a gridliner to see if we can draw the tick labels
             test_value = True
             try:
-                Gridliner(
-                    self.ax, self.ax.projection, draw_labels=test_value)
+                Gridliner(self.ax, self.ax.projection, draw_labels=test_value)
             except TypeError as e:  # labels cannot be drawn
                 if value:
                     warnings.warn(str(e), RuntimeWarning)
                 value = False
             else:
                 value = True
         for connection in self.connections:
-            getattr(self, connection)._kwargs['draw_labels'] = value
+            getattr(self, connection)._kwargs["draw_labels"] = value
 
 
 class GridSettings(DictFormatoption):
     """
     Modify the settings of the grid explicitly
 
     Possible types
@@ -1414,18 +1541,18 @@
         Items may be any key-value-pair of the
         :class:`matplotlib.collections.LineCollection` class
 
     See Also
     --------
     grid_color, grid_labels, grid_labelsize, xgrid, ygrid"""
 
-    children = ['grid_labels', 'grid_color']
-    connections = ['xgrid', 'ygrid']
+    children = ["grid_labels", "grid_color"]
+    connections = ["xgrid", "ygrid"]
 
-    name = 'Line properties of the latitude-longitude grid'
+    name = "Line properties of the latitude-longitude grid"
 
     def set_value(self, value, validate=True, todefault=False):
         if todefault:
             for connection in self.connections:
                 for key in self.value:
                     getattr(self, connection)._kwargs.pop(key, None)
         super(GridSettings, self).set_value(value, validate, todefault)
@@ -1443,38 +1570,40 @@
     --------------
     %(fontsizes)s
 
     See Also
     --------
     grid_color, grid_labels, xgrid, ygrid, grid_settings"""
 
-    dependencies = ['xgrid', 'ygrid']
+    dependencies = ["xgrid", "ygrid"]
 
-    name = 'Label size of the latitude-longitude grid'
+    name = "Label size of the latitude-longitude grid"
 
     def update(self, value):
         for fmto in map(lambda key: getattr(self, key), self.dependencies):
             try:
                 gl = fmto._gridliner
             except AttributeError:
                 continue
-            gl.xlabel_style['size'] = value
-            gl.ylabel_style['size'] = value
+            gl.xlabel_style["size"] = value
+            gl.ylabel_style["size"] = value
             try:
                 if cartopy_version < [0, 19]:
                     texts = [t[-1] for t in gl.label_artists]
                 else:
                     texts = gl.label_artists
             except AttributeError:  # cartopy < 0.18
                 texts = chain(gl.xlabel_artists, gl.ylabel_artists)
             for text in texts:
                 text.set_size(value)
 
 
-@docstrings.get_sections(base='GridBase', sections=['Possible types', 'See Also'])
+@docstrings.get_sections(
+    base="GridBase", sections=["Possible types", "See Also"]
+)
 class GridBase(psyps.DataTicksCalculator):
     """
     Abstract base class for x- and y- grid lines
 
     Possible types
     --------------
     None
@@ -1487,18 +1616,25 @@
         Specifies how many ticks to use with the ``'rounded'`` option. I.e. if
         integer ``i``, then this is the same as ``['rounded', i]``.
 
     See Also
     --------
     grid_color, grid_labels"""
 
-    dependencies = ['transform', 'grid_labels', 'grid_color', 'grid_settings',
-                    'projection', 'lonlatbox', 'map_extent']
+    dependencies = [
+        "transform",
+        "grid_labels",
+        "grid_color",
+        "grid_settings",
+        "projection",
+        "lonlatbox",
+        "map_extent",
+    ]
 
-    connections = ['plot']
+    connections = ["plot"]
 
     @abstractproperty
     def axis(self):
         """The axis string"""
         pass
 
     def __init__(self, *args, **kwargs):
@@ -1512,84 +1648,93 @@
         if value is True:
             loc = None
         elif isinstance(value[0], six.string_types):
             loc = ticker.FixedLocator(self.calc_funcs[value[0]](*value[1:]))
         elif isinstance(value, tuple):
             steps = 11 if len(value) == 2 else value[3]
             loc = ticker.FixedLocator(
-                np.linspace(value[0], value[1], steps, endpoint=True))
+                np.linspace(value[0], value[1], steps, endpoint=True)
+            )
         else:
             loc = ticker.FixedLocator(value)
         try:
             mappable = self.plot.mappable
         except AttributeError:
             zorder = 0.9
         else:
             try:
                 zorder = mappable.zorder
             except AttributeError:
-                    zorder = mappable.collections[0].zorder
+                zorder = mappable.collections[0].zorder
         self._gridliner = self.ax.gridlines(
-            crs=ccrs.PlateCarree(), zorder=zorder + 0.1,
-            **self.get_kwargs(loc))
+            crs=ccrs.PlateCarree(), zorder=zorder + 0.1, **self.get_kwargs(loc)
+        )
         self._modify_gridliner(self._gridliner)
         self._disable_other_axis()
 
     def get_kwargs(self, loc):
-        return dict(chain(self._kwargs.items(), [(self.axis + 'locs', loc)]))
+        return dict(chain(self._kwargs.items(), [(self.axis + "locs", loc)]))
 
     def _disable_other_axis(self):
-        label_positions = {'x': ['bottom', 'top'], 'y': ['left', 'right']}
-        other_axis = 'y' if self.axis == 'x' else 'x'
-        setattr(self._gridliner, other_axis + 'lines', False)
+        label_positions = {"x": ["bottom", "top"], "y": ["left", "right"]}
+        other_axis = "y" if self.axis == "x" else "x"
+        setattr(self._gridliner, other_axis + "lines", False)
         for pos in label_positions[other_axis]:
             if cartopy.__version__ < "0.18":  # cartopy < 0.18
-                setattr(self._gridliner, other_axis + 'labels_' + pos, False)
+                setattr(self._gridliner, other_axis + "labels_" + pos, False)
             else:
-                setattr(self._gridliner, pos + '_labels', False)
+                setattr(self._gridliner, pos + "_labels", False)
 
     def _modify_gridliner(self, gridliner):
         """Modify the formatting of the given `gridliner` before drawing"""
         if cartopy.__version__ < "0.18":  # cartopy < 0.18
             gridliner.xlabels_top = False
             gridliner.ylabels_right = False
         else:
             gridliner.top_labels = False
             gridliner.right_labels = False
         gridliner.yformatter = lat_formatter
         gridliner.xformatter = lon_formatter
 
     def get_fmt_widget(self, parent, project):
         from psy_maps.widgets import GridFmtWidget
+
         return GridFmtWidget(parent, self, project)
 
     def remove(self):
-        if not hasattr(self, '_gridliner'):
+        if not hasattr(self, "_gridliner"):
             return
         gl = self._gridliner
         try:
             if cartopy_version < [0, 19]:
-                artists = chain(gl.xline_artists, gl.yline_artists,
-                                [t[-1] for t in gl.label_artists])
+                artists = chain(
+                    gl.xline_artists,
+                    gl.yline_artists,
+                    [t[-1] for t in gl.label_artists],
+                )
             else:
                 artists = chain(
                     gl.xline_artists, gl.yline_artists, gl.label_artists
                 )
         except AttributeError:  # cartopy < 0.17
-            artists = chain(gl.xline_artists, gl.yline_artists,
-                            gl.xlabel_artists, gl.ylabel_artists)
+            artists = chain(
+                gl.xline_artists,
+                gl.yline_artists,
+                gl.xlabel_artists,
+                gl.ylabel_artists,
+            )
         for artist in artists:
             artist.remove()
         if gl in self.ax._gridliners:
             self.ax._gridliners.remove(gl)
         del self._gridliner
 
     def _round_min_max(self, vmin, vmax):
         exp = np.floor(np.log10(abs(vmax - vmin)))
-        return psyps.round_to_05([vmin, vmax], exp, mode='s')
+        return psyps.round_to_05([vmin, vmax], exp, mode="s")
 
 
 class XGrid(GridBase):
     """
     Draw vertical grid lines (meridians)
 
     This formatoption specifies at which longitudes to draw the meridians.
@@ -1598,30 +1743,31 @@
     --------------
     %(GridBase.possible_types)s
 
     See Also
     --------
     ygrid, %(GridBase.see_also)s"""
 
-    dependencies = GridBase.dependencies + ['clon']
+    dependencies = GridBase.dependencies + ["clon"]
 
-    name = 'Meridians'
+    name = "Meridians"
 
     @property
     def array(self):
         decoder = self.decoder
         coord = decoder.get_x(self.data, self.data.coords)
         arr = np.unique(decoder.get_plotbounds(coord, ignore_shape=True))
-        if hasattr(coord, 'units') and coord.units == 'radian':
-            arr *= 180. / np.pi
+        if hasattr(coord, "units") and coord.units == "radian":
+            arr *= 180.0 / np.pi
         arr = ccrs.PlateCarree().transform_points(
-            self.transform.projection, arr, np.zeros(arr.shape))[..., 0]
+            self.transform.projection, arr, np.zeros(arr.shape)
+        )[..., 0]
         return arr
 
-    axis = 'x'
+    axis = "x"
 
 
 class YGrid(GridBase):
     """
     Draw horizontal grid lines (parallels)
 
     This formatoption specifies at which latitudes to draw the parallels.
@@ -1630,208 +1776,254 @@
     --------------
     %(GridBase.possible_types)s
 
     See Also
     --------
     xgrid, %(GridBase.see_also)s"""
 
-    name = 'Parallels'
+    name = "Parallels"
 
     @property
     def array(self):
         decoder = self.decoder
         coord = decoder.get_y(self.data, self.data.coords)
         arr = np.unique(decoder.get_plotbounds(coord, ignore_shape=True))
-        if hasattr(coord, 'units') and coord.units == 'radian':
-            arr *= 180. / np.pi
+        if hasattr(coord, "units") and coord.units == "radian":
+            arr *= 180.0 / np.pi
         arr = ccrs.PlateCarree().transform_points(
-            self.transform.projection, arr, np.zeros(arr.shape))[..., 1]
+            self.transform.projection, arr, np.zeros(arr.shape)
+        )[..., 1]
         return arr
 
-    axis = 'y'
+    axis = "y"
 
 
 class MapPlot2D(psyps.Plot2D):
     __doc__ = psyps.Plot2D.__doc__
     # fixes the plot of unstructured unstructured data on round projections
 
-    connections = psyps.Plot2D.connections + ['transform', 'lonlatbox']
+    connections = psyps.Plot2D.connections + ["transform", "lonlatbox"]
 
-    dependencies = psyps.Plot2D.dependencies + ['clip']
+    dependencies = psyps.Plot2D.dependencies + ["clip"]
 
     @property
     def array(self):
         ret = super(MapPlot2D, self).array.astype(float)
         xcoord = self.xcoord
-        if xcoord.ndim == 2 and isinstance(self.transform.projection,
-                                           ccrs.PlateCarree):
+        if xcoord.ndim == 2 and isinstance(
+            self.transform.projection, ccrs.PlateCarree
+        ):
             lon = xcoord.values
             lat = self.ycoord.values
-            ret[np.any([lon <= -200, lon >= 400, lat <= -120, lat >= 120],
-                       axis=0)] = np.nan
+            ret[
+                np.any(
+                    [lon <= -200, lon >= 400, lat <= -120, lat >= 120], axis=0
+                )
+            ] = np.nan
         return ret
 
     def _get_xy_pcolormesh(self):
         """Use the bounds for non-global circumpolar plots"""
         interp_bounds = self.interp_bounds.value
         if interp_bounds is None and self.decoder.is_circumpolar(
-                self.raw_data):
+            self.raw_data
+        ):
             lola = self.lonlatbox
-            if (isinstance(self.transform.projection, ccrs.PlateCarree) and
-                    np.abs(np.diff(lola.data_lonlatbox[:2])[0]) < 355):
+            if (
+                isinstance(self.transform.projection, ccrs.PlateCarree)
+                and np.abs(np.diff(lola.data_lonlatbox[:2])[0]) < 355
+            ):
                 return self.xbounds, self.ybounds
         return super(MapPlot2D, self)._get_xy_pcolormesh()
 
     def _contourf(self):
         t = self.ax.projection
         if isinstance(t, ccrs.CRS) and not isinstance(t, ccrs.Projection):
-            raise ValueError('invalid transform:'
-                             ' Spherical contouring is not supported - '
-                             ' consider using PlateCarree/RotatedPole.')
+            raise ValueError(
+                "invalid transform:"
+                " Spherical contouring is not supported - "
+                " consider using PlateCarree/RotatedPole."
+            )
         elif self.decoder.is_unstructured(self.raw_data):
-            warnings.warn('Filled contour plots of unstructured data are not '
-                          'correctly warped around!')
+            warnings.warn(
+                "Filled contour plots of unstructured data are not "
+                "correctly warped around!"
+            )
         return super(MapPlot2D, self)._contourf()
 
     @property
     def cell_nodes_x(self):
         xbounds = super(MapPlot2D, self).cell_nodes_x
         if isinstance(self.transform.projection, ccrs.PlateCarree):
             xbounds = xbounds.copy()
             xbounds[xbounds - xbounds.min(axis=1, keepdims=True) > 180] -= 360
         return xbounds
 
     def _polycolor(self):
         from matplotlib.collections import PolyCollection
-        self.logger.debug('Retrieving data')
+
+        self.logger.debug("Retrieving data")
         arr = self.array
         cmap = self.cmap.get_cmap(arr)
-        if hasattr(self, '_plot'):
-            self.logger.debug('Updating plot')
+        if hasattr(self, "_plot"):
+            self.logger.debug("Updating plot")
             self._plot.update(dict(cmap=cmap, norm=self.bounds.norm))
-            if hasattr(self, '_wrapped_plot'):
-                self._wrapped_plot.update(dict(cmap=cmap,
-                                               norm=self.bounds.norm))
+            if hasattr(self, "_wrapped_plot"):
+                self._wrapped_plot.update(
+                    dict(cmap=cmap, norm=self.bounds.norm)
+                )
         else:
-            self.logger.debug('Retrieving bounds')
+            self.logger.debug("Retrieving bounds")
             xb = self.cell_nodes_x
             yb = self.cell_nodes_y
-            wrap_proj_types = (ccrs._RectangularProjection,
-                               ccrs._WarpedRectangularProjection,
-                               ccrs.InterruptedGoodeHomolosine,
-                               ccrs.Mercator)
+            wrap_proj_types = (
+                ccrs._RectangularProjection,
+                ccrs._WarpedRectangularProjection,
+                ccrs.InterruptedGoodeHomolosine,
+                ccrs.Mercator,
+            )
             t = self.transform.projection
             proj = self.ax.projection
             wrapped_arr = None
-            ### HACK: since the matplotlib transformation is very slow because
+            # HACK: since the matplotlib transformation is very slow because
             # it transforms every single polygon, we transform the coordinates
             # already here and do not specify the `transform` property for the
             # `PolyCollection` down below.
             # However, in order to wrap the boundaries correctly, we have to
             # identify the corresponding grid cells and then use the standard
             # matplotlib transform.
             if xb.ndim > 2:
                 xb = xb.reshape((-1, xb.shape[-1]))
                 yb = yb.reshape((-1, yb.shape[-1]))
                 arr = arr.reshape(-1)
             if arr.ndim > 1:
                 arr = arr.reshape(-1)
-            if isinstance(t, wrap_proj_types) and 'lon_0' in proj.proj4_params:
+            if isinstance(t, wrap_proj_types) and "lon_0" in proj.proj4_params:
                 # We adopt and copy some code from the methodology of cartopy
                 # _pcolormesh_patched method of the geoaxes. As such, we
                 # transform the coordinates using standard matplotlib
                 # transformation and check if the hypotenuse is larger than
                 # half of the available x-limit of the ax.projection
                 # By using the geodetic version of `t`, we place the center
                 # longitude to `lon_0` and cells at the boundary do have a
                 # distance of 180 degrees to lon_0
-                trans_to_data = t.as_geodetic()._as_mpl_transform(self.ax) - \
-                    self.ax.transData
+                trans_to_data = (
+                    t.as_geodetic()._as_mpl_transform(self.ax)
+                    - self.ax.transData
+                )
                 # now we identify the cells at the x-boundary by
                 # checking the hypotenuse
-                coords = np.column_stack((xb.flat, yb.flat)).astype(float, copy=False)
+                coords = np.column_stack((xb.flat, yb.flat)).astype(
+                    float, copy=False
+                )
                 transformed_pts = trans_to_data.transform(coords)
                 transformed_pts = transformed_pts.reshape(
-                    xb.shape + (transformed_pts.shape[-1], ))
+                    xb.shape + (transformed_pts.shape[-1],)
+                )
 
-                with np.errstate(invalid='ignore'):
+                with np.errstate(invalid="ignore"):
                     edge_lengths = np.hypot(
                         np.diff(transformed_pts[..., 0], axis=1),
-                        np.diff(transformed_pts[..., 1], axis=1)
+                        np.diff(transformed_pts[..., 1], axis=1),
                     )
                     mask = (
-                        (edge_lengths > abs(self.ax.projection.x_limits[1] -
-                                            self.ax.projection.x_limits[0]) / 2) |
-                        np.isnan(edge_lengths)
+                        (
+                            edge_lengths
+                            > abs(
+                                self.ax.projection.x_limits[1]
+                                - self.ax.projection.x_limits[0]
+                            )
+                            / 2
+                        )
+                        | np.isnan(edge_lengths)
                     ).any(1)
 
                 # if so, we create a wrapped collection that is transformed in
                 # the standard matplotlib way.
                 if mask.any():
                     wrapped_arr = arr[mask]
                     arr = arr[~mask]
                     xb_wrap = xb[mask]
                     yb_wrap = yb[mask]
                     xb = xb[~mask]
                     yb = yb[~mask]
-            self.logger.debug('Making plot with %i cells', arr.size)
-            transformed = proj.transform_points(
-                t, xb.ravel(), yb.ravel())[...,:2].reshape(xb.shape + (2,))
+            self.logger.debug("Making plot with %i cells", arr.size)
+            transformed = proj.transform_points(t, xb.ravel(), yb.ravel())[
+                ..., :2
+            ].reshape(xb.shape + (2,))
             arr = arr.ravel()
             self._plot = PolyCollection(
-                transformed, array=arr.ravel(),
-                norm=self.bounds.norm, rasterized=True, cmap=cmap,
-                edgecolors='none', antialiaseds=False)
-            self.logger.debug('Adding collection to axes')
+                transformed,
+                array=arr.ravel(),
+                norm=self.bounds.norm,
+                rasterized=True,
+                cmap=cmap,
+                edgecolors="none",
+                antialiaseds=False,
+            )
+            self.logger.debug("Adding collection to axes")
             self.ax.add_collection(self._plot)
             if cartopy.__version__ <= "0.18":
                 self._plot.set_clip_path(self.ax.outline_patch)
             if wrapped_arr is not None:
-                self.logger.debug('Making wrapped plot with %i cells',
-                                  wrapped_arr.size)
+                self.logger.debug(
+                    "Making wrapped plot with %i cells", wrapped_arr.size
+                )
                 self._wrapped_plot = PolyCollection(
-                    np.dstack([xb_wrap, yb_wrap]), array=wrapped_arr.ravel(),
-                    norm=self.bounds.norm, rasterized=True, cmap=cmap,
-                    transform=t, zorder=self._plot.zorder - 0.1,
-                    edgecolors='none', antialiaseds=False)
-                self.logger.debug('Adding wrapped collection to axes')
+                    np.dstack([xb_wrap, yb_wrap]),
+                    array=wrapped_arr.ravel(),
+                    norm=self.bounds.norm,
+                    rasterized=True,
+                    cmap=cmap,
+                    transform=t,
+                    zorder=self._plot.zorder - 0.1,
+                    edgecolors="none",
+                    antialiaseds=False,
+                )
+                self.logger.debug("Adding wrapped collection to axes")
                 self.ax.add_collection(self._wrapped_plot)
                 if cartopy.__version__ <= "0.18":
                     self._wrapped_plot.set_clip_path(self.ax.outline_patch)
-        self.logger.debug('Done.')
+        self.logger.debug("Done.")
 
     def remove(self, *args, **kwargs):
         super(MapPlot2D, self).remove(*args, **kwargs)
-        if hasattr(self, '_wrapped_plot'):
+        if hasattr(self, "_wrapped_plot"):
             self._wrapped_plot.remove()
             del self._wrapped_plot
 
     def add2format_coord(self, x, y):
         x, y = self.transform.projection.transform_point(
-            x, y, self.ax.projection)
+            x, y, self.ax.projection
+        )
         # shift if necessary
         if isinstance(self.transform.projection, ccrs.PlateCarree):
             coord = self.xcoord
             if coord.min() >= 0 and x < 0:
                 x -= 360
             elif coord.max() <= 180 and x > 180:
                 x -= 360
-            if 'rad' in coord.attrs.get('units', '').lower():
+            if "rad" in coord.attrs.get("units", "").lower():
                 x = np.deg2rad(x)
                 y = np.deg2rad(y)
         return super(MapPlot2D, self).add2format_coord(x, y)
 
 
 class MapDataGrid(psyps.DataGrid):
-
-    __doc__ = psyps.DataGrid.__doc__ + '\n' + docstrings.dedent("""
+    __doc__ = (
+        psyps.DataGrid.__doc__
+        + "\n"
+        + docstrings.dedent(
+            """
     See Also
     --------
     xgrid
-    ygrid""")
+    ygrid"""
+        )
+    )
 
     def update(self, value):
         self.remove()
         if value is None:
             return
         xb = self.cell_nodes_x
         yb = self.cell_nodes_y
@@ -1842,34 +2034,44 @@
         # HACK: We remove the cells at the boundary of the map projection
         xb_wrap = None
 
         if xb.ndim > 2:
             xb = xb.reshape((-1, xb.shape[-1]))
             yb = yb.reshape((-1, yb.shape[-1]))
 
-        if isinstance(t, wrap_proj_types) and 'lon_0' in proj.proj4_params:
+        if isinstance(t, wrap_proj_types) and "lon_0" in proj.proj4_params:
             # See the :meth:`MapPlot2D._polycolor` method for a documentation
             # of the steps
-            trans_to_data = t.as_geodetic()._as_mpl_transform(self.ax) - \
-                self.ax.transData
+            trans_to_data = (
+                t.as_geodetic()._as_mpl_transform(self.ax) - self.ax.transData
+            )
 
-            coords = np.column_stack((xb.flat, yb.flat)).astype(float, copy=False)
+            coords = np.column_stack((xb.flat, yb.flat)).astype(
+                float, copy=False
+            )
             transformed_pts = trans_to_data.transform(coords)
             transformed_pts = transformed_pts.reshape(
-                xb.shape + (transformed_pts.shape[-1], ))
+                xb.shape + (transformed_pts.shape[-1],)
+            )
 
-            with np.errstate(invalid='ignore'):
+            with np.errstate(invalid="ignore"):
                 edge_lengths = np.hypot(
                     np.diff(transformed_pts[..., 0], axis=1),
-                    np.diff(transformed_pts[..., 1], axis=1)
+                    np.diff(transformed_pts[..., 1], axis=1),
                 )
                 mask = (
-                    (edge_lengths > abs(self.ax.projection.x_limits[1] -
-                                        self.ax.projection.x_limits[0]) / 2) |
-                    np.isnan(edge_lengths)
+                    (
+                        edge_lengths
+                        > abs(
+                            self.ax.projection.x_limits[1]
+                            - self.ax.projection.x_limits[0]
+                        )
+                        / 2
+                    )
+                    | np.isnan(edge_lengths)
                 ).any(1)
 
             if mask.any():
                 xb_wrap = xb[mask]
                 yb_wrap = yb[mask]
                 xb = xb[~mask]
                 yb = yb[~mask]
@@ -1893,216 +2095,247 @@
             # first we drop all grid cells that have any NaN in their bounds
             # as we do not know, how to handle these
             valid = (~np.isnan(xb_wrap).any(-1)) & (~np.isnan(yb_wrap).any(-1))
             xb_wrap = xb_wrap[valid]
             yb_wrap = yb_wrap[valid]
 
             if isinstance(t, ccrs.PlateCarree):
-
                 # identify the grid cells at the boundary
                 xdiff2min = xb_wrap - xb_wrap.min(axis=-1, keepdims=True)
                 cross_world_mask = np.any(np.abs(xdiff2min) > 180, -1)
                 if cross_world_mask.any():
                     cross_world_x = xb_wrap[cross_world_mask]
                     cross_world_y = yb_wrap[cross_world_mask]
                     cross_world_diff = xdiff2min[cross_world_mask]
                     xdiff2max = cross_world_x - cross_world_x.max(
-                        axis=-1, keepdims=True)
+                        axis=-1, keepdims=True
+                    )
 
                     leftx = cross_world_x.copy()
                     leftx[cross_world_diff > 180] -= 360
 
                     rightx = cross_world_x.copy()
                     rightx[xdiff2max < -180] += 360
 
                     xb_wrap = np.r_[xb_wrap[~cross_world_mask], leftx, rightx]
                     yb_wrap = np.r_[
-                        yb_wrap[~cross_world_mask], cross_world_y, cross_world_y
+                        yb_wrap[~cross_world_mask],
+                        cross_world_y,
+                        cross_world_y,
                     ]
 
             n = len(xb_wrap)
             xb_wrap = np.c_[xb_wrap, xb_wrap[:, :1], [[np.nan]] * n].ravel()
             yb_wrap = np.c_[yb_wrap, yb_wrap[:, :1], [[np.nan]] * n].ravel()
             if isinstance(value, dict):
-                self._artists.extend(self.ax.plot(xb_wrap, yb_wrap,
-                                                  transform=t, **value))
+                self._artists.extend(
+                    self.ax.plot(xb_wrap, yb_wrap, transform=t, **value)
+                )
             else:
-                self._artists.extend(self.ax.plot(xb_wrap, yb_wrap, value,
-                                                  transform=t))
+                self._artists.extend(
+                    self.ax.plot(xb_wrap, yb_wrap, value, transform=t)
+                )
 
 
 class MapDensity(psyps.Density):
     """
     Change the density of the arrows
 
     Possible types
     --------------
     %(Density.possible_types)s"""
 
     dependencies = psyps.Density.dependencies + ["projection"]
 
     def _set_quiver_density(self, value):
         if all(val == 1.0 for val in value):
-            self.plot._kwargs.pop('regrid_shape', None)
-            self.plot._kwargs.pop('target_extent', None)
+            self.plot._kwargs.pop("regrid_shape", None)
+            self.plot._kwargs.pop("target_extent", None)
         elif self.decoder.is_unstructured(self.raw_data):
-            warnings.warn("Quiver plot of unstructered data does not support "
-                          "the density keyword!", RuntimeWarning)
+            warnings.warn(
+                "Quiver plot of unstructered data does not support "
+                "the density keyword!",
+                RuntimeWarning,
+            )
         elif self.decoder.is_circumpolar(self.raw_data):
-            warnings.warn("Quiver plot of circumpolar data does not support "
-                          "the density keyword!", RuntimeWarning)
+            warnings.warn(
+                "Quiver plot of circumpolar data does not support "
+                "the density keyword!",
+                RuntimeWarning,
+            )
         else:
             shape = self.data.shape[-2:]
-            value = map(int, [value[0]*shape[0], value[1]*shape[1]])
-            self.plot._kwargs['regrid_shape'] = tuple(value)
+            value = map(int, [value[0] * shape[0], value[1] * shape[1]])
+            self.plot._kwargs["regrid_shape"] = tuple(value)
             lonlatbox = self.projection.lonlatbox_transformed
             self.plot._kwargs["target_extent"] = lonlatbox
 
     def _unset_quiver_density(self):
-        self.plot._kwargs.pop('regrid_shape', None)
+        self.plot._kwargs.pop("regrid_shape", None)
 
 
 class MapVectorColor(psyps.VectorColor):
-
     __doc__ = psyps.VectorColor.__doc__
 
     def _maybe_ravel(self, arr):
         # no need to ravel the data for quiver plots
         return np.asarray(arr)
 
 
 class MapVectorPlot(psyps.VectorPlot):
-
     __doc__ = psyps.VectorPlot.__doc__
 
     dependencies = psyps.VectorPlot.dependencies + [
-        'lonlatbox', 'transform', 'clon', 'clat', 'clip', 'transpose']
+        "lonlatbox",
+        "transform",
+        "clon",
+        "clat",
+        "clip",
+        "transpose",
+    ]
 
     def set_value(self, value, *args, **kwargs):
         # stream plots for circumpolar grids is not supported
-        if (value == 'stream' and self.raw_data is not None and
-                self.decoder.is_circumpolar(self.raw_data[0])):
-            warnings.warn('Cannot make stream plots of circumpolar data!')
-            value = 'quiver'
+        if (
+            value == "stream"
+            and self.raw_data is not None
+            and self.decoder.is_circumpolar(self.raw_data[0])
+        ):
+            warnings.warn("Cannot make stream plots of circumpolar data!")
+            value = "quiver"
         super(MapVectorPlot, self).set_value(value, *args, **kwargs)
 
     set_value.__doc__ = psyps.VectorPlot.set_value.__doc__
 
     def _get_data(self):
         data = self.data
         base_data = self.raw_data
         base_var = next(base_data.psy.iter_base_variables)
         u, v = data[-2:].values
         x = base_data.psy.decoder.get_x(base_var, coords=data.coords)
         y = base_data.psy.decoder.get_y(base_var, coords=data.coords)
-        x = x.values * 180. / np.pi if x.attrs.get('units') == 'radian' else \
-            x.values
-        y = y.values * 180. / np.pi if y.attrs.get('units') == 'radian' else \
-            y.values
+        x = (
+            x.values * 180.0 / np.pi
+            if x.attrs.get("units") == "radian"
+            else x.values
+        )
+        y = (
+            y.values * 180.0 / np.pi
+            if y.attrs.get("units") == "radian"
+            else y.values
+        )
         # we transform here manually because the transform keyword does not
         # work with unstructered grids and it sometimes shifts the plot data
         # for quiver and stream plots
         transform = self.transform.projection
         if x.ndim == 1 and u.ndim == 2:
             x, y = np.meshgrid(x, y)
         if self.transpose.value and x.shape != u.shape:
             x = x.T
             y = y.T
         u, v = self.ax.projection.transform_vectors(transform, x, y, u, v)
         ret = self.ax.projection.transform_points(transform, x, y)
         x = ret[..., 0]
         y = ret[..., 1]
-        self._kwargs.pop('transform', None)  # = self.ax.projection
+        self._kwargs.pop("transform", None)  # = self.ax.projection
         return x, y, u, v
 
     def _stream_plot(self):
         if self.decoder.is_circumpolar(self.raw_data):
-            warnings.warn('Cannot make stream plots of circumpolar data!')
+            warnings.warn("Cannot make stream plots of circumpolar data!")
             return
         # update map extent such that it fits to the data limits (necessary
         # because streamplot scales the density based upon it). This however
         # does not work for matplotlib 1.5.0
-        if not (mpl.__version__ == '1.5.0' and self.color.colored):
-            self.ax.set_extent(self.lonlatbox.lonlatbox,
-                               crs=ccrs.PlateCarree())
+        if not (mpl.__version__ == "1.5.0" and self.color.colored):
+            self.ax.set_extent(
+                self.lonlatbox.lonlatbox, crs=ccrs.PlateCarree()
+            )
         else:
             self.ax.set_global()
         # Note that this method uses a bug fix through the
         # :class:`psyplot.plotter.colors.FixedColorMap` class
         # and one through the :class:`psyplot.plotter.colors.FixedBoundaryNorm`
         # class
         x, y, u, v = self._get_data()
-        norm = self._kwargs.get('norm')
+        norm = self._kwargs.get("norm")
         if isinstance(norm, BoundaryNorm):
-            self._kwargs['norm'] = FixedBoundaryNorm(
-                norm.boundaries, norm.Ncmap, norm.clip)
+            self._kwargs["norm"] = FixedBoundaryNorm(
+                norm.boundaries, norm.Ncmap, norm.clip
+            )
         self._plot = self.ax.streamplot(x, y, u, v, **self._kwargs)
 
     def add2format_coord(self, x, y):
         x, y = self.transform.projection.transform_point(
-            x, y, self.ax.projection)
+            x, y, self.ax.projection
+        )
         # shift if necessary
         if isinstance(self.transform.projection, ccrs.PlateCarree):
             coord = self.xcoord
             if coord.min() >= 0 and x < 0:
                 x -= 360
             elif coord.max() <= 180 and x > 180:
                 x -= 360
         return super(MapVectorPlot, self).add2format_coord(x, y)
 
 
 class CombinedMapVectorPlot(MapVectorPlot):
-
     __doc__ = MapVectorPlot.__doc__
 
     def update(self, *args, **kwargs):
-        self._kwargs['zorder'] = 2
+        self._kwargs["zorder"] = 2
         super(CombinedMapVectorPlot, self).update(*args, **kwargs)
 
 
 class MapPlotter(psyps.Base2D):
-    """Base plotter for visualizing data on a map
-    """
+    """Base plotter for visualizing data on a map"""
 
-    _rcparams_string = ['plotter.maps.']
+    _rcparams_string = ["plotter.maps."]
 
-    background = MapBackground('background')
+    background = MapBackground("background")
 
-    transpose = Transpose('transpose')
-    projection = Projection('projection')
-    transform = Transform('transform')
-    clon = CenterLon('clon')
-    clat = CenterLat('clat')
-    lonlatbox = LonLatBox('lonlatbox')
-    lsm = LSM('lsm')
-    stock_img = StockImage('stock_img')
-    grid_color = GridColor('grid_color')
-    grid_labels = GridLabels('grid_labels')
-    grid_labelsize = GridLabelSize('grid_labelsize')
-    grid_settings = GridSettings('grid_settings')
-    xgrid = XGrid('xgrid')
-    ygrid = YGrid('ygrid')
-    map_extent = MapExtent('map_extent')
-    datagrid = MapDataGrid('datagrid', index_in_list=0)
-    clip = ClipAxes('clip')
+    transpose = Transpose("transpose")
+    projection = Projection("projection")
+    transform = Transform("transform")
+    clon = CenterLon("clon")
+    clat = CenterLat("clat")
+    lonlatbox = LonLatBox("lonlatbox")
+    lsm = LSM("lsm")
+    stock_img = StockImage("stock_img")
+    grid_color = GridColor("grid_color")
+    grid_labels = GridLabels("grid_labels")
+    grid_labelsize = GridLabelSize("grid_labelsize")
+    grid_settings = GridSettings("grid_settings")
+    xgrid = XGrid("xgrid")
+    ygrid = YGrid("ygrid")
+    map_extent = MapExtent("map_extent")
+    google_map_detail = GoogleMap("google_map_detail")
+    datagrid = MapDataGrid("datagrid", index_in_list=0)
+    clip = ClipAxes("clip")
 
     @classmethod
     def _get_sample_projection(cls):
         """Returns None. May be subclassed to retumeshrn a projection that
         can be used when creating a subplot"""
         return ccrs.PlateCarree()
 
     @property
     def ax(self):
         """Axes instance of the plot"""
         if self._ax is None:
             import matplotlib.pyplot as plt
+
             plt.figure()
-            self._ax = plt.axes(projection=getattr(
-                self.projection, 'projection', self._get_sample_projection()))
+            self._ax = plt.axes(
+                projection=getattr(
+                    self.projection,
+                    "projection",
+                    self._get_sample_projection(),
+                )
+            )
         return self._ax
 
     @ax.setter
     def ax(self, value):
         self._ax = value
 
     @docstrings.dedent
@@ -2118,66 +2351,90 @@
 
         Returns
         -------
         %(Formatoption.convert_coordinate.returns)s
         """
 
         def in_rad(var):
-            return var.attrs.get('units', '').startswith('radian')
+            return var.attrs.get("units", "").startswith("radian")
 
         def in_km(var):
-            return var.attrs.get('units', '') == "km"
+            return var.attrs.get("units", "") == "km"
 
         if any(map(in_rad, chain([coord], variables))):
-            coord = coord.copy(data=coord * 180. / np.pi)
+            coord = coord.copy(data=coord * 180.0 / np.pi)
             coord.attrs["units"] = "degrees"
         elif any(map(in_km, chain([coord], variables))):
             coord = coord.copy(data=coord * 1000)
             coord.attrs["units"] = "m"
 
         return coord
 
+    def fix_map_extent(self):
+        """Fix the map extent to the current extent of the axes.
+
+        This method updates the :attr:`map_extent` formatoption to the
+        current extent of the axes of the plotter.
+        """
+        self["map_extent"] = self.ax.get_extent(ccrs.PlateCarree())
+
+    @docstrings.dedent
+    def fix_lonlatbox(self, *args, **kwargs):
+        """Fix the data to the current extent of the axes.
+
+        This method updates the :attr:`map_extent` formatoption to the
+        current extent of the axes of the plotter.
+
+        Parameters
+        ----------
+        %(Plotter.update.parameters)s
+        """
+        extent = self.ax.get_extent(ccrs.PlateCarree())
+        self.update(lonlatbox=extent)
+
 
 class FieldPlotter(psyps.Simple2DBase, MapPlotter, psyps.BasePlotter):
-    """Plotter for 2D scalar fields on a map
-    """
+    """Plotter for 2D scalar fields on a map"""
 
-    _rcparams_string = ['plotter.fieldplotter']
+    _rcparams_string = ["plotter.fieldplotter"]
 
-    levels = psyps.ContourLevels('levels', cbounds='bounds')
+    levels = psyps.ContourLevels("levels", cbounds="bounds")
     try:
-        interp_bounds = psyps.InterpolateBounds('interp_bounds')
+        interp_bounds = psyps.InterpolateBounds("interp_bounds")
     except AttributeError:
         pass
-    plot = MapPlot2D('plot')
+    plot = MapPlot2D("plot")
 
 
 class VectorPlotter(MapPlotter, psyps.BaseVectorPlotter, psyps.BasePlotter):
     """Plotter for visualizing 2-dimensional vector data on a map
 
     See Also
     --------
     psyplot.plotter.simple.SimpleVectorPlotter:
         for a simple version of drawing vector data
     FieldPlotter: for plotting scaler fields
     CombinedPlotter: for combined scalar and vector fields
     """
-    _rcparams_string = ['plotter.vectorplotter']
-    plot = MapVectorPlot('plot')
-    density = MapDensity('density')
-    color = MapVectorColor('color')
+
+    _rcparams_string = ["plotter.vectorplotter"]
+    plot = MapVectorPlot("plot")
+    density = MapDensity("density")
+    color = MapVectorColor("color")
 
 
 class CombinedPlotter(psyps.CombinedBase, FieldPlotter, VectorPlotter):
     """Combined 2D plotter and vector plotter on a map
 
     See Also
     --------
     psyplot.plotter.simple.CombinedSimplePlotter:
         for a simple version of this class
     FieldPlotter, VectorPlotter"""
-    plot = MapPlot2D('plot', index_in_list=0)
-    vplot = CombinedMapVectorPlot('vplot', cmap='vcmap', bounds='vbounds',
-                                  index_in_list=1)
-    density = MapDensity('density', plot='vplot', index_in_list=1)
-    xgrid = XGrid('xgrid', index_in_list=1)
-    ygrid = YGrid('ygrid', index_in_list=1)
+
+    plot = MapPlot2D("plot", index_in_list=0)
+    vplot = CombinedMapVectorPlot(
+        "vplot", cmap="vcmap", bounds="vbounds", index_in_list=1
+    )
+    density = MapDensity("density", plot="vplot", index_in_list=1)
+    xgrid = XGrid("xgrid", index_in_list=1)
+    ygrid = YGrid("ygrid", index_in_list=1)
```

### Comparing `psy-maps-1.4.2/psy_maps/plugin.py` & `psy-maps-1.5.0/psy_maps/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 """psy-maps psyplot plugin
 
 This module defines the rcParams for the psy-maps plugin"""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psy-maps and is released under the GNU LGPL-3.O license.
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
 
+from os.path import exists as validate_path_exists
 
 import six
 import yaml
-from psyplot.config.rcsetup import RcParams
-from os.path import exists as validate_path_exists
 from psy_simple.plugin import (
-    try_and_error, validate_none, validate_str, validate_float,
-    validate_bool_maybe_none, validate_fontsize,
-    validate_color, validate_dict, BoundsValidator, bound_strings,
-    ValidateInStrings, validate_bool, BoundsType, DictValValidator)
+    BoundsType,
+    BoundsValidator,
+    ValidateInStrings,
+    try_and_error,
+    validate_bool,
+    validate_bool_maybe_none,
+    validate_color,
+    validate_dict,
+    validate_float,
+    validate_fontsize,
+    validate_int,
+    validate_none,
+    validate_str,
+)
+from psyplot.config.rcsetup import RcParams
+
 from psy_maps import __version__ as plugin_version
 
 
 def get_versions(requirements=True):
     if requirements:
         import cartopy
-        return {'version': plugin_version,
-                'requirements': {'cartopy': cartopy.__version__}}
+
+        return {
+            "version": plugin_version,
+            "requirements": {"cartopy": cartopy.__version__},
+        }
     else:
-        return {'version': plugin_version}
+        return {"version": plugin_version}
 
 
 def patch_prior_1_0(plotter_d, versions):
     """Patch psy_maps plotters for versions smaller than 1.0
 
     Before psyplot 1.0.0, the plotters in the psy_maps package where part of
     the psyplot.plotter.maps module. This has to be corrected"""
-    plotter_d['cls'] = ('psy_maps.plotters', plotter_d['cls'][1])
+    plotter_d["cls"] = ("psy_maps.plotters", plotter_d["cls"][1])
 
 
 #: patches to apply when loading a project
 patches = {
-    ('psyplot.plotter.maps', 'MapPlotter'): patch_prior_1_0,
-    ('psyplot.plotter.maps', 'VectorPlotter'): patch_prior_1_0,
-    ('psyplot.plotter.maps', 'FieldPlotter'): patch_prior_1_0,
-    ('psyplot.plotter.maps', 'CombinedPlotter'): patch_prior_1_0,
-    }
+    ("psyplot.plotter.maps", "MapPlotter"): patch_prior_1_0,
+    ("psyplot.plotter.maps", "VectorPlotter"): patch_prior_1_0,
+    ("psyplot.plotter.maps", "FieldPlotter"): patch_prior_1_0,
+    ("psyplot.plotter.maps", "CombinedPlotter"): patch_prior_1_0,
+}
 
 
 # -----------------------------------------------------------------------------
 # ------------------------- validation functions ------------------------------
 # -----------------------------------------------------------------------------
 
 
@@ -75,70 +72,70 @@
     try:
         return validate_bool_maybe_none(val)
     except ValueError:
         return BoundsValidator(BoundsType)(val)
 
 
 def validate_lsm(val):
-    res_validation = ValidateInStrings('lsm', ['110m', '50m' ,'10m'])
+    res_validation = ValidateInStrings("lsm", ["110m", "50m", "10m"])
     if not val:
         val = {}
     elif isinstance(val, dict):
         invalid = set(val).difference(
-            ['coast', 'land', 'ocean', 'res', 'linewidth'])
+            ["coast", "land", "ocean", "res", "linewidth"]
+        )
         if invalid:
             raise ValueError(f"Invalid keys for lsm: {invalid}")
     else:
         # First try, if it's a bool, if yes, use 110m
         # then try, if it's a valid resolution
         # then try, if it's a float (i.e. the linewidth)
         # then try if it's a tuple [res, lw]
         try:
             validate_bool(val)
         except (ValueError, TypeError):
             pass
         else:
-            val = '110m'
+            val = "110m"
         try:
             val = res_validation(val)
         except (ValueError, TypeError):
             pass
         else:
             if not isinstance(val, str):
-                val = '110m'
-            val = {'res': val, 'linewidth': 1.0, 'coast': 'k'}
+                val = "110m"
+            val = {"res": val, "linewidth": 1.0, "coast": "k"}
         try:
             val = validate_float(val)
         except (ValueError, TypeError):
             pass
         else:
-            val = {'res': '110m', 'linewidth': val, 'coast': 'k'}
+            val = {"res": "110m", "linewidth": val, "coast": "k"}
     if not isinstance(val, dict):
         try:
             res, lw = val
         except (ValueError, TypeError):
             raise ValueError(f"Invalid lsm configuration: {val}")
         else:
-            val = {'res': res, 'linewidth': lw}
+            val = {"res": res, "linewidth": lw}
     val = dict(val)
     for key, v in val.items():
-        if key in ['coast', 'land', 'ocean']:
+        if key in ["coast", "land", "ocean"]:
             val[key] = validate_color(v)
-        elif key == 'res':
+        elif key == "res":
             val[key] = res_validation(v)
         else:
             val[key] = validate_float(v)  # linewidth
     # finally set black color if linewidth is in val
-    if 'linewidth' in val:
-        val.setdefault('coast', 'k')
+    if "linewidth" in val:
+        val.setdefault("coast", "k")
     return val
 
 
 class ProjectionValidator(ValidateInStrings):
-
     def __call__(self, val):
         if isinstance(val, six.string_types):
             return ValidateInStrings.__call__(self, val)
         return val  # otherwise we skip the validation
 
 
 def validate_dict_yaml(s):
@@ -155,134 +152,221 @@
     try:
         return validate_none(value)
     except (TypeError, ValueError):
         try:
             return validate_str(value)
         except (TypeError, ValueError):
             if len(value) != 4:
-                raise ValueError("Need 4 values for longitude-latitude box, "
-                                 "got %i" % len(value))
+                raise ValueError(
+                    "Need 4 values for longitude-latitude box, "
+                    "got %i" % len(value)
+                )
             return list(map(validate, value))
 
 
+def validate_google_map_detail(value):
+    if value is None:
+        return value
+    value = validate_int(value)
+    if value < 0:
+        raise ValueError("target_z must be an integer >=0.")
+    return value
+
+
 # -----------------------------------------------------------------------------
 # ------------------------------ rcParams -------------------------------------
 # -----------------------------------------------------------------------------
 
 
 #: the :class:`~psyplot.config.rcsetup.RcParams` for the psy-simple plugin
-rcParams = RcParams(defaultParams={
-
-    # -------------------------------------------------------------------------
-    # ----------------------- Registered plotters -----------------------------
-    # -------------------------------------------------------------------------
-
-    'project.plotters': [
-
-        {'maps': {
-             'module': 'psy_maps.plotters',
-             'plotter_name': 'MapPlotter',
-             'plot_func': False,
-             'summary': 'The data objects visualized on a map'},
-         'mapplot': {
-             'module': 'psy_maps.plotters',
-             'plotter_name': 'FieldPlotter',
-             'prefer_list': False,
-             'default_slice': 0,
-             'default_dims': {'x': slice(None), 'y': slice(None)},
-             'summary': 'Plot a 2D scalar field on a map'},
-         'mapvector': {
-             'module': 'psy_maps.plotters',
-             'plotter_name': 'VectorPlotter',
-             'prefer_list': False,
-             'default_slice': 0,
-             'default_dims': {'x': slice(None), 'y': slice(None)},
-             'summary': 'Plot a 2D vector field on a map',
-             'example_call': "filename, name=[['u_var', 'v_var']], ..."},
-         'mapcombined': {
-             'module': 'psy_maps.plotters',
-             'plotter_name': 'CombinedPlotter',
-             'prefer_list': True,
-             'default_slice': 0,
-             'default_dims': {'x': slice(None), 'y': slice(None)},
-             'summary': ('Plot a 2D scalar field with an overlying vector '
-                         'field on a map'),
-             'example_call': (
-                 "filename, name=[['my_variable', ['u_var', 'v_var']]], ...")},
-         }, validate_dict],
-
-    # -------------------------------------------------------------------------
-    # --------------------- Default formatoptions -----------------------------
-    # -------------------------------------------------------------------------
-    # MapBase
-    'plotter.maps.transpose': [
-        False, validate_bool, "Transpose the input data before plotting"],
-    'plotter.maps.lonlatbox': [
-        None, validate_lonlatbox,
-        'fmt key to define the longitude latitude box of the data'],
-    'plotter.maps.map_extent': [
-        None, validate_lonlatbox,
-        'fmt key to define the extent of the map plot'],
-    'plotter.maps.clip': [
-        None, validate_bool_maybe_none,
-        'fmt key to define clip the axes outside the latitudes'],
-    'plotter.maps.clon': [
-        None, try_and_error(validate_none, validate_float, validate_str),
-        'fmt key to specify the center longitude of the projection'],
-    'plotter.maps.clat': [
-        None, try_and_error(validate_none, validate_float, validate_str),
-        'fmt key to specify the center latitude of the projection'],
-    # TODO: Implement the drawing of shape files on a map
-    # 'plotter.maps.lineshapes': [None, try_and_error(
-    #     validate_none, validate_dict, validate_str, validate_stringlist)],
-    'plotter.maps.grid_labels': [
-        None, validate_bool_maybe_none,
-        'fmt key to draw labels of the lat-lon-grid'],
-    'plotter.maps.grid_labelsize': [
-        12.0, validate_fontsize,
-        'fmt key to modify the fontsize of the lat-lon-grid labels'],
-    'plotter.maps.grid_color': [
-        'k', try_and_error(validate_none, validate_color),
-        'fmt key to modify the color of the lat-lon-grid'],
-    'plotter.maps.grid_settings': [
-        {}, validate_dict,
-        'fmt key for additional line properties for the lat-lon-grid'],
-    'plotter.maps.xgrid': [
-        True, validate_grid, 'fmt key for drawing meridians on the map'],
-    'plotter.maps.ygrid': [
-        True, validate_grid, 'fmt key for drawing parallels on the map'],
-    'plotter.maps.projection': [
-        'cf', ProjectionValidator(
-            'projection', ['cf', 'northpole', 'ortho', 'southpole', 'moll', 'geo',
-                           'robin', 'cyl', 'stereo', 'near', 'rotated'],
-            True),
-        'fmt key to define the projection of the plot'],
-    'plotter.maps.transform': [
-        'cf', ProjectionValidator(
-            'projection', ['cf', 'northpole', 'ortho', 'southpole', 'moll', 'geo',
-                           'robin', 'cyl', 'stereo', 'near', 'rotated'],
-            True),
-        'fmt key to define the native projection of the data'],
-    'plotter.maps.lsm': [
-        True, validate_lsm,
-        'fmt key to draw a land sea mask'],
-    'plotter.maps.stock_img': [
-        False, validate_bool, 'fmt key to draw a stock_img on the map'],
-
-    # -------------------------------------------------------------------------
-    # ---------------------------- Miscallaneous ------------------------------
-    # -------------------------------------------------------------------------
-
-    # yaml file that holds definitions of lonlatboxes
-    'lonlatbox.boxes': [
-        {}, validate_dict_yaml,
-        'longitude-latitude boxes that shall be accessible for the lonlatbox, '
-        'map_extent, etc. keywords. May be a dictionary or the path to a '
-        'yaml file'],
-
-    })
+rcParams = RcParams(
+    defaultParams={
+        # -------------------------------------------------------------------------
+        # ----------------------- Registered plotters -----------------------------
+        # -------------------------------------------------------------------------
+        "project.plotters": [
+            {
+                "maps": {
+                    "module": "psy_maps.plotters",
+                    "plotter_name": "MapPlotter",
+                    "plot_func": False,
+                    "summary": "The data objects visualized on a map",
+                },
+                "mapplot": {
+                    "module": "psy_maps.plotters",
+                    "plotter_name": "FieldPlotter",
+                    "prefer_list": False,
+                    "default_slice": 0,
+                    "default_dims": {"x": slice(None), "y": slice(None)},
+                    "summary": "Plot a 2D scalar field on a map",
+                },
+                "mapvector": {
+                    "module": "psy_maps.plotters",
+                    "plotter_name": "VectorPlotter",
+                    "prefer_list": False,
+                    "default_slice": 0,
+                    "default_dims": {"x": slice(None), "y": slice(None)},
+                    "summary": "Plot a 2D vector field on a map",
+                    "example_call": "filename, name=[['u_var', 'v_var']], ...",
+                },
+                "mapcombined": {
+                    "module": "psy_maps.plotters",
+                    "plotter_name": "CombinedPlotter",
+                    "prefer_list": True,
+                    "default_slice": 0,
+                    "default_dims": {"x": slice(None), "y": slice(None)},
+                    "summary": (
+                        "Plot a 2D scalar field with an overlying vector "
+                        "field on a map"
+                    ),
+                    "example_call": (
+                        "filename, name=[['my_variable', ['u_var', 'v_var']]], ..."
+                    ),
+                },
+            },
+            validate_dict,
+        ],
+        # -------------------------------------------------------------------------
+        # --------------------- Default formatoptions -----------------------------
+        # -------------------------------------------------------------------------
+        # MapBase
+        "plotter.maps.transpose": [
+            False,
+            validate_bool,
+            "Transpose the input data before plotting",
+        ],
+        "plotter.maps.lonlatbox": [
+            None,
+            validate_lonlatbox,
+            "fmt key to define the longitude latitude box of the data",
+        ],
+        "plotter.maps.map_extent": [
+            None,
+            validate_lonlatbox,
+            "fmt key to define the extent of the map plot",
+        ],
+        "plotter.maps.google_map_detail": [
+            None,
+            validate_google_map_detail,
+            "fmt add a google image to the plot.",
+        ],
+        "plotter.maps.clip": [
+            None,
+            validate_bool_maybe_none,
+            "fmt key to define clip the axes outside the latitudes",
+        ],
+        "plotter.maps.clon": [
+            None,
+            try_and_error(validate_none, validate_float, validate_str),
+            "fmt key to specify the center longitude of the projection",
+        ],
+        "plotter.maps.clat": [
+            None,
+            try_and_error(validate_none, validate_float, validate_str),
+            "fmt key to specify the center latitude of the projection",
+        ],
+        # TODO: Implement the drawing of shape files on a map
+        # 'plotter.maps.lineshapes': [None, try_and_error(
+        #     validate_none, validate_dict, validate_str, validate_stringlist)],
+        "plotter.maps.grid_labels": [
+            None,
+            validate_bool_maybe_none,
+            "fmt key to draw labels of the lat-lon-grid",
+        ],
+        "plotter.maps.grid_labelsize": [
+            12.0,
+            validate_fontsize,
+            "fmt key to modify the fontsize of the lat-lon-grid labels",
+        ],
+        "plotter.maps.grid_color": [
+            "k",
+            try_and_error(validate_none, validate_color),
+            "fmt key to modify the color of the lat-lon-grid",
+        ],
+        "plotter.maps.grid_settings": [
+            {},
+            validate_dict,
+            "fmt key for additional line properties for the lat-lon-grid",
+        ],
+        "plotter.maps.xgrid": [
+            True,
+            validate_grid,
+            "fmt key for drawing meridians on the map",
+        ],
+        "plotter.maps.ygrid": [
+            True,
+            validate_grid,
+            "fmt key for drawing parallels on the map",
+        ],
+        "plotter.maps.projection": [
+            "cf",
+            ProjectionValidator(
+                "projection",
+                [
+                    "cf",
+                    "northpole",
+                    "ortho",
+                    "southpole",
+                    "moll",
+                    "geo",
+                    "robin",
+                    "cyl",
+                    "stereo",
+                    "near",
+                    "rotated",
+                ],
+                True,
+            ),
+            "fmt key to define the projection of the plot",
+        ],
+        "plotter.maps.transform": [
+            "cf",
+            ProjectionValidator(
+                "projection",
+                [
+                    "cf",
+                    "northpole",
+                    "ortho",
+                    "southpole",
+                    "moll",
+                    "geo",
+                    "robin",
+                    "cyl",
+                    "stereo",
+                    "near",
+                    "rotated",
+                ],
+                True,
+            ),
+            "fmt key to define the native projection of the data",
+        ],
+        "plotter.maps.lsm": [
+            True,
+            validate_lsm,
+            "fmt key to draw a land sea mask",
+        ],
+        "plotter.maps.stock_img": [
+            False,
+            validate_bool,
+            "fmt key to draw a stock_img on the map",
+        ],
+        # -------------------------------------------------------------------------
+        # ---------------------------- Miscallaneous ------------------------------
+        # -------------------------------------------------------------------------
+        # yaml file that holds definitions of lonlatboxes
+        "lonlatbox.boxes": [
+            {},
+            validate_dict_yaml,
+            "longitude-latitude boxes that shall be accessible for the lonlatbox, "
+            "map_extent, etc. keywords. May be a dictionary or the path to a "
+            "yaml file",
+        ],
+    }
+)
 
 
-rcParams._deprecated_map['plotter.maps.plot.min_circle_ratio'] = (
-    'plotter.plot2d.plot.min_circle_ratio', 0.05)
+rcParams._deprecated_map["plotter.maps.plot.min_circle_ratio"] = (
+    "plotter.plot2d.plot.min_circle_ratio",
+    0.05,
+)
 
 rcParams.update_from_defaultParams()
```

### Comparing `psy-maps-1.4.2/psy_maps/widgets/__init__.py` & `psy-maps-1.5.0/psy_maps/widgets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,45 @@
 """Formatoption widgets for psy-maps."""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psy-maps and is released under the GNU LGPL-3.O license.
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
 
 import contextlib
-from PyQt5 import QtWidgets, QtGui
+
 import psy_simple.widgets.colors as psyps_wcol
+from PyQt5 import QtGui, QtWidgets
 
 
 class LSMFmtWidget(QtWidgets.QWidget):
     """The widget for the land-sea-mask formatoption"""
 
     def __init__(self, parent, fmto, project):
         super().__init__()
         import cartopy.feature as cf
+
         self.editor = parent
 
-        self.cb_land = QtWidgets.QCheckBox('Land')
-        self.cb_ocean = QtWidgets.QCheckBox('Ocean')
-        self.cb_coast = QtWidgets.QCheckBox('Coastlines')
-
-        self.land_color = psyps_wcol.ColorLabel(cf.LAND._kwargs['facecolor'])
-        self.ocean_color = psyps_wcol.ColorLabel(cf.OCEAN._kwargs['facecolor'])
-        self.coast_color = psyps_wcol.ColorLabel('k')
+        self.cb_land = QtWidgets.QCheckBox("Land")
+        self.cb_ocean = QtWidgets.QCheckBox("Ocean")
+        self.cb_coast = QtWidgets.QCheckBox("Coastlines")
+
+        self.land_color = psyps_wcol.ColorLabel(cf.LAND._kwargs["facecolor"])
+        self.ocean_color = psyps_wcol.ColorLabel(cf.OCEAN._kwargs["facecolor"])
+        self.coast_color = psyps_wcol.ColorLabel("k")
 
         self.txt_linewidth = QtWidgets.QLineEdit()
         self.txt_linewidth.setValidator(QtGui.QDoubleValidator(0, 100, 4))
-        self.txt_linewidth.setPlaceholderText('Linewidth of coastlines')
-        self.txt_linewidth.setToolTip('Linewidth of coastlines')
+        self.txt_linewidth.setPlaceholderText("Linewidth of coastlines")
+        self.txt_linewidth.setToolTip("Linewidth of coastlines")
 
         self.combo_resolution = QtWidgets.QComboBox()
-        self.combo_resolution.addItems(['110m', '50m', '10m'])
+        self.combo_resolution.addItems(["110m", "50m", "10m"])
 
         self.refresh(fmto.value)
 
         hbox = QtWidgets.QHBoxLayout()
         hbox.addWidget(self.cb_land)
         hbox.addWidget(self.land_color)
         hbox.addWidget(self.cb_ocean)
@@ -65,30 +50,31 @@
         hbox.addWidget(self.combo_resolution)
         self.setLayout(hbox)
 
         for cb in [self.cb_land, self.cb_ocean, self.cb_coast]:
             cb.stateChanged.connect(self.toggle_and_update)
         self.txt_linewidth.textEdited.connect(self.toggle_and_update)
         self.combo_resolution.currentIndexChanged.connect(
-            self.toggle_and_update)
+            self.toggle_and_update
+        )
         for lbl in [self.land_color, self.ocean_color, self.coast_color]:
             lbl.color_changed.connect(self.toggle_and_update)
 
     @property
     def value(self):
         ret = {}
         if self.cb_land.isChecked():
-            ret['land'] = list(self.land_color.color.getRgbF())
+            ret["land"] = list(self.land_color.color.getRgbF())
         if self.cb_ocean.isChecked():
-            ret['ocean'] = list(self.ocean_color.color.getRgbF())
+            ret["ocean"] = list(self.ocean_color.color.getRgbF())
         if self.cb_coast.isChecked():
-            ret['coast'] = list(self.coast_color.color.getRgbF())
-            ret['linewidth'] = float(self.txt_linewidth.text().strip() or 0.0)
+            ret["coast"] = list(self.coast_color.color.getRgbF())
+            ret["linewidth"] = float(self.txt_linewidth.text().strip() or 0.0)
         if ret:
-            ret['res'] = self.combo_resolution.currentText()
+            ret["res"] = self.combo_resolution.currentText()
         return ret
 
     def toggle_and_update(self):
         self.toggle_color_labels()
         value = self.value
         self.editor.set_obj(value)
 
@@ -97,82 +83,88 @@
         self.ocean_color.setEnabled(self.cb_ocean.isChecked())
 
         self.coast_color.setEnabled(self.cb_coast.isChecked())
         self.txt_linewidth.setEnabled(self.cb_coast.isChecked())
 
     @contextlib.contextmanager
     def block_widgets(self, *widgets):
-        widgets = widgets or [self.cb_land, self.cb_ocean, self.cb_coast,
-                              self.land_color, self.ocean_color,
-                              self.coast_color,
-                              self.txt_linewidth, self.combo_resolution]
+        widgets = widgets or [
+            self.cb_land,
+            self.cb_ocean,
+            self.cb_coast,
+            self.land_color,
+            self.ocean_color,
+            self.coast_color,
+            self.txt_linewidth,
+            self.combo_resolution,
+        ]
         for w in widgets:
             w.blockSignals(True)
         yield
         for w in widgets:
             w.blockSignals(False)
 
     def refresh(self, value):
         with self.block_widgets():
-            self.cb_land.setChecked('land' in value)
-            self.cb_ocean.setChecked('ocean' in value)
-            self.cb_coast.setChecked('coast' in value)
-
-            if 'linewidth' in value:
-                self.txt_linewidth.setText(str(value['linewidth']))
-            elif 'coast' in value:
-                self.txt_linewidth.setText('1.0')
+            self.cb_land.setChecked("land" in value)
+            self.cb_ocean.setChecked("ocean" in value)
+            self.cb_coast.setChecked("coast" in value)
+
+            if "linewidth" in value:
+                self.txt_linewidth.setText(str(value["linewidth"]))
+            elif "coast" in value:
+                self.txt_linewidth.setText("1.0")
             else:
-                self.txt_linewidth.setText('')
+                self.txt_linewidth.setText("")
 
-            if 'res' in value:
-                self.combo_resolution.setCurrentText(value['res'])
+            if "res" in value:
+                self.combo_resolution.setCurrentText(value["res"])
             else:
-                self.combo_resolution.setCurrentText('110m')
+                self.combo_resolution.setCurrentText("110m")
 
-            if 'land' in value:
-                self.land_color._set_color(value['land'])
-            if 'ocean' in value:
-                self.ocean_color._set_color(value['ocean'])
-            if 'coast' in value:
-                self.coast_color._set_color(value['coast'])
+            if "land" in value:
+                self.land_color._set_color(value["land"])
+            if "ocean" in value:
+                self.ocean_color._set_color(value["ocean"])
+            if "coast" in value:
+                self.coast_color._set_color(value["coast"])
 
             self.toggle_color_labels()
 
 
 class GridFmtWidget(psyps_wcol.CTicksFmtWidget):
     """The formatoption widget for xgrid and ygrid"""
 
-    methods = ['Discrete', 'Auto', 'Disable']
+    methods = ["Discrete", "Auto", "Disable"]
 
     methods_type = psyps_wcol.BoundsType
 
     auto_val = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs, properties=False)
 
     def set_value(self, value):
         if value is False or value is None:
             with self.block_widgets(self.method_combo, self.type_combo):
-                self.type_combo.setCurrentText('Disable')
-            self.refresh_methods('Disable')
+                self.type_combo.setCurrentText("Disable")
+            self.refresh_methods("Disable")
         else:
             super().set_value(value)
 
     def refresh_methods(self, text):
-        if text == 'Disable':
+        if text == "Disable":
             with self.block_widgets(self.method_combo):
                 self.method_combo.clear()
             self.set_obj(False)
             self.refresh_current_widget()
         else:
             super().refresh_methods(text)
 
     def refresh_current_widget(self):
         w = self.current_widget
-        no_lines = self.type_combo.currentText() == 'Disable'
+        no_lines = self.type_combo.currentText() == "Disable"
         if no_lines and w is not None:
             w.setVisible(False)
             self.current_widget = None
         if not no_lines:
-            super().refresh_current_widget()
+            super().refresh_current_widget()
```

