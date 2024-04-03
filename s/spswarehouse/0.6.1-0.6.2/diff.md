# Comparing `tmp/spswarehouse-0.6.1.tar.gz` & `tmp/spswarehouse-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spswarehouse-0.6.1.tar", last modified: Tue Nov 14 20:42:02 2023, max compression
+gzip compressed data, was "spswarehouse-0.6.2.tar", last modified: Wed Apr  3 17:48:11 2024, max compression
```

## Comparing `spswarehouse-0.6.1.tar` & `spswarehouse-0.6.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-11-14 20:42:02.521600 spswarehouse-0.6.1/
--rw-rw-rw-   0        0        0    35149 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/LICENSE
--rw-rw-rw-   0        0        0      438 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8200 2023-11-14 20:42:02.520595 spswarehouse-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     7614 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/README.md
--rw-rw-rw-   0        0        0       42 2023-11-14 20:42:02.522574 spswarehouse-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-11-14 20:41:35.000000 spswarehouse-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-14 20:42:02.394530 spswarehouse-0.6.1/spswarehouse/
--rw-rw-rw-   0        0        0      561 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-14 20:42:02.447578 spswarehouse-0.6.1/spswarehouse/calpads/
--rw-rw-rw-   0        0        0        0 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/calpads/__init__.py
--rw-rw-rw-   0        0        0    39927 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/calpads/calpads.py
--rw-rw-rw-   0        0        0     6024 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/calpads/calpads_config.py
--rw-rw-rw-   0        0        0     1143 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/credentials.py.template
-drwxrwxrwx   0        0        0        0 2023-11-14 20:42:02.471589 spswarehouse-0.6.1/spswarehouse/general/
--rw-rw-rw-   0        0        0        0 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/general/__init__.py
--rw-rw-rw-   0        0        0      708 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/general/os.py
--rw-rw-rw-   0        0        0    13727 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/general/selenium.py
--rw-rw-rw-   0        0        0     2090 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/googledrive.py
--rw-rw-rw-   0        0        0     1980 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/googlesheets.py
--rw-rw-rw-   0        0        0     2013 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/googleslides.py
--rw-rw-rw-   0        0        0    34403 2023-11-14 20:41:35.000000 spswarehouse-0.6.1/spswarehouse/magic_spreadsheet.py
-drwxrwxrwx   0        0        0        0 2023-11-14 20:42:02.517577 spswarehouse-0.6.1/spswarehouse/powerschool/
--rw-rw-rw-   0        0        0        0 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/powerschool/__init__.py
--rw-rw-rw-   0        0        0    36009 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/powerschool/powerschool.py
--rw-rw-rw-   0        0        0    34757 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/powerschool/powerschool_calpads.py
--rw-rw-rw-   0        0        0     4008 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/powerschool/student_passwords.py
--rw-rw-rw-   0        0        0      342 2023-11-14 20:41:35.000000 spswarehouse-0.6.1/spswarehouse/requirements.txt
--rw-rw-rw-   0        0        0     1220 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/table_names.py
--rw-rw-rw-   0        0        0     8056 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/table_utils.py
--rw-rw-rw-   0        0        0     4689 2023-11-13 20:32:38.000000 spswarehouse-0.6.1/spswarehouse/warehouse.py
-drwxrwxrwx   0        0        0        0 2023-11-14 20:42:02.419658 spswarehouse-0.6.1/spswarehouse.egg-info/
--rw-rw-rw-   0        0        0     8200 2023-11-14 20:42:01.000000 spswarehouse-0.6.1/spswarehouse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2023-11-14 20:42:02.000000 spswarehouse-0.6.1/spswarehouse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-14 20:42:01.000000 spswarehouse-0.6.1/spswarehouse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-14 20:42:01.000000 spswarehouse-0.6.1/spswarehouse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.439124 spswarehouse-0.6.2/
+-rw-rw-rw-   0        0        0    35823 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     8200 2024-04-03 17:48:11.436160 spswarehouse-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7815 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 17:48:11.440298 spswarehouse-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      744 2024-04-03 17:19:19.000000 spswarehouse-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.059018 spswarehouse-0.6.2/spswarehouse/
+-rw-rw-rw-   0        0        0      582 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.234994 spswarehouse-0.6.2/spswarehouse/calpads/
+-rw-rw-rw-   0        0        0        0 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/calpads/__init__.py
+-rw-rw-rw-   0        0        0    40824 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/calpads/calpads.py
+-rw-rw-rw-   0        0        0     6136 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/calpads/calpads_config.py
+-rw-rw-rw-   0        0        0     1187 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/credentials.py.template
+drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.302831 spswarehouse-0.6.2/spswarehouse/general/
+-rw-rw-rw-   0        0        0        0 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/general/__init__.py
+-rw-rw-rw-   0        0        0      730 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/general/os.py
+-rw-rw-rw-   0        0        0    14021 2024-04-03 17:13:50.000000 spswarehouse-0.6.2/spswarehouse/general/selenium.py
+-rw-rw-rw-   0        0        0     2347 2024-04-03 17:47:17.000000 spswarehouse-0.6.2/spswarehouse/googledrive.py
+-rw-rw-rw-   0        0        0     2044 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/googlesheets.py
+-rw-rw-rw-   0        0        0     2078 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/googleslides.py
+-rw-rw-rw-   0        0        0    35075 2024-04-03 17:14:06.000000 spswarehouse-0.6.2/spswarehouse/magic_spreadsheet.py
+drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.424368 spswarehouse-0.6.2/spswarehouse/powerschool/
+-rw-rw-rw-   0        0        0        0 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/powerschool/__init__.py
+-rw-rw-rw-   0        0        0    36921 2024-04-03 17:16:40.000000 spswarehouse-0.6.2/spswarehouse/powerschool/powerschool.py
+-rw-rw-rw-   0        0        0    35449 2024-04-03 17:14:06.000000 spswarehouse-0.6.2/spswarehouse/powerschool/powerschool_calpads.py
+-rw-rw-rw-   0        0        0     4122 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/powerschool/student_passwords.py
+-rw-rw-rw-   0        0        0      357 2024-04-03 17:14:06.000000 spswarehouse-0.6.2/spswarehouse/requirements.txt
+-rw-rw-rw-   0        0        0     1269 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/table_names.py
+-rw-rw-rw-   0        0        0     8313 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/table_utils.py
+-rw-rw-rw-   0        0        0     4812 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/warehouse.py
+drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.153958 spswarehouse-0.6.2/spswarehouse.egg-info/
+-rw-rw-rw-   0        0        0     8200 2024-04-03 17:48:09.000000 spswarehouse-0.6.2/spswarehouse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-04-03 17:48:10.000000 spswarehouse-0.6.2/spswarehouse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 17:48:09.000000 spswarehouse-0.6.2/spswarehouse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-03 17:48:09.000000 spswarehouse-0.6.2/spswarehouse.egg-info/top_level.txt
```

### Comparing `spswarehouse-0.6.1/LICENSE` & `spswarehouse-0.6.2/LICENSE`

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

### Comparing `spswarehouse-0.6.1/PKG-INFO` & `spswarehouse-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.6.1
+Version: 0.6.2
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.6.1/README.md` & `spswarehouse-0.6.2/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-# spswarehouse
-
-# Prerequisites
-
-- Anaconda & Python 3
-- Jupyter Notebook
-
-# Installation
-
-- To install, run: `pip install spswarehouse`
-    - This can be done from `Anaconda Prompt` from the Start Menu.
-- Locate the install directory by running: `pip show pip | grep "Location:" | cut -d " " -f2`
-    - If this doesn't work, run `pip show pip`, then look at the line "Location:".
-    - Take note of the install directory for the "Set up credentials" step.
-
-The files referred to in this `README` are in `<install-directory>/spswarehouse/`.
-
-## Set up dependencies
-
-- Change to the `spswarehouse` directory
-    - `cd <install-directory>\spswarehouse`
-    - The default for Anaconda3 is `cd Anaconda3\Lib\site-packages\spswarehouse`
-- Run: `pip install -r requirements.txt`
-
-You can `exit` the Anaconda Prompt; the next step is more easily done in the File Explorer.
-
-## Updating to new version
-
-When a new version of spswarehouse is released, there are two steps:
-
-- `pip install --upgrade spswarehouse`
-- Redo the "Set up dependencies" section.
-
-## Set up credentials
-
-- Navigate to the install directory.
-    - The default directory where this module is installed is `Users\<your name>\Anaconda3\Lib\site-packages\spswarehouse`.
-    - If you are using a custom environment, the directory will probably be `Users\<your name>\Anaconda3\envs\<env name>\Lib\site-packages\spswarehouse`.
-
-- Copy the `credentials.py.template` file to `credentials.py`.
-- Fill in `credentials.py` with the warehouse information and the Google Service Account information provided by your technical admin.
-
-### Snowflake
-
-This allows you to access the Snowflake data warehouse.
-
-- Fill in your Snowflake `user` and `password`  credentials between quotation marks.
-
-### Google
-
-This allows you to access your Google Apps.
-
-- Fill in all the blank fields in `google_config.service_account`. See Developer Notes below if you need to generate credentials.
-
-# Usage
-
-## Snowflake
-
-Your Snowflake connection is configured in `credentials.py` (see above).
-
-Snowflake access is implemented in by `Warehouse`. You can:
-- Read data using `read_sql()`
-- Reflect a table using `reflect_table()`
-- Run a SQL command using `execute()`
-
-### Table & column name tab-completion
-
-When you run `import spswarehouse`, some tab-completion for table and column names is automatically set up.
-
-The format is:
-
-```
-spswarehouse.<schema_name>.<table name>.c_<column name>
-```
-
-To reduce load time, tab-completion is automatically set up for only a few schemas when `spswarehouse`is imported.
-
-If the schema you're using isn't tab-completing you can manually import it.
-
-For example, to enable tab-competion for the schema `schoolmint`, run:
-
-```
-from spswarehouse.table_names import *
-
-initialize_schema_object(SchoolMint)
-schoolmint = SchoolMint()
-```
-
-### Uploading data
-
-The `table_utils` module implements uploading data to the Snowflake warehouse.
-
-The data sources you can upload from are:
-
-- pandas.DataFrame `dataframe`
-- CSV file `csv_filename`
-- Google Sheet `google_sheet`
-- Google Drive files `google_drive_id`
-
-The two major methods are `create_table_stmt` and `upload_to_warehouse`. Both support the above data sources as optional arguments:
-
- - `dataframe`
- - `csv_filename`
- - `google_sheet`
- - `google_drive_id`
-
-From Jupyter Notebook, open `snowflake-upload-example.ipynb` for a basic example.
-
-### Column types
-
-`create_table_stmt()` will try to guess column types when given a DataFrame, CSV file, or Google Sheet.  
-
-If you want to explicitly name and type your columns, you can pass in the `columns` argument instead.
-
-Alternatively, if you want to force all columns to be strings, pass `force_string=True`. This works for both `create_table_stmt()` and `upload_to_warehouse()`. This does not work if you pass a dataframe.
-
-See the documentation for `guess_col_types()` for best practices for types.
-
-## Google Functions
-### GoogleDrive, GoogleSheets, GoogleSlides
-
-Make sure you've set up `credentials.py` first and shared your spreadsheet with the Google service account email. You can also get the email by running any of the following:
-
-```
-GoogleSheets.get_google_service_account_email()
-GoogleDrive.get_google_service_account_email()
-GoogleSlides..get_google_service_account_email()
-```
-
-`GoogleSheets` is really an instance of `gspread.Client`, so you can use the entire
-[`gspread`](https://gspread.readthedocs.io/en/latest/) Python API.
-
-`GoogleDrive` is an instance of `pydrive2.GoogleDrive`, so you can use the [`PyDrive2`](https://iterative.github.io/PyDrive2/docs/build/html/index.html) Python API.
-
-`GoogleSlides` builds directly on the Google Slides API (https://developers.google.com/resources/api-libraries/documentation/slides/v1/python/latest/)
-
-### Accessing data
-
-From Jupyter Notebook, open and run `googlesheets-example.ipynb` for a basic example on loading a spreadsheet and reading sheet data into `pandas.DataFrame`.
-
-`googledrive-example.ipynb` contains basic examples of exploring Drive via Jupyter. Note that this class only handles files uploaded to Drive; it's not useful for handling Google Sheets, Google Docs, etc.
-
-### Uploading to warehouse
-
-From Jupyter Notebook open and run `snowflake-upload-example.ipynb` for a basic example on uploading Google Sheet data to the Snowflake warehouse.
-
-### Column types
-
-# Developer notes
-
-## Google service account key
-
-This lets us use the Google Sheets API to access sheet data. It only has to be done once and added to `credentials.py.template`.
-
-- Use an existing Google Developer project, or create a new one: https://console.cloud.google.com
-- Enable the Google Sheets API
-  - Go to **API & Services** for the project, then **Libraries**.
-  - Search for "Google Sheets" and select the result.
-  - Click **Enable**.
-- Create the OAuth client credentials
-  - Go to **API & Services** for the project, then **Credentials**.
-  - Under **Create credentials**, select **Service account key**
-  - Choose an existing service account or create a new one to associate this key with.
-  - Create the key and download the key as a JSON file.
-- Copy OAuth client credentials to `credentials.py.template` in `google_client` under `service-account`.
-- **Delete the private_key** and leave just the quotation marks when you check in `credentials.template.py`.
-- You will need to distribute the private key securely so it can be added to `credentials.py`.
-
-## PyPI
-
-We use [PyPI](https://pypi.org/) to distribute the `spswarehouse` module and [Test PyPI](https://test.pypi.org/)  for testing.
-
-The `spswarehouse` project is [here](https://pypi.org/project/spswarehouse/).
-
-### Set up
-
-Create PyPI and Test PyPI accounts to test and upload packages.
-
-### Packaging
-
-See https://packaging.python.org/tutorials/packaging-projects/ for an overview and walk-through of PyPI packaging.
-
-Specifics for `spswarehouse`:
-
-- Only build the `sdist` package. Otherwise, `credentials.py` and potentially passwords will get distributed in the binary distribution.
-- If you need to include non-Python files, add them to `MANIFEST.in`.
-
-### Testing
-
-- Update version number in `setup.py`.
-- Create the package:
-`python setup.py sdist`
-- Upload to Test PyPI:
-`python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
-- Install on local machine to test: `pip install spswarehouse==<insert version number> -i https://test.pypi.org/simple/`
-
-### Pushing a new package
-
-Make sure all of your changes are checked into the GitHub repository and your local repository is up-to-date before you do this.
-
-The steps are the same as in the above section, omitting the `test.pypi` URLs.
+# spswarehouse
+
+# Prerequisites
+
+- Anaconda & Python 3
+- Jupyter Notebook
+
+# Installation
+
+- To install, run: `pip install spswarehouse`
+    - This can be done from `Anaconda Prompt` from the Start Menu.
+- Locate the install directory by running: `pip show pip | grep "Location:" | cut -d " " -f2`
+    - If this doesn't work, run `pip show pip`, then look at the line "Location:".
+    - Take note of the install directory for the "Set up credentials" step.
+
+The files referred to in this `README` are in `<install-directory>/spswarehouse/`.
+
+## Set up dependencies
+
+- Change to the `spswarehouse` directory
+    - `cd <install-directory>\spswarehouse`
+    - The default for Anaconda3 is `cd Anaconda3\Lib\site-packages\spswarehouse`
+- Run: `pip install -r requirements.txt`
+
+You can `exit` the Anaconda Prompt; the next step is more easily done in the File Explorer.
+
+## Updating to new version
+
+When a new version of spswarehouse is released, there are two steps:
+
+- `pip install --upgrade spswarehouse`
+- Redo the "Set up dependencies" section.
+
+## Set up credentials
+
+- Navigate to the install directory.
+    - The default directory where this module is installed is `Users\<your name>\Anaconda3\Lib\site-packages\spswarehouse`.
+    - If you are using a custom environment, the directory will probably be `Users\<your name>\Anaconda3\envs\<env name>\Lib\site-packages\spswarehouse`.
+
+- Copy the `credentials.py.template` file to `credentials.py`.
+- Fill in `credentials.py` with the warehouse information and the Google Service Account information provided by your technical admin.
+
+### Snowflake
+
+This allows you to access the Snowflake data warehouse.
+
+- Fill in your Snowflake `user` and `password`  credentials between quotation marks.
+
+### Google
+
+This allows you to access your Google Apps.
+
+- Fill in all the blank fields in `google_config.service_account`. See Developer Notes below if you need to generate credentials.
+
+# Usage
+
+## Snowflake
+
+Your Snowflake connection is configured in `credentials.py` (see above).
+
+Snowflake access is implemented in by `Warehouse`. You can:
+- Read data using `read_sql()`
+- Reflect a table using `reflect_table()`
+- Run a SQL command using `execute()`
+
+### Table & column name tab-completion
+
+When you run `import spswarehouse`, some tab-completion for table and column names is automatically set up.
+
+The format is:
+
+```
+spswarehouse.<schema_name>.<table name>.c_<column name>
+```
+
+To reduce load time, tab-completion is automatically set up for only a few schemas when `spswarehouse`is imported.
+
+If the schema you're using isn't tab-completing you can manually import it.
+
+For example, to enable tab-competion for the schema `schoolmint`, run:
+
+```
+from spswarehouse.table_names import *
+
+initialize_schema_object(SchoolMint)
+schoolmint = SchoolMint()
+```
+
+### Uploading data
+
+The `table_utils` module implements uploading data to the Snowflake warehouse.
+
+The data sources you can upload from are:
+
+- pandas.DataFrame `dataframe`
+- CSV file `csv_filename`
+- Google Sheet `google_sheet`
+- Google Drive files `google_drive_id`
+
+The two major methods are `create_table_stmt` and `upload_to_warehouse`. Both support the above data sources as optional arguments:
+
+ - `dataframe`
+ - `csv_filename`
+ - `google_sheet`
+ - `google_drive_id`
+
+From Jupyter Notebook, open `snowflake-upload-example.ipynb` for a basic example.
+
+### Column types
+
+`create_table_stmt()` will try to guess column types when given a DataFrame, CSV file, or Google Sheet.  
+
+If you want to explicitly name and type your columns, you can pass in the `columns` argument instead.
+
+Alternatively, if you want to force all columns to be strings, pass `force_string=True`. This works for both `create_table_stmt()` and `upload_to_warehouse()`. This does not work if you pass a dataframe.
+
+See the documentation for `guess_col_types()` for best practices for types.
+
+## Google Functions
+### GoogleDrive, GoogleSheets, GoogleSlides
+
+Make sure you've set up `credentials.py` first and shared your spreadsheet with the Google service account email. You can also get the email by running any of the following:
+
+```
+GoogleSheets.get_google_service_account_email()
+GoogleDrive.get_google_service_account_email()
+GoogleSlides..get_google_service_account_email()
+```
+
+`GoogleSheets` is really an instance of `gspread.Client`, so you can use the entire
+[`gspread`](https://gspread.readthedocs.io/en/latest/) Python API.
+
+`GoogleDrive` is an instance of `pydrive2.GoogleDrive`, so you can use the [`PyDrive2`](https://iterative.github.io/PyDrive2/docs/build/html/index.html) Python API.
+
+`GoogleSlides` builds directly on the Google Slides API (https://developers.google.com/resources/api-libraries/documentation/slides/v1/python/latest/)
+
+### Accessing data
+
+From Jupyter Notebook, open and run `googlesheets-example.ipynb` for a basic example on loading a spreadsheet and reading sheet data into `pandas.DataFrame`.
+
+`googledrive-example.ipynb` contains basic examples of exploring Drive via Jupyter. Note that this class only handles files uploaded to Drive; it's not useful for handling Google Sheets, Google Docs, etc.
+
+### Uploading to warehouse
+
+From Jupyter Notebook open and run `snowflake-upload-example.ipynb` for a basic example on uploading Google Sheet data to the Snowflake warehouse.
+
+### Column types
+
+# Developer notes
+
+## Google service account key
+
+This lets us use the Google Sheets API to access sheet data. It only has to be done once and added to `credentials.py.template`.
+
+- Use an existing Google Developer project, or create a new one: https://console.cloud.google.com
+- Enable the Google Sheets API
+  - Go to **API & Services** for the project, then **Libraries**.
+  - Search for "Google Sheets" and select the result.
+  - Click **Enable**.
+- Create the OAuth client credentials
+  - Go to **API & Services** for the project, then **Credentials**.
+  - Under **Create credentials**, select **Service account key**
+  - Choose an existing service account or create a new one to associate this key with.
+  - Create the key and download the key as a JSON file.
+- Copy OAuth client credentials to `credentials.py.template` in `google_client` under `service-account`.
+- **Delete the private_key** and leave just the quotation marks when you check in `credentials.template.py`.
+- You will need to distribute the private key securely so it can be added to `credentials.py`.
+
+## PyPI
+
+We use [PyPI](https://pypi.org/) to distribute the `spswarehouse` module and [Test PyPI](https://test.pypi.org/)  for testing.
+
+The `spswarehouse` project is [here](https://pypi.org/project/spswarehouse/).
+
+### Set up
+
+Create PyPI and Test PyPI accounts to test and upload packages.
+
+### Packaging
+
+See https://packaging.python.org/tutorials/packaging-projects/ for an overview and walk-through of PyPI packaging.
+
+Specifics for `spswarehouse`:
+
+- Only build the `sdist` package. Otherwise, `credentials.py` and potentially passwords will get distributed in the binary distribution.
+- If you need to include non-Python files, add them to `MANIFEST.in`.
+
+### Testing
+
+- Update version number in `setup.py`.
+- Create the package:
+`python setup.py sdist`
+- Upload to Test PyPI:
+`python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
+- Install on local machine to test: `pip install spswarehouse==<insert version number> -i https://test.pypi.org/simple/`
+
+### Pushing a new package
+
+Make sure all of your changes are checked into the GitHub repository and your local repository is up-to-date before you do this.
+
+The steps are the same as in the above section, omitting the `test.pypi` URLs.
```

### Comparing `spswarehouse-0.6.1/spswarehouse/__init__.py` & `spswarehouse-0.6.2/spswarehouse/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pandas as pd
-import numpy as np
-# import seaborn as sns
-
-from sqlalchemy import *
-from sqlalchemy.sql import label, select, literal_column
-from sqlalchemy.sql.expression import cast
-
-import datetime
-
-now = datetime.datetime.now
-timedelta = datetime.timedelta
-
-# from .googlesheets import GoogleSheets, get_google_service_account_email
-# from .warehouse import describe, Warehouse
-# from .table_names import public, wild_west
-
-# from matplotlib import pyplot
-
-# To avoid missing font warnings, set a default font that exists
-# sns.set(font="DejaVu Sans")
+import pandas as pd
+import numpy as np
+# import seaborn as sns
+
+from sqlalchemy import *
+from sqlalchemy.sql import label, select, literal_column
+from sqlalchemy.sql.expression import cast
+
+import datetime
+
+now = datetime.datetime.now
+timedelta = datetime.timedelta
+
+# from .googlesheets import GoogleSheets, get_google_service_account_email
+# from .warehouse import describe, Warehouse
+# from .table_names import public, wild_west
+
+# from matplotlib import pyplot
+
+# To avoid missing font warnings, set a default font that exists
+# sns.set(font="DejaVu Sans")
```

### Comparing `spswarehouse-0.6.1/spswarehouse/calpads/calpads.py` & `spswarehouse-0.6.2/spswarehouse/calpads/calpads.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,898 +1,898 @@
-# Code adapted from original code by Yusuph in the dops-calpad repo
-
-# Author: Howard Shen
-# Last Edited 5/25/2023
-
-import logging
-import os
-import pandas as pd
-import tempfile
-import time
-
-from datetime import date, datetime
-
-from selenium.webdriver.support.ui import Select, WebDriverWait
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.common.keys import Keys
-from selenium.common.exceptions import (
-    TimeoutException,
-    NoSuchElementException,
-    ElementNotInteractableException
-)
-
-from ducttape.utils import (
-    DriverBuilder,
-    get_most_recent_file_in_dir,
-    wait_for_any_file_in_folder
-)
-    
-try:
-    from spswarehouse.credentials import calpads_config
-except ModuleNotFoundError:
-    print("No credentials file found in spswarehouse. This could cause issues.")
-
-from spswarehouse.calpads.calpads_config import (
-    monitoring_report_base,
-    monitoring_links,
-    snapshot_report_base,
-    snapshot_links,
-)
-    
-class CALPADS():
-    
-    def __init__(
-        self,
-        config=None,
-        username=None,
-        password=None,
-        host=None,
-        download_location=None,
-        headless=True,
-    ):
-        """
-        By default, the class will pull the username and password from the
-        credentials file in the module. You can override the credentials file
-        by passing either a config dictionary or both a username and password.
-        
-        Parameters:
-        config: A dictionary containing a username and password key. Optional.
-            Supercedes the username and password in credentials.py in this module.
-            Also supercedes a username and password combo passed to this function in
-            addition to the config.  May also contain a host key that will supercede
-            both the host parameter and the host from credentials.py
-        username: A CALPADS username, which should be in the form of an email address.
-            Must be paired with a password. Supercedes credentials.py.
-        password: Password for the given CALPADS username. Must be paired with a username
-            Supercedes credentials.py
-        host: The URL for CALPADS, in the format `https://www.calpads.org`. Optional.
-            Supercedes the host from credentials.py
-        download_location: The local folder that you want to save files too. If no
-            folder path passed, creates a temporary directory for this object.
-        headless: Selenium headless value. Default to True. If using this in a notebook,
-            recommend setting to False.
-        """
-        
-        self.host = None
-        if config is not None:
-            username = config['username']
-            password = config['password']
-            if 'host' in config:
-                self.host = config['host']
-        elif username is not None and password is not None:
-            username = username
-            password = password
-        else:
-            username = calpads_config['username']
-            password = calpads_config['password']
-        
-        if self.host is None and host is not None:
-            self.host = host
-        elif self.host is None:
-            self.host = calpads_config['host']
-        else:
-            pass
-        
-        if download_location is None:
-            self.download_location = tempfile.mkdtemp()
-        else:
-            self.download_location = download_location
-    
-        self.driver = DriverBuilder().get_driver(
-            download_location=self.download_location,
-            headless=headless
-        )
-        self._login_to_calpads(username, password)
-
-    def quit(self):
-        self.driver.quit()
-
-    def upload_file(self, lea, submission_type, file_path):
-        """
-        To be used in conjunction with the create_extract method, uploads the extract via File Submission on CALPADS.
-
-        Parameters:
-        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
-            dropdown on the CALPADS page.
-        submission_type: The four letter code, in all caps, for the file type you're 
-            uploading
-        file_path: The file path to the file you want to upload. Absolute path is
-            recommended (`os.path.abspath()`). Relative path behavior untested
-
-        Returns:
-        bool: True for a successful upload, else False
-        """
-        
-        self._select_lea(lea)
-        self.driver.get(f'{self.host}/FileSubmission/FileUpload')
-#         self.driver.refresh()
-        
-        try:
-            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((
-                By.XPATH,
-                '//*[@id="btnSearch"]'
-            )))
-        except TimeoutException:
-            logging.info('Unable to successfully reach the File Submission web page for {}. Closing the driver.'.format(lea))
-            return False
-
-        #Choose file type for the upload
-        select = Select(self.driver.find_element(By.XPATH, '//*[@id="tbFileUpload"]/tbody/tr/td[2]/select'))
-        select.select_by_value(submission_type)
-
-        #Find the file to upload by pulling the most recent file in the specific illuminate extract folder
-        choose_file = self.driver.find_element(By.XPATH, '//*[@id="tbFileUpload"]/tbody/tr/td[4]/input')
-        choose_file.send_keys(os.path.abspath(file_path))
-
-        #Upload
-        button = self.driver.find_element(By.XPATH, '//*[@id="btnSearch"]')
-        button.click()
-
-        try:
-            success = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located(
-            (By.CSS_SELECTOR, 'div.alert.alert-success.alert-dismissible.fade.in'))) #TODO: Confirm this reliably works. Otherwise, use text.
-        except TimeoutException:
-            logging.info('Something went wrong with the file upload for {}. Review files in directories and try again.'.format(lea)) #TODO: CALPADS provides error alerts in red on same page, should send to user
-            #TODO: Provide more information on error if possible?
-            return False
-        else:
-            logging.info('{} extract successfully uploaded for {}. Check the file submission status later.'.format(type(self).__name__, lea))
-            return True
-        
-    def get_upload_results(self, lea, submission_type, max_wait=5):
-        """
-        Retrieves the validation errors for the most recent upload of the given
-        submission type for the given LEA. Must be used within seven days of the upload
-        (default range on CALPADS).
-
-        Parameters:
-        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
-            dropdown on the CALPADS page.
-        submission_type: The four letter code, in all caps, for the file type you're 
-            uploading
-        max_wait: The maximum number of minutes to wait if the submission is still processing.
-            Default is 5 minutes. Must be at least 1.
-
-        Returns:
-        submitted_date_string (string): ISO formate date of the submission whose errors were checked. Returns None if the file submission can't be found for whatever reason
-        job_results_df (DataFrame): Returns a dataframe of the job results or False if the job is not yet in a final status.
-        error_details (DataFrame): Returns a dataframe of error details, False if unable to find error details, True if file posted.
-        """
-
-        if(max_wait < 1):
-            raise Exception('max_wait parameter must be 1 or more.')
-
-        self._select_lea(lea)
-        self.driver.get(f'{self.host}/FileSubmission/')
-        try:
-            file_elem = WebDriverWait(self.driver, 15).until(
-                EC.presence_of_element_located((By.ID, 'FileType'))
-            )
-        except TimeoutException:
-            logging.info("Can't load View Submission page")
-            return None, False
-
-        # Filter the file list
-        file_select = Select(file_elem)
-        file_select.select_by_value(submission_type)
-        apply_button = self.driver.find_element(By.ID, "fileSubSearch")
-        apply_button.click()
-        try:
-            # The filtered page is identical, so sleep for a moment
-            time.sleep(2)
-            WebDriverWait(self.driver, 20).until(EC.text_to_be_present_in_element(
-                (By.XPATH, '//*[@id="FileSubmissionSearchResults"]/table/tbody/tr[1]/td[6]'),
-                submission_type
-            ))
-        except TimeoutException:
-            logging.info(f"No recent submissions of type {submission_type}")
-            return None, False
-
-        # Process submission date
-        date_text = self.driver.find_element(
-            By.XPATH,
-            '//*[@id="FileSubmissionSearchResults"]/table/tbody/tr[1]/td[3]'
-        ).text
-
-        submitted_datetime = datetime.strptime(date_text, "%m/%d/%Y %I:%M:%S %p")
-        submitted_date_string = submitted_datetime.date().isoformat()
-
-        for i in range(max_wait):
-            file_status = self.driver.find_element(
-                By.XPATH,
-                '//*[@id="FileSubmissionSearchResults"]/table/tbody/tr[1]/td[8]'
-            ).text
-            if file_status in ['Posted', 'Failed', 'Rejected']:
-                logging.info('Found final job results. Storing them.')
-                job_results_df = pd.read_html(self.driver.page_source)[0].head(1)
-                break
-            else:
-                if((i+1)< max_wait):
-                    logging.info(f'Try #{i+1}: Did not find finished job. Will try again in 60 seconds.')
-                    time.sleep(60)
-                    self.driver.refresh()
-                    time.sleep(3)
-                else:
-                    logging.info(f'Try #{i+1}: Did not find finished job.')
-
-        # Branch based on file status
-        if file_status == 'Posted':
-            logging.info(f"{submission_type} Posted on {submitted_date_string}")
-            return submitted_date_string, job_results_df, True
-        elif file_status == 'Failed':
-            logging.info(f"{submission_type} Failed on {submitted_date_string}. Check manually")
-            return submitted_date_string, job_results_df, False
-        elif file_status == 'Rejected':
-            view_errors = self.driver.find_element(
-                By.XPATH,
-                '//*[@id="FileSubmissionSearchResults"]/table/tbody/tr[1]/td[1]/a'
-            )
-            view_errors.click()
-        else:
-            logging.info(f"{submitted_date_string} {submission_type} not complete after {max_wait} minute{'s' if max_wait > 1 else ''}.")
-            return submitted_date_string, False, False
-
-        try:
-            WebDriverWait(self.driver, 30).until(EC.text_to_be_present_in_element((
-                By.XPATH,
-                '//*[@id="main"]/div/div[2]/header/h1'), 'View Submission Details'
-            ))
-            time.sleep(10) # The file errors takes a moment to load; extended from 2 to 10 seconds after some rejected files didn't have errors captured
-        except TimeoutException as t:
-            logging.info('Something went wrong with loading the submission error details page.')
-            return submitted_date_string, job_results_df, False
-
-         #We expect the error details to be the second table in the HTML source
-        error_details_df = pd.read_html(self.driver.page_source)[1]
-
-        # Get errors if there are multiple pages
-        error_has_next = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH, '//*[@id="FileErrors"]/div/a[3]')))
-
-        all_error_details = []
-        all_error_details.append(error_details_df)
-
-        while 'disabled' not in error_has_next.get_attribute('class'):
-            logging.info('Next Page')
-            error_has_next.click()
-            # Give time for next page to load
-            time.sleep(10)
-            next_details_df = pd.read_html(self.driver.page_source)[1] #TODO: Confirm that this is a completely new df
-            all_error_details.append(next_details_df)
-            error_has_next = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH, '//*[@id="FileErrors"]/div/a[3]')))
-
-        all_error_details = pd.concat(all_error_details)
-        logging.info("Successfully collected all errors from file submission error details for the {} {} extract.".format(submitted_date_string, submission_type))
-        return submitted_date_string, job_results_df, all_error_details
-    
-    def get_certification_status(self, lea, academic_year, submission_name, **kwargs):
-        """
-        Retrieves the status of a Certification window.
-
-        Parameters:
-        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
-            dropdown on the CALPADS page.
-        academic_year: Integer representing the academic year that you want to check
-            (per team norms, this is the year when the school year ends)
-        submission_name: The name of the certification window. As of this edit, the
-            certification windows are Fall1, Fall2, EOY1, EOY2, EOY3, and EOY4.
-        optional arguments (kwargs):
-            rollover_date: Applies only to EOY3. An ISO format string (YYYY-MM-DD)
-                representing the expected rollover date of your SIS. The SIS rollover
-                is when exit dates and exit codes get put on enrollment records.
-                Prior to this, CALPADS will return CERT131 errors for every actively
-                enrolled student. This function will begin scraping CERT131 the day
-                after the rollover date. If you do not pass a rollover date, CERT131
-                will be scraped.
-
-        Returns:
-        cert_status (Boolean): Returns False if the certification window isn't open yet;
-            returns True if it is.
-        error_details (DataFrame): Returns a dataframe of error details, None if no errors,
-            None if certification window isn't open.
-        warning_details (DataFrame): Returns a dataframe of warningsdetails, None if no
-            warnings, None if certification window isn't open.
-        """
-        
-        # Fall1, EOY3, EOY4 have a SELPA approval, which
-        # creates an extra table on the Cert status page, altering the XPATH
-        if submission_name in ['Fall1', 'EOY3', 'EOY4']:
-            data_div_num = 5
-            data_table_num = 3
-            error_table_num = 1
-            warning_table_num = 2
-        else:
-            data_div_num = 4
-            data_table_num = 2
-            error_table_num = 0
-            warning_table_num = 1
-        
-        # CERT131 is somewhat meaningless prior to the end of the year
-        if submission_name == 'EOY3':
-            try:
-                rollover_date = date.fromisoformat(kwargs['rollover_date'])
-                cert131_flag = date.today() > rollover_date
-                logging.info(f"Today is {date.today()}, Rollover date is {rollover_date}, CERT131 = {cert131_flag}")
-            except KeyError:
-                # KeyError means rollover_date was not passed as an argument
-                logging.info("No rollover date passed; scraping CERT131")
-                cert131_flag = True
-        else:
-            cert131_flag = True
-        
-        self._select_lea(lea)
-        
-        academic_year_string = f"{academic_year-1}-{academic_year}"
-        self.driver.get(f"https://www.calpads.org/StateReporting/Certification?AcademicYear={academic_year_string}&Snapshot={submission_name}")
-        
-        try:
-            WebDriverWait(self.driver, 20).until(EC.presence_of_element_located((
-                By.XPATH,
-                '/html/body/div[1]/main/div/div[2]/div[3]/div/div/div/div/table/tbody/tr/td[1]'
-            )))
-        except TimeoutException:
-            logging.info(f"{submission_name} certification errors not available yet")
-            return False, None, None
-        
-        error_and_warn_text = self.driver.find_element(
-            By.XPATH,
-            "/html/body/div[1]/main/div/div[2]/div[3]/div/div/div/div/table/tbody/tr/td[9]"
-        ).text
-        error_and_warn_count = int(error_and_warn_text)
-
-        if error_and_warn_count > 0:
-            cert_status_link = self.driver.find_element(
-                By.XPATH,
-                '/html/body/div[1]/main/div/div[2]/div[3]/div/div/div/div/table/tbody/tr/td[1]/a'
-            )
-            cert_status_link.click()
-            try:
-                WebDriverWait(self.driver, 20).until(EC.text_to_be_present_in_element(
-                    (
-                        By.XPATH,
-                        '/html/body/div/main/div/div[2]/header/h1'
-                    ),
-                    'Certification Details - LEA'
-                ))
-            except TimeoutException:
-                logging.info("Failed to load Certification Status page")
-                raise RuntimeError("Failed to load Certification Status page")
-            try:
-                WebDriverWait(self.driver, 15).until(EC.presence_of_element_located((
-                    By.XPATH,
-                    f'/html/body/div/main/div/div[2]/div[{data_div_num}]/div[1]/div[1]/div/ul/li/div/div/div/table/tbody/tr/td[4]/a'
-                )))
-                # Error list should be the second table
-                errors_table = pd.read_html(self.driver.page_source)[error_table_num]
-                error_df = pd.DataFrame()
-                
-                error_list_has_next = self.driver.find_element(
-                    By.XPATH,
-                    '//*[@id="RequiredGrid_FATAL"]/div/a[3]'
-                )
-                while 'disabled' not in error_list_has_next.get_attribute('class'):
-                    logging.info("Getting next page of errors list")
-                    try:
-                        error_list_has_next.click()
-                    except ElementNotInteractableException:
-                        banner = self.driver.find_element(
-                            By.XPATH,
-                            '//*[@id="CertificationErrorSummary"]/li/a'
-                        )
-                        banner.click()
-                        error_list_has_next.click()
-                    time.sleep(2)
-                    errors_table = pd.concat(
-                        [errors_table, pd.read_html(self.driver.page_source)[error_table_num]],
-                        axis=0,
-                        ignore_index=True
-                    )
-                    error_list_has_next = self.driver.find_element(
-                        By.XPATH,
-                        '//*[@id="RequiredGrid_FATAL"]/div/a[3]'
-                    )
-                
-                for i in range(len(errors_table)):
-                    error_id = errors_table["Message ID"][i]
-
-                    if error_id == 'CERT131' and not cert131_flag:
-                        logging.info("Skipping CERT131")
-                        continue
-                        
-                    logging.info(f"Getting list for {error_id}")
-                    error_dropdown = self.driver.find_element(
-                        By.ID,
-                        'CertificationEditQuery_ChildErrorCategory'
-                    )
-                    error_select = Select(error_dropdown)
-                    error_select.select_by_value(error_id)
-                    apply_button = self.driver.find_element(
-                        By.XPATH,
-                        '//*[@id="certDetails"]/div[1]/div[3]/div/div/form/div[3]/button'
-                    )
-                    apply_button.click()
-                    
-                    try:
-                        WebDriverWait(self.driver, 30).until(EC.text_to_be_present_in_element(
-                            (
-                                By.XPATH,
-                                f'/html/body/div/main/div/div[2]/div[{data_div_num}]/div[1]/div[4]/div/div/table/tbody/tr/td[10]/a'
-                            ),
-                            error_id
-                        ))
-                    except TimeoutException:
-                        logging.info(f"Can't load errors for {error_id}")
-                        raise RuntimeError(f"Can't load errors for {error_id}")
-                    
-                    error_has_next = self.driver.find_element(
-                        By.XPATH,
-                        '//*[@id="RequiredGrid"]/div/a[3]'
-                    )
-                    
-                    error_df = pd.concat(
-                        [error_df, pd.read_html(self.driver.page_source)[data_table_num]],
-                        axis=0,
-                        ignore_index=True,
-                    )
-                    
-                    while 'disabled' not in error_has_next.get_attribute('class'):
-                        logging.info("Getting next page")
-                        error_has_next.click()
-                        time.sleep(2)
-                        error_df = pd.concat(
-                            [error_df, pd.read_html(self.driver.page_source)[data_table_num]],
-                            axis=0,
-                            ignore_index=True,
-                        )
-                        error_has_next = self.driver.find_element(
-                        By.XPATH,
-                        '//*[@id="RequiredGrid"]/div/a[3]'
-                        )
-                    
-                # Drop the "View" button column
-                if len(error_df) == 0:
-                    logging.info("Only Cert Error was CERT131, and rollover has not passed.")
-                    error_df = None
-                else:
-                    error_df.drop(columns="Error Record", inplace=True)
-                
-            except TimeoutException:
-                logging.info(f"No errors for {submission_name}")
-                error_df = None
-            
-            # Get Warnings
-            try:
-                WebDriverWait(self.driver, 5).until(EC.presence_of_element_located((
-                    By.XPATH,
-                    f'/html/body/div/main/div/div[2]/div[{data_div_num}]/div[1]/div[2]/div/ul/li/div/div/div/table/tbody/tr/td[4]/a'
-                )))
-                # Warning list should be the third table
-                warnings_table = pd.read_html(self.driver.page_source)[warning_table_num]
-                warning_df = pd.DataFrame()
-                
-                warning_list_has_next = self.driver.find_element(
-                    By.XPATH,
-                    '//*[@id="RequiredGrid_WARN"]/div/a[3]'
-                )
-                while 'disabled' not in warning_list_has_next.get_attribute('class'):
-                    logging.info("Getting next page of warnings list")
-                    try:
-                        warning_list_has_next.click()
-                    except ElementNotInteractableException:
-                        banner = self.driver.find_element(
-                            By.XPATH,
-                            '//*[@id="CertificationWarnSummary"]/li/a'
-                        )
-                        banner.click()
-                        warning_list_has_next.click()
-                    time.sleep(2)
-                    warnings_table = pd.concat(
-                        [warnings_table, pd.read_html(self.driver.page_source)[warning_table_num]],
-                        axis=0,
-                        ignore_index=True
-                    )
-                    warning_list_has_next = self.driver.find_element(
-                        By.XPATH,
-                        '//*[@id="RequiredGrid_WARN"]/div/a[3]'
-                    )
-                
-                for i in range(len(warnings_table)):
-                    warning_id = warnings_table["Message ID"][i]
-                        
-                    logging.info(f"Getting list for {warning_id}")
-                    warning_dropdown = self.driver.find_element(
-                        By.ID,
-                        'CertificationEditQuery_ChildErrorCategory'
-                    )
-                    warning_select = Select(warning_dropdown)
-                    warning_select.select_by_value(warning_id)
-                    apply_button = self.driver.find_element(
-                        By.XPATH,
-                        '//*[@id="certDetails"]/div[1]/div[3]/div/div/form/div[3]/button'
-                    )
-                    apply_button.click()
-                    
-                    try:
-                        WebDriverWait(self.driver, 15).until(EC.text_to_be_present_in_element(
-                            (
-                                By.XPATH,
-                               f'/html/body/div/main/div/div[2]/div[{data_div_num}]/div[1]/div[4]/div/div/table/tbody/tr/td[10]/a'
-                            ),
-                            warning_id
-                        ))
-                    except TimeoutException:
-                        logging.info(f"Can't load errors for {warning_id}")
-                        raise RuntimeError(f"Can't load errors for {warning_id}")
-                    
-                    warning_has_next = self.driver.find_element(
-                        By.XPATH,
-                        '//*[@id="RequiredGrid"]/div/a[3]'
-                    )
-                    
-                    warning_df = pd.concat(
-                        [warning_df, pd.read_html(self.driver.page_source)[data_table_num]],
-                        axis=0,
-                        ignore_index=True,
-                    )
-                    
-                    while 'disabled' not in warning_has_next.get_attribute('class'):
-                        logging.info("Getting next page")
-                        warning_has_next.click()
-                        time.sleep(2)
-                        warning_df = pd.concat(
-                            [warning_df, pd.read_html(self.driver.page_source)[data_table_num]],
-                            axis=0,
-                            ignore_index=True,
-                        )
-                        warning_has_next = self.driver.find_element(
-                            By.XPATH,
-                            '//*[@id="RequiredGrid"]/div/a[3]'
-                        )
-                    
-                # Drop the "View" button column
-                warning_df.drop(columns="Error Record", inplace=True)
-                
-            except TimeoutException:
-                logging.info(f"No warnings for {submission_name}")
-                warning_df = None
-                
-            return True, error_df, warning_df
-        elif error_and_warn_count == 0:
-            logging.info(f"No errors or warnings for {submission_name}")
-            return True, None, None
-        else:
-            raise RuntimeError("Impossible part of error_and_warn_count if-elif-else reached.")
-
-    def download_monitoring_report(
-        self,
-        lea,
-        academic_year,
-        report_code,
-        report_date=None,
-        download_type='csv',
-        max_wait_time=10
-    ):
-        """
-        Download a CALPADS snapshot report.
-        
-        Known issue: The download folder needs to be empty when this function is called.
-        
-        Parameters:
-        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
-            dropdown on the CALPADS page.
-        academic_year: Integer representing the academic year that you want to check
-            (per team norms, this is the year when the school year ends)
-        submission_name: The name of the certification window. As of this edit, the
-            certification windows are Fall1, Fall2, EOY1, EOY2, EOY3, and EOY4.
-        report_code: The code for the report that you want. Should be a string in
-            the form of "#.#". Check calpads_config.py for the list of available
-            report_code + submission_name combos
-        report_date (str): An ISO format date string ('YYYY-MM-DD') indicating the 
-            desired date for the report. If None, the function will download whatever
-            the default date on the report is (usually today).
-            Note that the function only uses the month and day. (E.g., if you pass
-            academic_year=2023 and report_date="2024-10-01", the report downloaded will be
-            for October 1 of academic year 2023, which is actually "2022-10-01")
-        download_type (str): The format in which you want the download for the report.
-            Currently supports csv, excel, and pdf.
-        max_wait_time: Integer >=0 indicating the maximum number of minutes to wait
-            for the report to generate and for the download to succeed. This means
-            this function can actually take up to 2*max_wait_time to run.
-        
-        Returns:
-        string: The filepath to the downloaded file
-        """
-        url_tail = monitoring_links[report_code]
-        report_url = self.host + monitoring_report_base + url_tail
-        
-        return self._download_report(
-            lea,
-            report_url,
-            academic_year,
-            download_type,
-            max_wait_time,
-            report_date=report_date
-        )
-            
-    def download_snapshot_report(
-        self,
-        lea,
-        academic_year,
-        submission_name,
-        report_code,
-        cert_status=None,
-        download_type='csv',
-        max_wait_time=10
-    ):
-        """
-        Download a CALPADS snapshot report.
-        
-        Known issue: The download folder needs to be empty when this function is called.
-        
-        Parameters:
-        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
-            dropdown on the CALPADS page.
-        academic_year: Integer representing the academic year that you want to check
-            (per team norms, this is the year when the school year ends)
-        submission_name: The name of the certification window. As of this edit, the
-            certification windows are Fall1, Fall2, EOY1, EOY2, EOY3, and EOY4.
-        report_code: The code for the report that you want. Should be a string in
-            the form of "#.#". Check calpads_config.py for the list of available
-            report_code + submission_name combos
-        cert_status: If there are multiple snapshots, which version you want. If
-            `None`, the top most option is selected (usually some variant of
-            "Certified" if the snapshot is certified). Will raise an error if the
-            given cert_status is not available.
-        download_type (str): The format in which you want the download for the report.
-            Currently supports csv, excel, and pdf.
-        max_wait_time: Integer >=0 indicating the maximum number of minutes to wait
-            for the report to generate and for the download to succeed. This means
-            this function can actually take up to 2*max_wait_time to run.
-        
-        Returns:
-        string: The filepath to the downloaded file
-        """
-        url_tail = snapshot_links[submission_name][report_code]
-        report_url = self.host + snapshot_report_base + url_tail
-        
-        return self._download_report(
-            lea,
-            report_url,
-            academic_year,
-            download_type,
-            max_wait_time,
-            cert_status=cert_status
-        )
-            
-    def _login_to_calpads(self, username, password):
-        self.driver.get(self.host)
-        try:
-            WebDriverWait(self.driver, 15).until(EC.presence_of_element_located((
-                By.XPATH,
-                '/html/body/div[3]/div/form/div/div[2]/fieldset/div[4]/div/button'
-            )))
-        except TimeoutException:
-            logging.info("Was unable to reach the login page. Check the browser: {}".format(self.driver.title))
-            return False
-        except NoSuchElementException:
-            logging.info("Was unable to reach the login page. Check the browser: {}".format(self.driver.title))
-            return False
-        user = self.driver.find_element(By.ID, "Username")
-        user.send_keys(username)
-        pw = self.driver.find_element(By.ID, "Password")
-        pw.send_keys(password)
-        agreement = self.driver.find_element(By.ID, "AgreementConfirmed")
-        self.driver.execute_script("arguments[0].click();", agreement)
-        btn = self.driver.find_element(
-            By.XPATH,
-            "/html/body/div[3]/div/form/div/div[2]/fieldset/div[4]/div/button"
-        )
-        btn.click()
-        try:
-            WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((
-                By.ID,
-                'org-select'
-            )))
-        except TimeoutException:
-            logging.info('Something went wrong with the login. Checking to see if there was an expected error message.')
-            try:
-                alert = WebDriverWait(self.driver, 15).until(EC.presence_of_element_located((
-                    By.XPATH,
-                    '/html/body/div[3]/div/form/div[1]'
-                )))
-                if 'alert' in alert.get_attribute('class'):
-                    logging.info("Found an expected alert during login: '{}'".format(
-                        self.driver.find_element(
-                            By.XPATH, '/html/body/div[3]/div/form/div[1]/div/ul/li'
-                        ).text
-                    ))
-                    return False
-                else:
-                    logging.info('There was an unexpected message during login. See driver.')
-                    return False
-            except TimeoutException:
-                logging.info('There was an unexpected error during login. See driver.')
-                return False
-
-        return True
-    
-    def _select_lea(self, lea):
-        """
-        Factored out common process for switching to a different LEA in the dropdown
-
-        Parameters:
-        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
-            dropdown on the CALPADS page.
-        """
-        select = Select(self.driver.find_element(By.ID, 'org-select'))
-        select.select_by_value(lea)
-        WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.ID, 'org-select')))
-
-    def _download_report(
-        self,
-        lea,
-        url,
-        academic_year,
-        download_type,
-        max_wait_time,
-        **kwargs
-    ):
-        """
-        Helper function for downloading from the reports iframe
-        Will crash if you pass "cert_status" in kwargs but the report is not a Snapshot
-            report
-        Will also crash if you pass a value othere than None for "report_date" in kwargs
-            but the report is not an Accountability/Monitoring report
-        """
-        
-        self._select_lea(lea)
-        self.driver.get(url)
-        try:
-            # The Reports module is in an iframe
-            iframe = WebDriverWait(self.driver, 30).until(
-                EC.presence_of_element_located((
-                    By.XPATH,
-                    '//*[@id="reports"]/div/div/div/iframe'
-                ))
-            )
-        except TimeoutException:
-            logging.info("Failed to load report page.")
-            raise
-        
-        self.driver.switch_to.frame(iframe)
-        self._select_report_academic_year(academic_year)
-        
-        if "cert_status" in kwargs:
-            cert_status = kwargs["cert_status"]
-            cert_status_select = Select(self.driver.find_element(
-                By.XPATH,
-                '//*[@id="ReportViewer1_ctl08_ctl07_ddValue"]'
-            ))
-            if cert_status is None:
-                cert_status_select.select_by_value("1")
-            else:
-                cert_status.select_by_visible_text(cert_status)
-        
-        elif "report_date" in kwargs:
-            report_date = kwargs["report_date"]
-            if report_date is None:
-                pass
-            else:
-                # You need the month and day as strings without leading zeroes
-                month = str(int(report_date[5:7]))
-                day = str(int(report_date[8:10]))
-                
-                month_select = Select(self.driver.find_element(
-                    By.XPATH,
-                    '//*[@id="ReportViewer1_ctl08_ctl05_ddValue"]'
-                ))
-                month_select.select_by_value(month)
-                self._wait_for_view_report_clickable()
-                
-                day_select = Select(self.driver.find_element(
-                    By.XPATH,
-                    '//*[@id="ReportViewer1_ctl08_ctl07_ddValue"]'
-                ))
-                day_select.select_by_value(day)
-                
-        submit_button = self._wait_for_view_report_clickable()
-        submit_button.click()
-        
-        self._wait_for_view_report_clickable(max_wait_time)
-        filepath = self._download_loaded_report(download_type, max_wait_time)
-        return filepath
-        
-    def _select_report_academic_year(self, academic_year):
-        """
-        Select the given academic_year for the the reports module. Assumes the driver
-        is already clicked into the iframe. This function waits for the "View Report"
-        button to be clickable before returning.
-        """
-        academic_year_string = f"{academic_year-1}-{academic_year}"
-        yr = Select(self.driver.find_element(
-            By.XPATH,
-            '//*[@id="ReportViewer1_ctl08_ctl03_ddValue"]'
-        ))
-        yr.select_by_visible_text(academic_year_string)
-        self._wait_for_view_report_clickable()
-        
-        
-    def _wait_for_view_report_clickable(self, max_attempts=3):
-        """
-        Check for the delay before webpage allows another change in value
-        for the report request
-        """
-        try:
-            max_attempts = int(max_attempts)
-        except:
-            max_attempts = 1
-        for attempt in range(max_attempts):
-            try:
-                view_report = WebDriverWait(self.driver, 60).until(
-                    EC.element_to_be_clickable((
-                        By.XPATH,
-                        '//*[@id="ReportViewer1_ctl08_ctl00"]'
-                    ))
-                )
-                return view_report
-            except TimeoutException:
-                logging.info('The Report button has not loaded after 1 minute. Attempt: {}'.format(attempt+1))
-        logging.info('Max number of attempts waiting for View Report to be clickable reached and all failed.')
-        raise TimeoutException
-        
-    def _download_loaded_report(self, download_type='csv', max_wait_time=3):
-        """
-        Downloads the report that is already loaded on the page. Assumes the driver
-        is still clicked into the iframe with the report controls.
-        
-        Return:
-        string: The filepath to the downloaded file.
-        """
-        dl_types = {
-            'csv': '//*[@id="ReportViewer1_ctl09_ctl04_ctl00_Menu"]/div[7]/a',
-            'pdf': '//*[@id="ReportViewer1_ctl09_ctl04_ctl00_Menu"]/div[4]/a',
-            'excel': '//*[@id="ReportViewer1_ctl09_ctl04_ctl00_Menu"]/div[2]/a'
-        }
-        
-        dropdown_btn = self.driver.find_element(
-            By.XPATH,
-            '//*[@id="ReportViewer1_ctl09_ctl04_ctl00"]'
-        )
-        dropdown_btn.click()
-        try:
-            dl_button = WebDriverWait(self.driver, 10).until(
-                EC.visibility_of_element_located((
-                    By.XPATH,
-                    dl_types[download_type]
-                ))
-            )
-        except TimeoutException:
-            logging.info("Dropdown menu for download not loading")
-            raise
-        dl_button.send_keys(Keys.ENTER)
-        if wait_for_any_file_in_folder(self.download_location, timeout=max_wait_time*60):
-            file_path = get_most_recent_file_in_dir(self.download_location)
-            logging.info(f"File found: {file_path}")
-            return file_path
-        else:
-            logging.info("No file found")
+# Code adapted from original code by Yusuph in the dops-calpad repo
+
+# Author: Howard Shen
+# Last Edited 5/25/2023
+
+import logging
+import os
+import pandas as pd
+import tempfile
+import time
+
+from datetime import date, datetime
+
+from selenium.webdriver.support.ui import Select, WebDriverWait
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.common.keys import Keys
+from selenium.common.exceptions import (
+    TimeoutException,
+    NoSuchElementException,
+    ElementNotInteractableException
+)
+
+from ducttape.utils import (
+    DriverBuilder,
+    get_most_recent_file_in_dir,
+    wait_for_any_file_in_folder
+)
+    
+try:
+    from spswarehouse.credentials import calpads_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
+
+from spswarehouse.calpads.calpads_config import (
+    monitoring_report_base,
+    monitoring_links,
+    snapshot_report_base,
+    snapshot_links,
+)
+    
+class CALPADS():
+    
+    def __init__(
+        self,
+        config=None,
+        username=None,
+        password=None,
+        host=None,
+        download_location=None,
+        headless=True,
+    ):
+        """
+        By default, the class will pull the username and password from the
+        credentials file in the module. You can override the credentials file
+        by passing either a config dictionary or both a username and password.
+        
+        Parameters:
+        config: A dictionary containing a username and password key. Optional.
+            Supercedes the username and password in credentials.py in this module.
+            Also supercedes a username and password combo passed to this function in
+            addition to the config.  May also contain a host key that will supercede
+            both the host parameter and the host from credentials.py
+        username: A CALPADS username, which should be in the form of an email address.
+            Must be paired with a password. Supercedes credentials.py.
+        password: Password for the given CALPADS username. Must be paired with a username
+            Supercedes credentials.py
+        host: The URL for CALPADS, in the format `https://www.calpads.org`. Optional.
+            Supercedes the host from credentials.py
+        download_location: The local folder that you want to save files too. If no
+            folder path passed, creates a temporary directory for this object.
+        headless: Selenium headless value. Default to True. If using this in a notebook,
+            recommend setting to False.
+        """
+        
+        self.host = None
+        if config is not None:
+            username = config['username']
+            password = config['password']
+            if 'host' in config:
+                self.host = config['host']
+        elif username is not None and password is not None:
+            username = username
+            password = password
+        else:
+            username = calpads_config['username']
+            password = calpads_config['password']
+        
+        if self.host is None and host is not None:
+            self.host = host
+        elif self.host is None:
+            self.host = calpads_config['host']
+        else:
+            pass
+        
+        if download_location is None:
+            self.download_location = tempfile.mkdtemp()
+        else:
+            self.download_location = download_location
+    
+        self.driver = DriverBuilder().get_driver(
+            download_location=self.download_location,
+            headless=headless
+        )
+        self._login_to_calpads(username, password)
+
+    def quit(self):
+        self.driver.quit()
+
+    def upload_file(self, lea, submission_type, file_path):
+        """
+        To be used in conjunction with the create_extract method, uploads the extract via File Submission on CALPADS.
+
+        Parameters:
+        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
+            dropdown on the CALPADS page.
+        submission_type: The four letter code, in all caps, for the file type you're 
+            uploading
+        file_path: The file path to the file you want to upload. Absolute path is
+            recommended (`os.path.abspath()`). Relative path behavior untested
+
+        Returns:
+        bool: True for a successful upload, else False
+        """
+        
+        self._select_lea(lea)
+        self.driver.get(f'{self.host}/FileSubmission/FileUpload')
+#         self.driver.refresh()
+        
+        try:
+            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((
+                By.XPATH,
+                '//*[@id="btnSearch"]'
+            )))
+        except TimeoutException:
+            logging.info('Unable to successfully reach the File Submission web page for {}. Closing the driver.'.format(lea))
+            return False
+
+        #Choose file type for the upload
+        select = Select(self.driver.find_element(By.XPATH, '//*[@id="tbFileUpload"]/tbody/tr/td[2]/select'))
+        select.select_by_value(submission_type)
+
+        #Find the file to upload by pulling the most recent file in the specific illuminate extract folder
+        choose_file = self.driver.find_element(By.XPATH, '//*[@id="tbFileUpload"]/tbody/tr/td[4]/input')
+        choose_file.send_keys(os.path.abspath(file_path))
+
+        #Upload
+        button = self.driver.find_element(By.XPATH, '//*[@id="btnSearch"]')
+        button.click()
+
+        try:
+            success = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located(
+            (By.CSS_SELECTOR, 'div.alert.alert-success.alert-dismissible.fade.in'))) #TODO: Confirm this reliably works. Otherwise, use text.
+        except TimeoutException:
+            logging.info('Something went wrong with the file upload for {}. Review files in directories and try again.'.format(lea)) #TODO: CALPADS provides error alerts in red on same page, should send to user
+            #TODO: Provide more information on error if possible?
+            return False
+        else:
+            logging.info('{} extract successfully uploaded for {}. Check the file submission status later.'.format(type(self).__name__, lea))
+            return True
+        
+    def get_upload_results(self, lea, submission_type, max_wait=5):
+        """
+        Retrieves the validation errors for the most recent upload of the given
+        submission type for the given LEA. Must be used within seven days of the upload
+        (default range on CALPADS).
+
+        Parameters:
+        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
+            dropdown on the CALPADS page.
+        submission_type: The four letter code, in all caps, for the file type you're 
+            uploading
+        max_wait: The maximum number of minutes to wait if the submission is still processing.
+            Default is 5 minutes. Must be at least 1.
+
+        Returns:
+        submitted_date_string (string): ISO formate date of the submission whose errors were checked. Returns None if the file submission can't be found for whatever reason
+        job_results_df (DataFrame): Returns a dataframe of the job results or False if the job is not yet in a final status.
+        error_details (DataFrame): Returns a dataframe of error details, False if unable to find error details, True if file posted.
+        """
+
+        if(max_wait < 1):
+            raise Exception('max_wait parameter must be 1 or more.')
+
+        self._select_lea(lea)
+        self.driver.get(f'{self.host}/FileSubmission/')
+        try:
+            file_elem = WebDriverWait(self.driver, 15).until(
+                EC.presence_of_element_located((By.ID, 'FileType'))
+            )
+        except TimeoutException:
+            logging.info("Can't load View Submission page")
+            return None, False
+
+        # Filter the file list
+        file_select = Select(file_elem)
+        file_select.select_by_value(submission_type)
+        apply_button = self.driver.find_element(By.ID, "fileSubSearch")
+        apply_button.click()
+        try:
+            # The filtered page is identical, so sleep for a moment
+            time.sleep(2)
+            WebDriverWait(self.driver, 20).until(EC.text_to_be_present_in_element(
+                (By.XPATH, '//*[@id="FileSubmissionSearchResults"]/table/tbody/tr[1]/td[6]'),
+                submission_type
+            ))
+        except TimeoutException:
+            logging.info(f"No recent submissions of type {submission_type}")
+            return None, False
+
+        # Process submission date
+        date_text = self.driver.find_element(
+            By.XPATH,
+            '//*[@id="FileSubmissionSearchResults"]/table/tbody/tr[1]/td[3]'
+        ).text
+
+        submitted_datetime = datetime.strptime(date_text, "%m/%d/%Y %I:%M:%S %p")
+        submitted_date_string = submitted_datetime.date().isoformat()
+
+        for i in range(max_wait):
+            file_status = self.driver.find_element(
+                By.XPATH,
+                '//*[@id="FileSubmissionSearchResults"]/table/tbody/tr[1]/td[8]'
+            ).text
+            if file_status in ['Posted', 'Failed', 'Rejected']:
+                logging.info('Found final job results. Storing them.')
+                job_results_df = pd.read_html(self.driver.page_source)[0].head(1)
+                break
+            else:
+                if((i+1)< max_wait):
+                    logging.info(f'Try #{i+1}: Did not find finished job. Will try again in 60 seconds.')
+                    time.sleep(60)
+                    self.driver.refresh()
+                    time.sleep(3)
+                else:
+                    logging.info(f'Try #{i+1}: Did not find finished job.')
+
+        # Branch based on file status
+        if file_status == 'Posted':
+            logging.info(f"{submission_type} Posted on {submitted_date_string}")
+            return submitted_date_string, job_results_df, True
+        elif file_status == 'Failed':
+            logging.info(f"{submission_type} Failed on {submitted_date_string}. Check manually")
+            return submitted_date_string, job_results_df, False
+        elif file_status == 'Rejected':
+            view_errors = self.driver.find_element(
+                By.XPATH,
+                '//*[@id="FileSubmissionSearchResults"]/table/tbody/tr[1]/td[1]/a'
+            )
+            view_errors.click()
+        else:
+            logging.info(f"{submitted_date_string} {submission_type} not complete after {max_wait} minute{'s' if max_wait > 1 else ''}.")
+            return submitted_date_string, False, False
+
+        try:
+            WebDriverWait(self.driver, 30).until(EC.text_to_be_present_in_element((
+                By.XPATH,
+                '//*[@id="main"]/div/div[2]/header/h1'), 'View Submission Details'
+            ))
+            time.sleep(10) # The file errors takes a moment to load; extended from 2 to 10 seconds after some rejected files didn't have errors captured
+        except TimeoutException as t:
+            logging.info('Something went wrong with loading the submission error details page.')
+            return submitted_date_string, job_results_df, False
+
+         #We expect the error details to be the second table in the HTML source
+        error_details_df = pd.read_html(self.driver.page_source)[1]
+
+        # Get errors if there are multiple pages
+        error_has_next = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH, '//*[@id="FileErrors"]/div/a[3]')))
+
+        all_error_details = []
+        all_error_details.append(error_details_df)
+
+        while 'disabled' not in error_has_next.get_attribute('class'):
+            logging.info('Next Page')
+            error_has_next.click()
+            # Give time for next page to load
+            time.sleep(10)
+            next_details_df = pd.read_html(self.driver.page_source)[1] #TODO: Confirm that this is a completely new df
+            all_error_details.append(next_details_df)
+            error_has_next = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH, '//*[@id="FileErrors"]/div/a[3]')))
+
+        all_error_details = pd.concat(all_error_details)
+        logging.info("Successfully collected all errors from file submission error details for the {} {} extract.".format(submitted_date_string, submission_type))
+        return submitted_date_string, job_results_df, all_error_details
+    
+    def get_certification_status(self, lea, academic_year, submission_name, **kwargs):
+        """
+        Retrieves the status of a Certification window.
+
+        Parameters:
+        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
+            dropdown on the CALPADS page.
+        academic_year: Integer representing the academic year that you want to check
+            (per team norms, this is the year when the school year ends)
+        submission_name: The name of the certification window. As of this edit, the
+            certification windows are Fall1, Fall2, EOY1, EOY2, EOY3, and EOY4.
+        optional arguments (kwargs):
+            rollover_date: Applies only to EOY3. An ISO format string (YYYY-MM-DD)
+                representing the expected rollover date of your SIS. The SIS rollover
+                is when exit dates and exit codes get put on enrollment records.
+                Prior to this, CALPADS will return CERT131 errors for every actively
+                enrolled student. This function will begin scraping CERT131 the day
+                after the rollover date. If you do not pass a rollover date, CERT131
+                will be scraped.
+
+        Returns:
+        cert_status (Boolean): Returns False if the certification window isn't open yet;
+            returns True if it is.
+        error_details (DataFrame): Returns a dataframe of error details, None if no errors,
+            None if certification window isn't open.
+        warning_details (DataFrame): Returns a dataframe of warningsdetails, None if no
+            warnings, None if certification window isn't open.
+        """
+        
+        # Fall1, EOY3, EOY4 have a SELPA approval, which
+        # creates an extra table on the Cert status page, altering the XPATH
+        if submission_name in ['Fall1', 'EOY3', 'EOY4']:
+            data_div_num = 5
+            data_table_num = 3
+            error_table_num = 1
+            warning_table_num = 2
+        else:
+            data_div_num = 4
+            data_table_num = 2
+            error_table_num = 0
+            warning_table_num = 1
+        
+        # CERT131 is somewhat meaningless prior to the end of the year
+        if submission_name == 'EOY3':
+            try:
+                rollover_date = date.fromisoformat(kwargs['rollover_date'])
+                cert131_flag = date.today() > rollover_date
+                logging.info(f"Today is {date.today()}, Rollover date is {rollover_date}, CERT131 = {cert131_flag}")
+            except KeyError:
+                # KeyError means rollover_date was not passed as an argument
+                logging.info("No rollover date passed; scraping CERT131")
+                cert131_flag = True
+        else:
+            cert131_flag = True
+        
+        self._select_lea(lea)
+        
+        academic_year_string = f"{academic_year-1}-{academic_year}"
+        self.driver.get(f"https://www.calpads.org/StateReporting/Certification?AcademicYear={academic_year_string}&Snapshot={submission_name}")
+        
+        try:
+            WebDriverWait(self.driver, 20).until(EC.presence_of_element_located((
+                By.XPATH,
+                '/html/body/div[1]/main/div/div[2]/div[3]/div/div/div/div/table/tbody/tr/td[1]'
+            )))
+        except TimeoutException:
+            logging.info(f"{submission_name} certification errors not available yet")
+            return False, None, None
+        
+        error_and_warn_text = self.driver.find_element(
+            By.XPATH,
+            "/html/body/div[1]/main/div/div[2]/div[3]/div/div/div/div/table/tbody/tr/td[9]"
+        ).text
+        error_and_warn_count = int(error_and_warn_text)
+
+        if error_and_warn_count > 0:
+            cert_status_link = self.driver.find_element(
+                By.XPATH,
+                '/html/body/div[1]/main/div/div[2]/div[3]/div/div/div/div/table/tbody/tr/td[1]/a'
+            )
+            cert_status_link.click()
+            try:
+                WebDriverWait(self.driver, 20).until(EC.text_to_be_present_in_element(
+                    (
+                        By.XPATH,
+                        '/html/body/div/main/div/div[2]/header/h1'
+                    ),
+                    'Certification Details - LEA'
+                ))
+            except TimeoutException:
+                logging.info("Failed to load Certification Status page")
+                raise RuntimeError("Failed to load Certification Status page")
+            try:
+                WebDriverWait(self.driver, 15).until(EC.presence_of_element_located((
+                    By.XPATH,
+                    f'/html/body/div/main/div/div[2]/div[{data_div_num}]/div[1]/div[1]/div/ul/li/div/div/div/table/tbody/tr/td[4]/a'
+                )))
+                # Error list should be the second table
+                errors_table = pd.read_html(self.driver.page_source)[error_table_num]
+                error_df = pd.DataFrame()
+                
+                error_list_has_next = self.driver.find_element(
+                    By.XPATH,
+                    '//*[@id="RequiredGrid_FATAL"]/div/a[3]'
+                )
+                while 'disabled' not in error_list_has_next.get_attribute('class'):
+                    logging.info("Getting next page of errors list")
+                    try:
+                        error_list_has_next.click()
+                    except ElementNotInteractableException:
+                        banner = self.driver.find_element(
+                            By.XPATH,
+                            '//*[@id="CertificationErrorSummary"]/li/a'
+                        )
+                        banner.click()
+                        error_list_has_next.click()
+                    time.sleep(2)
+                    errors_table = pd.concat(
+                        [errors_table, pd.read_html(self.driver.page_source)[error_table_num]],
+                        axis=0,
+                        ignore_index=True
+                    )
+                    error_list_has_next = self.driver.find_element(
+                        By.XPATH,
+                        '//*[@id="RequiredGrid_FATAL"]/div/a[3]'
+                    )
+                
+                for i in range(len(errors_table)):
+                    error_id = errors_table["Message ID"][i]
+
+                    if error_id == 'CERT131' and not cert131_flag:
+                        logging.info("Skipping CERT131")
+                        continue
+                        
+                    logging.info(f"Getting list for {error_id}")
+                    error_dropdown = self.driver.find_element(
+                        By.ID,
+                        'CertificationEditQuery_ChildErrorCategory'
+                    )
+                    error_select = Select(error_dropdown)
+                    error_select.select_by_value(error_id)
+                    apply_button = self.driver.find_element(
+                        By.XPATH,
+                        '//*[@id="certDetails"]/div[1]/div[3]/div/div/form/div[3]/button'
+                    )
+                    apply_button.click()
+                    
+                    try:
+                        WebDriverWait(self.driver, 30).until(EC.text_to_be_present_in_element(
+                            (
+                                By.XPATH,
+                                f'/html/body/div/main/div/div[2]/div[{data_div_num}]/div[1]/div[4]/div/div/table/tbody/tr/td[10]/a'
+                            ),
+                            error_id
+                        ))
+                    except TimeoutException:
+                        logging.info(f"Can't load errors for {error_id}")
+                        raise RuntimeError(f"Can't load errors for {error_id}")
+                    
+                    error_has_next = self.driver.find_element(
+                        By.XPATH,
+                        '//*[@id="RequiredGrid"]/div/a[3]'
+                    )
+                    
+                    error_df = pd.concat(
+                        [error_df, pd.read_html(self.driver.page_source)[data_table_num]],
+                        axis=0,
+                        ignore_index=True,
+                    )
+                    
+                    while 'disabled' not in error_has_next.get_attribute('class'):
+                        logging.info("Getting next page")
+                        error_has_next.click()
+                        time.sleep(2)
+                        error_df = pd.concat(
+                            [error_df, pd.read_html(self.driver.page_source)[data_table_num]],
+                            axis=0,
+                            ignore_index=True,
+                        )
+                        error_has_next = self.driver.find_element(
+                        By.XPATH,
+                        '//*[@id="RequiredGrid"]/div/a[3]'
+                        )
+                    
+                # Drop the "View" button column
+                if len(error_df) == 0:
+                    logging.info("Only Cert Error was CERT131, and rollover has not passed.")
+                    error_df = None
+                else:
+                    error_df.drop(columns="Error Record", inplace=True)
+                
+            except TimeoutException:
+                logging.info(f"No errors for {submission_name}")
+                error_df = None
+            
+            # Get Warnings
+            try:
+                WebDriverWait(self.driver, 5).until(EC.presence_of_element_located((
+                    By.XPATH,
+                    f'/html/body/div/main/div/div[2]/div[{data_div_num}]/div[1]/div[2]/div/ul/li/div/div/div/table/tbody/tr/td[4]/a'
+                )))
+                # Warning list should be the third table
+                warnings_table = pd.read_html(self.driver.page_source)[warning_table_num]
+                warning_df = pd.DataFrame()
+                
+                warning_list_has_next = self.driver.find_element(
+                    By.XPATH,
+                    '//*[@id="RequiredGrid_WARN"]/div/a[3]'
+                )
+                while 'disabled' not in warning_list_has_next.get_attribute('class'):
+                    logging.info("Getting next page of warnings list")
+                    try:
+                        warning_list_has_next.click()
+                    except ElementNotInteractableException:
+                        banner = self.driver.find_element(
+                            By.XPATH,
+                            '//*[@id="CertificationWarnSummary"]/li/a'
+                        )
+                        banner.click()
+                        warning_list_has_next.click()
+                    time.sleep(2)
+                    warnings_table = pd.concat(
+                        [warnings_table, pd.read_html(self.driver.page_source)[warning_table_num]],
+                        axis=0,
+                        ignore_index=True
+                    )
+                    warning_list_has_next = self.driver.find_element(
+                        By.XPATH,
+                        '//*[@id="RequiredGrid_WARN"]/div/a[3]'
+                    )
+                
+                for i in range(len(warnings_table)):
+                    warning_id = warnings_table["Message ID"][i]
+                        
+                    logging.info(f"Getting list for {warning_id}")
+                    warning_dropdown = self.driver.find_element(
+                        By.ID,
+                        'CertificationEditQuery_ChildErrorCategory'
+                    )
+                    warning_select = Select(warning_dropdown)
+                    warning_select.select_by_value(warning_id)
+                    apply_button = self.driver.find_element(
+                        By.XPATH,
+                        '//*[@id="certDetails"]/div[1]/div[3]/div/div/form/div[3]/button'
+                    )
+                    apply_button.click()
+                    
+                    try:
+                        WebDriverWait(self.driver, 15).until(EC.text_to_be_present_in_element(
+                            (
+                                By.XPATH,
+                               f'/html/body/div/main/div/div[2]/div[{data_div_num}]/div[1]/div[4]/div/div/table/tbody/tr/td[10]/a'
+                            ),
+                            warning_id
+                        ))
+                    except TimeoutException:
+                        logging.info(f"Can't load errors for {warning_id}")
+                        raise RuntimeError(f"Can't load errors for {warning_id}")
+                    
+                    warning_has_next = self.driver.find_element(
+                        By.XPATH,
+                        '//*[@id="RequiredGrid"]/div/a[3]'
+                    )
+                    
+                    warning_df = pd.concat(
+                        [warning_df, pd.read_html(self.driver.page_source)[data_table_num]],
+                        axis=0,
+                        ignore_index=True,
+                    )
+                    
+                    while 'disabled' not in warning_has_next.get_attribute('class'):
+                        logging.info("Getting next page")
+                        warning_has_next.click()
+                        time.sleep(2)
+                        warning_df = pd.concat(
+                            [warning_df, pd.read_html(self.driver.page_source)[data_table_num]],
+                            axis=0,
+                            ignore_index=True,
+                        )
+                        warning_has_next = self.driver.find_element(
+                            By.XPATH,
+                            '//*[@id="RequiredGrid"]/div/a[3]'
+                        )
+                    
+                # Drop the "View" button column
+                warning_df.drop(columns="Error Record", inplace=True)
+                
+            except TimeoutException:
+                logging.info(f"No warnings for {submission_name}")
+                warning_df = None
+                
+            return True, error_df, warning_df
+        elif error_and_warn_count == 0:
+            logging.info(f"No errors or warnings for {submission_name}")
+            return True, None, None
+        else:
+            raise RuntimeError("Impossible part of error_and_warn_count if-elif-else reached.")
+
+    def download_monitoring_report(
+        self,
+        lea,
+        academic_year,
+        report_code,
+        report_date=None,
+        download_type='csv',
+        max_wait_time=10
+    ):
+        """
+        Download a CALPADS snapshot report.
+        
+        Known issue: The download folder needs to be empty when this function is called.
+        
+        Parameters:
+        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
+            dropdown on the CALPADS page.
+        academic_year: Integer representing the academic year that you want to check
+            (per team norms, this is the year when the school year ends)
+        submission_name: The name of the certification window. As of this edit, the
+            certification windows are Fall1, Fall2, EOY1, EOY2, EOY3, and EOY4.
+        report_code: The code for the report that you want. Should be a string in
+            the form of "#.#". Check calpads_config.py for the list of available
+            report_code + submission_name combos
+        report_date (str): An ISO format date string ('YYYY-MM-DD') indicating the 
+            desired date for the report. If None, the function will download whatever
+            the default date on the report is (usually today).
+            Note that the function only uses the month and day. (E.g., if you pass
+            academic_year=2023 and report_date="2024-10-01", the report downloaded will be
+            for October 1 of academic year 2023, which is actually "2022-10-01")
+        download_type (str): The format in which you want the download for the report.
+            Currently supports csv, excel, and pdf.
+        max_wait_time: Integer >=0 indicating the maximum number of minutes to wait
+            for the report to generate and for the download to succeed. This means
+            this function can actually take up to 2*max_wait_time to run.
+        
+        Returns:
+        string: The filepath to the downloaded file
+        """
+        url_tail = monitoring_links[report_code]
+        report_url = self.host + monitoring_report_base + url_tail
+        
+        return self._download_report(
+            lea,
+            report_url,
+            academic_year,
+            download_type,
+            max_wait_time,
+            report_date=report_date
+        )
+            
+    def download_snapshot_report(
+        self,
+        lea,
+        academic_year,
+        submission_name,
+        report_code,
+        cert_status=None,
+        download_type='csv',
+        max_wait_time=10
+    ):
+        """
+        Download a CALPADS snapshot report.
+        
+        Known issue: The download folder needs to be empty when this function is called.
+        
+        Parameters:
+        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
+            dropdown on the CALPADS page.
+        academic_year: Integer representing the academic year that you want to check
+            (per team norms, this is the year when the school year ends)
+        submission_name: The name of the certification window. As of this edit, the
+            certification windows are Fall1, Fall2, EOY1, EOY2, EOY3, and EOY4.
+        report_code: The code for the report that you want. Should be a string in
+            the form of "#.#". Check calpads_config.py for the list of available
+            report_code + submission_name combos
+        cert_status: If there are multiple snapshots, which version you want. If
+            `None`, the top most option is selected (usually some variant of
+            "Certified" if the snapshot is certified). Will raise an error if the
+            given cert_status is not available.
+        download_type (str): The format in which you want the download for the report.
+            Currently supports csv, excel, and pdf.
+        max_wait_time: Integer >=0 indicating the maximum number of minutes to wait
+            for the report to generate and for the download to succeed. This means
+            this function can actually take up to 2*max_wait_time to run.
+        
+        Returns:
+        string: The filepath to the downloaded file
+        """
+        url_tail = snapshot_links[submission_name][report_code]
+        report_url = self.host + snapshot_report_base + url_tail
+        
+        return self._download_report(
+            lea,
+            report_url,
+            academic_year,
+            download_type,
+            max_wait_time,
+            cert_status=cert_status
+        )
+            
+    def _login_to_calpads(self, username, password):
+        self.driver.get(self.host)
+        try:
+            WebDriverWait(self.driver, 15).until(EC.presence_of_element_located((
+                By.XPATH,
+                '/html/body/div[3]/div/form/div/div[2]/fieldset/div[4]/div/button'
+            )))
+        except TimeoutException:
+            logging.info("Was unable to reach the login page. Check the browser: {}".format(self.driver.title))
+            return False
+        except NoSuchElementException:
+            logging.info("Was unable to reach the login page. Check the browser: {}".format(self.driver.title))
+            return False
+        user = self.driver.find_element(By.ID, "Username")
+        user.send_keys(username)
+        pw = self.driver.find_element(By.ID, "Password")
+        pw.send_keys(password)
+        agreement = self.driver.find_element(By.ID, "AgreementConfirmed")
+        self.driver.execute_script("arguments[0].click();", agreement)
+        btn = self.driver.find_element(
+            By.XPATH,
+            "/html/body/div[3]/div/form/div/div[2]/fieldset/div[4]/div/button"
+        )
+        btn.click()
+        try:
+            WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((
+                By.ID,
+                'org-select'
+            )))
+        except TimeoutException:
+            logging.info('Something went wrong with the login. Checking to see if there was an expected error message.')
+            try:
+                alert = WebDriverWait(self.driver, 15).until(EC.presence_of_element_located((
+                    By.XPATH,
+                    '/html/body/div[3]/div/form/div[1]'
+                )))
+                if 'alert' in alert.get_attribute('class'):
+                    logging.info("Found an expected alert during login: '{}'".format(
+                        self.driver.find_element(
+                            By.XPATH, '/html/body/div[3]/div/form/div[1]/div/ul/li'
+                        ).text
+                    ))
+                    return False
+                else:
+                    logging.info('There was an unexpected message during login. See driver.')
+                    return False
+            except TimeoutException:
+                logging.info('There was an unexpected error during login. See driver.')
+                return False
+
+        return True
+    
+    def _select_lea(self, lea):
+        """
+        Factored out common process for switching to a different LEA in the dropdown
+
+        Parameters:
+        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
+            dropdown on the CALPADS page.
+        """
+        select = Select(self.driver.find_element(By.ID, 'org-select'))
+        select.select_by_value(lea)
+        WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.ID, 'org-select')))
+
+    def _download_report(
+        self,
+        lea,
+        url,
+        academic_year,
+        download_type,
+        max_wait_time,
+        **kwargs
+    ):
+        """
+        Helper function for downloading from the reports iframe
+        Will crash if you pass "cert_status" in kwargs but the report is not a Snapshot
+            report
+        Will also crash if you pass a value othere than None for "report_date" in kwargs
+            but the report is not an Accountability/Monitoring report
+        """
+        
+        self._select_lea(lea)
+        self.driver.get(url)
+        try:
+            # The Reports module is in an iframe
+            iframe = WebDriverWait(self.driver, 30).until(
+                EC.presence_of_element_located((
+                    By.XPATH,
+                    '//*[@id="reports"]/div/div/div/iframe'
+                ))
+            )
+        except TimeoutException:
+            logging.info("Failed to load report page.")
+            raise
+        
+        self.driver.switch_to.frame(iframe)
+        self._select_report_academic_year(academic_year)
+        
+        if "cert_status" in kwargs:
+            cert_status = kwargs["cert_status"]
+            cert_status_select = Select(self.driver.find_element(
+                By.XPATH,
+                '//*[@id="ReportViewer1_ctl08_ctl07_ddValue"]'
+            ))
+            if cert_status is None:
+                cert_status_select.select_by_value("1")
+            else:
+                cert_status.select_by_visible_text(cert_status)
+        
+        elif "report_date" in kwargs:
+            report_date = kwargs["report_date"]
+            if report_date is None:
+                pass
+            else:
+                # You need the month and day as strings without leading zeroes
+                month = str(int(report_date[5:7]))
+                day = str(int(report_date[8:10]))
+                
+                month_select = Select(self.driver.find_element(
+                    By.XPATH,
+                    '//*[@id="ReportViewer1_ctl08_ctl05_ddValue"]'
+                ))
+                month_select.select_by_value(month)
+                self._wait_for_view_report_clickable()
+                
+                day_select = Select(self.driver.find_element(
+                    By.XPATH,
+                    '//*[@id="ReportViewer1_ctl08_ctl07_ddValue"]'
+                ))
+                day_select.select_by_value(day)
+                
+        submit_button = self._wait_for_view_report_clickable()
+        submit_button.click()
+        
+        self._wait_for_view_report_clickable(max_wait_time)
+        filepath = self._download_loaded_report(download_type, max_wait_time)
+        return filepath
+        
+    def _select_report_academic_year(self, academic_year):
+        """
+        Select the given academic_year for the the reports module. Assumes the driver
+        is already clicked into the iframe. This function waits for the "View Report"
+        button to be clickable before returning.
+        """
+        academic_year_string = f"{academic_year-1}-{academic_year}"
+        yr = Select(self.driver.find_element(
+            By.XPATH,
+            '//*[@id="ReportViewer1_ctl08_ctl03_ddValue"]'
+        ))
+        yr.select_by_visible_text(academic_year_string)
+        self._wait_for_view_report_clickable()
+        
+        
+    def _wait_for_view_report_clickable(self, max_attempts=3):
+        """
+        Check for the delay before webpage allows another change in value
+        for the report request
+        """
+        try:
+            max_attempts = int(max_attempts)
+        except:
+            max_attempts = 1
+        for attempt in range(max_attempts):
+            try:
+                view_report = WebDriverWait(self.driver, 60).until(
+                    EC.element_to_be_clickable((
+                        By.XPATH,
+                        '//*[@id="ReportViewer1_ctl08_ctl00"]'
+                    ))
+                )
+                return view_report
+            except TimeoutException:
+                logging.info('The Report button has not loaded after 1 minute. Attempt: {}'.format(attempt+1))
+        logging.info('Max number of attempts waiting for View Report to be clickable reached and all failed.')
+        raise TimeoutException
+        
+    def _download_loaded_report(self, download_type='csv', max_wait_time=3):
+        """
+        Downloads the report that is already loaded on the page. Assumes the driver
+        is still clicked into the iframe with the report controls.
+        
+        Return:
+        string: The filepath to the downloaded file.
+        """
+        dl_types = {
+            'csv': '//*[@id="ReportViewer1_ctl09_ctl04_ctl00_Menu"]/div[7]/a',
+            'pdf': '//*[@id="ReportViewer1_ctl09_ctl04_ctl00_Menu"]/div[4]/a',
+            'excel': '//*[@id="ReportViewer1_ctl09_ctl04_ctl00_Menu"]/div[2]/a'
+        }
+        
+        dropdown_btn = self.driver.find_element(
+            By.XPATH,
+            '//*[@id="ReportViewer1_ctl09_ctl04_ctl00"]'
+        )
+        dropdown_btn.click()
+        try:
+            dl_button = WebDriverWait(self.driver, 10).until(
+                EC.visibility_of_element_located((
+                    By.XPATH,
+                    dl_types[download_type]
+                ))
+            )
+        except TimeoutException:
+            logging.info("Dropdown menu for download not loading")
+            raise
+        dl_button.send_keys(Keys.ENTER)
+        if wait_for_any_file_in_folder(self.download_location, timeout=max_wait_time*60):
+            file_path = get_most_recent_file_in_dir(self.download_location)
+            logging.info(f"File found: {file_path}")
+            return file_path
+        else:
+            logging.info("No file found")
             return None
```

### Comparing `spswarehouse-0.6.1/spswarehouse/general/os.py` & `spswarehouse-0.6.2/spswarehouse/general/os.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import os
-from glob import glob
-
-def make_directory_if_does_not_exist(path):
-    if not os.path.exists(path):
-        os.makedirs(path)
-        print(f'Directory "{path}" created.')
-    else:
-        print(f'Directory "{path}" already exists.')
-
-def get_most_recent_file_in_dir(folder_path):
-    """Returns the most recently changed file in a folder.
-
-    Args:
-        folder_path: The path to the folder to search
-    Returns:
-        A string with the filename of the most recently changed file in the
-        folder.
-    """
-    # * means all if need specific format then *.csv
-    list_of_files = glob(folder_path + '/*')
-    latest_file = max(list_of_files, key=os.path.getctime)
+import os
+from glob import glob
+
+def make_directory_if_does_not_exist(path):
+    if not os.path.exists(path):
+        os.makedirs(path)
+        print(f'Directory "{path}" created.')
+    else:
+        print(f'Directory "{path}" already exists.')
+
+def get_most_recent_file_in_dir(folder_path):
+    """Returns the most recently changed file in a folder.
+
+    Args:
+        folder_path: The path to the folder to search
+    Returns:
+        A string with the filename of the most recently changed file in the
+        folder.
+    """
+    # * means all if need specific format then *.csv
+    list_of_files = glob(folder_path + '/*')
+    latest_file = max(list_of_files, key=os.path.getctime)
     return latest_file
```

### Comparing `spswarehouse-0.6.1/spswarehouse/general/selenium.py` & `spswarehouse-0.6.2/spswarehouse/general/selenium.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,295 +1,295 @@
-import time
-
-from selenium.webdriver.support.ui import WebDriverWait, Select
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-
-
-### Click Elements
-
-def click_element_by_css_selector(driver, css_selector: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by CSS Selector and clicks it.
-    """
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.CSS_SELECTOR, css_selector, wait_time_in_seconds)
-
-def click_element_by_id(driver, element_id: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by ID and clicks it.
-    """
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.ID, element_id, wait_time_in_seconds)
-
-def click_element_by_name(driver, element_name: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by name and clicks it.
-    """
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.NAME, element_name, wait_time_in_seconds)
-
-def click_element_by_link_text(driver, link_text, wait_time_in_seconds=30):
-    """
-    Waits for an element by (full) link text and clicks it.
-    """
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.LINK_TEXT, link_text, wait_time_in_seconds)
-
-def click_element_by_partial_link_text(driver, partial_link_text: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by partial link text and clicks it.
-    """
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.PARTIAL_LINK_TEXT, partial_link_text, wait_time_in_seconds)
-
-def click_element_by_xpath(driver, xpath: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by XPATH and clicks it.
-    """
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.XPATH, xpath, wait_time_in_seconds)
-
-
-### Checkboxes
-
-def ensure_checkbox_is_checked_by_name(driver, checkbox_name: str, wait_time_in_seconds=30):
-    """
-    Waits for a checkbox element by name and clicks it if it is not already selected.
-    """
-    checkbox = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, f"//input[@type='checkbox' and @name='{checkbox_name}']", 
-        wait_time_in_seconds)
-    
-    if checkbox.is_selected() == False:
-        checkbox.click()
-
-def ensure_checkbox_is_unchecked_by_name(driver, checkbox_name: str, wait_time_in_seconds=30):
-    """
-    Waits for a checkbox element by name and clicks it if it is already selected, to make
-    sure it is not checked.
-    """
-    checkbox = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, f"//input[@type='checkbox' and @name='{checkbox_name}']", 
-        wait_time_in_seconds)
-    
-    if checkbox.is_selected():
-        checkbox.click()
-
-
-### Element Text Matches
-
-def ensure_element_text_matches_expected_value_by_xpath(driver, element_xpath, expected_text, wait_time_in_seconds=30):
-    """
-    Waits for an element by XPATH and checks whether its text matches the expected text.
-    """
-    elem = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, element_xpath, wait_time_in_seconds)
-    return elem.text == expected_text
-
-
-### Get Element(s)
-
-def get_element_by_css_selector(driver, css_selector: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by CSS Selector and returns it.
-    """
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.CSS_SELECTOR, css_selector, wait_time_in_seconds)
-    return elem
-
-def get_element_by_id(driver, element_id, wait_time_in_seconds=30):
-    """
-    Waits for an element by ID and returns it.
-    """
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
-    return elem
-
-def get_element_by_link_text(driver, link_text, wait_time_in_seconds=30):
-    """
-    Waits for an element by (full) link text and returns it.
-    """
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.LINK_TEXT, link_text, wait_time_in_seconds)
-    return elem
-
-def get_element_by_xpath(driver, xpath: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by XPATH and returns it.
-    """
-    elem = WebDriverWait(driver, wait_time_in_seconds).until(EC.presence_of_element_located((By.XPATH, xpath)))
-    return elem
-
-def get_multiple_elements_by_class_name(driver, class_name: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by class name, then retrieves the full list of elements with that class name.
-    """
-    _wait_for_element_to_be_present_and_return_it(driver, By.CLASS_NAME, class_name, wait_time_in_seconds)
-
-    # Pause to give all elements with that class_name time to load
-    time.sleep(5)
-
-    elements_list = driver.find_elements(By.CLASS_NAME, class_name)
-
-    return elements_list
-
-
-### Select Text in Element
-
-def select_visible_text_in_element_by_id(driver, element_id: str, text_to_select: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by ID and selects it by specified text.
-    """
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
-    select = Select(elem)
-    select.select_by_visible_text(text_to_select)
-
-def select_visible_text_in_element_by_name(driver, element_name: str, text_to_select: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by name and selects it by specified text.
-    """
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.NAME, element_name, wait_time_in_seconds)
-    select = Select(elem)
-    select.select_by_visible_text(text_to_select)
-
-
-### Type in Element
-
-def type_in_element_by_id(driver, element_id: str, input_to_type: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by ID, clears it, and types in the input.
-    """
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
-    elem.clear()
-    elem.send_keys(input_to_type)
-
-def type_in_element_by_name(driver, element_name: str, input_to_type: str, wait_time_in_seconds=30):
-    """
-    Waits for an element by name, clears it, and types in the input.
-    """
-    elem =  _wait_for_element_to_be_present_and_return_it(driver, By.NAME, element_name, wait_time_in_seconds)
-    elem.clear()
-    elem.send_keys(input_to_type)
-
-
-### Wait for Element
-    
-def wait_for_element_containing_specific_text(driver, expected_element_text, wait_time_in_seconds=30):
-    """
-    Waits for an element containing the specific text. Will crash if it does not 
-    appear in the time allotted (default = 30 seconds).
-    """
-    xpath_text = f"//*[contains(text(), '{expected_element_text}')]"
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.XPATH, xpath_text, wait_time_in_seconds)
-    return elem
-    
-
-### Internal Functions
-
-def _wait_for_element_to_be_clickable_and_return_it(driver, by_object, target_identifier, wait_time_in_seconds=30):
-    elem = WebDriverWait(driver, wait_time_in_seconds).until(EC.element_to_be_clickable((by_object, target_identifier)))
-    return elem
-
-def _wait_for_element_to_be_clickable_and_click_it(driver, by_object, target_identifier, wait_time_in_seconds=30):
-    elem = _wait_for_element_to_be_clickable_and_return_it(driver, by_object, target_identifier, wait_time_in_seconds)
-    elem.click()
-
-def _wait_for_element_to_be_present_and_return_it(driver, by_object, target_identifier, wait_time_in_seconds=30):
-    elem = WebDriverWait(driver, wait_time_in_seconds).until(EC.presence_of_element_located((by_object, target_identifier)))
-    return elem
-
-
-### Deprecated old functions, do not delete until v1.0.0
-def helper_click_element_by_css_selector(driver, css_selector: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.CSS_SELECTOR, css_selector, wait_time_in_seconds)
-
-def helper_click_element_by_id(driver, element_id: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.ID, element_id, wait_time_in_seconds)
-
-def helper_click_element_by_name(driver, element_name: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.NAME, element_name, wait_time_in_seconds)
-
-def helper_click_element_by_link_text(driver, link_text, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.LINK_TEXT, link_text, wait_time_in_seconds)
-
-def helper_click_element_by_partial_link_text(driver, partial_link_text: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.PARTIAL_LINK_TEXT, partial_link_text, wait_time_in_seconds)
-
-def helper_click_element_by_xpath(driver, xpath: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    _wait_for_element_to_be_clickable_and_click_it(driver, By.XPATH, xpath, wait_time_in_seconds)
-    
-def helper_ensure_checkbox_is_checked_by_name(driver, checkbox_name: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    checkbox = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, f"//input[@type='checkbox' and @name='{checkbox_name}']", 
-        wait_time_in_seconds)
-    
-    if checkbox.is_selected() == False:
-        checkbox.click()
-
-def helper_ensure_checkbox_is_unchecked_by_name(driver, checkbox_name: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    checkbox = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, f"//input[@type='checkbox' and @name='{checkbox_name}']", 
-        wait_time_in_seconds)
-    
-    if checkbox.is_selected():
-        checkbox.click()
-
-def helper_ensure_element_text_matches_expected_value_by_xpath(driver, element_xpath, expected_text, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    elem = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, element_xpath, wait_time_in_seconds)
-    return elem.text == expected_text
-
-def helper_get_element_by_css_selector(driver, css_selector: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.CSS_SELECTOR, css_selector, wait_time_in_seconds)
-    return elem
-
-def helper_get_element_by_id(driver, element_id, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
-    return elem
-
-def helper_get_element_by_link_text(driver, link_text, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.LINK_TEXT, link_text, wait_time_in_seconds)
-    return elem
-
-def helper_get_element_by_xpath(driver, xpath: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    elem = WebDriverWait(driver, wait_time_in_seconds).until(EC.presence_of_element_located((By.XPATH, xpath)))
-    return elem
-
-def helper_get_multiple_elements_by_class_name(driver, class_name: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    _wait_for_element_to_be_present_and_return_it(driver, By.CLASS_NAME, class_name, wait_time_in_seconds)
-
-    # Pause to give all elements with that class_name time to load
-    time.sleep(5)
-
-    elements_list = driver.find_elements(By.CLASS_NAME, class_name)
-
-    return elements_list
-
-def helper_select_visible_text_in_element_by_id(driver, element_id: str, text_to_select: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
-    select = Select(elem)
-    select.select_by_visible_text(text_to_select)
-
-def helper_select_visible_text_in_element_by_name(driver, element_name: str, text_to_select: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.NAME, element_name, wait_time_in_seconds)
-    select = Select(elem)
-    select.select_by_visible_text(text_to_select)
-
-def helper_type_in_element_by_id(driver, element_id: str, input_to_type: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
-    elem.clear()
-    elem.send_keys(input_to_type)
-
-def helper_type_in_element_by_name(driver, element_name: str, input_to_type: str, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    elem =  _wait_for_element_to_be_present_and_return_it(driver, By.NAME, element_name, wait_time_in_seconds)
-    elem.clear()
-    elem.send_keys(input_to_type)
-    
-def helper_wait_for_element_containing_specific_text(driver, expected_element_text, wait_time_in_seconds=30):
-    print("Deprecated. Please remove helper_ prefix from function name")
-    xpath_text = f"//*[contains(text(), '{expected_element_text}')]"
-    elem = _wait_for_element_to_be_present_and_return_it(driver, By.XPATH, xpath_text, wait_time_in_seconds)
+import time
+
+from selenium.webdriver.support.ui import WebDriverWait, Select
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+
+
+### Click Elements
+
+def click_element_by_css_selector(driver, css_selector: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by CSS Selector and clicks it.
+    """
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.CSS_SELECTOR, css_selector, wait_time_in_seconds)
+
+def click_element_by_id(driver, element_id: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by ID and clicks it.
+    """
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.ID, element_id, wait_time_in_seconds)
+
+def click_element_by_name(driver, element_name: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by name and clicks it.
+    """
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.NAME, element_name, wait_time_in_seconds)
+
+def click_element_by_link_text(driver, link_text, wait_time_in_seconds=30):
+    """
+    Waits for an element by (full) link text and clicks it.
+    """
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.LINK_TEXT, link_text, wait_time_in_seconds)
+
+def click_element_by_partial_link_text(driver, partial_link_text: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by partial link text and clicks it.
+    """
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.PARTIAL_LINK_TEXT, partial_link_text, wait_time_in_seconds)
+
+def click_element_by_xpath(driver, xpath: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by XPATH and clicks it.
+    """
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.XPATH, xpath, wait_time_in_seconds)
+
+
+### Checkboxes
+
+def ensure_checkbox_is_checked_by_name(driver, checkbox_name: str, wait_time_in_seconds=30):
+    """
+    Waits for a checkbox element by name and clicks it if it is not already selected.
+    """
+    checkbox = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, f"//input[@type='checkbox' and @name='{checkbox_name}']", 
+        wait_time_in_seconds)
+    
+    if checkbox.is_selected() == False:
+        checkbox.click()
+
+def ensure_checkbox_is_unchecked_by_name(driver, checkbox_name: str, wait_time_in_seconds=30):
+    """
+    Waits for a checkbox element by name and clicks it if it is already selected, to make
+    sure it is not checked.
+    """
+    checkbox = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, f"//input[@type='checkbox' and @name='{checkbox_name}']", 
+        wait_time_in_seconds)
+    
+    if checkbox.is_selected():
+        checkbox.click()
+
+
+### Element Text Matches
+
+def ensure_element_text_matches_expected_value_by_xpath(driver, element_xpath, expected_text, wait_time_in_seconds=30):
+    """
+    Waits for an element by XPATH and checks whether its text matches the expected text.
+    """
+    elem = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, element_xpath, wait_time_in_seconds)
+    return elem.text == expected_text
+
+
+### Get Element(s)
+
+def get_element_by_css_selector(driver, css_selector: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by CSS Selector and returns it.
+    """
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.CSS_SELECTOR, css_selector, wait_time_in_seconds)
+    return elem
+
+def get_element_by_id(driver, element_id, wait_time_in_seconds=30):
+    """
+    Waits for an element by ID and returns it.
+    """
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
+    return elem
+
+def get_element_by_link_text(driver, link_text, wait_time_in_seconds=30):
+    """
+    Waits for an element by (full) link text and returns it.
+    """
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.LINK_TEXT, link_text, wait_time_in_seconds)
+    return elem
+
+def get_element_by_xpath(driver, xpath: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by XPATH and returns it.
+    """
+    elem = WebDriverWait(driver, wait_time_in_seconds).until(EC.presence_of_element_located((By.XPATH, xpath)))
+    return elem
+
+def get_multiple_elements_by_class_name(driver, class_name: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by class name, then retrieves the full list of elements with that class name.
+    """
+    _wait_for_element_to_be_present_and_return_it(driver, By.CLASS_NAME, class_name, wait_time_in_seconds)
+
+    # Pause to give all elements with that class_name time to load
+    time.sleep(5)
+
+    elements_list = driver.find_elements(By.CLASS_NAME, class_name)
+
+    return elements_list
+
+
+### Select Text in Element
+
+def select_visible_text_in_element_by_id(driver, element_id: str, text_to_select: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by ID and selects it by specified text.
+    """
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
+    select = Select(elem)
+    select.select_by_visible_text(text_to_select)
+
+def select_visible_text_in_element_by_name(driver, element_name: str, text_to_select: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by name and selects it by specified text.
+    """
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.NAME, element_name, wait_time_in_seconds)
+    select = Select(elem)
+    select.select_by_visible_text(text_to_select)
+
+
+### Type in Element
+
+def type_in_element_by_id(driver, element_id: str, input_to_type: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by ID, clears it, and types in the input.
+    """
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
+    elem.clear()
+    elem.send_keys(input_to_type)
+
+def type_in_element_by_name(driver, element_name: str, input_to_type: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by name, clears it, and types in the input.
+    """
+    elem =  _wait_for_element_to_be_present_and_return_it(driver, By.NAME, element_name, wait_time_in_seconds)
+    elem.clear()
+    elem.send_keys(input_to_type)
+
+
+### Wait for Element
+    
+def wait_for_element_containing_specific_text(driver, expected_element_text, wait_time_in_seconds=30):
+    """
+    Waits for an element containing the specific text. Will crash if it does not 
+    appear in the time allotted (default = 30 seconds).
+    """
+    xpath_text = f"//*[contains(text(), '{expected_element_text}')]"
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.XPATH, xpath_text, wait_time_in_seconds)
+    return elem
+    
+
+### Internal Functions
+
+def _wait_for_element_to_be_clickable_and_return_it(driver, by_object, target_identifier, wait_time_in_seconds=30):
+    elem = WebDriverWait(driver, wait_time_in_seconds).until(EC.element_to_be_clickable((by_object, target_identifier)))
+    return elem
+
+def _wait_for_element_to_be_clickable_and_click_it(driver, by_object, target_identifier, wait_time_in_seconds=30):
+    elem = _wait_for_element_to_be_clickable_and_return_it(driver, by_object, target_identifier, wait_time_in_seconds)
+    elem.click()
+
+def _wait_for_element_to_be_present_and_return_it(driver, by_object, target_identifier, wait_time_in_seconds=30):
+    elem = WebDriverWait(driver, wait_time_in_seconds).until(EC.presence_of_element_located((by_object, target_identifier)))
+    return elem
+
+
+### Deprecated old functions, do not delete until v1.0.0
+def helper_click_element_by_css_selector(driver, css_selector: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.CSS_SELECTOR, css_selector, wait_time_in_seconds)
+
+def helper_click_element_by_id(driver, element_id: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.ID, element_id, wait_time_in_seconds)
+
+def helper_click_element_by_name(driver, element_name: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.NAME, element_name, wait_time_in_seconds)
+
+def helper_click_element_by_link_text(driver, link_text, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.LINK_TEXT, link_text, wait_time_in_seconds)
+
+def helper_click_element_by_partial_link_text(driver, partial_link_text: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.PARTIAL_LINK_TEXT, partial_link_text, wait_time_in_seconds)
+
+def helper_click_element_by_xpath(driver, xpath: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    _wait_for_element_to_be_clickable_and_click_it(driver, By.XPATH, xpath, wait_time_in_seconds)
+    
+def helper_ensure_checkbox_is_checked_by_name(driver, checkbox_name: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    checkbox = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, f"//input[@type='checkbox' and @name='{checkbox_name}']", 
+        wait_time_in_seconds)
+    
+    if checkbox.is_selected() == False:
+        checkbox.click()
+
+def helper_ensure_checkbox_is_unchecked_by_name(driver, checkbox_name: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    checkbox = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, f"//input[@type='checkbox' and @name='{checkbox_name}']", 
+        wait_time_in_seconds)
+    
+    if checkbox.is_selected():
+        checkbox.click()
+
+def helper_ensure_element_text_matches_expected_value_by_xpath(driver, element_xpath, expected_text, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    elem = _wait_for_element_to_be_clickable_and_return_it(driver, By.XPATH, element_xpath, wait_time_in_seconds)
+    return elem.text == expected_text
+
+def helper_get_element_by_css_selector(driver, css_selector: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.CSS_SELECTOR, css_selector, wait_time_in_seconds)
+    return elem
+
+def helper_get_element_by_id(driver, element_id, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
+    return elem
+
+def helper_get_element_by_link_text(driver, link_text, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.LINK_TEXT, link_text, wait_time_in_seconds)
+    return elem
+
+def helper_get_element_by_xpath(driver, xpath: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    elem = WebDriverWait(driver, wait_time_in_seconds).until(EC.presence_of_element_located((By.XPATH, xpath)))
+    return elem
+
+def helper_get_multiple_elements_by_class_name(driver, class_name: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    _wait_for_element_to_be_present_and_return_it(driver, By.CLASS_NAME, class_name, wait_time_in_seconds)
+
+    # Pause to give all elements with that class_name time to load
+    time.sleep(5)
+
+    elements_list = driver.find_elements(By.CLASS_NAME, class_name)
+
+    return elements_list
+
+def helper_select_visible_text_in_element_by_id(driver, element_id: str, text_to_select: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
+    select = Select(elem)
+    select.select_by_visible_text(text_to_select)
+
+def helper_select_visible_text_in_element_by_name(driver, element_name: str, text_to_select: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.NAME, element_name, wait_time_in_seconds)
+    select = Select(elem)
+    select.select_by_visible_text(text_to_select)
+
+def helper_type_in_element_by_id(driver, element_id: str, input_to_type: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.ID, element_id, wait_time_in_seconds)
+    elem.clear()
+    elem.send_keys(input_to_type)
+
+def helper_type_in_element_by_name(driver, element_name: str, input_to_type: str, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    elem =  _wait_for_element_to_be_present_and_return_it(driver, By.NAME, element_name, wait_time_in_seconds)
+    elem.clear()
+    elem.send_keys(input_to_type)
+    
+def helper_wait_for_element_containing_specific_text(driver, expected_element_text, wait_time_in_seconds=30):
+    print("Deprecated. Please remove helper_ prefix from function name")
+    xpath_text = f"//*[contains(text(), '{expected_element_text}')]"
+    elem = _wait_for_element_to_be_present_and_return_it(driver, By.XPATH, xpath_text, wait_time_in_seconds)
     return elem
```

### Comparing `spswarehouse-0.6.1/spswarehouse/googledrive.py` & `spswarehouse-0.6.2/spswarehouse/googlesheets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,64 @@
-import os
-import pickle
-
-try:
-    from .credentials import google_config
-except ModuleNotFoundError:
-    print("No credentials file found in spswarehouse. This could cause issues.")
-
-from pydrive2.auth import GoogleAuth
-from pydrive2.drive import GoogleDrive
-
-from oauth2client.service_account import ServiceAccountCredentials
-
-def get_google_service_account_email():
-    """
-    Returns the service account email to share Drive files with.
-    """
-    return google_config['service-account']['client_email']
-
-def initialize_credentials():
-    """
-    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
-
-    Returns credentials that allows you to access your Google Drive &
-    Sheets using the Google Sheets API.
-
-    You still need to share spreadsheets with the service account email.
-    """
-
-    # This prevents us from erroring out trying to construct credentials
-    # from incomplete information.
-    service_account = google_config.get('service-account', {})
-    private_key = service_account.get('private_key', None)
-    if not private_key:
-        print(
-            "You're missing Google service account credentials",
-            "in credentials.py.",
-            "To access your Google Drive data,",
-            "fill out the Google service account information."
-        )
-        return None
-
-    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
-        google_config['service-account'],
-        scopes=google_config['scopes'],
-    )
-    print(
-        'To access your Google Drive file, share the file with {email}'
-        .format(email=get_google_service_account_email())
-    )
-    return credentials
-
-def create_client(credentials):
-    """
-    create_engine:
-
-    Sets up Google Drive API access using credentials (see above).
-    """
-    gauth = GoogleAuth()
-    gauth.credentials = credentials
-    drive = GoogleDrive(gauth)
-    return drive
-
-# Set up credentials
-credentials = initialize_credentials()
-
-# This is a wrapper for pydrive.GoogleDrive
-GoogleDrive = None if credentials is None else create_client(credentials)
+import gspread
+import os
+import pickle
+
+try:
+    from .credentials import google_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
+
+from oauth2client.service_account import ServiceAccountCredentials
+
+def get_google_service_account_email():
+    """
+    Returns the service account email to share spreadsheets with.
+    """
+    return google_config['service-account']['client_email']
+
+def initialize_credentials():
+    """
+    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
+
+    Returns credentials that allows you to access your Google Drive &
+    Sheets using the Google Sheets API.
+
+    You still need to share spreadsheets with the service account email.
+    """
+
+    # This prevents us from erroring out trying to construct credentials
+    # from incomplete information.
+    service_account = google_config.get('service-account', {})
+    private_key = service_account.get('private_key', None)
+    if not private_key:
+        print(
+            "You're missing Google service account credentials",
+            "in credentials.py.",
+            "To access your Google spreadsheet data,",
+            "fill out the Google service account information."
+        )
+        return None
+
+    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
+        google_config['service-account'],
+        scopes=google_config['scopes'],
+    )
+    print(
+        'To access your Google files, share the file with {email}'
+        .format(email=get_google_service_account_email())
+    )
+    return credentials
+
+def create_client(credentials):
+    """
+    create_engine:
+
+    Sets up Google Sheets API access using credentials (see above).
+    """
+    client = gspread.authorize(credentials)
+    return client
+
+# Set up credentials
+credentials = initialize_credentials()
+
+# This is a wrapper for gspread.Client
+GoogleSheets = None if credentials is None else create_client(credentials)
```

### Comparing `spswarehouse-0.6.1/spswarehouse/googlesheets.py` & `spswarehouse-0.6.2/spswarehouse/googleslides.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,65 @@
-import gspread
-import os
-import pickle
-
-try:
-    from .credentials import google_config
-except ModuleNotFoundError:
-    print("No credentials file found in spswarehouse. This could cause issues.")
-
-from oauth2client.service_account import ServiceAccountCredentials
-
-def get_google_service_account_email():
-    """
-    Returns the service account email to share spreadsheets with.
-    """
-    return google_config['service-account']['client_email']
-
-def initialize_credentials():
-    """
-    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
-
-    Returns credentials that allows you to access your Google Drive &
-    Sheets using the Google Sheets API.
-
-    You still need to share spreadsheets with the service account email.
-    """
-
-    # This prevents us from erroring out trying to construct credentials
-    # from incomplete information.
-    service_account = google_config.get('service-account', {})
-    private_key = service_account.get('private_key', None)
-    if not private_key:
-        print(
-            "You're missing Google service account credentials",
-            "in credentials.py.",
-            "To access your Google spreadsheet data,",
-            "fill out the Google service account information."
-        )
-        return None
-
-    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
-        google_config['service-account'],
-        scopes=google_config['scopes'],
-    )
-    print(
-        'To access your Google files, share the file with {email}'
-        .format(email=get_google_service_account_email())
-    )
-    return credentials
-
-def create_client(credentials):
-    """
-    create_engine:
-
-    Sets up Google Sheets API access using credentials (see above).
-    """
-    client = gspread.authorize(credentials)
-    return client
-
-# Set up credentials
-credentials = initialize_credentials()
-
-# This is a wrapper for gspread.Client
-GoogleSheets = None if credentials is None else create_client(credentials)
+import os
+import pickle
+
+try:
+    from .credentials import google_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
+
+from googleapiclient.discovery import build
+
+from oauth2client.service_account import ServiceAccountCredentials
+
+def get_google_service_account_email():
+    """
+    Returns the service account email to share slides with.
+    """
+    return google_config['service-account']['client_email']
+
+def initialize_credentials():
+    """
+    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
+
+    Returns credentials that allows you to access your Google Slides
+    using the Google Sheets API.
+
+    You still need to share slides with the service account email.
+    """
+
+    # This prevents us from erroring out trying to construct credentials
+    # from incomplete information.
+    service_account = google_config.get('service-account', {})
+    private_key = service_account.get('private_key', None)
+    if not private_key:
+        print(
+            "You're missing Google service account credentials",
+            "in credentials.py.",
+            "To access your Google Slides,",
+            "fill out the Google service account information."
+        )
+        return None
+
+    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
+        google_config['service-account'],
+        scopes=google_config['scopes'],
+    )
+    print(
+        'To access your Google Slides, share the file with {email}'
+        .format(email=get_google_service_account_email())
+    )
+    return credentials
+
+def create_client(credentials):
+    """
+    create_engine:
+
+    Sets up Google Drive API access using credentials (see above).
+    """
+    slides = build('slides', 'v1', credentials=credentials)
+    return slides
+
+# Set up credentials
+credentials = initialize_credentials()
+
+# This is a wrapper for a standard Google Slides engine
+GoogleSlides = None if credentials is None else create_client(credentials)
```

### Comparing `spswarehouse-0.6.1/spswarehouse/googleslides.py` & `spswarehouse-0.6.2/spswarehouse/googledrive.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,70 @@
-import os
-import pickle
-
-try:
-    from .credentials import google_config
-except ModuleNotFoundError:
-    print("No credentials file found in spswarehouse. This could cause issues.")
-
-from googleapiclient.discovery import build
-
-from oauth2client.service_account import ServiceAccountCredentials
-
-def get_google_service_account_email():
-    """
-    Returns the service account email to share slides with.
-    """
-    return google_config['service-account']['client_email']
-
-def initialize_credentials():
-    """
-    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
-
-    Returns credentials that allows you to access your Google Slides
-    using the Google Sheets API.
-
-    You still need to share slides with the service account email.
-    """
-
-    # This prevents us from erroring out trying to construct credentials
-    # from incomplete information.
-    service_account = google_config.get('service-account', {})
-    private_key = service_account.get('private_key', None)
-    if not private_key:
-        print(
-            "You're missing Google service account credentials",
-            "in credentials.py.",
-            "To access your Google Slides,",
-            "fill out the Google service account information."
-        )
-        return None
-
-    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
-        google_config['service-account'],
-        scopes=google_config['scopes'],
-    )
-    print(
-        'To access your Google Slides, share the file with {email}'
-        .format(email=get_google_service_account_email())
-    )
-    return credentials
-
-def create_client(credentials):
-    """
-    create_engine:
-
-    Sets up Google Drive API access using credentials (see above).
-    """
-    slides = build('slides', 'v1', credentials=credentials)
-    return slides
-
-# Set up credentials
-credentials = initialize_credentials()
-
-# This is a wrapper for a standard Google Slides engine
-GoogleSlides = None if credentials is None else create_client(credentials)
+import os
+import pickle
+
+try:
+    from .credentials import google_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
+
+from pydrive2.auth import GoogleAuth
+from pydrive2.drive import GoogleDrive
+
+from oauth2client.service_account import ServiceAccountCredentials
+
+def get_google_service_account_email():
+    """
+    Returns the service account email to share Drive files with.
+    """
+    return google_config['service-account']['client_email']
+
+def initialize_auth():
+    """
+    initialize_auth: -> pydrive2.auth.GoogleAuth
+
+    Returns an Auth object that allows you to access your Google Drive &
+    Sheets using the Google Drive API.
+
+    You still need to share files with the service account email.
+
+    Note: we use a GoogleAuth object rather than just passing a credentials
+    file so that pydrive can create refresh tokens if necessary. This only
+    is an issue when you want run a notebook for longer than an hour, but it
+    does come up.
+    """
+    # This prevents us from erroring out trying to construct credentials
+    # from incomplete information.
+    service_account = google_config.get('service-account', {})
+    private_key = service_account.get('private_key', None)
+    if not private_key:
+        print(
+            "You're missing Google service account credentials",
+            "in credentials.py.",
+            "To access your Google Drive data,",
+            "fill out the Google service account information."
+        )
+        return None
+
+    gauth = GoogleAuth()
+    gauth.client_config["client_user_email"] = get_google_service_account_email()
+    gauth.client_config["client_json_dict"] = service_account
+    gauth.settings["oauth_scope"] = google_config['scopes']
+    gauth.ServiceAuth()
+    print(
+        'To access your Google Drive file, share the file with {email}'
+        .format(email=gauth.client_config["client_user_email"])
+    )
+    return gauth
+
+def create_client(gauth):
+    """
+    create_engine:
+
+    Sets up Google Drive API access using an Auth object (see above).
+    """
+    return GoogleDrive(gauth)
+
+# Set up credentials
+gauth = initialize_auth()
+
+# This is a wrapper for pydrive.GoogleDrive
+GoogleDrive = None if gauth is None else create_client(gauth)
```

### Comparing `spswarehouse-0.6.1/spswarehouse/magic_spreadsheet.py` & `spswarehouse-0.6.2/spswarehouse/magic_spreadsheet.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,672 +1,672 @@
-import pandas as pd
-import logging
-
-from .warehouse import create_warehouse
-from .googlesheets import create_sheets
-from .googledrive import create_drive
-
-from gspread_formatting import (
-    set_data_validation_for_cell_range,
-    BooleanCondition,
-    BooleanRule,
-    CellFormat,
-    ConditionalFormatRule,
-    get_conditional_format_rules,
-    GridRange,
-    textFormat,
-    format_cell_range,
-    color,
-)
-
-"""
-This module defines a number of functions to create and manage 
-"Magic Spreadsheets" - Google Sheets that automatically update based on
-the results of a SQL query run against the warehouse.
-
-Magic Spreadsheets are more sophisticated than a simple export in that they 
-preserve existing columns, so they support users of the sheet adding notes
-and other columns that will maintain their associations even as students
-are added/removed from the sheet.
-
-We use this in production in the SY24 "Main Enrollment Forms Tracker" (MEFT)
-and the SY24 Child Find tool.
-
-Typical sequence of calls:
-    * Create or fetch the spreadsheets: `spreadsheet_object, spreadsheet_already_exists = create_or_retrieve_magic_spreadsheet_and_add_missing_worksheets(...)`
-    * Add the static worksheets: `check_for_static_worksheets_and_add_them_with_protection(...)`
-    * Update the spreadsheet with query results: `update_magic_spreadsheet_with_new_query_results(...)`
-    * If desired, update specific cells (like the "Last Updated" field): `update_specific_cell(...)`
-"""
-
-def _run_warehouse_query_for_worksheet(query_list: list):
-    """
-    Take a list of queries stored as dictionaries. Run each query at the provided
-    path with the provided parameters. Take the output of all queries in the list,
-    combine them, remove NAs, and return the resulting combined dataframe.
-    """
-    df_combined_query_output = None
-
-    for query_dict in query_list:
-        query_path = query_dict['path']
-        query_parameters = query_dict['parameters']
-
-        with open(query_path, "r") as f:
-            if query_parameters == {}:
-                warehouse_query = f.read()
-            else:
-                warehouse_query = f.read().format(**query_parameters)
-
-        Warehouse = create_warehouse()
-
-        # Raise logging level to limit warehouse output to logs
-        logger = logging.getLogger()
-        logger.setLevel(logging.WARNING)
-
-        df_query_output = Warehouse.read_sql(warehouse_query)
-
-         # Reset logging level
-        logger.setLevel(logging.INFO)
-
-        if df_combined_query_output is None:
-            df_combined_query_output = df_query_output
-        else:
-            df_combined_query_output = pd.concat([df_combined_query_output, df_query_output], axis=0)
-        
-    df_combined_query_output.fillna('', inplace=True)
-
-    return df_combined_query_output
-
-def _add_formulas_to_worksheet(worksheet_object, formulas_list):
-    """
-    Given a list of formulas in the format below, add the formula to the specified row of the
-    column, then copy it down the entire column.
-    """
-    
-    for formula in formulas_list:
-        formula_column = formula['column']
-        formula_row_start = formula['row_of_first_formula_cell']
-        formula_text = formula['formula_text']
-        
-        # First, add the formula to the specified row of the given column
-        source_cell = f'{formula_column}{formula_row_start}'
-        worksheet_object.update(source_cell, formula_text, value_input_option='USER_ENTERED')
-        
-        # Then, copy that formula down the whole column
-        destination_range = f'{formula_column}{formula_row_start}:{formula_column}'
-        
-        worksheet_object.copy_range(source_cell, destination_range, paste_type='PASTE_FORMULA')
-
-def _add_data_validations_to_worksheet(worksheet_object, data_validations_list):
-    """
-    Given a list of data validations in the format below, clears any existing rules in
-    the provided range and adds each rule from the list to the worksheet object. This
-    function assumes one validation rule for any given range; otherwise, later rules 
-    in the list would overwrite earlier ones.
-    
-    List format:
-        [
-            {
-                'range': 'P4:P',
-                'validation_rule' : DataValidationRule(
-                    BooleanCondition('ONE_OF_LIST', ['True', 'False']),
-                    showCustomUi=True
-                )
-            },
-        ]
-    """
-    for data_validation in data_validations_list:
-        validation_range = data_validation['range']
-        validation_rule = data_validation['validation_rule']
-        
-        # Clear any existing validation rules in the range
-        set_data_validation_for_cell_range(worksheet_object, validation_range, None)
-    
-        # Add validation rule from list to the range
-        set_data_validation_for_cell_range(worksheet_object, validation_range, validation_rule)
-
-def _hide_header_rows_and_left_columns_in_worksheet(worksheet_object, num_header_rows_to_hide, num_left_columns_to_hide):
-
-    worksheet_object.hide_rows(0, num_header_rows_to_hide)
-    worksheet_object.hide_columns(0, num_left_columns_to_hide)
-
-def _set_basic_filter_on_worksheet(worksheet_object, row_number_for_filter, final_row_number):
-    num_columns = worksheet_object.col_count
-    final_col_letter = col_to_letter(num_columns)
-
-    worksheet_object.set_basic_filter(f'A{row_number_for_filter}:{final_col_letter}{final_row_number}')
-
-def _refresh_conditional_formatting_on_worksheet(worksheet_object, num_header_rows: int,
-    conditional_formatting_rules_dict: dict, colors_dict: dict):
-
-    # logging.info("Store the current conditional formatting rules.")
-    rules = get_conditional_format_rules(worksheet_object)
-    
-    # logging.info("Delete all the existing rules.")
-    rules.clear()
-
-    # logging.info("Iterating through conditional formatting rules.")
-    for color in conditional_formatting_rules_dict.keys():
-        for new_rule in conditional_formatting_rules_dict[color]:
-            new_rule_starts_with_text = new_rule[0]
-            new_rule_start_column = new_rule[1]
-            new_rule_end_column = new_rule[2]
-
-            color_object = colors_dict[color]
-
-            new_rule_range = f'{new_rule_start_column}{num_header_rows+1}:{new_rule_end_column}'
-
-            new_condition = ConditionalFormatRule(
-                ranges=[GridRange.from_a1_range(new_rule_range, worksheet_object)],
-                booleanRule=BooleanRule(
-                    condition=BooleanCondition("TEXT_STARTS_WITH", [new_rule_starts_with_text]),
-                    format=CellFormat(
-                        textFormat=textFormat(
-                            foregroundColor=color_object
-                        )
-                    )
-                )
-            )
-
-            # logging.info(f'Appending rule to rules list: text starting with "{new_rule_starts_with_text}" in column {new_rule_start_column} through column {new_rule_end_column} is {color}.')
-            rules.append(new_condition)
-
-    # logging.info("Posting the new rules back to the worksheet.")
-    rules.save()
-
-    # logging.info("Conditional formatting updated.")
-
-def create_or_retrieve_magic_spreadsheet_and_add_missing_worksheets(drive_folder_id: str,
-    spreadsheet_name: str, template_spreadsheet_id: str, worksheet_name_list):
-
-    gs = create_sheets()
-
-    spreadsheet_already_exists, spreadsheet_object = _check_if_spreadsheet_exists_and_retrieve_it(
-        drive_folder_id=drive_folder_id,
-        spreadsheet_name=spreadsheet_name,
-        gs = gs,
-    )
-
-    if spreadsheet_already_exists == False:
-        spreadsheet_object = _create_spreadsheet_from_template(
-            output_spreadsheet_name = spreadsheet_name, 
-            output_folder_id = drive_folder_id, 
-            template_spreadsheet_id = template_spreadsheet_id, 
-            worksheet_name_list = worksheet_name_list,
-            gs = gs,
-            )
-    else:
-        template_spreadsheet_object = gs.open_by_key(template_spreadsheet_id)
-
-        _check_for_missing_worksheets_and_create_them(target_spreadsheet_object = spreadsheet_object, 
-            template_spreadsheet_object = template_spreadsheet_object, 
-            worksheet_name_list = worksheet_name_list)
-        
-    return spreadsheet_object, spreadsheet_already_exists
-
-def _check_if_spreadsheet_exists_and_retrieve_it(drive_folder_id: str, spreadsheet_name: str, gs):
-    
-    google_drive = create_drive()
-
-    folder_files = google_drive.ListFile({'q': f"'{drive_folder_id}' in parents"}).GetList()
-
-    spreadsheet_already_exists = False
-
-    # Get spreadsheet if it exists
-    for file in folder_files:
-        if file['title'] == spreadsheet_name:
-            spreadsheet_already_exists = True
-            current_spreadsheet = gs.open_by_key(file['id'])
-
-    if spreadsheet_already_exists == True:
-        return spreadsheet_already_exists, current_spreadsheet
-    else:
-        return spreadsheet_already_exists, None
-
-def _create_worksheet_from_template_if_does_not_exist(target_spreadsheet_object, template_spreadsheet_object, worksheet_name):
-
-    new_worksheet_created = False
-
-    # Get the list of worksheet titles in the target spreadsheet
-    worksheet_list = target_spreadsheet_object.worksheets()
-
-    # Check if a specific worksheet exists
-    worksheet_exists = any(worksheet.title == worksheet_name for worksheet in worksheet_list)
-
-    if worksheet_exists == False:
-        # Get worksheet in template
-        template_worksheet = template_spreadsheet_object.worksheet(worksheet_name)
-        
-        # Copy worksheet to the target spreadsheet
-        target_worksheet_info_dict = template_worksheet.copy_to(target_spreadsheet_object.id)
-        target_worksheet_object = target_spreadsheet_object.worksheet(target_worksheet_info_dict['title'])
-        
-        # Rename worksheet at destination to remove 'Copy of'
-        target_worksheet_object.update_title(worksheet_name)
-
-        new_worksheet_created = True
-       
-    return new_worksheet_created
-
-def _check_for_missing_worksheets_and_create_them(target_spreadsheet_object, template_spreadsheet_object, worksheet_name_list):
-    for worksheet_name in worksheet_name_list:
-        _create_worksheet_from_template_if_does_not_exist(target_spreadsheet_object = target_spreadsheet_object, 
-            template_spreadsheet_object = template_spreadsheet_object, worksheet_name = worksheet_name)
-
-def _create_spreadsheet_from_template(output_spreadsheet_name: str, output_folder_id: str, 
-    template_spreadsheet_id: str, worksheet_name_list: list, gs):
-    
-    # Create spreadsheet
-    spreadsheet = gs.create(output_spreadsheet_name, folder_id=output_folder_id)
-    
-    # Get the template
-    template_spreadsheet = gs.open_by_key(template_spreadsheet_id)
-    
-    # Copy tabs from template to the spreadsheet
-    _check_for_missing_worksheets_and_create_them(target_spreadsheet_object = spreadsheet, 
-        template_spreadsheet_object = template_spreadsheet, 
-        worksheet_name_list = worksheet_name_list)
-
-    # Delete the default sheet
-    default_worksheet_to_delete = spreadsheet.worksheet("Sheet1")
-    spreadsheet.del_worksheet(default_worksheet_to_delete)
-    
-    return spreadsheet
-
-def update_magic_spreadsheet_with_new_query_results(spreadsheet_object, worksheet_information_dict: dict, 
-        school_information_dict: dict, other_query_parameters_dict: dict, primary_identifier: str,
-        secondary_optional_identifier: str = '', colors_dict: dict = {}, worksheet_order_name_list = [], 
-        general_editor_list = [],
-        # Optional Parameters: Getting Data From Different Source
-        # get_data_from_different_source: bool = False, 
-        **kwargs,
-        # different_source_worksheet_object = None, 
-        # different_source_number_of_header_rows = None, different_source_num_columns_on_left_not_to_keep = None,
-        # different_source_columns_to_rename = [],
-    ):
-
-    # Update all worksheets with fresh query results
-    for worksheet_name in worksheet_information_dict.keys():
-        logging.info('='*75)
-        logging.info(f'Begin updating "{worksheet_name}" worksheet.')
-
-        worksheet_to_update = spreadsheet_object.worksheet(worksheet_name)
-        _update_magic_spreadsheet_worksheet_with_new_query_results(
-            worksheet_object = worksheet_to_update,
-            single_worksheet_information_dict = worksheet_information_dict[worksheet_name],
-            query_parameters_dict = {**school_information_dict, **other_query_parameters_dict},
-            colors_dict = colors_dict,
-            primary_identifier = primary_identifier,
-            secondary_optional_identifier = secondary_optional_identifier,
-            # get_data_from_different_source = get_data_from_different_source, 
-            **kwargs,
-            # different_source_worksheet_object = different_source_worksheet_object, 
-            # different_source_number_of_header_rows = different_source_number_of_header_rows, 
-            # different_source_num_columns_on_left_not_to_keep = different_source_num_columns_on_left_not_to_keep,
-            # different_source_columns_to_rename = different_source_columns_to_rename,
-        )
-
-        logging.info(f'Done updating "{worksheet_name}" worksheet.')
-        
-    # Reorder worksheets
-    if len(worksheet_order_name_list) > 0:
-        _reorder_worksheets(spreadsheet_object, worksheet_order_name_list)
-        
-    # Re-confirm spreadsheet is shared with all general editors and all school editors
-    spreadsheet_editor_list = school_information_dict['spreadsheet_editors']
-    full_editor_list = general_editor_list + spreadsheet_editor_list
-
-    for editor in full_editor_list:
-        spreadsheet_object.share(editor, perm_type='user', role='writer', notify=False)
-
-def col_to_letter(column_int):
-    """
-    Adapted from: https://stackoverflow.com/a/23862195
-    """
-    start_index = 1   #  it can start either at 0 or at 1
-    letter = ''
-    while column_int > 25 + start_index:   
-        letter += chr(65 + int((column_int-start_index)/26) - 1)
-        column_int = column_int - (int((column_int-start_index)/26))*26
-    letter += chr(65 - start_index + (int(column_int)))
-
-    return letter
-
-def check_for_static_worksheets_and_add_them_with_protection(target_spreadsheet_object, 
-    template_spreadsheet_id, static_worksheets_list, primary_editor_email = '', 
-    info_team_group_email = '', other_individual_editors_list=[]):
-
-    gs = create_sheets()
-
-    template_spreadsheet_object = gs.open_by_key(template_spreadsheet_id)
-
-    for static_worksheet in static_worksheets_list:
-        static_worksheet_name = static_worksheet['worksheet_name']
-        _create_worksheet_from_template_if_does_not_exist(target_spreadsheet_object, template_spreadsheet_object, static_worksheet_name)
-
-        if static_worksheet['protected'] == True:
-            static_worksheet_object = target_spreadsheet_object.worksheet(static_worksheet_name)
-            protected_range_list = target_spreadsheet_object.list_protected_ranges(static_worksheet_object.id)
-
-            target_description = f'"{static_worksheet_name}" Sheet-wide Protection'
-
-            if any(protected_range["description"] == target_description for protected_range in protected_range_list):
-                logging.info('Protected range already exists.')
-            else:
-                logging.info('Protect range not found. Creating new one.')
-
-                individual_editors = [primary_editor_email] + other_individual_editors_list
-
-                num_worksheet_columns = static_worksheet_object.col_count
-                final_column_letter = col_to_letter(num_worksheet_columns)
-
-                static_worksheet_object.add_protected_range(name=f'A:{final_column_letter}', 
-                    editor_users_emails = individual_editors, 
-                    editor_groups_emails=[info_team_group_email], 
-                    description = target_description
-                )
-
-def update_specific_cell(spreadsheet_object, worksheet_name, cell_a1_notation, text_string):
-    worksheet = spreadsheet_object.worksheet(worksheet_name)
-    cell = worksheet.acell(cell_a1_notation)
-    cell.value = text_string
-    worksheet.update_cell(cell.row, cell.col, cell.value)
-
-def _apply_worksheet_formatting(worksheet_object, single_worksheet_information_dict: dict, number_of_header_rows: int, 
-    updated_worksheet_row_count: int, colors_dict: dict):
-    # Add any validation rules to the worksheet
-    if 'data_validations' in single_worksheet_information_dict:
-        logging.info('Add the data validations to the worksheet.')
-        data_validations_list = single_worksheet_information_dict['data_validations']
-        _add_data_validations_to_worksheet(worksheet_object, data_validations_list)
-    
-    # Re-add any formulas to the worksheet, since they would have been overwritten by hard-coded existing data
-    if 'formulas' in single_worksheet_information_dict:
-        logging.info('Add the formulas to the worksheet.')
-        formulas_list = single_worksheet_information_dict['formulas']
-        _add_formulas_to_worksheet(worksheet_object, formulas_list)
-
-    # Hide rows and columns as specified
-    if ('num_header_rows_to_hide' in single_worksheet_information_dict or 'num_left_columns_to_hide' in single_worksheet_information_dict):
-        logging.info('Hide the specified rows and columns.')
-        _hide_header_rows_and_left_columns_in_worksheet(
-            worksheet_object = worksheet_object, 
-            num_header_rows_to_hide = single_worksheet_information_dict['num_header_rows_to_hide'] if 'num_header_rows_to_hide' in single_worksheet_information_dict else 0,
-            num_left_columns_to_hide = single_worksheet_information_dict['num_left_columns_to_hide'] if 'num_left_columns_to_hide' in single_worksheet_information_dict else 0
-        )
-
-    # Set basic filter
-    if 'filter_on_final_header_row' in single_worksheet_information_dict and single_worksheet_information_dict['filter_on_final_header_row'] == True:
-        logging.info('Set the filter on the worksheet.')
-        _set_basic_filter_on_worksheet(
-            worksheet_object = worksheet_object, 
-            row_number_for_filter = number_of_header_rows, 
-            final_row_number = updated_worksheet_row_count
-        )
-
-    # Refresh conditional formatting
-    if 'conditional_formatting_rules' in single_worksheet_information_dict:
-        logging.info('Refresh the conditional formatting on the worksheet.')
-        _refresh_conditional_formatting_on_worksheet(
-            worksheet_object = worksheet_object,
-            num_header_rows = number_of_header_rows,
-            conditional_formatting_rules_dict = single_worksheet_information_dict['conditional_formatting_rules'],
-            colors_dict = colors_dict,
-        )
-
-    # Get the last column of the query
-    query_column_end = col_to_letter(single_worksheet_information_dict['warehouse_query_number_of_columns'])
-
-    # Update background color for query data to light gray
-    background_color_row_start = number_of_header_rows + 1
-
-    background_color_range = f'A{background_color_row_start}:{query_column_end}'
-
-    background_color_format = CellFormat(
-        backgroundColor = color(245/255, 245/255, 245/255), # Light Gray
-        )
-
-    logging.info('Format the warehouse data cells with the background color.')
-    format_cell_range(worksheet_object, background_color_range, background_color_format)
-
-    # Set cell dividing line on right side of query data
-    query_data_border_range = f'{query_column_end}:{query_column_end}'
-    borders_format = CellFormat(
-        borders = {
-            'right' : 
-                {
-                    "style": 'SOLID',
-                    "width": 1,
-                    "color": {
-                        "red": 0,
-                        "green": 0,
-                        "blue": 0,
-                        "alpha": 1
-                        }, # Black
-                }
-            
-        }
-    )
-
-    logging.info('Set the cell dividing line on the right side of the warehouse data cells.')
-    format_cell_range(worksheet_object, query_data_border_range, borders_format)
-
-def _reorder_worksheets(spreadsheet_object, worksheet_order_name_list):
-    worksheet_objects_in_desired_order = []
-
-    for worksheet_name in worksheet_order_name_list:
-        worksheet = spreadsheet_object.worksheet(worksheet_name)
-        worksheet_objects_in_desired_order.append(worksheet)
-
-    spreadsheet_object.reorder_worksheets(worksheet_objects_in_desired_order)
-
-def _get_all_manual_values_from_existing_worksheet(data_source_worksheet_object, data_source_number_of_header_rows,
-    primary_identifier, secondary_optional_identifier, num_columns_on_left_not_to_keep, source_columns_to_rename = []):
-
-    # Clear the filter on the worksheet
-    data_source_worksheet_object.clear_basic_filter()
-
-    ### Get all data from existing tab
-    all_values = data_source_worksheet_object.get_all_values()
-
-    # Turn all_values into a dataframe
-    # These values are 0-based but number_of_header_rows is 1-based
-    df_all_values = pd.DataFrame(all_values[data_source_number_of_header_rows:], columns=all_values[data_source_number_of_header_rows-1])
-
-    # Rename columns in the different source if needed
-    for column_tuple in source_columns_to_rename:
-        original_column_name = column_tuple[0]
-        new_column_name = column_tuple[1]
-
-        if original_column_name in df_all_values.columns:
-            # Rename the column
-            df_all_values = df_all_values.rename(columns={original_column_name: new_column_name})
-
-    # Keep only the columns from the spreadsheet that are not getting updated by the query + the identifiers
-    # Assume that all worksheets need a primary_identifier column; they may or may not have an secondary_optional_identifier column
-    identifier_columns_to_keep = [primary_identifier]
-
-    secondary_optional_identifier_used_on_sheet = (secondary_optional_identifier in df_all_values.columns)
-
-    if secondary_optional_identifier_used_on_sheet == True:
-        identifier_columns_to_keep.append(secondary_optional_identifier)
-
-    spreadsheet_keep_columns = identifier_columns_to_keep + list(df_all_values.columns[(num_columns_on_left_not_to_keep):])
-    df_spreadsheet_values_to_keep = df_all_values[spreadsheet_keep_columns]
-
-    return df_spreadsheet_values_to_keep, secondary_optional_identifier_used_on_sheet
-
-def _update_magic_spreadsheet_worksheet_with_new_query_results(worksheet_object, single_worksheet_information_dict: dict,
-        query_parameters_dict: dict, colors_dict: dict, primary_identifier: str,
-        # Optional Parameters: Secondary Identifier
-        secondary_optional_identifier: str = '', 
-        # Optional Parameters: Getting Data from Different Source
-        **kwargs
-    ):
-
-    # Add query to query_list and run query
-    # TODO: Do we ever need to run multiple queries in one sheet? If not, refactor to run a single query
-
-    query_list = [{
-        'path' : single_worksheet_information_dict['warehouse_query_path'],
-        'parameters' : query_parameters_dict,
-    }]
-
-    logging.info('Run worksheet query in data warehouse.')
-    df_query_output = _run_warehouse_query_for_worksheet(query_list)
-
-    # Load key metadata
-
-    number_of_header_rows = single_worksheet_information_dict['number_of_header_rows']
-    num_columns_in_query = single_worksheet_information_dict['warehouse_query_number_of_columns']
-    
-    ### Get all data from existing tab
-    gs = create_sheets()
-
-    # Check if parameters passed to get data from a different source
-    if 'get_data_from_different_source' in kwargs and kwargs['get_data_from_different_source'] == True:
-        # Atypical path: Loading data from a different worksheet than will be writing to
-        logging.info('Load data from specified external worksheet.')
-        different_source_spreadsheet_object = gs.open_by_key(kwargs['different_source_spreadsheet_id'])
-        different_source_worksheet_object = different_source_spreadsheet_object.worksheet(kwargs['different_source_worksheet_name'])
-
-        df_spreadsheet_values_to_keep, secondary_optional_identifier_used_on_sheet = _get_all_manual_values_from_existing_worksheet(
-            data_source_worksheet_object = different_source_worksheet_object, 
-            data_source_number_of_header_rows = kwargs['different_source_number_of_header_rows'],
-            primary_identifier = primary_identifier, 
-            secondary_optional_identifier = secondary_optional_identifier, 
-            num_columns_on_left_not_to_keep = kwargs['different_source_num_columns_on_left_not_to_keep'],
-            source_columns_to_rename = kwargs['different_source_columns_to_rename'],
-        )
-    else:
-        # Standard path: loading data from same worksheet will be writing to
-        logging.info('Load data from existing worksheet.')
-        df_spreadsheet_values_to_keep, secondary_optional_identifier_used_on_sheet = _get_all_manual_values_from_existing_worksheet(
-            data_source_worksheet_object = worksheet_object, 
-            data_source_number_of_header_rows = number_of_header_rows,
-            primary_identifier = primary_identifier, 
-            secondary_optional_identifier = secondary_optional_identifier, 
-            num_columns_on_left_not_to_keep = num_columns_in_query
-        )
-        
-    logging.info('Connect user data from existing worksheet to new query output.')
-    # Blank out the 'Not Assigned Yet' values in the primary_identifier column of the spreadsheet dataframe to avoid an incorrect join
-    df_spreadsheet_values_to_keep[primary_identifier] = df_spreadsheet_values_to_keep[primary_identifier].apply(lambda x: '' if x == 'Not Assigned Yet' else x)
-        
-    ### Connect data from existing tab to query output in a new dataframe
-
-    # Attempt a match on primary_identifier first
-    df_matched_based_on_primary_identifier = df_query_output.merge(df_spreadsheet_values_to_keep, on=primary_identifier, how='left', indicator='primary_identifier_match')
-
-    # Drop duplicate secondary_optional_identifier column
-    df_matched_based_on_primary_identifier = df_matched_based_on_primary_identifier.rename(columns={f'{secondary_optional_identifier}_x': secondary_optional_identifier}).drop(f'{secondary_optional_identifier}_y', axis=1)
-
-    # logging.info('Post primary_identifier_match:', df_matched_based_on_primary_identifier.columns)
-
-    # Create a dataframe of successful matches on primary_identifier
-    df_only_primary_identifier_matches = df_matched_based_on_primary_identifier[df_matched_based_on_primary_identifier['primary_identifier_match'] == 'both']
-    df_only_primary_identifier_matches = df_only_primary_identifier_matches.drop('primary_identifier_match', axis=1)
-    
-    # Create df_only_failed_primary_identifier_matches for further processing
-    df_only_failed_primary_identifier_matches = df_matched_based_on_primary_identifier[df_matched_based_on_primary_identifier['primary_identifier_match'] != 'both']
-    df_only_failed_primary_identifier_matches = df_only_failed_primary_identifier_matches.drop('primary_identifier_match', axis=1)
-
-    # Drop blank columns from first match attempt
-    df_only_failed_primary_identifier_matches = df_only_failed_primary_identifier_matches.iloc[:,:(num_columns_in_query)]  
-
-    # Adjustments based on whether there is a second identifier column
-    if secondary_optional_identifier_used_on_sheet == True:
-
-        # If a row in df_only_failed_primary_identifier_matches contains a number for primary_identifier and 'N/A' for secondary_optional_identifier,
-        #   then they are likely a student newly added to the list. Put them in a dataframe so they can be stacked later.
-        df_newly_added_students_with_no_primary_identifier_match_and_na_secondary_identifier = df_only_failed_primary_identifier_matches[pd.to_numeric(df_only_failed_primary_identifier_matches[primary_identifier], errors='coerce').notnull() & (df_only_failed_primary_identifier_matches[secondary_optional_identifier] == 'N/A')]
-        
-        # And then drop these students from df_only_failed_primary_identifier_matches
-        df_only_failed_primary_identifier_matches = df_only_failed_primary_identifier_matches.drop(df_newly_added_students_with_no_primary_identifier_match_and_na_secondary_identifier.index)
-        
-        # Drop rows from existing spreadsheet data where secondary_optional_identifier is 'N/A' and convert columns for merging to numeric
-        df_spreadsheet_values_to_keep = df_spreadsheet_values_to_keep[df_spreadsheet_values_to_keep[secondary_optional_identifier] != 'N/A']
-        df_spreadsheet_values_to_keep[secondary_optional_identifier] = pd.to_numeric(df_spreadsheet_values_to_keep[secondary_optional_identifier])
-        df_only_failed_primary_identifier_matches[secondary_optional_identifier] = pd.to_numeric(df_only_failed_primary_identifier_matches[secondary_optional_identifier])
-        
-        # Merge on secondary_optional_identifier
-        df_secondary_optional_identifier_matches = df_only_failed_primary_identifier_matches.merge(df_spreadsheet_values_to_keep, on=secondary_optional_identifier, how='left')
-        
-        # Deal with duplicate primary_identifier column
-        df_secondary_optional_identifier_matches = df_secondary_optional_identifier_matches.drop(f'{primary_identifier}_y', axis=1).rename(columns={f'{primary_identifier}_x': primary_identifier})
-    else:
-        # If a row in df_only_failed_primary_identifier_matches contains a number for primary_identifier and there is no secondary_optional_identifier column,
-        #   then they are likely a student newly added to the list. Put them in a dataframe so they can be stacked later.
-        df_newly_added_students_with_no_primary_identifier_match_and_na_secondary_identifier = df_only_failed_primary_identifier_matches[pd.to_numeric(df_only_failed_primary_identifier_matches[primary_identifier], errors='coerce').notnull()]
-        
-    # Successful primary_identifier matches and newly added students with no primary_identifier match are always included
-    dataframes_to_combine = [
-        df_only_primary_identifier_matches, 
-        df_newly_added_students_with_no_primary_identifier_match_and_na_secondary_identifier
-    ]
-
-    # If there is an secondary_optional_identifier column, include secondary_optional_identifier matches (including matches that failed both primary_identifier and secondary_optional_identifier merges)
-    if secondary_optional_identifier_used_on_sheet == True:
-        dataframes_to_combine.append(df_secondary_optional_identifier_matches)
-    # If there is no secondary_optional_identifier column, include failed primary_identifier matches
-    else:
-        dataframes_to_combine.append(df_only_failed_primary_identifier_matches)
-
-    # Create single dataframe combining the initial primary_identifier matches, newly added students with no primary_identifier match, failed matches, and if necessary, the secondary_optional_identifier matches
-    df_combined_matches = pd.concat(dataframes_to_combine, axis=0)
-
-    # If sorting lists provided, sort the dataframe
-    if 'sorting_column_list' in single_worksheet_information_dict and 'sorting_ascending_list' in single_worksheet_information_dict:
-        df_combined_matches = df_combined_matches.sort_values(by=single_worksheet_information_dict['sorting_column_list'], 
-            ascending=single_worksheet_information_dict['sorting_ascending_list'])
-
-    # Fill NA's so they don't fail when updating the spreadsheet
-    df_combined_matches.fillna('', inplace=True)
-
-    # Drop duplicate rows to prevent duplicate identifiers from adding new rows exponentially
-    df_combined_matches = df_combined_matches.drop_duplicates()
-    
-    ### Update existing tab with data from new dataframe
-
-    # Prepare to clear existing tab
-    existing_num_worksheet_columns = worksheet_object.col_count
-    final_column_letter = col_to_letter(existing_num_worksheet_columns)
-
-    # Check that the df_combined_matches dataframe is not too large for the worksheet before deleting any data
-    new_num_worksheet_columns = df_combined_matches.shape[1]
-
-    if(new_num_worksheet_columns > existing_num_worksheet_columns):
-        logging.info('existing_num_worksheet_columns:', existing_num_worksheet_columns)
-        logging.info('new_num_worksheet_columns:', new_num_worksheet_columns)
-        logging.info('df_combined_matches columns:', df_combined_matches.columns.to_list())
-        assert False, "Dataframe of updated data has more columns than the existing worksheet. Check for duplicate column names in source worksheet."
-
-    # Clear existing tab
-    logging.info('Clear the existing worksheet.')
-    worksheet_object.batch_clear([f'A{number_of_header_rows+1}:{final_column_letter}'])
-
-    # Delete all rows on worksheet after headers + first data row
-    num_rows_to_delete = worksheet_object.row_count - number_of_header_rows - 1
-    if num_rows_to_delete > 0:
-        # Indexes are 1-based
-        # First row to delete
-        delete_start_index = number_of_header_rows + 2 
-        # Last row to delete; subtract 1 from the number of rows to delete to get the row # of the last row to delete
-        # e.g., deleting 1 row means start and end indexes are the same; deleting 2 rows means end index is 1 more than the start index
-        delete_end_index = delete_start_index + num_rows_to_delete - 1
-        worksheet_object.delete_rows(delete_start_index, delete_end_index)
-
-    # Calculate the range for the destination worksheet
-    updated_worksheet_row_count = df_combined_matches.shape[0] + number_of_header_rows # Number of records + number of header rows
-    destination_range = f'A{number_of_header_rows+1}:{final_column_letter}{updated_worksheet_row_count}'
-
-    # Update the destination worksheet
-    logging.info('Update the existing worksheet with the new combined data.')
-    worksheet_object.update(destination_range, df_combined_matches.values.tolist(), value_input_option='USER_ENTERED')
-
-    # Apply worksheet formatting
-    _apply_worksheet_formatting(
-        worksheet_object = worksheet_object, 
-        single_worksheet_information_dict = single_worksheet_information_dict, 
-        number_of_header_rows = number_of_header_rows, 
-        updated_worksheet_row_count = updated_worksheet_row_count, 
-        colors_dict = colors_dict)
+import pandas as pd
+import logging
+
+from .warehouse import create_warehouse
+from .googlesheets import create_sheets
+from .googledrive import create_drive
+
+from gspread_formatting import (
+    set_data_validation_for_cell_range,
+    BooleanCondition,
+    BooleanRule,
+    CellFormat,
+    ConditionalFormatRule,
+    get_conditional_format_rules,
+    GridRange,
+    textFormat,
+    format_cell_range,
+    color,
+)
+
+"""
+This module defines a number of functions to create and manage 
+"Magic Spreadsheets" - Google Sheets that automatically update based on
+the results of a SQL query run against the warehouse.
+
+Magic Spreadsheets are more sophisticated than a simple export in that they 
+preserve existing columns, so they support users of the sheet adding notes
+and other columns that will maintain their associations even as students
+are added/removed from the sheet.
+
+We use this in production in the SY24 "Main Enrollment Forms Tracker" (MEFT)
+and the SY24 Child Find tool.
+
+Typical sequence of calls:
+    * Create or fetch the spreadsheets: `spreadsheet_object, spreadsheet_already_exists = create_or_retrieve_magic_spreadsheet_and_add_missing_worksheets(...)`
+    * Add the static worksheets: `check_for_static_worksheets_and_add_them_with_protection(...)`
+    * Update the spreadsheet with query results: `update_magic_spreadsheet_with_new_query_results(...)`
+    * If desired, update specific cells (like the "Last Updated" field): `update_specific_cell(...)`
+"""
+
+def _run_warehouse_query_for_worksheet(query_list: list):
+    """
+    Take a list of queries stored as dictionaries. Run each query at the provided
+    path with the provided parameters. Take the output of all queries in the list,
+    combine them, remove NAs, and return the resulting combined dataframe.
+    """
+    df_combined_query_output = None
+
+    for query_dict in query_list:
+        query_path = query_dict['path']
+        query_parameters = query_dict['parameters']
+
+        with open(query_path, "r") as f:
+            if query_parameters == {}:
+                warehouse_query = f.read()
+            else:
+                warehouse_query = f.read().format(**query_parameters)
+
+        Warehouse = create_warehouse()
+
+        # Raise logging level to limit warehouse output to logs
+        logger = logging.getLogger()
+        logger.setLevel(logging.WARNING)
+
+        df_query_output = Warehouse.read_sql(warehouse_query)
+
+         # Reset logging level
+        logger.setLevel(logging.INFO)
+
+        if df_combined_query_output is None:
+            df_combined_query_output = df_query_output
+        else:
+            df_combined_query_output = pd.concat([df_combined_query_output, df_query_output], axis=0)
+        
+    df_combined_query_output.fillna('', inplace=True)
+
+    return df_combined_query_output
+
+def _add_formulas_to_worksheet(worksheet_object, formulas_list):
+    """
+    Given a list of formulas in the format below, add the formula to the specified row of the
+    column, then copy it down the entire column.
+    """
+    
+    for formula in formulas_list:
+        formula_column = formula['column']
+        formula_row_start = formula['row_of_first_formula_cell']
+        formula_text = formula['formula_text']
+        
+        # First, add the formula to the specified row of the given column
+        source_cell = f'{formula_column}{formula_row_start}'
+        worksheet_object.update(source_cell, formula_text, value_input_option='USER_ENTERED')
+        
+        # Then, copy that formula down the whole column
+        destination_range = f'{formula_column}{formula_row_start}:{formula_column}'
+        
+        worksheet_object.copy_range(source_cell, destination_range, paste_type='PASTE_FORMULA')
+
+def _add_data_validations_to_worksheet(worksheet_object, data_validations_list):
+    """
+    Given a list of data validations in the format below, clears any existing rules in
+    the provided range and adds each rule from the list to the worksheet object. This
+    function assumes one validation rule for any given range; otherwise, later rules 
+    in the list would overwrite earlier ones.
+    
+    List format:
+        [
+            {
+                'range': 'P4:P',
+                'validation_rule' : DataValidationRule(
+                    BooleanCondition('ONE_OF_LIST', ['True', 'False']),
+                    showCustomUi=True
+                )
+            },
+        ]
+    """
+    for data_validation in data_validations_list:
+        validation_range = data_validation['range']
+        validation_rule = data_validation['validation_rule']
+        
+        # Clear any existing validation rules in the range
+        set_data_validation_for_cell_range(worksheet_object, validation_range, None)
+    
+        # Add validation rule from list to the range
+        set_data_validation_for_cell_range(worksheet_object, validation_range, validation_rule)
+
+def _hide_header_rows_and_left_columns_in_worksheet(worksheet_object, num_header_rows_to_hide, num_left_columns_to_hide):
+
+    worksheet_object.hide_rows(0, num_header_rows_to_hide)
+    worksheet_object.hide_columns(0, num_left_columns_to_hide)
+
+def _set_basic_filter_on_worksheet(worksheet_object, row_number_for_filter, final_row_number):
+    num_columns = worksheet_object.col_count
+    final_col_letter = col_to_letter(num_columns)
+
+    worksheet_object.set_basic_filter(f'A{row_number_for_filter}:{final_col_letter}{final_row_number}')
+
+def _refresh_conditional_formatting_on_worksheet(worksheet_object, num_header_rows: int,
+    conditional_formatting_rules_dict: dict, colors_dict: dict):
+
+    # logging.info("Store the current conditional formatting rules.")
+    rules = get_conditional_format_rules(worksheet_object)
+    
+    # logging.info("Delete all the existing rules.")
+    rules.clear()
+
+    # logging.info("Iterating through conditional formatting rules.")
+    for color in conditional_formatting_rules_dict.keys():
+        for new_rule in conditional_formatting_rules_dict[color]:
+            new_rule_starts_with_text = new_rule[0]
+            new_rule_start_column = new_rule[1]
+            new_rule_end_column = new_rule[2]
+
+            color_object = colors_dict[color]
+
+            new_rule_range = f'{new_rule_start_column}{num_header_rows+1}:{new_rule_end_column}'
+
+            new_condition = ConditionalFormatRule(
+                ranges=[GridRange.from_a1_range(new_rule_range, worksheet_object)],
+                booleanRule=BooleanRule(
+                    condition=BooleanCondition("TEXT_STARTS_WITH", [new_rule_starts_with_text]),
+                    format=CellFormat(
+                        textFormat=textFormat(
+                            foregroundColor=color_object
+                        )
+                    )
+                )
+            )
+
+            # logging.info(f'Appending rule to rules list: text starting with "{new_rule_starts_with_text}" in column {new_rule_start_column} through column {new_rule_end_column} is {color}.')
+            rules.append(new_condition)
+
+    # logging.info("Posting the new rules back to the worksheet.")
+    rules.save()
+
+    # logging.info("Conditional formatting updated.")
+
+def create_or_retrieve_magic_spreadsheet_and_add_missing_worksheets(drive_folder_id: str,
+    spreadsheet_name: str, template_spreadsheet_id: str, worksheet_name_list):
+
+    gs = create_sheets()
+
+    spreadsheet_already_exists, spreadsheet_object = _check_if_spreadsheet_exists_and_retrieve_it(
+        drive_folder_id=drive_folder_id,
+        spreadsheet_name=spreadsheet_name,
+        gs = gs,
+    )
+
+    if spreadsheet_already_exists == False:
+        spreadsheet_object = _create_spreadsheet_from_template(
+            output_spreadsheet_name = spreadsheet_name, 
+            output_folder_id = drive_folder_id, 
+            template_spreadsheet_id = template_spreadsheet_id, 
+            worksheet_name_list = worksheet_name_list,
+            gs = gs,
+            )
+    else:
+        template_spreadsheet_object = gs.open_by_key(template_spreadsheet_id)
+
+        _check_for_missing_worksheets_and_create_them(target_spreadsheet_object = spreadsheet_object, 
+            template_spreadsheet_object = template_spreadsheet_object, 
+            worksheet_name_list = worksheet_name_list)
+        
+    return spreadsheet_object, spreadsheet_already_exists
+
+def _check_if_spreadsheet_exists_and_retrieve_it(drive_folder_id: str, spreadsheet_name: str, gs):
+    
+    google_drive = create_drive()
+
+    folder_files = google_drive.ListFile({'q': f"'{drive_folder_id}' in parents"}).GetList()
+
+    spreadsheet_already_exists = False
+
+    # Get spreadsheet if it exists
+    for file in folder_files:
+        if file['title'] == spreadsheet_name:
+            spreadsheet_already_exists = True
+            current_spreadsheet = gs.open_by_key(file['id'])
+
+    if spreadsheet_already_exists == True:
+        return spreadsheet_already_exists, current_spreadsheet
+    else:
+        return spreadsheet_already_exists, None
+
+def _create_worksheet_from_template_if_does_not_exist(target_spreadsheet_object, template_spreadsheet_object, worksheet_name):
+
+    new_worksheet_created = False
+
+    # Get the list of worksheet titles in the target spreadsheet
+    worksheet_list = target_spreadsheet_object.worksheets()
+
+    # Check if a specific worksheet exists
+    worksheet_exists = any(worksheet.title == worksheet_name for worksheet in worksheet_list)
+
+    if worksheet_exists == False:
+        # Get worksheet in template
+        template_worksheet = template_spreadsheet_object.worksheet(worksheet_name)
+        
+        # Copy worksheet to the target spreadsheet
+        target_worksheet_info_dict = template_worksheet.copy_to(target_spreadsheet_object.id)
+        target_worksheet_object = target_spreadsheet_object.worksheet(target_worksheet_info_dict['title'])
+        
+        # Rename worksheet at destination to remove 'Copy of'
+        target_worksheet_object.update_title(worksheet_name)
+
+        new_worksheet_created = True
+       
+    return new_worksheet_created
+
+def _check_for_missing_worksheets_and_create_them(target_spreadsheet_object, template_spreadsheet_object, worksheet_name_list):
+    for worksheet_name in worksheet_name_list:
+        _create_worksheet_from_template_if_does_not_exist(target_spreadsheet_object = target_spreadsheet_object, 
+            template_spreadsheet_object = template_spreadsheet_object, worksheet_name = worksheet_name)
+
+def _create_spreadsheet_from_template(output_spreadsheet_name: str, output_folder_id: str, 
+    template_spreadsheet_id: str, worksheet_name_list: list, gs):
+    
+    # Create spreadsheet
+    spreadsheet = gs.create(output_spreadsheet_name, folder_id=output_folder_id)
+    
+    # Get the template
+    template_spreadsheet = gs.open_by_key(template_spreadsheet_id)
+    
+    # Copy tabs from template to the spreadsheet
+    _check_for_missing_worksheets_and_create_them(target_spreadsheet_object = spreadsheet, 
+        template_spreadsheet_object = template_spreadsheet, 
+        worksheet_name_list = worksheet_name_list)
+
+    # Delete the default sheet
+    default_worksheet_to_delete = spreadsheet.worksheet("Sheet1")
+    spreadsheet.del_worksheet(default_worksheet_to_delete)
+    
+    return spreadsheet
+
+def update_magic_spreadsheet_with_new_query_results(spreadsheet_object, worksheet_information_dict: dict, 
+        school_information_dict: dict, other_query_parameters_dict: dict, primary_identifier: str,
+        secondary_optional_identifier: str = '', colors_dict: dict = {}, worksheet_order_name_list = [], 
+        general_editor_list = [],
+        # Optional Parameters: Getting Data From Different Source
+        # get_data_from_different_source: bool = False, 
+        **kwargs,
+        # different_source_worksheet_object = None, 
+        # different_source_number_of_header_rows = None, different_source_num_columns_on_left_not_to_keep = None,
+        # different_source_columns_to_rename = [],
+    ):
+
+    # Update all worksheets with fresh query results
+    for worksheet_name in worksheet_information_dict.keys():
+        logging.info('='*75)
+        logging.info(f'Begin updating "{worksheet_name}" worksheet.')
+
+        worksheet_to_update = spreadsheet_object.worksheet(worksheet_name)
+        _update_magic_spreadsheet_worksheet_with_new_query_results(
+            worksheet_object = worksheet_to_update,
+            single_worksheet_information_dict = worksheet_information_dict[worksheet_name],
+            query_parameters_dict = {**school_information_dict, **other_query_parameters_dict},
+            colors_dict = colors_dict,
+            primary_identifier = primary_identifier,
+            secondary_optional_identifier = secondary_optional_identifier,
+            # get_data_from_different_source = get_data_from_different_source, 
+            **kwargs,
+            # different_source_worksheet_object = different_source_worksheet_object, 
+            # different_source_number_of_header_rows = different_source_number_of_header_rows, 
+            # different_source_num_columns_on_left_not_to_keep = different_source_num_columns_on_left_not_to_keep,
+            # different_source_columns_to_rename = different_source_columns_to_rename,
+        )
+
+        logging.info(f'Done updating "{worksheet_name}" worksheet.')
+        
+    # Reorder worksheets
+    if len(worksheet_order_name_list) > 0:
+        _reorder_worksheets(spreadsheet_object, worksheet_order_name_list)
+        
+    # Re-confirm spreadsheet is shared with all general editors and all school editors
+    spreadsheet_editor_list = school_information_dict['spreadsheet_editors']
+    full_editor_list = general_editor_list + spreadsheet_editor_list
+
+    for editor in full_editor_list:
+        spreadsheet_object.share(editor, perm_type='user', role='writer', notify=False)
+
+def col_to_letter(column_int):
+    """
+    Adapted from: https://stackoverflow.com/a/23862195
+    """
+    start_index = 1   #  it can start either at 0 or at 1
+    letter = ''
+    while column_int > 25 + start_index:   
+        letter += chr(65 + int((column_int-start_index)/26) - 1)
+        column_int = column_int - (int((column_int-start_index)/26))*26
+    letter += chr(65 - start_index + (int(column_int)))
+
+    return letter
+
+def check_for_static_worksheets_and_add_them_with_protection(target_spreadsheet_object, 
+    template_spreadsheet_id, static_worksheets_list, primary_editor_email = '', 
+    info_team_group_email = '', other_individual_editors_list=[]):
+
+    gs = create_sheets()
+
+    template_spreadsheet_object = gs.open_by_key(template_spreadsheet_id)
+
+    for static_worksheet in static_worksheets_list:
+        static_worksheet_name = static_worksheet['worksheet_name']
+        _create_worksheet_from_template_if_does_not_exist(target_spreadsheet_object, template_spreadsheet_object, static_worksheet_name)
+
+        if static_worksheet['protected'] == True:
+            static_worksheet_object = target_spreadsheet_object.worksheet(static_worksheet_name)
+            protected_range_list = target_spreadsheet_object.list_protected_ranges(static_worksheet_object.id)
+
+            target_description = f'"{static_worksheet_name}" Sheet-wide Protection'
+
+            if any(protected_range["description"] == target_description for protected_range in protected_range_list):
+                logging.info('Protected range already exists.')
+            else:
+                logging.info('Protect range not found. Creating new one.')
+
+                individual_editors = [primary_editor_email] + other_individual_editors_list
+
+                num_worksheet_columns = static_worksheet_object.col_count
+                final_column_letter = col_to_letter(num_worksheet_columns)
+
+                static_worksheet_object.add_protected_range(name=f'A:{final_column_letter}', 
+                    editor_users_emails = individual_editors, 
+                    editor_groups_emails=[info_team_group_email], 
+                    description = target_description
+                )
+
+def update_specific_cell(spreadsheet_object, worksheet_name, cell_a1_notation, text_string):
+    worksheet = spreadsheet_object.worksheet(worksheet_name)
+    cell = worksheet.acell(cell_a1_notation)
+    cell.value = text_string
+    worksheet.update_cell(cell.row, cell.col, cell.value)
+
+def _apply_worksheet_formatting(worksheet_object, single_worksheet_information_dict: dict, number_of_header_rows: int, 
+    updated_worksheet_row_count: int, colors_dict: dict):
+    # Add any validation rules to the worksheet
+    if 'data_validations' in single_worksheet_information_dict:
+        logging.info('Add the data validations to the worksheet.')
+        data_validations_list = single_worksheet_information_dict['data_validations']
+        _add_data_validations_to_worksheet(worksheet_object, data_validations_list)
+    
+    # Re-add any formulas to the worksheet, since they would have been overwritten by hard-coded existing data
+    if 'formulas' in single_worksheet_information_dict:
+        logging.info('Add the formulas to the worksheet.')
+        formulas_list = single_worksheet_information_dict['formulas']
+        _add_formulas_to_worksheet(worksheet_object, formulas_list)
+
+    # Hide rows and columns as specified
+    if ('num_header_rows_to_hide' in single_worksheet_information_dict or 'num_left_columns_to_hide' in single_worksheet_information_dict):
+        logging.info('Hide the specified rows and columns.')
+        _hide_header_rows_and_left_columns_in_worksheet(
+            worksheet_object = worksheet_object, 
+            num_header_rows_to_hide = single_worksheet_information_dict['num_header_rows_to_hide'] if 'num_header_rows_to_hide' in single_worksheet_information_dict else 0,
+            num_left_columns_to_hide = single_worksheet_information_dict['num_left_columns_to_hide'] if 'num_left_columns_to_hide' in single_worksheet_information_dict else 0
+        )
+
+    # Set basic filter
+    if 'filter_on_final_header_row' in single_worksheet_information_dict and single_worksheet_information_dict['filter_on_final_header_row'] == True:
+        logging.info('Set the filter on the worksheet.')
+        _set_basic_filter_on_worksheet(
+            worksheet_object = worksheet_object, 
+            row_number_for_filter = number_of_header_rows, 
+            final_row_number = updated_worksheet_row_count
+        )
+
+    # Refresh conditional formatting
+    if 'conditional_formatting_rules' in single_worksheet_information_dict:
+        logging.info('Refresh the conditional formatting on the worksheet.')
+        _refresh_conditional_formatting_on_worksheet(
+            worksheet_object = worksheet_object,
+            num_header_rows = number_of_header_rows,
+            conditional_formatting_rules_dict = single_worksheet_information_dict['conditional_formatting_rules'],
+            colors_dict = colors_dict,
+        )
+
+    # Get the last column of the query
+    query_column_end = col_to_letter(single_worksheet_information_dict['warehouse_query_number_of_columns'])
+
+    # Update background color for query data to light gray
+    background_color_row_start = number_of_header_rows + 1
+
+    background_color_range = f'A{background_color_row_start}:{query_column_end}'
+
+    background_color_format = CellFormat(
+        backgroundColor = color(245/255, 245/255, 245/255), # Light Gray
+        )
+
+    logging.info('Format the warehouse data cells with the background color.')
+    format_cell_range(worksheet_object, background_color_range, background_color_format)
+
+    # Set cell dividing line on right side of query data
+    query_data_border_range = f'{query_column_end}:{query_column_end}'
+    borders_format = CellFormat(
+        borders = {
+            'right' : 
+                {
+                    "style": 'SOLID',
+                    "width": 1,
+                    "color": {
+                        "red": 0,
+                        "green": 0,
+                        "blue": 0,
+                        "alpha": 1
+                        }, # Black
+                }
+            
+        }
+    )
+
+    logging.info('Set the cell dividing line on the right side of the warehouse data cells.')
+    format_cell_range(worksheet_object, query_data_border_range, borders_format)
+
+def _reorder_worksheets(spreadsheet_object, worksheet_order_name_list):
+    worksheet_objects_in_desired_order = []
+
+    for worksheet_name in worksheet_order_name_list:
+        worksheet = spreadsheet_object.worksheet(worksheet_name)
+        worksheet_objects_in_desired_order.append(worksheet)
+
+    spreadsheet_object.reorder_worksheets(worksheet_objects_in_desired_order)
+
+def _get_all_manual_values_from_existing_worksheet(data_source_worksheet_object, data_source_number_of_header_rows,
+    primary_identifier, secondary_optional_identifier, num_columns_on_left_not_to_keep, source_columns_to_rename = []):
+
+    # Clear the filter on the worksheet
+    data_source_worksheet_object.clear_basic_filter()
+
+    ### Get all data from existing tab
+    all_values = data_source_worksheet_object.get_all_values()
+
+    # Turn all_values into a dataframe
+    # These values are 0-based but number_of_header_rows is 1-based
+    df_all_values = pd.DataFrame(all_values[data_source_number_of_header_rows:], columns=all_values[data_source_number_of_header_rows-1])
+
+    # Rename columns in the different source if needed
+    for column_tuple in source_columns_to_rename:
+        original_column_name = column_tuple[0]
+        new_column_name = column_tuple[1]
+
+        if original_column_name in df_all_values.columns:
+            # Rename the column
+            df_all_values = df_all_values.rename(columns={original_column_name: new_column_name})
+
+    # Keep only the columns from the spreadsheet that are not getting updated by the query + the identifiers
+    # Assume that all worksheets need a primary_identifier column; they may or may not have an secondary_optional_identifier column
+    identifier_columns_to_keep = [primary_identifier]
+
+    secondary_optional_identifier_used_on_sheet = (secondary_optional_identifier in df_all_values.columns)
+
+    if secondary_optional_identifier_used_on_sheet == True:
+        identifier_columns_to_keep.append(secondary_optional_identifier)
+
+    spreadsheet_keep_columns = identifier_columns_to_keep + list(df_all_values.columns[(num_columns_on_left_not_to_keep):])
+    df_spreadsheet_values_to_keep = df_all_values[spreadsheet_keep_columns]
+
+    return df_spreadsheet_values_to_keep, secondary_optional_identifier_used_on_sheet
+
+def _update_magic_spreadsheet_worksheet_with_new_query_results(worksheet_object, single_worksheet_information_dict: dict,
+        query_parameters_dict: dict, colors_dict: dict, primary_identifier: str,
+        # Optional Parameters: Secondary Identifier
+        secondary_optional_identifier: str = '', 
+        # Optional Parameters: Getting Data from Different Source
+        **kwargs
+    ):
+
+    # Add query to query_list and run query
+    # TODO: Do we ever need to run multiple queries in one sheet? If not, refactor to run a single query
+
+    query_list = [{
+        'path' : single_worksheet_information_dict['warehouse_query_path'],
+        'parameters' : query_parameters_dict,
+    }]
+
+    logging.info('Run worksheet query in data warehouse.')
+    df_query_output = _run_warehouse_query_for_worksheet(query_list)
+
+    # Load key metadata
+
+    number_of_header_rows = single_worksheet_information_dict['number_of_header_rows']
+    num_columns_in_query = single_worksheet_information_dict['warehouse_query_number_of_columns']
+    
+    ### Get all data from existing tab
+    gs = create_sheets()
+
+    # Check if parameters passed to get data from a different source
+    if 'get_data_from_different_source' in kwargs and kwargs['get_data_from_different_source'] == True:
+        # Atypical path: Loading data from a different worksheet than will be writing to
+        logging.info('Load data from specified external worksheet.')
+        different_source_spreadsheet_object = gs.open_by_key(kwargs['different_source_spreadsheet_id'])
+        different_source_worksheet_object = different_source_spreadsheet_object.worksheet(kwargs['different_source_worksheet_name'])
+
+        df_spreadsheet_values_to_keep, secondary_optional_identifier_used_on_sheet = _get_all_manual_values_from_existing_worksheet(
+            data_source_worksheet_object = different_source_worksheet_object, 
+            data_source_number_of_header_rows = kwargs['different_source_number_of_header_rows'],
+            primary_identifier = primary_identifier, 
+            secondary_optional_identifier = secondary_optional_identifier, 
+            num_columns_on_left_not_to_keep = kwargs['different_source_num_columns_on_left_not_to_keep'],
+            source_columns_to_rename = kwargs['different_source_columns_to_rename'],
+        )
+    else:
+        # Standard path: loading data from same worksheet will be writing to
+        logging.info('Load data from existing worksheet.')
+        df_spreadsheet_values_to_keep, secondary_optional_identifier_used_on_sheet = _get_all_manual_values_from_existing_worksheet(
+            data_source_worksheet_object = worksheet_object, 
+            data_source_number_of_header_rows = number_of_header_rows,
+            primary_identifier = primary_identifier, 
+            secondary_optional_identifier = secondary_optional_identifier, 
+            num_columns_on_left_not_to_keep = num_columns_in_query
+        )
+        
+    logging.info('Connect user data from existing worksheet to new query output.')
+    # Blank out the 'Not Assigned Yet' values in the primary_identifier column of the spreadsheet dataframe to avoid an incorrect join
+    df_spreadsheet_values_to_keep[primary_identifier] = df_spreadsheet_values_to_keep[primary_identifier].apply(lambda x: '' if x == 'Not Assigned Yet' else x)
+        
+    ### Connect data from existing tab to query output in a new dataframe
+
+    # Attempt a match on primary_identifier first
+    df_matched_based_on_primary_identifier = df_query_output.merge(df_spreadsheet_values_to_keep, on=primary_identifier, how='left', indicator='primary_identifier_match')
+
+    # Drop duplicate secondary_optional_identifier column
+    df_matched_based_on_primary_identifier = df_matched_based_on_primary_identifier.rename(columns={f'{secondary_optional_identifier}_x': secondary_optional_identifier}).drop(f'{secondary_optional_identifier}_y', axis=1)
+
+    # logging.info('Post primary_identifier_match:', df_matched_based_on_primary_identifier.columns)
+
+    # Create a dataframe of successful matches on primary_identifier
+    df_only_primary_identifier_matches = df_matched_based_on_primary_identifier[df_matched_based_on_primary_identifier['primary_identifier_match'] == 'both']
+    df_only_primary_identifier_matches = df_only_primary_identifier_matches.drop('primary_identifier_match', axis=1)
+    
+    # Create df_only_failed_primary_identifier_matches for further processing
+    df_only_failed_primary_identifier_matches = df_matched_based_on_primary_identifier[df_matched_based_on_primary_identifier['primary_identifier_match'] != 'both']
+    df_only_failed_primary_identifier_matches = df_only_failed_primary_identifier_matches.drop('primary_identifier_match', axis=1)
+
+    # Drop blank columns from first match attempt
+    df_only_failed_primary_identifier_matches = df_only_failed_primary_identifier_matches.iloc[:,:(num_columns_in_query)]  
+
+    # Adjustments based on whether there is a second identifier column
+    if secondary_optional_identifier_used_on_sheet == True:
+
+        # If a row in df_only_failed_primary_identifier_matches contains a number for primary_identifier and 'N/A' for secondary_optional_identifier,
+        #   then they are likely a student newly added to the list. Put them in a dataframe so they can be stacked later.
+        df_newly_added_students_with_no_primary_identifier_match_and_na_secondary_identifier = df_only_failed_primary_identifier_matches[pd.to_numeric(df_only_failed_primary_identifier_matches[primary_identifier], errors='coerce').notnull() & (df_only_failed_primary_identifier_matches[secondary_optional_identifier] == 'N/A')]
+        
+        # And then drop these students from df_only_failed_primary_identifier_matches
+        df_only_failed_primary_identifier_matches = df_only_failed_primary_identifier_matches.drop(df_newly_added_students_with_no_primary_identifier_match_and_na_secondary_identifier.index)
+        
+        # Drop rows from existing spreadsheet data where secondary_optional_identifier is 'N/A' and convert columns for merging to numeric
+        df_spreadsheet_values_to_keep = df_spreadsheet_values_to_keep[df_spreadsheet_values_to_keep[secondary_optional_identifier] != 'N/A']
+        df_spreadsheet_values_to_keep[secondary_optional_identifier] = pd.to_numeric(df_spreadsheet_values_to_keep[secondary_optional_identifier])
+        df_only_failed_primary_identifier_matches[secondary_optional_identifier] = pd.to_numeric(df_only_failed_primary_identifier_matches[secondary_optional_identifier])
+        
+        # Merge on secondary_optional_identifier
+        df_secondary_optional_identifier_matches = df_only_failed_primary_identifier_matches.merge(df_spreadsheet_values_to_keep, on=secondary_optional_identifier, how='left')
+        
+        # Deal with duplicate primary_identifier column
+        df_secondary_optional_identifier_matches = df_secondary_optional_identifier_matches.drop(f'{primary_identifier}_y', axis=1).rename(columns={f'{primary_identifier}_x': primary_identifier})
+    else:
+        # If a row in df_only_failed_primary_identifier_matches contains a number for primary_identifier and there is no secondary_optional_identifier column,
+        #   then they are likely a student newly added to the list. Put them in a dataframe so they can be stacked later.
+        df_newly_added_students_with_no_primary_identifier_match_and_na_secondary_identifier = df_only_failed_primary_identifier_matches[pd.to_numeric(df_only_failed_primary_identifier_matches[primary_identifier], errors='coerce').notnull()]
+        
+    # Successful primary_identifier matches and newly added students with no primary_identifier match are always included
+    dataframes_to_combine = [
+        df_only_primary_identifier_matches, 
+        df_newly_added_students_with_no_primary_identifier_match_and_na_secondary_identifier
+    ]
+
+    # If there is an secondary_optional_identifier column, include secondary_optional_identifier matches (including matches that failed both primary_identifier and secondary_optional_identifier merges)
+    if secondary_optional_identifier_used_on_sheet == True:
+        dataframes_to_combine.append(df_secondary_optional_identifier_matches)
+    # If there is no secondary_optional_identifier column, include failed primary_identifier matches
+    else:
+        dataframes_to_combine.append(df_only_failed_primary_identifier_matches)
+
+    # Create single dataframe combining the initial primary_identifier matches, newly added students with no primary_identifier match, failed matches, and if necessary, the secondary_optional_identifier matches
+    df_combined_matches = pd.concat(dataframes_to_combine, axis=0)
+
+    # If sorting lists provided, sort the dataframe
+    if 'sorting_column_list' in single_worksheet_information_dict and 'sorting_ascending_list' in single_worksheet_information_dict:
+        df_combined_matches = df_combined_matches.sort_values(by=single_worksheet_information_dict['sorting_column_list'], 
+            ascending=single_worksheet_information_dict['sorting_ascending_list'])
+
+    # Fill NA's so they don't fail when updating the spreadsheet
+    df_combined_matches.fillna('', inplace=True)
+
+    # Drop duplicate rows to prevent duplicate identifiers from adding new rows exponentially
+    df_combined_matches = df_combined_matches.drop_duplicates()
+    
+    ### Update existing tab with data from new dataframe
+
+    # Prepare to clear existing tab
+    existing_num_worksheet_columns = worksheet_object.col_count
+    final_column_letter = col_to_letter(existing_num_worksheet_columns)
+
+    # Check that the df_combined_matches dataframe is not too large for the worksheet before deleting any data
+    new_num_worksheet_columns = df_combined_matches.shape[1]
+
+    if(new_num_worksheet_columns > existing_num_worksheet_columns):
+        logging.info('existing_num_worksheet_columns:', existing_num_worksheet_columns)
+        logging.info('new_num_worksheet_columns:', new_num_worksheet_columns)
+        logging.info('df_combined_matches columns:', df_combined_matches.columns.to_list())
+        assert False, "Dataframe of updated data has more columns than the existing worksheet. Check for duplicate column names in source worksheet."
+
+    # Clear existing tab
+    logging.info('Clear the existing worksheet.')
+    worksheet_object.batch_clear([f'A{number_of_header_rows+1}:{final_column_letter}'])
+
+    # Delete all rows on worksheet after headers + first data row
+    num_rows_to_delete = worksheet_object.row_count - number_of_header_rows - 1
+    if num_rows_to_delete > 0:
+        # Indexes are 1-based
+        # First row to delete
+        delete_start_index = number_of_header_rows + 2 
+        # Last row to delete; subtract 1 from the number of rows to delete to get the row # of the last row to delete
+        # e.g., deleting 1 row means start and end indexes are the same; deleting 2 rows means end index is 1 more than the start index
+        delete_end_index = delete_start_index + num_rows_to_delete - 1
+        worksheet_object.delete_rows(delete_start_index, delete_end_index)
+
+    # Calculate the range for the destination worksheet
+    updated_worksheet_row_count = df_combined_matches.shape[0] + number_of_header_rows # Number of records + number of header rows
+    destination_range = f'A{number_of_header_rows+1}:{final_column_letter}{updated_worksheet_row_count}'
+
+    # Update the destination worksheet
+    logging.info('Update the existing worksheet with the new combined data.')
+    worksheet_object.update(destination_range, df_combined_matches.values.tolist(), value_input_option='USER_ENTERED')
+
+    # Apply worksheet formatting
+    _apply_worksheet_formatting(
+        worksheet_object = worksheet_object, 
+        single_worksheet_information_dict = single_worksheet_information_dict, 
+        number_of_header_rows = number_of_header_rows, 
+        updated_worksheet_row_count = updated_worksheet_row_count, 
+        colors_dict = colors_dict)
```

### Comparing `spswarehouse-0.6.1/spswarehouse/powerschool/powerschool.py` & `spswarehouse-0.6.2/spswarehouse/powerschool/powerschool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,891 +1,891 @@
-import logging
-import time
-import os
-import math
-import pandas as pd
-
-try:
-    from spswarehouse.credentials import powerschool_config
-except ModuleNotFoundError:
-    powerschool_config = None
-    print("No credentials file found in spswarehouse. This could cause issues.")
-
-from ducttape.utils import (
-    DriverBuilder,
-    get_most_recent_file_in_dir,
-)
-
-from spswarehouse.general.selenium import (
-    type_in_element_by_id,
-    select_visible_text_in_element_by_id,
-    click_element_by_id,
-    click_element_by_name,
-    click_element_by_partial_link_text,
-    wait_for_element_containing_specific_text,
-)
-    
-from selenium.webdriver.support.ui import WebDriverWait, Select
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.common.action_chains import ActionChains
-from selenium.common.exceptions import NoSuchElementException
-
-ADMIN_LOGIN_PAGE_PATH = 'admin/pw.html'
-ADMIN_HOME_PAGE_PATH = 'admin/home.html'
-ADMIN_URL_SCHEME = 'https://'
-STATE_REPORTS_PAGE_PATH = 'admin/reports/statereports.html?repType=state'
-REPORT_QUEUE_REPORTWORKS_PAGE_PATH = 'admin/reportqueue/prhome.html'
-REPORT_QUEUE_SYSTEM_PAGE_PATH = 'admin/reportqueue/home.html'
-DATA_IMPORT_MANAGER_PATH = 'admin/datamgmt/importmanager.action'
-
-DEPRECATION_WARNING_MESSAGE = "DEPRECATION_WARNING: This helper function in the PowerSchool class will be deprecated in a future release. Use the helper functions in general.selenium instead."
-
-class PowerSchool:
-    """
-    This class is an abstraction for interacting with the PowerSchool Admin user 
-    interface via Selenium.
-    """
-
-    def __init__(
-        self,
-        config: dict=None,
-        username: str=None,
-        password: str=None,
-        host: str=None,
-        headless: bool=True, 
-        download_location: str='.',
-        chrome_option_prefs: dict=None,
-    ):
-        
-        if config is None:
-            config = powerschool_config
-        
-        if username is None: 
-            username = config['username']
-        else:
-            username = username
-
-        if password is None:
-            password = config['password']
-        else:
-            password = password
-
-        if host is None:
-            self.host = config['host']
-        else:
-            self.host = host
-
-        self.driver = DriverBuilder().get_driver(
-            headless=headless,
-            download_location=download_location,
-            chrome_option_prefs=chrome_option_prefs,
-        )
-        
-        self._log_into_powerschool_admin(username, password)
-
-    def quit(self):
-        self.driver.quit()
-
-    def refresh(self):
-        self.driver.refresh()
-
-    def ensure_on_desired_path(self, desired_path: str):
-        """
-        Checks whether the WebDriver is on the desired path. If not, navigates there.
-        When using this function, consider a WebDriverWait afterwards to confirm the
-        desired page has loaded.
-
-        Parameters:
-        self
-        desired_path: The path to be checked against
-
-        Returns:
-        n/a
-        """
-
-        current_path = self._get_current_path()
-
-        logging.info(f"The current path is: {current_path}")
-
-        if(current_path == desired_path):
-            logging.info("The current path is the desired path. No action taken.")
-        else:
-            logging.info(f"This does not match {desired_path}, so going to that path")
-            self.driver.get('https://' + self._get_current_domain() + "/" + desired_path)
-            time.sleep(3) # Give new page time to load
-            logging.info(f"Moved to {desired_path}.")
-
-    def check_whether_desired_school_selected(self, school_name: str) -> bool:
-        """
-        Checks whether the specified school is currently selected in PowerSchool but
-        takes no action either way.
-
-        Parameters:
-        self
-        school_name: The school name for selecting from the drop-down in the upper-right of the user 
-        interface. Should be the complete school name to avoid incorrect partial matches.
-
-        Returns:
-        bool: True indicates the desired school is selected, and False indicates it is not.
-        """
-
-        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
-            'school_picker_adminSchoolPicker_toggle_btn')))
-
-        elem.click()
-        time.sleep(1)
-
-        selected_element = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((
-            By.CSS_SELECTOR, '.list-item.selectable.selected')))
-
-        school_element_text = selected_element.find_element(By.XPATH, ".//div").text
-
-        result_message = f"Found the {school_name} in the school element text. Match!"
-        outcome = True
-
-        if(school_name not in school_element_text):
-            result_message = f"Did not find {school_name} in the school element text. No match."
-            outcome = False
-
-        logging.info(result_message)
-
-        logging.info(f"Pressing escape to leave dropdown selection.")
-        actions = ActionChains(self.driver)
-        actions.send_keys(Keys.ESCAPE).perform()
-        
-        return outcome
-    
-    def check_whether_desired_school_year_selected(self, school_year_dropdown: str):
-        """
-        Checks whether the specified school year is currently selected in PowerSchool but
-        takes no action either way.
-
-        Parameters:
-        self
-        school_year_dropdown: The exact text of the school year that appears in the dropdown in 
-            PowerSchool. Should be 'XX-YY 20XX-20YY' format.
-
-        Returns:
-        bool: True indicates the desired school year is selected, and False indicates it is not.
-        """
-
-        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
-            'term_picker_adminTermPicker_toggle_btn')))
-
-        elem.click()
-        time.sleep(1)
-
-        selected_element = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((
-            By.CSS_SELECTOR, '.list-item.selectable.selected')))
-
-        school_year_element_text = selected_element.find_element(By.XPATH, ".//div").text
-
-        result_message = f"Found '{school_year_dropdown}' in the school year element text. Match!"
-        outcome = True
-
-        if(school_year_dropdown not in school_year_element_text):
-            result_message = f"Did not find '{school_year_dropdown}' in the school year element text. No match."
-            outcome = False
-
-        logging.info(result_message)
-
-        logging.info(f"Pressing escape to leave dropdown selection.")
-        actions = ActionChains(self.driver)
-        actions.send_keys(Keys.ESCAPE).perform()
-        
-        return outcome
-    
-    def switch_to_school_year(self, school_year_dropdown: str):
-        """
-        Switches to a specified school year in PowerSchool.
-
-        Parameters:
-        self
-        school_year_dropdown: The exact text of the school year that appears in the dropdown in 
-            PowerSchool. Should be 'XX-YY 20XX-20YY' format.
-
-        Returns:
-        n/a
-        """
-        if self.check_whether_desired_school_year_selected(school_year_dropdown) == False:
-            logging.info(f"'{school_year_dropdown}' is not already selected. Selecting now.")
-
-            self.ensure_on_desired_path(ADMIN_HOME_PAGE_PATH)
-
-            logging.info("Waiting for School Year Picker")
-            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
-                'term_picker_adminTermPicker_toggle_btn')))
-            logging.info("School Year Picker found. Click it.")
-
-            elem.click()
-
-            time.sleep(1)
-
-            logging.info("Waiting for School Year Search Field")
-            elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.ID, 
-                'termText')))
-            logging.info("Found School Year Search Field. Typing in school year text.")
-
-            # Only send the XX-YY portion of the dropdown text
-            elem.send_keys(school_year_dropdown[:5])
-
-            time.sleep(1)
-
-            logging.info("Looking for first school year in list")
-            
-            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.XPATH, 
-                "//ul[@id='term_choices']/li[2]"))) # This is li[2] instead of li[1] because there is read-only school year item displayed
-
-            logging.info("Found first school year in results list. Clicking.")
-            elem.click()
-            logging.info("Click. Waiting for page to refresh.")
-            time.sleep(1)
-            
-            assert self.check_whether_desired_school_year_selected(school_year_dropdown), "Failed to select \
-                desired school year."
-        else:
-            logging.info(f"'{school_year_dropdown}' is already selected. No action taken.")
-
-    def switch_to_school(self, school_name: str):
-        """
-        Switches to a specified school in PowerSchool.
-
-        Parameters:
-        self
-        school_name: The school name for selecting from the drop-down in the upper-right of the user 
-            interface. Should be the complete school name to avoid incorrect partial matches.
-
-        Returns:
-        n/a
-        """
-
-        if self.check_whether_desired_school_selected(school_name) == False:
-            logging.info(f"{school_name} is not already selected. Selecting now.")
-
-            self.ensure_on_desired_path(ADMIN_HOME_PAGE_PATH)
-
-            logging.info("Waiting for School Picker")
-            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
-                'school_picker_adminSchoolPicker_toggle_btn')))
-            logging.info("School Picker found. Click it.")
-
-            elem.click()
-
-            time.sleep(1)
-
-            logging.info("Waiting for School Search Field")
-            elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.ID, 
-                'schoolSearchField_value')))
-            logging.info("Found School Search Field. Typing in school name.")
-
-            elem.send_keys(school_name)
-
-            time.sleep(1)
-
-            logging.info("Looking for first school in list")
-            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.XPATH, 
-                "//ul[@id='school_choices']/li[1]")))
-
-            logging.info("Found first school in results list. Clicking.")
-            elem.click()
-            logging.info("Click. Waiting for page to refresh.")
-            time.sleep(1)
-            
-            assert self.check_whether_desired_school_selected(school_name), "Failed to select \
-                desired school."
-        else:
-            logging.info(f"{school_name} is already selected. No action taken.")
-    
-    def navigate_to_state_reports_page(self):
-        """
-        Navigates to the state reports page in PowerSchool.
-
-        Parameters:
-        self
-        
-        Returns:
-        n/a
-        """
-
-        self.driver.get(ADMIN_URL_SCHEME + self._get_current_domain() + '/' + STATE_REPORTS_PAGE_PATH)
-
-        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.CSS_SELECTOR, 
-            'ul li.selected')))
-        assert elem.text == 'State', "'State' tab is not selected"
-
-    def navigate_to_specific_state_report(self, report_link_text: str):
-        """
-        Navigates to the state reports page in PowerSchool and clicks on the report containing
-        the report_link_text string.
-
-        Parameters:
-        self
-        report_link_text: The string to uniquely identify the report. Can be partial text.
-
-        Returns:
-        n/a
-        """
-        self.navigate_to_state_reports_page()
-
-        click_element_by_partial_link_text(self.driver, report_link_text)
-
-
-
-### START TODO: These helper functions inside the PowerSchool class will be removed in a future release. ##############
-###             The functions in general.selenium should be used instead. #############################################
-
-    def helper_type_in_element_by_id(self, element_id: str, input_to_type: str):
-        """
-        Waits for an element by ID, clears it, and types in the input.
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, element_id)))
-        elem.clear()
-        elem.send_keys(input_to_type)
-
-    def helper_type_in_element_by_name(self, element_name: str, input_to_type: str):
-        """
-        Waits for an element by name, clears it, and types in the input.
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.NAME, 
-            element_name)))
-        elem.clear()
-        elem.send_keys(input_to_type)
-
-    def helper_select_visible_text_in_element_by_id(self, element_id: str, 
-        text_to_select: str):
-        """
-        Waits for an element by ID and selects it by specified text.
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, element_id)))
-        select = Select(elem)
-        select.select_by_visible_text(text_to_select)
-
-    def helper_select_visible_text_in_element_by_name(self, element_name: str, 
-        text_to_select: str):
-        """
-        Waits for an element by name and selects it by specified text.
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.NAME, 
-            element_name)))
-        select = Select(elem)
-        select.select_by_visible_text(text_to_select)
-
-    def helper_click_element_by_id(self, element_id: str):
-        """
-        Waits for an element by ID and clicks it.
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.ID, element_id)))
-        elem.click()
-
-    def helper_click_element_by_name(self, element_name: str):
-        """
-        Waits for an element by name and clicks it.
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.NAME, element_name)))
-        elem.click()
-
-    def helper_click_element_by_partial_link_text(self, partial_link_text: str):
-        """
-        Waits for an element by partial link text and clicks it.
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.PARTIAL_LINK_TEXT, 
-            f"{partial_link_text}")))
-        elem.click()
-
-    def helper_ensure_checkbox_is_checked_by_name(self, checkbox_name: str):
-        """
-        Waits for a checkbox element by name and clicks it if it is not already selected.
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        checkbox = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH, 
-            f"//input[@type='checkbox' and @name='{checkbox_name}']")))
-        
-        if checkbox.is_selected() == False:
-            checkbox.click()
-    
-    def helper_ensure_checkbox_is_unchecked_by_name(self, checkbox_name: str):
-        """
-        Waits for a checkbox element by name and clicks it if it is already selected, to make
-        sure it is not checked.
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        checkbox = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH, 
-            f"//input[@type='checkbox' and @name='{checkbox_name}']")))
-        
-        if checkbox.is_selected():
-            checkbox.click()
-
-    def helper_ensure_element_text_matches_expected_value_by_xpath(self, element_xpath, expected_text):
-        """
-        Waits for an element by XPATH and checks whether its text matches the expected text.
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH, 
-            element_xpath)))
-        
-        return elem.text == expected_text
-    
-    def helper_wait_for_element_containing_specific_text(self, expected_element_text, wait_time_in_seconds=30):
-        """
-        Waits for an element containing specific text raises an exception if it does not 
-        appear in the time allotted (default = 30 seconds).
-        """
-        print(DEPRECATION_WARNING_MESSAGE)
-
-        try:
-            WebDriverWait(self.driver, wait_time_in_seconds).until(EC.presence_of_element_located((By.XPATH, f"//*[contains(text(), '{expected_element_text}')]")))
-        except:
-            raise Exception(f'Element with text "{expected_element_text}" not found within {wait_time_in_seconds} seconds.')
-
-### END TODO #########################################################################################################
-
-
-
-    def download_latest_report_from_report_queue_reportworks(self, destination_directory_path: str = '.', 
-        file_postfix: str = ''):
-        """
-        Navigates to the PowerSchool Report Queue (ReportWorks), confirms the most recent report is 
-        done generating, and downloads it.
-
-        Parameters:
-        self
-        destination_directory_path: Where to download the PowerSchool report to.
-        file_postfix: Optional postfix to attach to the end of the downloaded file's filename.
-
-        Returns:
-        bool: True once successfully downloads the report. Otherwise, function keeps looping.
-        """
-        self.ensure_on_desired_path(REPORT_QUEUE_REPORTWORKS_PAGE_PATH)
-
-        # Pause briefly to give the just-submitted report time to get into the queue
-        time.sleep(5)
-
-        # Confirm that the page has loaded
-        elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
-        elem.click()
-        logging.info('Refresh button on report page has loaded. Refreshing.')
-        
-        while True:
-            # TODO: Add a counter so this function can't get stuck in an infinte loop.
-            try:
-                # Confirm no reports are running
-                self.driver.find_element(By.XPATH, "//p[contains(text(), 'No reports running or pending!')]")
-                
-                # TODO: Is the below refresh necessary when we're refreshing upon first hitting this page?
-                # There is occasional flakiness where the "No reports running or pending!" message 
-                #    shows up but the latest report is not in the list for downloading yet, so refresh 
-                #    the page one more time.
-                time.sleep(1)
-                elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
-                elem.click()
-                time.sleep(1)
-            except NoSuchElementException: # Because reports ARE running
-                time.sleep(5)
-                elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
-                elem.click()
-                logging.info('PowerSchool report is not ready, refreshing and waiting.')
-                time.sleep(3)
-            else:
-                # Download the first report in table
-                queued_reports = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((
-                    By.XPATH, '//*[@id="queuecontent"]/table/tbody/tr[2]/td[8]/a')))
-                download_link = queued_reports.get_attribute('href')
-                original_files_list = os.listdir(destination_directory_path)
-                self.driver.get(download_link) #downloads the file
-                logging.info('PowerSchool report downloaded.')
-                break
-
-        self._wait_for_new_file_in_folder(destination_directory_path, original_files_list)
-        self._rename_recent_file_in_dir(destination_directory_path, file_postfix)
-        logging.info('Successfully renamed the downloaded file.')
-
-        return True
-
-    def download_latest_report_from_report_queue_system(self, destination_directory_path: str = '.', 
-        file_postfix: str = ''):
-        """
-        Navigates to the PowerSchool Report Queue (System), confirms the most recent report is done 
-        generating, and downloads it.
-
-        Parameters:
-        driver: A Selenium WebDriver
-        destination_directory_path: Where to download the PowerSchool report to.
-        file_postfix: Optional postfix to attach to the end of the downloaded file's filename.
-
-        Returns:
-        bool: True if successfully downloads a report, or False if it cannot, either because the 
-            report generated no results from the previously-submitted parameters or the report
-            download page is in a format this function does not handle.
-        """
-        self.ensure_on_desired_path(REPORT_QUEUE_SYSTEM_PAGE_PATH)
-
-        # Pause briefly to give the just-submitted report time to get into the queue
-        time.sleep(5)
-
-        # Confirm that the page has loaded
-        elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
-        elem.click()
-        logging.info('Refresh button on report page has loaded. Refreshing.')
-
-        while True:
-            try:
-                # Try to find a running report
-                self.driver.find_element(By.XPATH, "//td[text()='Running']")
-
-                # If yes, keep going here
-                time.sleep(5)
-                elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
-                elem.click()
-                logging.info('PowerSchool report is not ready, refreshing and waiting.')
-                time.sleep(3)
-            except NoSuchElementException: # Because all reports are done running
-                logging.info('No currently running reports. Downloading the most recently completed report.')
-                break
-
-        top_completed_report_view_link = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH,
-            "//*[@id='content-main']/div[3]/table/tbody/tr[1]/td[a[text()='View']][1]/a"))) 
-            # Note: The above XPATH seems to change a lot as PowerSchool makes changes to which column the link is in.
-            # This is the hard-coded XPATH for the 6th column: '//*[@id="content-main"]/div[3]/table/tbody/tr[1]/td[6]/a'
-            # The above XPATH tries to dynamically determine which column the link is in to be robust to these changes.
-        top_completed_report_view_link.click()
-
-        try:
-            # Look for a result file link
-            logging.info('Looking for the result file link.')
-            download_link = WebDriverWait(self.driver, 10).until(EC.element_to_be_clickable((
-                By.LINK_TEXT, 'Click to Download Result File')))
-            original_files_list = os.listdir(destination_directory_path)
-            download_link.click()
-            logging.info('Downloading PowerSchool report.')
-
-            self._wait_for_new_file_in_folder(destination_directory_path, original_files_list)
-            self._rename_recent_file_in_dir(destination_directory_path, file_postfix)
-            logging.info('Successfully renamed the downloaded file.')
-
-            return True
-        except:
-            try:
-                # If no result file link is found, look for a confirmation that no file was generated
-                WebDriverWait(self.driver, 10).until(EC.element_to_be_clickable((By.XPATH, 
-                    "//h1[text()='No records found']")))
-                logging.info('PowerSchool reports "No records found"')
-                return False
-            except:
-                # TODO: Check for the SCSC validation errors page and download it appropriately
-                logging.info(f"Unable to confirm results. Please check manually for postfix \
-                    {file_postfix}.")
-                self.driver.back()
-                return False
-    
-    def upload_student_csv_quick_import(self, filename):
-        """
-        Uploads a file to Quick Import. Requires your file to
-        1. be a CSV
-        2. have a header row
-        3. have header names that can be auto-matched by PowerSchool
-        4. have a column called "student_number"
-        """
-        
-        import_data = pd.read_csv(filename)
-        final_student_number = import_data.iloc[-1]['student_number']
-        
-        self.upload_csv_quick_import(filename, final_student_number, 'Students')
-        
-    def upload_csv_quick_import(self, filename, final_value, table_name):
-        """
-        Uploads a CSV file to quick import.
-        
-        Arguments:
-        filename: Path to the file.
-        final_value: A value in the final row of the file that can be used to identify
-            when PS is done processing the file.
-        table_name: Exact value of the table name from the PS UI
-        """
-        
-        # Convert the file to a tab-delimited file
-        import_data = pd.read_csv(filename, encoding='mac_roman')
-        
-        new_filename = filename + ".tsv"
-        
-        import_data.to_csv(
-            new_filename,
-            index=False,
-            sep='\t',
-            encoding='mac_roman',
-            # The "CR" option in PS's quick import, which is the default, is in fact "\n"
-            lineterminator = "\r",
-        )
-        
-        self.upload_quick_import(new_filename, final_value, table_name)
-        
-    def upload_quick_import(self, filename, final_value, table_name):
-        """
-        Uploads a tab-delimited file to quick import.
-        
-        Arguments:
-        filename: Path to the file.
-        final_value: A value in the final row of the file that can be used to identify
-            when PS is done processing the file.
-        """
-        
-        # Upload may cover multiple schools, so should be done at the District Office level
-        self.switch_to_school('District Office')
-
-        # Go to Quick Import page
-        self.ensure_on_desired_path('admin/importexport/quickimport/quickimport1.html')
-
-        # Upload to designated table
-        logging.info(f"Selecting {table_name} for table")
-        select_visible_text_in_element_by_id(self.driver, 'filenumber', table_name)
-        
-        # Choose file to upload
-        type_in_element_by_id(self.driver, 'filename', filename)
-
-        # Submit file
-        click_element_by_id(self.driver, 'btnImport')
-
-        # Choose "Check to exclude first row"
-        click_element_by_name(self.driver, 'skipFirstRow')
-
-        # Choose "Update the student's record with the information from the file being imported."
-        click_element_by_id(self.driver, 'rdioc_update')
-
-        # Submit
-        click_element_by_id(self.driver, 'btnSubmit')
-        logging.info("Submitting file")
-
-        # Check that file finished processing
-        logging.info(f'Waiting for student ID #{final_value} to appear to indicate that the file is finished processing.')
-        wait_for_element_containing_specific_text(self.driver, final_value, 60)
-        logging.info('Final student found. Upload file finished processing.')
-        
-    def upload_data_import_manager(self, file_path, table_name, max_processing_wait_time_in_seconds = 60, 
-        override_existing_record = False):
-        """
-        Uploads a tab-delimited file to the Data Import Manager.
-        
-        Arguments:
-        file_path: Path to the tab-delimited file.
-        table_name: The name of the PowerSchool table to upload to.
-        max_processing_wait_time_in_seconds: The maximum number of seconds to wait for the file to processing.
-            The processing check happens every 10 seconds, so this number will be divided by 10 and rounded down
-            to determine how many checks to make. e.g., a value of 35 will check 3 times, which is roughly 30 seconds.
-        override_existing_record: Defaults to False. Submit as True to have the function select the option to override
-            existing records as part of the import. WARNING: Be very careful when using this feature, since overriding 
-            records in PowerSchool requires very precisely formatted files, and if anything is incorrect, the system
-            will likely create duplicate records. Please extensively test the file you are importing.
-        """
-
-        df_row_count = pd.read_csv(file_path)
-        num_data_rows = df_row_count.shape[0]
-
-        if num_data_rows == 0:
-            raise Exception(f'Upload file at path "{file_path}" does not contain any rows of data.')
-
-        num_rows_in_file = num_data_rows + 1 # Add 1 to account for the header row
-
-        logging.info('Switching to the "District Office" for a Data Import Manager upload.')
-        self.switch_to_school('District Office')
-
-        self.ensure_on_desired_path(DATA_IMPORT_MANAGER_PATH)
-
-        logging.info('Choosing the upload file.')
-        type_in_element_by_id(self.driver, 'idFilename', file_path)
-
-        logging.info('Selecting the upload table.')
-        select_visible_text_in_element_by_id(self.driver, 'moduleSelect', table_name)
-        
-        # Need to give the UI a moment to catch up to the fact that a table has been selected.
-        # (The button is already clickable when a table is unselected, but gives an error)
-        time.sleep(5)
-        logging.info('Clicking Next')
-        click_element_by_id(self.driver, 'nextButton0')
-
-        # Brief pause to allow for loading next part of the screen
-        time.sleep(10)
-
-        logging.info('Assuming all fields mapped properly.')
-        click_element_by_id(self.driver, 'nextButton1')
-
-        # WARNING: Be VERY careful when overriding existing records, because PowerSchool can create duplicates if the upload
-        #   file is not precisely what the system expects.
-        if override_existing_record:
-            logging.info('Because override_existing_record was specified as True, clicking the corresponding radio button.')
-            click_element_by_id(self.driver, 'override_existing_value_override')
-
-        logging.info('Beginning import.')
-        click_element_by_id(self.driver, 'btnImport')
-
-        logging.info('Checking for message to indicate processing is complete.')
-        finished_processing_text = f'Processed {num_rows_in_file} out of {num_rows_in_file} records'
-        done_processing = False
-
-        num_of_loops = math.floor(max_processing_wait_time_in_seconds // 10)
-        
-        for i in range(num_of_loops):
-            try:
-                logging.info(f'Check #{i + 1} of {num_of_loops}')
-                wait_for_element_containing_specific_text(self.driver, finished_processing_text, 10)
-                logging.info('File is done processing.')
-                done_processing = True
-                break
-            except:
-                logging.info('Message not found yet. Refreshing.')
-                self.refresh()
-
-        if done_processing == False:
-            raise Exception(f'Something went wrong. File did not finish processing within {max_processing_wait_time_in_seconds} seconds.')
-
-        logging.info('Checking whether all records imported successfully.')
-            
-        successful_import_text = f'Imported:  {num_rows_in_file}'
-        imported_element_text = self.driver.find_element(By.XPATH, '/html/body/div[2]/div[4]/div[2]/div[2]/h3').text 
-        # Using the old wait_for_element_containing_specific_text() function did not work for finding the right message, so the above
-        #    line gets the "Imported:  X" message 
-
-        assert imported_element_text == successful_import_text, 'Import message indicates not all files imported successfully.'
-
-        logging.info('All records imported successfully. Upload is complete.')
-
-    def _log_into_powerschool_admin(self, username, password):
-        """
-        Log into PowerSchool Admin and confirm the login was successful.
-        
-        Parameters:
-        n/a
-            
-        Returns:
-        n/a
-        """
-        
-        logging.info("Create webpage URL for PowerSchool Admin")
-        host_full = self.host + "/" + ADMIN_LOGIN_PAGE_PATH
-        logging.info(f"The webpage url is: {host_full}")
-        
-        logging.info("Go to webpage URL for PowerSchool Admin")
-        self.driver.get(host_full)
-        
-        logging.info("Find the username field within the login page")
-        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
-            'fieldUsername')))
-        
-        logging.info("Clear any pre-filled values within the username field")
-        elem.clear()
-        
-        logging.info("Type your PowerSchool username")
-        elem.send_keys(username)
-        
-        logging.info("Find the password field within the HTML page")
-        elem = self.driver.find_element(By.ID, 'fieldPassword')
-        
-        logging.info("Type your PowerSchool password")
-        elem.send_keys(password)
-        
-        logging.info("Press enter to submit your credentials and complete your login.")
-        elem.send_keys(Keys.RETURN)
-
-        try:
-            logging.info("Waiting for 'Start Page' element to be visible to confirm successful login")
-            elem = WebDriverWait(self.driver, 30).until(EC.visibility_of_element_located((By.XPATH, 
-                "//h1[text()='Start Page']")))
-
-            logging.info("Successful login confirmed!")
-        except:
-            raise Exception("Unable to confirm successful login to PowerSchool. Please check your \
-                credentials.")
-
-    def _get_current_domain(self):
-        """
-        Retrieves the current domain.
-        
-        Parameters:
-        self
-
-        Returns:
-        str: The current domain
-        """
-
-        return self.driver.current_url[8:].split("/",1)[:1][0]
-
-    def _get_current_path(self):
-        """
-        Retrieves the current path, minus the 'https://'.
-        
-        Parameters:
-        self
-
-        Returns:
-        str: The current path
-        """
-
-        return self.driver.current_url[8:].split("/",1)[1:][0]
-
-    def _wait_for_new_file_in_folder(self, folder_path, original_files, max_attempts=20000):
-        """
-        Waits until a new file shows up in a folder. Loops until that is true or max_attempts is 
-        reached.
-
-        Parameters:
-        self
-        folder_path: The folder being monitored.
-        original_files: The list of files originally in the folder, before the new one is added.
-        max_attmepts: Optional parameter that sets how many loops the function will do.
-
-        Returns:
-        n/a
-        """
-        file_added = False
-        attempts = 0
-        while True and attempts < max_attempts:
-            for root, folders, files in os.walk(folder_path):
-                # break 'for' loop if files found
-                if len(files) > len(original_files):
-                    file_added = True
-                    break
-                else:
-                    continue
-            # break 'while' loop if files found
-            if file_added:
-                # wait for download to complete fully after it's been added - hopefully 3 seconds 
-                #    is enough.
-                time.sleep(3)
-                break
-            attempts +=1
-
-    def _rename_recent_file_in_dir(self, folder, append_text):
-        """
-        Gets the most recent file in a folder and appends text to its filename.
-
-        Parameters:
-        self
-        folder: The path of the folder
-        append_text: The text to appended to the filename before the extension.
-
-        Returns:
-        n/a
-        """
-
-        recent_file = get_most_recent_file_in_dir(folder)
-        recent_file = recent_file.replace('\\', '/')
-        new_file, file_ext = os.path.splitext(recent_file)
-        new_file += append_text
-        new_file += file_ext
+import logging
+import time
+import os
+import math
+import pandas as pd
+
+try:
+    from spswarehouse.credentials import powerschool_config
+except ModuleNotFoundError:
+    powerschool_config = None
+    print("No credentials file found in spswarehouse. This could cause issues.")
+
+from ducttape.utils import (
+    DriverBuilder,
+    get_most_recent_file_in_dir,
+)
+
+from spswarehouse.general.selenium import (
+    type_in_element_by_id,
+    select_visible_text_in_element_by_id,
+    click_element_by_id,
+    click_element_by_name,
+    click_element_by_partial_link_text,
+    wait_for_element_containing_specific_text,
+)
+    
+from selenium.webdriver.support.ui import WebDriverWait, Select
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.common.action_chains import ActionChains
+from selenium.common.exceptions import NoSuchElementException
+
+ADMIN_LOGIN_PAGE_PATH = 'admin/pw.html'
+ADMIN_HOME_PAGE_PATH = 'admin/home.html'
+ADMIN_URL_SCHEME = 'https://'
+STATE_REPORTS_PAGE_PATH = 'admin/reports/statereports.html?repType=state'
+REPORT_QUEUE_REPORTWORKS_PAGE_PATH = 'admin/reportqueue/prhome.html'
+REPORT_QUEUE_SYSTEM_PAGE_PATH = 'admin/reportqueue/home.html'
+DATA_IMPORT_MANAGER_PATH = 'admin/datamgmt/importmanager.action'
+
+DEPRECATION_WARNING_MESSAGE = "DEPRECATION_WARNING: This helper function in the PowerSchool class will be deprecated in a future release. Use the helper functions in general.selenium instead."
+
+class PowerSchool:
+    """
+    This class is an abstraction for interacting with the PowerSchool Admin user 
+    interface via Selenium.
+    """
+
+    def __init__(
+        self,
+        config: dict=None,
+        username: str=None,
+        password: str=None,
+        host: str=None,
+        headless: bool=True, 
+        download_location: str='.',
+        chrome_option_prefs: dict=None,
+    ):
+        
+        if config is None:
+            config = powerschool_config
+        
+        if username is None: 
+            username = config['username']
+        else:
+            username = username
+
+        if password is None:
+            password = config['password']
+        else:
+            password = password
+
+        if host is None:
+            self.host = config['host']
+        else:
+            self.host = host
+
+        self.driver = DriverBuilder().get_driver(
+            headless=headless,
+            download_location=download_location,
+            chrome_option_prefs=chrome_option_prefs,
+        )
+        
+        self._log_into_powerschool_admin(username, password)
+
+    def quit(self):
+        self.driver.quit()
+
+    def refresh(self):
+        self.driver.refresh()
+
+    def ensure_on_desired_path(self, desired_path: str):
+        """
+        Checks whether the WebDriver is on the desired path. If not, navigates there.
+        When using this function, consider a WebDriverWait afterwards to confirm the
+        desired page has loaded.
+
+        Parameters:
+        self
+        desired_path: The path to be checked against
+
+        Returns:
+        n/a
+        """
+
+        current_path = self._get_current_path()
+
+        logging.info(f"The current path is: {current_path}")
+
+        if(current_path == desired_path):
+            logging.info("The current path is the desired path. No action taken.")
+        else:
+            logging.info(f"This does not match {desired_path}, so going to that path")
+            self.driver.get('https://' + self._get_current_domain() + "/" + desired_path)
+            time.sleep(3) # Give new page time to load
+            logging.info(f"Moved to {desired_path}.")
+
+    def check_whether_desired_school_selected(self, school_name: str) -> bool:
+        """
+        Checks whether the specified school is currently selected in PowerSchool but
+        takes no action either way.
+
+        Parameters:
+        self
+        school_name: The school name for selecting from the drop-down in the upper-right of the user 
+        interface. Should be the complete school name to avoid incorrect partial matches.
+
+        Returns:
+        bool: True indicates the desired school is selected, and False indicates it is not.
+        """
+
+        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
+            'school_picker_adminSchoolPicker_toggle_btn')))
+
+        elem.click()
+        time.sleep(1)
+
+        selected_element = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((
+            By.CSS_SELECTOR, '.list-item.selectable.selected')))
+
+        school_element_text = selected_element.find_element(By.XPATH, ".//div").text
+
+        result_message = f"Found the {school_name} in the school element text. Match!"
+        outcome = True
+
+        if(school_name not in school_element_text):
+            result_message = f"Did not find {school_name} in the school element text. No match."
+            outcome = False
+
+        logging.info(result_message)
+
+        logging.info(f"Pressing escape to leave dropdown selection.")
+        actions = ActionChains(self.driver)
+        actions.send_keys(Keys.ESCAPE).perform()
+        
+        return outcome
+    
+    def check_whether_desired_school_year_selected(self, school_year_dropdown: str):
+        """
+        Checks whether the specified school year is currently selected in PowerSchool but
+        takes no action either way.
+
+        Parameters:
+        self
+        school_year_dropdown: The exact text of the school year that appears in the dropdown in 
+            PowerSchool. Should be 'XX-YY 20XX-20YY' format.
+
+        Returns:
+        bool: True indicates the desired school year is selected, and False indicates it is not.
+        """
+
+        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
+            'term_picker_adminTermPicker_toggle_btn')))
+
+        elem.click()
+        time.sleep(1)
+
+        selected_element = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((
+            By.CSS_SELECTOR, '.list-item.selectable.selected')))
+
+        school_year_element_text = selected_element.find_element(By.XPATH, ".//div").text
+
+        result_message = f"Found '{school_year_dropdown}' in the school year element text. Match!"
+        outcome = True
+
+        if(school_year_dropdown not in school_year_element_text):
+            result_message = f"Did not find '{school_year_dropdown}' in the school year element text. No match."
+            outcome = False
+
+        logging.info(result_message)
+
+        logging.info(f"Pressing escape to leave dropdown selection.")
+        actions = ActionChains(self.driver)
+        actions.send_keys(Keys.ESCAPE).perform()
+        
+        return outcome
+    
+    def switch_to_school_year(self, school_year_dropdown: str):
+        """
+        Switches to a specified school year in PowerSchool.
+
+        Parameters:
+        self
+        school_year_dropdown: The exact text of the school year that appears in the dropdown in 
+            PowerSchool. Should be 'XX-YY 20XX-20YY' format.
+
+        Returns:
+        n/a
+        """
+        if self.check_whether_desired_school_year_selected(school_year_dropdown) == False:
+            logging.info(f"'{school_year_dropdown}' is not already selected. Selecting now.")
+
+            self.ensure_on_desired_path(ADMIN_HOME_PAGE_PATH)
+
+            logging.info("Waiting for School Year Picker")
+            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
+                'term_picker_adminTermPicker_toggle_btn')))
+            logging.info("School Year Picker found. Click it.")
+
+            elem.click()
+
+            time.sleep(1)
+
+            logging.info("Waiting for School Year Search Field")
+            elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.ID, 
+                'termText')))
+            logging.info("Found School Year Search Field. Typing in school year text.")
+
+            # Only send the XX-YY portion of the dropdown text
+            elem.send_keys(school_year_dropdown[:5])
+
+            time.sleep(1)
+
+            logging.info("Looking for first school year in list")
+            
+            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.XPATH, 
+                "//ul[@id='term_choices']/li[2]"))) # This is li[2] instead of li[1] because there is read-only school year item displayed
+
+            logging.info("Found first school year in results list. Clicking.")
+            elem.click()
+            logging.info("Click. Waiting for page to refresh.")
+            time.sleep(1)
+            
+            assert self.check_whether_desired_school_year_selected(school_year_dropdown), "Failed to select \
+                desired school year."
+        else:
+            logging.info(f"'{school_year_dropdown}' is already selected. No action taken.")
+
+    def switch_to_school(self, school_name: str):
+        """
+        Switches to a specified school in PowerSchool.
+
+        Parameters:
+        self
+        school_name: The school name for selecting from the drop-down in the upper-right of the user 
+            interface. Should be the complete school name to avoid incorrect partial matches.
+
+        Returns:
+        n/a
+        """
+
+        if self.check_whether_desired_school_selected(school_name) == False:
+            logging.info(f"{school_name} is not already selected. Selecting now.")
+
+            self.ensure_on_desired_path(ADMIN_HOME_PAGE_PATH)
+
+            logging.info("Waiting for School Picker")
+            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
+                'school_picker_adminSchoolPicker_toggle_btn')))
+            logging.info("School Picker found. Click it.")
+
+            elem.click()
+
+            time.sleep(1)
+
+            logging.info("Waiting for School Search Field")
+            elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.ID, 
+                'schoolSearchField_value')))
+            logging.info("Found School Search Field. Typing in school name.")
+
+            elem.send_keys(school_name)
+
+            time.sleep(1)
+
+            logging.info("Looking for first school in list")
+            elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.XPATH, 
+                "//ul[@id='school_choices']/li[1]")))
+
+            logging.info("Found first school in results list. Clicking.")
+            elem.click()
+            logging.info("Click. Waiting for page to refresh.")
+            time.sleep(1)
+            
+            assert self.check_whether_desired_school_selected(school_name), "Failed to select \
+                desired school."
+        else:
+            logging.info(f"{school_name} is already selected. No action taken.")
+    
+    def navigate_to_state_reports_page(self):
+        """
+        Navigates to the state reports page in PowerSchool.
+
+        Parameters:
+        self
+        
+        Returns:
+        n/a
+        """
+
+        self.driver.get(ADMIN_URL_SCHEME + self._get_current_domain() + '/' + STATE_REPORTS_PAGE_PATH)
+
+        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.CSS_SELECTOR, 
+            'ul li.selected')))
+        assert elem.text == 'State', "'State' tab is not selected"
+
+    def navigate_to_specific_state_report(self, report_link_text: str):
+        """
+        Navigates to the state reports page in PowerSchool and clicks on the report containing
+        the report_link_text string.
+
+        Parameters:
+        self
+        report_link_text: The string to uniquely identify the report. Can be partial text.
+
+        Returns:
+        n/a
+        """
+        self.navigate_to_state_reports_page()
+
+        click_element_by_partial_link_text(self.driver, report_link_text)
+
+
+
+### START TODO: These helper functions inside the PowerSchool class will be removed in a future release. ##############
+###             The functions in general.selenium should be used instead. #############################################
+
+    def helper_type_in_element_by_id(self, element_id: str, input_to_type: str):
+        """
+        Waits for an element by ID, clears it, and types in the input.
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, element_id)))
+        elem.clear()
+        elem.send_keys(input_to_type)
+
+    def helper_type_in_element_by_name(self, element_name: str, input_to_type: str):
+        """
+        Waits for an element by name, clears it, and types in the input.
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.NAME, 
+            element_name)))
+        elem.clear()
+        elem.send_keys(input_to_type)
+
+    def helper_select_visible_text_in_element_by_id(self, element_id: str, 
+        text_to_select: str):
+        """
+        Waits for an element by ID and selects it by specified text.
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, element_id)))
+        select = Select(elem)
+        select.select_by_visible_text(text_to_select)
+
+    def helper_select_visible_text_in_element_by_name(self, element_name: str, 
+        text_to_select: str):
+        """
+        Waits for an element by name and selects it by specified text.
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.NAME, 
+            element_name)))
+        select = Select(elem)
+        select.select_by_visible_text(text_to_select)
+
+    def helper_click_element_by_id(self, element_id: str):
+        """
+        Waits for an element by ID and clicks it.
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.ID, element_id)))
+        elem.click()
+
+    def helper_click_element_by_name(self, element_name: str):
+        """
+        Waits for an element by name and clicks it.
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.NAME, element_name)))
+        elem.click()
+
+    def helper_click_element_by_partial_link_text(self, partial_link_text: str):
+        """
+        Waits for an element by partial link text and clicks it.
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.PARTIAL_LINK_TEXT, 
+            f"{partial_link_text}")))
+        elem.click()
+
+    def helper_ensure_checkbox_is_checked_by_name(self, checkbox_name: str):
+        """
+        Waits for a checkbox element by name and clicks it if it is not already selected.
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        checkbox = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH, 
+            f"//input[@type='checkbox' and @name='{checkbox_name}']")))
+        
+        if checkbox.is_selected() == False:
+            checkbox.click()
+    
+    def helper_ensure_checkbox_is_unchecked_by_name(self, checkbox_name: str):
+        """
+        Waits for a checkbox element by name and clicks it if it is already selected, to make
+        sure it is not checked.
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        checkbox = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH, 
+            f"//input[@type='checkbox' and @name='{checkbox_name}']")))
+        
+        if checkbox.is_selected():
+            checkbox.click()
+
+    def helper_ensure_element_text_matches_expected_value_by_xpath(self, element_xpath, expected_text):
+        """
+        Waits for an element by XPATH and checks whether its text matches the expected text.
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        elem = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH, 
+            element_xpath)))
+        
+        return elem.text == expected_text
+    
+    def helper_wait_for_element_containing_specific_text(self, expected_element_text, wait_time_in_seconds=30):
+        """
+        Waits for an element containing specific text raises an exception if it does not 
+        appear in the time allotted (default = 30 seconds).
+        """
+        print(DEPRECATION_WARNING_MESSAGE)
+
+        try:
+            WebDriverWait(self.driver, wait_time_in_seconds).until(EC.presence_of_element_located((By.XPATH, f"//*[contains(text(), '{expected_element_text}')]")))
+        except:
+            raise Exception(f'Element with text "{expected_element_text}" not found within {wait_time_in_seconds} seconds.')
+
+### END TODO #########################################################################################################
+
+
+
+    def download_latest_report_from_report_queue_reportworks(self, destination_directory_path: str = '.', 
+        file_postfix: str = ''):
+        """
+        Navigates to the PowerSchool Report Queue (ReportWorks), confirms the most recent report is 
+        done generating, and downloads it.
+
+        Parameters:
+        self
+        destination_directory_path: Where to download the PowerSchool report to.
+        file_postfix: Optional postfix to attach to the end of the downloaded file's filename.
+
+        Returns:
+        bool: True once successfully downloads the report. Otherwise, function keeps looping.
+        """
+        self.ensure_on_desired_path(REPORT_QUEUE_REPORTWORKS_PAGE_PATH)
+
+        # Pause briefly to give the just-submitted report time to get into the queue
+        time.sleep(5)
+
+        # Confirm that the page has loaded
+        elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
+        elem.click()
+        logging.info('Refresh button on report page has loaded. Refreshing.')
+        
+        while True:
+            # TODO: Add a counter so this function can't get stuck in an infinte loop.
+            try:
+                # Confirm no reports are running
+                self.driver.find_element(By.XPATH, "//p[contains(text(), 'No reports running or pending!')]")
+                
+                # TODO: Is the below refresh necessary when we're refreshing upon first hitting this page?
+                # There is occasional flakiness where the "No reports running or pending!" message 
+                #    shows up but the latest report is not in the list for downloading yet, so refresh 
+                #    the page one more time.
+                time.sleep(1)
+                elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
+                elem.click()
+                time.sleep(1)
+            except NoSuchElementException: # Because reports ARE running
+                time.sleep(5)
+                elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
+                elem.click()
+                logging.info('PowerSchool report is not ready, refreshing and waiting.')
+                time.sleep(3)
+            else:
+                # Download the first report in table
+                queued_reports = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((
+                    By.XPATH, '//*[@id="queuecontent"]/table/tbody/tr[2]/td[8]/a')))
+                download_link = queued_reports.get_attribute('href')
+                original_files_list = os.listdir(destination_directory_path)
+                self.driver.get(download_link) #downloads the file
+                logging.info('PowerSchool report downloaded.')
+                break
+
+        self._wait_for_new_file_in_folder(destination_directory_path, original_files_list)
+        self._rename_recent_file_in_dir(destination_directory_path, file_postfix)
+        logging.info('Successfully renamed the downloaded file.')
+
+        return True
+
+    def download_latest_report_from_report_queue_system(self, destination_directory_path: str = '.', 
+        file_postfix: str = ''):
+        """
+        Navigates to the PowerSchool Report Queue (System), confirms the most recent report is done 
+        generating, and downloads it.
+
+        Parameters:
+        driver: A Selenium WebDriver
+        destination_directory_path: Where to download the PowerSchool report to.
+        file_postfix: Optional postfix to attach to the end of the downloaded file's filename.
+
+        Returns:
+        bool: True if successfully downloads a report, or False if it cannot, either because the 
+            report generated no results from the previously-submitted parameters or the report
+            download page is in a format this function does not handle.
+        """
+        self.ensure_on_desired_path(REPORT_QUEUE_SYSTEM_PAGE_PATH)
+
+        # Pause briefly to give the just-submitted report time to get into the queue
+        time.sleep(5)
+
+        # Confirm that the page has loaded
+        elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
+        elem.click()
+        logging.info('Refresh button on report page has loaded. Refreshing.')
+
+        while True:
+            try:
+                # Try to find a running report
+                self.driver.find_element(By.XPATH, "//td[text()='Running']")
+
+                # If yes, keep going here
+                time.sleep(5)
+                elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
+                elem.click()
+                logging.info('PowerSchool report is not ready, refreshing and waiting.')
+                time.sleep(3)
+            except NoSuchElementException: # Because all reports are done running
+                logging.info('No currently running reports. Downloading the most recently completed report.')
+                break
+
+        top_completed_report_view_link = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.XPATH,
+            "//*[@id='content-main']/div[3]/table/tbody/tr[1]/td[a[text()='View']][1]/a"))) 
+            # Note: The above XPATH seems to change a lot as PowerSchool makes changes to which column the link is in.
+            # This is the hard-coded XPATH for the 6th column: '//*[@id="content-main"]/div[3]/table/tbody/tr[1]/td[6]/a'
+            # The above XPATH tries to dynamically determine which column the link is in to be robust to these changes.
+        top_completed_report_view_link.click()
+
+        try:
+            # Look for a result file link
+            logging.info('Looking for the result file link.')
+            download_link = WebDriverWait(self.driver, 10).until(EC.element_to_be_clickable((
+                By.LINK_TEXT, 'Click to Download Result File')))
+            original_files_list = os.listdir(destination_directory_path)
+            download_link.click()
+            logging.info('Downloading PowerSchool report.')
+
+            self._wait_for_new_file_in_folder(destination_directory_path, original_files_list)
+            self._rename_recent_file_in_dir(destination_directory_path, file_postfix)
+            logging.info('Successfully renamed the downloaded file.')
+
+            return True
+        except:
+            try:
+                # If no result file link is found, look for a confirmation that no file was generated
+                WebDriverWait(self.driver, 10).until(EC.element_to_be_clickable((By.XPATH, 
+                    "//h1[text()='No records found']")))
+                logging.info('PowerSchool reports "No records found"')
+                return False
+            except:
+                # TODO: Check for the SCSC validation errors page and download it appropriately
+                logging.info(f"Unable to confirm results. Please check manually for postfix \
+                    {file_postfix}.")
+                self.driver.back()
+                return False
+    
+    def upload_student_csv_quick_import(self, filename):
+        """
+        Uploads a file to Quick Import. Requires your file to
+        1. be a CSV
+        2. have a header row
+        3. have header names that can be auto-matched by PowerSchool
+        4. have a column called "student_number"
+        """
+        
+        import_data = pd.read_csv(filename, dtype=str)
+        final_student_number = import_data.iloc[-1]['student_number']
+        
+        self.upload_csv_quick_import(filename, final_student_number, 'Students')
+        
+    def upload_csv_quick_import(self, filename, final_value, table_name):
+        """
+        Uploads a CSV file to quick import.
+        
+        Arguments:
+        filename: Path to the file.
+        final_value: A value in the final row of the file that can be used to identify
+            when PS is done processing the file.
+        table_name: Exact value of the table name from the PS UI
+        """
+        
+        # Convert the file to a tab-delimited file
+        import_data = pd.read_csv(filename, encoding='mac_roman', dtype=str)
+        
+        new_filename = filename + ".tsv"
+        
+        import_data.to_csv(
+            new_filename,
+            index=False,
+            sep='\t',
+            encoding='mac_roman',
+            # The "CR" option in PS's quick import, which is the default, is in fact "\n"
+            lineterminator = "\r",
+        )
+        
+        self.upload_quick_import(new_filename, final_value, table_name)
+        
+    def upload_quick_import(self, filename, final_value, table_name):
+        """
+        Uploads a tab-delimited file to quick import.
+        
+        Arguments:
+        filename: Path to the file.
+        final_value: A value in the final row of the file that can be used to identify
+            when PS is done processing the file.
+        """
+        
+        # Upload may cover multiple schools, so should be done at the District Office level
+        self.switch_to_school('District Office')
+
+        # Go to Quick Import page
+        self.ensure_on_desired_path('admin/importexport/quickimport/quickimport1.html')
+
+        # Upload to designated table
+        logging.info(f"Selecting {table_name} for table")
+        select_visible_text_in_element_by_id(self.driver, 'filenumber', table_name)
+        
+        # Choose file to upload
+        type_in_element_by_id(self.driver, 'filename', filename)
+
+        # Submit file
+        click_element_by_id(self.driver, 'btnImport')
+
+        # Choose "Check to exclude first row"
+        click_element_by_name(self.driver, 'skipFirstRow')
+
+        # Choose "Update the student's record with the information from the file being imported."
+        click_element_by_id(self.driver, 'rdioc_update')
+
+        # Submit
+        click_element_by_id(self.driver, 'btnSubmit')
+        logging.info("Submitting file")
+
+        # Check that file finished processing
+        logging.info(f'Waiting for student ID #{final_value} to appear to indicate that the file is finished processing.')
+        wait_for_element_containing_specific_text(self.driver, final_value, 60)
+        logging.info('Final student found. Upload file finished processing.')
+        
+    def upload_data_import_manager(self, file_path, table_name, max_processing_wait_time_in_seconds = 60, 
+        override_existing_record = False):
+        """
+        Uploads a tab-delimited file to the Data Import Manager.
+        
+        Arguments:
+        file_path: Path to the tab-delimited file.
+        table_name: The name of the PowerSchool table to upload to.
+        max_processing_wait_time_in_seconds: The maximum number of seconds to wait for the file to processing.
+            The processing check happens every 10 seconds, so this number will be divided by 10 and rounded down
+            to determine how many checks to make. e.g., a value of 35 will check 3 times, which is roughly 30 seconds.
+        override_existing_record: Defaults to False. Submit as True to have the function select the option to override
+            existing records as part of the import. WARNING: Be very careful when using this feature, since overriding 
+            records in PowerSchool requires very precisely formatted files, and if anything is incorrect, the system
+            will likely create duplicate records. Please extensively test the file you are importing.
+        """
+
+        df_row_count = pd.read_csv(file_path)
+        num_data_rows = df_row_count.shape[0]
+
+        if num_data_rows == 0:
+            raise Exception(f'Upload file at path "{file_path}" does not contain any rows of data.')
+
+        num_rows_in_file = num_data_rows + 1 # Add 1 to account for the header row
+
+        logging.info('Switching to the "District Office" for a Data Import Manager upload.')
+        self.switch_to_school('District Office')
+
+        self.ensure_on_desired_path(DATA_IMPORT_MANAGER_PATH)
+
+        logging.info('Choosing the upload file.')
+        type_in_element_by_id(self.driver, 'idFilename', file_path)
+
+        logging.info('Selecting the upload table.')
+        select_visible_text_in_element_by_id(self.driver, 'moduleSelect', table_name)
+        
+        # Need to give the UI a moment to catch up to the fact that a table has been selected.
+        # (The button is already clickable when a table is unselected, but gives an error)
+        time.sleep(5)
+        logging.info('Clicking Next')
+        click_element_by_id(self.driver, 'nextButton0')
+
+        # Brief pause to allow for loading next part of the screen
+        time.sleep(10)
+
+        logging.info('Assuming all fields mapped properly.')
+        click_element_by_id(self.driver, 'nextButton1')
+
+        # WARNING: Be VERY careful when overriding existing records, because PowerSchool can create duplicates if the upload
+        #   file is not precisely what the system expects.
+        if override_existing_record:
+            logging.info('Because override_existing_record was specified as True, clicking the corresponding radio button.')
+            click_element_by_id(self.driver, 'override_existing_value_override')
+
+        logging.info('Beginning import.')
+        click_element_by_id(self.driver, 'btnImport')
+
+        logging.info('Checking for message to indicate processing is complete.')
+        finished_processing_text = f'Processed {num_rows_in_file} out of {num_rows_in_file} records'
+        done_processing = False
+
+        num_of_loops = math.floor(max_processing_wait_time_in_seconds // 10)
+        
+        for i in range(num_of_loops):
+            try:
+                logging.info(f'Check #{i + 1} of {num_of_loops}')
+                wait_for_element_containing_specific_text(self.driver, finished_processing_text, 10)
+                logging.info('File is done processing.')
+                done_processing = True
+                break
+            except:
+                logging.info('Message not found yet. Refreshing.')
+                self.refresh()
+
+        if done_processing == False:
+            raise Exception(f'Something went wrong. File did not finish processing within {max_processing_wait_time_in_seconds} seconds.')
+
+        logging.info('Checking whether all records imported successfully.')
+            
+        successful_import_text = f'Imported:  {num_rows_in_file}'
+        imported_element_text = self.driver.find_element(By.XPATH, '/html/body/div[2]/div[4]/div[2]/div[2]/h3').text 
+        # Using the old wait_for_element_containing_specific_text() function did not work for finding the right message, so the above
+        #    line gets the "Imported:  X" message 
+
+        assert imported_element_text == successful_import_text, 'Import message indicates not all files imported successfully.'
+
+        logging.info('All records imported successfully. Upload is complete.')
+
+    def _log_into_powerschool_admin(self, username, password):
+        """
+        Log into PowerSchool Admin and confirm the login was successful.
+        
+        Parameters:
+        n/a
+            
+        Returns:
+        n/a
+        """
+        
+        logging.info("Create webpage URL for PowerSchool Admin")
+        host_full = self.host + "/" + ADMIN_LOGIN_PAGE_PATH
+        logging.info(f"The webpage url is: {host_full}")
+        
+        logging.info("Go to webpage URL for PowerSchool Admin")
+        self.driver.get(host_full)
+        
+        logging.info("Find the username field within the login page")
+        elem = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.ID, 
+            'fieldUsername')))
+        
+        logging.info("Clear any pre-filled values within the username field")
+        elem.clear()
+        
+        logging.info("Type your PowerSchool username")
+        elem.send_keys(username)
+        
+        logging.info("Find the password field within the HTML page")
+        elem = self.driver.find_element(By.ID, 'fieldPassword')
+        
+        logging.info("Type your PowerSchool password")
+        elem.send_keys(password)
+        
+        logging.info("Press enter to submit your credentials and complete your login.")
+        elem.send_keys(Keys.RETURN)
+
+        try:
+            logging.info("Waiting for 'Start Page' element to be visible to confirm successful login")
+            elem = WebDriverWait(self.driver, 30).until(EC.visibility_of_element_located((By.XPATH, 
+                "//h1[text()='Start Page']")))
+
+            logging.info("Successful login confirmed!")
+        except:
+            raise Exception("Unable to confirm successful login to PowerSchool. Please check your \
+                credentials.")
+
+    def _get_current_domain(self):
+        """
+        Retrieves the current domain.
+        
+        Parameters:
+        self
+
+        Returns:
+        str: The current domain
+        """
+
+        return self.driver.current_url[8:].split("/",1)[:1][0]
+
+    def _get_current_path(self):
+        """
+        Retrieves the current path, minus the 'https://'.
+        
+        Parameters:
+        self
+
+        Returns:
+        str: The current path
+        """
+
+        return self.driver.current_url[8:].split("/",1)[1:][0]
+
+    def _wait_for_new_file_in_folder(self, folder_path, original_files, max_attempts=20000):
+        """
+        Waits until a new file shows up in a folder. Loops until that is true or max_attempts is 
+        reached.
+
+        Parameters:
+        self
+        folder_path: The folder being monitored.
+        original_files: The list of files originally in the folder, before the new one is added.
+        max_attmepts: Optional parameter that sets how many loops the function will do.
+
+        Returns:
+        n/a
+        """
+        file_added = False
+        attempts = 0
+        while True and attempts < max_attempts:
+            for root, folders, files in os.walk(folder_path):
+                # break 'for' loop if files found
+                if len(files) > len(original_files):
+                    file_added = True
+                    break
+                else:
+                    continue
+            # break 'while' loop if files found
+            if file_added:
+                # wait for download to complete fully after it's been added - hopefully 3 seconds 
+                #    is enough.
+                time.sleep(3)
+                break
+            attempts +=1
+
+    def _rename_recent_file_in_dir(self, folder, append_text):
+        """
+        Gets the most recent file in a folder and appends text to its filename.
+
+        Parameters:
+        self
+        folder: The path of the folder
+        append_text: The text to appended to the filename before the extension.
+
+        Returns:
+        n/a
+        """
+
+        recent_file = get_most_recent_file_in_dir(folder)
+        recent_file = recent_file.replace('\\', '/')
+        new_file, file_ext = os.path.splitext(recent_file)
+        new_file += append_text
+        new_file += file_ext
         os.rename(recent_file, new_file)
```

### Comparing `spswarehouse-0.6.1/spswarehouse/powerschool/powerschool_calpads.py` & `spswarehouse-0.6.2/spswarehouse/powerschool/powerschool_calpads.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,693 +1,693 @@
-from datetime import datetime, date
-import time
-import pandas as pd
-
-from .powerschool import PowerSchool
-
-from spswarehouse.general.selenium import (
-    helper_type_in_element_by_name,
-    helper_select_visible_text_in_element_by_name,
-    helper_click_element_by_id,
-    helper_ensure_checkbox_is_unchecked_by_name,
-    helper_ensure_checkbox_is_checked_by_name,
-    helper_type_in_element_by_id,
-    helper_select_visible_text_in_element_by_id,
-    ensure_checkbox_is_checked_by_name,
-    type_in_element_by_name,
-    select_visible_text_in_element_by_name,
-    click_element_by_id,
-)
-
-# Used for making the standard modifications to the Student English Language Acquistion (SELA) upload file; column #'s from the CALPADS file specifications
-SELA_COLUMN_NAMES = [
-    'Record Type Code', # 12.01
-    'Transaction Type Code', # 12.02
-    'Local Record ID', #12.03
-    'Reporting LEA', #12.04
-    'School of Attendance', #12.05
-    'Academic Year ID', #12.06
-    'SSID', #12.07
-    'Student Legal First Name', #12.08
-    'Student Legal Last Name', #12.09
-    'Student Birth Date', #12.10
-    'Student Gender Code', #12.11
-    'Local Student ID', #12.12
-    'English Language Acquisition Status Code', #12.13
-    'English Language Acquisition Status Start Date', #12.14
-    'Primary Language Code', #12.15
-    'Correction Reason Code', #12.16
-]
-
-class PowerSchoolCALPADS(PowerSchool):
-    """
-    This class extends the PowerSchool class in order to download CALPADS
-    reports.
-    """
-    
-    def __init__(
-        self,
-        config: dict=None,
-        username: str=None,
-        password: str=None,
-        host: str=None,
-        headless: bool=True,
-        download_location: str='.',
-        chrome_option_prefs: dict=None,
-    ):
-        super().__init__(config, username, password, host, headless, download_location, chrome_option_prefs)    
-        
-    def download_calpads_report_for_school(self, school_full_name: str, submission_window: str, 
-        calpads_report_abbreviation: str, ps_school_subdistrict_name: str, file_postfix: str, 
-        destination_directory_path: str, report_parameters: dict, ps_school_year_dropdown=None, 
-        validation_only_run: bool=False):
-        """
-        Switches to the desired school in PowerSchool and calls the function to generate the desired
-        report for the specified submission window. Note: This function currently only supports EOY 
-        reports and some All Year reports. Fall 1 and Fall 2 reports should not use this function until 
-        it is expanded.
-        """
-
-        if calpads_report_abbreviation not in self.CALPADS_REPORT_TYPES:
-            raise KeyError(f"{calpads_report_abbreviation} not found in report types")
-            
-        report_kwargs = {
-            'ps_report_link_text': self.CALPADS_REPORT_TYPES[calpads_report_abbreviation]['ps_title'], 
-            'file_postfix': file_postfix, 
-            'destination_directory_path': destination_directory_path, 
-            'report_parameters': report_parameters,
-            'validation_only_run': validation_only_run
-        }
-        
-        # Choose the school year if one is provided
-        if ps_school_year_dropdown is not None:
-            self.switch_to_school_year(ps_school_year_dropdown)
-
-        # The SCSC/SCSE reports need to be run from the District Office level in order to properly generate 
-        #   LEA IDs without dropping leading zeros
-        #   SCSC also requires an additional parameter
-        if calpads_report_abbreviation in ["SCSC", "SCSE"]:
-            self.switch_to_school('District Office')
-            report_kwargs['ps_school_subdistrict_name'] = ps_school_subdistrict_name
-        else:
-            self.switch_to_school(school_full_name)
-
-        # Must pass self to the function explicitly
-        # Howard's note: I'm not certain the cause, but I think it's because the functions in the
-        # dictionary are not (and cannot be) defined as `self.function`, thus requiring that self
-        # be passed explicitly instead
-        return self.CALPADS_REPORT_TYPES[calpads_report_abbreviation]['function'](self, **report_kwargs)
-    
-    # All Year Reports #################
-
-    def _download_all_year_report_for_ssid_enrollment_records_senr(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        validation_only_run: bool=False):
-        """
-        Switches to the SSID Enrollment Records (SENR) report in PowerSchool and downloads it.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Enter specific parameters for this report
-        helper_type_in_element_by_name(self.driver, 'StartDate', 
-            report_parameters['report_start_date'])
-        helper_type_in_element_by_name(self.driver, 'EndDate', 
-            report_parameters['report_end_date'])
-        helper_select_visible_text_in_element_by_name(self.driver, 'submissionMode', 
-            'Non-submission mode (all records)') # Only 'Non-submission mode' is supported by this tool
-        time.sleep(1) # Give page time to react
-        helper_select_visible_text_in_element_by_name(self.driver, 'ssidOption', 
-            report_parameters['student_selection_filter'])
-        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
-            'No' if validation_only_run else 'Yes')
-
-        # Submit report
-        helper_click_element_by_id(self.driver, 'btnSubmit')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
-            file_postfix)
-    
-    def _download_all_year_report_for_student_english_language_acquisition_records_sela(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        validation_only_run: bool=False):
-        """
-        Switches to the Student English Language Acquisition (SELA) report in 
-        PowerSchool and downloads it.
-
-        IMPORTANT NOTE #1: You need to run the remove_sela_records_beginning_before_report_start_date()
-        function on the final text file to filter out any records whose start
-        dates are before your intended report start date. PowerSchool's
-        filtering does not work properly for this.
-
-        IMPORTANT NOTE #2: There is an edge case that this code and PowerSchool 
-        are not equipped to handle. If you have a student who received an English
-        Language Acquisition status at another district before your report_start_date
-        and you store that status in PowerSchool, there is no easy way to decline to
-        report that record to CALPADS. But if you do report that record, CALPADS will
-        reject it and your whole upload file. 
-        
-        For instance, if a student enrolled at another district and received a TBD 
-        status in September and then they joined your district in October, if you 
-        enter that TBD status into PowerSchool, the SELA file will error out in CALPADS.
-        
-        The proper fix is to only include records that start when a student is enrolled
-        with you, but that would be complicated to do through the PowerSchool UI. Summit
-        will likely solve this issue by manually setting any impacted English Language
-        Acquisition statuses to have a start date in PowerSchool of before the school year 
-        begins. That way, they'll be excluded from this tool. If this is a problem for you, 
-        you may want to do something similar or find a way to pull enrollment data into 
-        your code to do additional filtering on the upload file.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-
-        # SELA requires some very specific setup to export in a way that CALPADS will accept. Specifically,
-        #   you can only include students that are currently rostered to you in CALPADS, so this function
-        #   will only pull currently enrolled students or students who were enrolled on the report end date
-        #   if that date is in the past. Usually, the report end date will be the last day of school, so this
-        #   will enable submissions after the school year has ended.
-
-        report_end_date_datetime_object = datetime.strptime(report_parameters['report_end_date'], '%m/%d/%Y').date()
-        today_datetime_object = date.today()
-
-        if today_datetime_object > report_end_date_datetime_object:
-            date_for_report = report_parameters['report_end_date']
-        else:
-            date_for_report = today_datetime_object.strftime('%m/%d/%Y')
-        
-        # Enter specific parameters for this report
-        helper_type_in_element_by_name(self.driver, 'startDate', date_for_report)
-        helper_type_in_element_by_name(self.driver, 'endDate', date_for_report)
-
-        helper_type_in_element_by_name(self.driver, 'status_start_date', '') # Make sure this field is cleared
-        helper_type_in_element_by_name(self.driver, 'status_end_date', '') # Make sure this field is cleared
-
-        helper_select_visible_text_in_element_by_name(self.driver, 'deltaOff', # Unclear why this is the element name
-            'Non-submission mode (all records)') # Only 'Non-submission mode' is supported by this tool
-        time.sleep(1) # Give page time to react
-
-        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
-            'No' if validation_only_run else 'Yes')
-        
-        # Below defaults to "No Group Selected" because school should already be chosen
-        helper_select_visible_text_in_element_by_name(self.driver, 'schoolGroup', '[No Group Selected]') 
-
-        # Submit report
-        helper_click_element_by_id(self.driver, 'btnSubmit')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
-            file_postfix)
-
-    def _download_all_year_report_for_student_information_records_sinf(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        validation_only_run: bool=False):
-        """
-        Switches to the Student Information Records (SINF) report in PowerSchool and downloads it.
-        This function assumes that the export will be run repeatedly over the course of the year
-        and therefore doesn't use the "Check for Fall Submission" functionality. This is because
-        there are occasionally needs for updating SINF outside of Fall 1, such as for Pandemic
-        EBT benefits.
-
-        Uploading an updated SINF file does not seem to close out existing Demographics and
-        Address  records, except when the "Effective Start Date" is greater than the most 
-        recent "Effective Start Date" in CALPADS. Thus, the "Make Effective Start Date Match 
-        Enrollment Start Date" checkbox (described just below) should mean existing records
-        just get updated, rather than new records being created.
-
-        Important notes about how the SINF report parameters in PowerSchool work:
-        - The "Check for Fall Submission" checkbox means it will only submit records for students
-        enrolled on the Census Date that you enter. This function intentionally does not use
-        this setting, so it will guarantee that box is not checked.
-        - The "Make Effective Start Date Match Enrollment Start Date" will give all records the 
-        student's enrollment date for the year as the start date.
-        - The "Start Date" will be the date at which the report looks for enrollments, and it will
-        report data for any student enrolled any time up to the "End Date". The "Effective Start
-        Date" in the final file will be the student's enrollment date for the year, so long as the
-        "Make Effective Start Date Match Enrollment Start Date" box is checked.
-        - The "End Date" cannot be greater than the current date for this report, so this function
-        will enter the report_end_date or the current date, whichever is earlier.
-        - The "Include Students' Preferred Names (If Different From Legal)" will include data in
-        those fields if "Yes" is selected. For student privacy reasons, defaulting to "No" here is 
-        preferred, especially for students whose lived name may differ from their legal name.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Enter specific parameters for this report
-        helper_ensure_checkbox_is_unchecked_by_name(self.driver, 'SubmissionType')
-        time.sleep(1) # Give page time to react
-
-        helper_ensure_checkbox_is_checked_by_name(self.driver, 'effectiveStartDate')
-
-        helper_type_in_element_by_name(self.driver, 'StartDate', 
-            report_parameters['report_start_date'])
-        
-        # If the provided report_end_date is in the future, use today's date instead
-        end_date_string = report_parameters['report_end_date']
-        report_end_date_object = datetime.strptime(end_date_string, '%m/%d/%Y').date()
-        current_date = date.today()
-        if report_end_date_object > current_date:
-            end_date_string = current_date.strftime("%m/%d/%Y")
-        helper_type_in_element_by_name(self.driver, 'EndDate', end_date_string)
-
-        helper_select_visible_text_in_element_by_name(self.driver, 'deltaOff',
-            'Non-submission mode (all records)') # Only 'Non-submission mode' is supported by this tool
-        time.sleep(1) # Give page time to react
-
-        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
-            'No' if validation_only_run else 'Yes')
-        
-        # See note in function definition
-        helper_select_visible_text_in_element_by_name(self.driver, 'includePreferredName', 'No')
-
-        # Submit report
-        helper_click_element_by_id(self.driver, 'btnSubmit')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
-            file_postfix)
-
-
-    # Fall 2 Reports ######################
-
-    def _download_fall_2_report_for_staff_demographics_records_sdem(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        validation_only_run: bool=False):
-        """
-        Switches to the Staff Demographics Records (SDEM) report in PowerSchool and downloads it.
-        Note: This function assumes that the report will be run with data as of Census Day and
-        not using the more general Start Date and End Date parameters.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Check the box to indicate this is a Fall submission
-        ensure_checkbox_is_checked_by_name(self.driver, 'SubmissionType')
-        
-        # Date field needs time to appear
-        time.sleep(1) 
-        type_in_element_by_name(self.driver, 'CensusDate', report_parameters['census_date'])
-        
-        select_visible_text_in_element_by_name(self.driver, 'deltaOff', 'Non-submission mode (all records)')
-        select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
-            'No' if validation_only_run else 'Yes')
-        select_visible_text_in_element_by_name(self.driver, 'schoolGroup', 
-            '[No Group Selected]') 
-
-        # Submit report
-        click_element_by_id(self.driver, 'btnSubmit')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
-            file_postfix)
-
-    def _download_fall_2_report_for_staff_assignment_records_sass(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        validation_only_run: bool=False):
-        """
-        Switches to the Staff Assignment Records (SASS) report in PowerSchool and downloads it.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        type_in_element_by_name(self.driver, 'reportDate', report_parameters['census_date'])
-        
-        select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
-            'No' if validation_only_run else 'Yes')
-        select_visible_text_in_element_by_name(self.driver, 'schoolGroup', 
-            '[No Group Selected]') 
-
-        # Submit report
-        click_element_by_id(self.driver, 'btnSubmit')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
-            file_postfix)
-
-    # TODO: Refactor CRSC/CRSE to be a shared function rather than two totally separate ones
-    def _download_fall2_report_for_course_section_records_crse(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        validation_only_run: bool=False):
-        """
-        Switches to the Course Section Enrollment (CRSE) report in PowerSchool and downloads it.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Enter specific parameters for this report
-        helper_select_visible_text_in_element_by_id(self.driver, 'submission', 
-            report_parameters['submission_type'])
-
-        # Date fields need time to appear
-        time.sleep(1) 
-        helper_select_visible_text_in_element_by_id(self.driver, 'useTracks', 
-            report_parameters['use_tracks'])
-        helper_type_in_element_by_id(self.driver, 'censusDate', 
-            report_parameters['census_date'])
-        helper_select_visible_text_in_element_by_id(self.driver, 'bypassValidation', 
-            'No' if validation_only_run else 'Yes')
-        # The below indicates to not "Include Records For Course Code 1000"
-        helper_select_visible_text_in_element_by_id(self.driver, 'selectCourseCode', 'No') 
-
-        # Submit report
-        helper_click_element_by_id(self.driver, 'submitReportSDKRuntimeParams')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_reportworks(destination_directory_path, 
-            file_postfix)
-
-    # TODO: Make SCSC and SCSE a shared function
-    def _download_fall2_report_for_student_course_section_records_scse(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        ps_school_subdistrict_name:str, validation_only_run: bool=False):
-        """
-        Switches to the Student Course Enrollment (SCSE) report in PowerSchool and downloads it.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Enter specific parameters for this report
-        helper_select_visible_text_in_element_by_name(self.driver, 'submission', 
-            report_parameters['submission_type'])
-        helper_select_visible_text_in_element_by_name(self.driver, 'term', 
-            report_parameters['term'])
-
-        helper_type_in_element_by_name(self.driver, 'censusDate', 
-            report_parameters['census_date'])
-
-        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
-            'No' if validation_only_run else 'Yes')
-        helper_select_visible_text_in_element_by_name(self.driver, 'selectCourseCode', 
-            'No') # Do not "Include Records For Course Code 1000"
-
-        helper_select_visible_text_in_element_by_name(self.driver, 'subDistrict', 
-            ps_school_subdistrict_name)
-
-        # Submit report
-        helper_click_element_by_id(self.driver, 'btnSubmit')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
-            file_postfix)
-    
-    # EOY Reports ######################
-
-    def _download_eoy_report_for_student_incident_records_sinc(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        validation_only_run: bool=False):
-        """
-        Switches to the Student Incident Records (SINC) report in PowerSchool and downloads it.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Enter specific parameters for this report
-        helper_type_in_element_by_id(self.driver, 'reportStartDate', 
-            report_parameters['report_start_date'])
-        helper_type_in_element_by_id(self.driver, 'reportEndDate', 
-            report_parameters['report_end_date'])
-        helper_select_visible_text_in_element_by_id(self.driver, 'reportMode', 
-            'Submission mode') # Only 'Submission mode' is supported by this tool
-        time.sleep(1) # Give page time to react
-        helper_select_visible_text_in_element_by_id(self.driver, 'bypassValidation', 
-            'No' if validation_only_run else 'Yes')
-
-        # Submit report
-        helper_click_element_by_id(self.driver, 'submitReportSDKRuntimeParams')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_reportworks(destination_directory_path, 
-            file_postfix)
-
-    def _download_eoy_report_for_student_incident_results_records_sirs_or_student_offense_records_soff(
-        self, file_postfix: str, destination_directory_path: str, ps_report_link_text: str, 
-        report_parameters: dict, validation_only_run: bool=False):
-        """
-        Switches to the Student Incident Results Records (SIRS) or Student Offense Records (SOFF) 
-        report in PowerSchool and downloads it.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Enter specific parameters for this report
-        helper_type_in_element_by_id(self.driver, 'reportStartDate', 
-            report_parameters['report_start_date'])
-        helper_type_in_element_by_id(self.driver, 'reportEndDate', 
-            report_parameters['report_end_date'])
-        helper_select_visible_text_in_element_by_id(self.driver, 'bypassValidation', 
-            'No' if validation_only_run else 'Yes')
-        
-        # Submit report
-        helper_click_element_by_id(self.driver, 'submitReportSDKRuntimeParams')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_reportworks(destination_directory_path, 
-            file_postfix)
-
-    def _download_eoy_report_for_student_absence_summary_stas(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        validation_only_run: bool=False):
-        """
-        Switches to the Student Absence Summary (STAS) report in PowerSchool and downloads it.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Enter specific parameters for this report
-        helper_type_in_element_by_name(self.driver, 'StartDate', 
-            report_parameters['report_start_date'])
-        helper_type_in_element_by_name(self.driver, 'EndDate', 
-            report_parameters['report_end_date'])
-        # Below 'adaFlag' defaults to 'Yes'
-        helper_select_visible_text_in_element_by_name(self.driver, 'adaFlag', 'Yes') 
-        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
-            'No' if validation_only_run else 'Yes')
-        # Below defaults to "No Group Selected" because school should already be chosen
-        helper_select_visible_text_in_element_by_name(self.driver, 'schoolGroup', 
-            '[No Group Selected]') 
-        
-        # Submit report
-        helper_click_element_by_id(self.driver, 'btnSubmit')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
-            file_postfix)
-
-    def _download_student_program_records_sprg(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        validation_only_run: bool=False):
-        """
-        Switches to the Student Program Records (SPRG) report in PowerSchool and downloads it.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Enter specific parameters for this report
-        helper_type_in_element_by_name(self.driver, 'startDate', 
-            report_parameters['report_start_date'])
-        helper_type_in_element_by_name(self.driver, 'endDate', 
-            report_parameters['report_end_date'])
-        helper_select_visible_text_in_element_by_name(self.driver, 'selectProgs', 
-            report_parameters['submission_type'])
-
-        # I believe 'Non-submission mode (all records)' is the one we want to use for repeated 
-        #   submissions, but there's also 'Replacement Submission Mode' which has a different flow 
-        #   after clicking Submit.
-        helper_select_visible_text_in_element_by_name(self.driver, 'submissionMode', 
-            'Non-submission mode (all records)') 
-
-        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
-            'No' if validation_only_run else 'Yes')
-        # Below defaults to "No Group Selected" because school should already be chosen
-        helper_select_visible_text_in_element_by_name(self.driver, 'schoolGroup', 
-            '[No Group Selected]')
-
-        # Submit report
-        helper_click_element_by_id(self.driver, 'btnSubmit')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
-            file_postfix)
-
-    def _download_eoy_report_for_student_program_records_sprg(self, **kwargs):
-        print("_download_eoy_report_for_student_program_records_sprg deprecated; use _download_student_program_records_sprg")
-        return self._download_student_program_records_sprg(**kwargs)
-    
-    
-    # TODO: Refactor CRSC/CRSE to be a shared function rather than two totally separate ones
-    def _download_eoy_report_for_course_section_records_crsc(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        validation_only_run: bool=False):
-        """
-        Switches to the Course Section Completion (CRSC) report in PowerSchool and downloads it.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Enter specific parameters for this report
-        helper_select_visible_text_in_element_by_id(self.driver, 'submission', 
-            report_parameters['submission_type'])
-
-        # Date fields need time to appear
-        time.sleep(1) 
-        helper_type_in_element_by_id(self.driver, 'startDate', 
-            report_parameters['report_start_date'])
-        helper_type_in_element_by_id(self.driver, 'endDate', 
-            report_parameters['report_end_date'])
-        helper_select_visible_text_in_element_by_id(self.driver, 'bypassValidation', 
-            'No' if validation_only_run else 'Yes')
-        # The below indicates to not "Include Records For Course Code 1000"
-        helper_select_visible_text_in_element_by_id(self.driver, 'selectCourseCode', 'No') 
-
-        # Submit report
-        helper_click_element_by_id(self.driver, 'submitReportSDKRuntimeParams')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_reportworks(destination_directory_path, 
-            file_postfix)
-    
-    # TODO: Make SCSC and SCSE a shared function
-    def _download_eoy_report_for_student_course_section_records_scsc(self, file_postfix: str, 
-        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
-        ps_school_subdistrict_name:str, validation_only_run: bool=False):
-        """
-        Switches to the Student Course Completion (SCSC) report in PowerSchool and downloads it.
-        """
-        self.navigate_to_specific_state_report(ps_report_link_text)
-        
-        # Enter specific parameters for this report
-        helper_select_visible_text_in_element_by_name(self.driver, 'submission', 
-            report_parameters['submission_type'])
-        helper_type_in_element_by_name(self.driver, 'storeCodeList', 
-            report_parameters['eoy_store_code_list'])
-        # Below defaults to 'No' for 'Extract Credits for Grades 7 and 8' 
-        # TODO: Research if this is correct
-        helper_select_visible_text_in_element_by_name(self.driver, 'msExtract', 'No') 
-
-        helper_type_in_element_by_name(self.driver, 'startDate', 
-            report_parameters['report_start_date'])
-        helper_type_in_element_by_name(self.driver, 'endDate', 
-            report_parameters['report_end_date'])
-
-        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
-            'No' if validation_only_run else 'Yes')
-        helper_select_visible_text_in_element_by_name(self.driver, 'selectCourseCode', 
-            'No') # Do not "Include Records For Course Code 1000"
-
-        helper_select_visible_text_in_element_by_name(self.driver, 'subDistrict', 
-            ps_school_subdistrict_name)
-
-        # Submit report
-        helper_click_element_by_id(self.driver, 'btnSubmit')
-
-        # Download report zipfile
-        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
-            file_postfix)
-    
-    CALPADS_REPORT_TYPES = {
-        'CRSC': {
-            'ps_title': 'Course Section Records',
-            'function': _download_eoy_report_for_course_section_records_crsc,
-        },
-        'CRSE': {
-            'ps_title': 'Course Section Records',
-            'function': _download_fall2_report_for_course_section_records_crse,
-        },
-        'SASS': {
-            'ps_title': 'Staff Assignment Records',
-            'function': _download_fall_2_report_for_staff_assignment_records_sass,
-        },
-        'SCSC': {
-            'ps_title': 'Student Course Section Records',
-            'function': _download_eoy_report_for_student_course_section_records_scsc,
-        },
-        'SCSE': {
-            'ps_title': 'Student Course Section Records',
-            'function': _download_fall2_report_for_student_course_section_records_scse,
-        },
-        'SDEM': {
-            'ps_title': 'Staff Demographic Records',
-            'function': _download_fall_2_report_for_staff_demographics_records_sdem,
-        },    
-        'SELA': {
-            'ps_title': 'Student EL Acquisition Records',
-            'function': _download_all_year_report_for_student_english_language_acquisition_records_sela,
-        },
-        'SENR': {
-            'ps_title': 'SSID Enrollment Records',
-            'function': _download_all_year_report_for_ssid_enrollment_records_senr,
-        },
-        'SINC': {
-            'ps_title': 'Student Incident Records (SINC)',
-            'function': _download_eoy_report_for_student_incident_records_sinc,
-        },
-        'SINF': {
-            'ps_title': 'Student Information Records',
-            'function': _download_all_year_report_for_student_information_records_sinf,
-        },
-        'SIRS': {
-            'ps_title': 'Student Incident Results Records (SIRS)',
-            'function': _download_eoy_report_for_student_incident_results_records_sirs_or_student_offense_records_soff,
-        },
-        'SOFF': {
-            'ps_title': 'Student Offense Records (SOFF)',
-            'function': _download_eoy_report_for_student_incident_results_records_sirs_or_student_offense_records_soff,
-        },
-        'SPRG': {
-            'ps_title': 'Student Program Records',
-            'function': _download_student_program_records_sprg,
-        },
-        'STAS': {
-            'ps_title': 'Student Absence Summary',
-            'function': _download_eoy_report_for_student_absence_summary_stas,
-        },
-    }
-    
-# Helper Functions #################
-
-#    Note: These functions are intentionally not in the class, because one may want to access
-#    them separately from downloading files from PowerSchool.
-
-def swap_value_in_column_of_calpads_file(file_path: str, column_names_of_file: list, 
-    column_name_for_swap: str, existing_value: str, new_value: str, encoding: str='utf-8'):
-    """
-    Opens a CALPADS upload file, looks for the existing_value in the provided column and replaces it
-    with the new_value. Writes the new file to the same folder but with "_modified" added to the
-    filename. Returns the new file path.
-
-    Parameters:
-    file_path: The path of the file that needs to be modified.
-    column_names_of_file: A list storing the CALPADS column names for the relevant file. Needs to be 
-        in order and exactly matching the number of columns in the file. File specifications available at: https://www.cde.ca.gov/ds/sp/cl/systemdocs.asp
-    column_name_for_swap: The name of the column being modified.
-    existing_value: The existing value in that column that needs to be swapped out.
-    new_value: The value that will replace the existing_value.
-
-    Returns:
-    str: The path of the modified file
-    """
-
-    df_to_edit = pd.read_csv(file_path, sep='^', header=None, names=column_names_of_file, dtype=str, encoding=encoding)
-
-    df_to_edit.loc[df_to_edit[column_name_for_swap] == existing_value, column_name_for_swap] = new_value
-
-    df_to_edit.fillna('', inplace=True)
-
-    updated_file_path = file_path.replace('.txt', '_modified.txt')
-    df_to_edit.to_csv(updated_file_path, sep='^', header=False, index=False, na_rep='')
-
-    return updated_file_path
-
-def remove_sela_records_beginning_before_report_start_date(sela_file_path: str, 
-    report_start_date: str):
-    """
-    Take the SELA file at the provided path, filter so it contains only the
-    records with an ELA status start date greater than or equal to the report
-    start date, and return the path to the modified file.
-    """
-
-    # Load existing upload file
-    df_to_edit = pd.read_csv(sela_file_path, sep='^', header=None, names=SELA_COLUMN_NAMES, dtype=str, encoding='cp1252')
-
-    # Convert report_start_date to a string in the format of 'YYYYMMDD' to match the upload file column
-    report_start_date_object = datetime.strptime(report_start_date, '%m/%d/%Y')
-    reformatted_report_start_date_string = report_start_date_object.strftime('%Y%m%d')
-
-    # Keep only records greater than or equal to the report_start_date
-    filtered_df = df_to_edit[df_to_edit['English Language Acquisition Status Start Date'] >= reformatted_report_start_date_string]
-
-    # Output new upload file
-    updated_file_path = sela_file_path.replace('.txt', '_modified.txt')
-    filtered_df.to_csv(updated_file_path, sep='^', header=False, index=False, na_rep='')
-
+from datetime import datetime, date
+import time
+import pandas as pd
+
+from .powerschool import PowerSchool
+
+from spswarehouse.general.selenium import (
+    helper_type_in_element_by_name,
+    helper_select_visible_text_in_element_by_name,
+    helper_click_element_by_id,
+    helper_ensure_checkbox_is_unchecked_by_name,
+    helper_ensure_checkbox_is_checked_by_name,
+    helper_type_in_element_by_id,
+    helper_select_visible_text_in_element_by_id,
+    ensure_checkbox_is_checked_by_name,
+    type_in_element_by_name,
+    select_visible_text_in_element_by_name,
+    click_element_by_id,
+)
+
+# Used for making the standard modifications to the Student English Language Acquistion (SELA) upload file; column #'s from the CALPADS file specifications
+SELA_COLUMN_NAMES = [
+    'Record Type Code', # 12.01
+    'Transaction Type Code', # 12.02
+    'Local Record ID', #12.03
+    'Reporting LEA', #12.04
+    'School of Attendance', #12.05
+    'Academic Year ID', #12.06
+    'SSID', #12.07
+    'Student Legal First Name', #12.08
+    'Student Legal Last Name', #12.09
+    'Student Birth Date', #12.10
+    'Student Gender Code', #12.11
+    'Local Student ID', #12.12
+    'English Language Acquisition Status Code', #12.13
+    'English Language Acquisition Status Start Date', #12.14
+    'Primary Language Code', #12.15
+    'Correction Reason Code', #12.16
+]
+
+class PowerSchoolCALPADS(PowerSchool):
+    """
+    This class extends the PowerSchool class in order to download CALPADS
+    reports.
+    """
+    
+    def __init__(
+        self,
+        config: dict=None,
+        username: str=None,
+        password: str=None,
+        host: str=None,
+        headless: bool=True,
+        download_location: str='.',
+        chrome_option_prefs: dict=None,
+    ):
+        super().__init__(config, username, password, host, headless, download_location, chrome_option_prefs)    
+        
+    def download_calpads_report_for_school(self, school_full_name: str, submission_window: str, 
+        calpads_report_abbreviation: str, ps_school_subdistrict_name: str, file_postfix: str, 
+        destination_directory_path: str, report_parameters: dict, ps_school_year_dropdown=None, 
+        validation_only_run: bool=False):
+        """
+        Switches to the desired school in PowerSchool and calls the function to generate the desired
+        report for the specified submission window. Note: This function currently only supports EOY 
+        reports and some All Year reports. Fall 1 and Fall 2 reports should not use this function until 
+        it is expanded.
+        """
+
+        if calpads_report_abbreviation not in self.CALPADS_REPORT_TYPES:
+            raise KeyError(f"{calpads_report_abbreviation} not found in report types")
+            
+        report_kwargs = {
+            'ps_report_link_text': self.CALPADS_REPORT_TYPES[calpads_report_abbreviation]['ps_title'], 
+            'file_postfix': file_postfix, 
+            'destination_directory_path': destination_directory_path, 
+            'report_parameters': report_parameters,
+            'validation_only_run': validation_only_run
+        }
+        
+        # Choose the school year if one is provided
+        if ps_school_year_dropdown is not None:
+            self.switch_to_school_year(ps_school_year_dropdown)
+
+        # The SCSC/SCSE reports need to be run from the District Office level in order to properly generate 
+        #   LEA IDs without dropping leading zeros
+        #   SCSC also requires an additional parameter
+        if calpads_report_abbreviation in ["SCSC", "SCSE"]:
+            self.switch_to_school('District Office')
+            report_kwargs['ps_school_subdistrict_name'] = ps_school_subdistrict_name
+        else:
+            self.switch_to_school(school_full_name)
+
+        # Must pass self to the function explicitly
+        # Howard's note: I'm not certain the cause, but I think it's because the functions in the
+        # dictionary are not (and cannot be) defined as `self.function`, thus requiring that self
+        # be passed explicitly instead
+        return self.CALPADS_REPORT_TYPES[calpads_report_abbreviation]['function'](self, **report_kwargs)
+    
+    # All Year Reports #################
+
+    def _download_all_year_report_for_ssid_enrollment_records_senr(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        validation_only_run: bool=False):
+        """
+        Switches to the SSID Enrollment Records (SENR) report in PowerSchool and downloads it.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Enter specific parameters for this report
+        helper_type_in_element_by_name(self.driver, 'StartDate', 
+            report_parameters['report_start_date'])
+        helper_type_in_element_by_name(self.driver, 'EndDate', 
+            report_parameters['report_end_date'])
+        helper_select_visible_text_in_element_by_name(self.driver, 'submissionMode', 
+            'Non-submission mode (all records)') # Only 'Non-submission mode' is supported by this tool
+        time.sleep(1) # Give page time to react
+        helper_select_visible_text_in_element_by_name(self.driver, 'ssidOption', 
+            report_parameters['student_selection_filter'])
+        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
+            'No' if validation_only_run else 'Yes')
+
+        # Submit report
+        helper_click_element_by_id(self.driver, 'btnSubmit')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
+            file_postfix)
+    
+    def _download_all_year_report_for_student_english_language_acquisition_records_sela(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        validation_only_run: bool=False):
+        """
+        Switches to the Student English Language Acquisition (SELA) report in 
+        PowerSchool and downloads it.
+
+        IMPORTANT NOTE #1: You need to run the remove_sela_records_beginning_before_report_start_date()
+        function on the final text file to filter out any records whose start
+        dates are before your intended report start date. PowerSchool's
+        filtering does not work properly for this.
+
+        IMPORTANT NOTE #2: There is an edge case that this code and PowerSchool 
+        are not equipped to handle. If you have a student who received an English
+        Language Acquisition status at another district before your report_start_date
+        and you store that status in PowerSchool, there is no easy way to decline to
+        report that record to CALPADS. But if you do report that record, CALPADS will
+        reject it and your whole upload file. 
+        
+        For instance, if a student enrolled at another district and received a TBD 
+        status in September and then they joined your district in October, if you 
+        enter that TBD status into PowerSchool, the SELA file will error out in CALPADS.
+        
+        The proper fix is to only include records that start when a student is enrolled
+        with you, but that would be complicated to do through the PowerSchool UI. Summit
+        will likely solve this issue by manually setting any impacted English Language
+        Acquisition statuses to have a start date in PowerSchool of before the school year 
+        begins. That way, they'll be excluded from this tool. If this is a problem for you, 
+        you may want to do something similar or find a way to pull enrollment data into 
+        your code to do additional filtering on the upload file.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+
+        # SELA requires some very specific setup to export in a way that CALPADS will accept. Specifically,
+        #   you can only include students that are currently rostered to you in CALPADS, so this function
+        #   will only pull currently enrolled students or students who were enrolled on the report end date
+        #   if that date is in the past. Usually, the report end date will be the last day of school, so this
+        #   will enable submissions after the school year has ended.
+
+        report_end_date_datetime_object = datetime.strptime(report_parameters['report_end_date'], '%m/%d/%Y').date()
+        today_datetime_object = date.today()
+
+        if today_datetime_object > report_end_date_datetime_object:
+            date_for_report = report_parameters['report_end_date']
+        else:
+            date_for_report = today_datetime_object.strftime('%m/%d/%Y')
+        
+        # Enter specific parameters for this report
+        helper_type_in_element_by_name(self.driver, 'startDate', date_for_report)
+        helper_type_in_element_by_name(self.driver, 'endDate', date_for_report)
+
+        helper_type_in_element_by_name(self.driver, 'status_start_date', '') # Make sure this field is cleared
+        helper_type_in_element_by_name(self.driver, 'status_end_date', '') # Make sure this field is cleared
+
+        helper_select_visible_text_in_element_by_name(self.driver, 'deltaOff', # Unclear why this is the element name
+            'Non-submission mode (all records)') # Only 'Non-submission mode' is supported by this tool
+        time.sleep(1) # Give page time to react
+
+        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
+            'No' if validation_only_run else 'Yes')
+        
+        # Below defaults to "No Group Selected" because school should already be chosen
+        helper_select_visible_text_in_element_by_name(self.driver, 'schoolGroup', '[No Group Selected]') 
+
+        # Submit report
+        helper_click_element_by_id(self.driver, 'btnSubmit')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
+            file_postfix)
+
+    def _download_all_year_report_for_student_information_records_sinf(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        validation_only_run: bool=False):
+        """
+        Switches to the Student Information Records (SINF) report in PowerSchool and downloads it.
+        This function assumes that the export will be run repeatedly over the course of the year
+        and therefore doesn't use the "Check for Fall Submission" functionality. This is because
+        there are occasionally needs for updating SINF outside of Fall 1, such as for Pandemic
+        EBT benefits.
+
+        Uploading an updated SINF file does not seem to close out existing Demographics and
+        Address  records, except when the "Effective Start Date" is greater than the most 
+        recent "Effective Start Date" in CALPADS. Thus, the "Make Effective Start Date Match 
+        Enrollment Start Date" checkbox (described just below) should mean existing records
+        just get updated, rather than new records being created.
+
+        Important notes about how the SINF report parameters in PowerSchool work:
+        - The "Check for Fall Submission" checkbox means it will only submit records for students
+        enrolled on the Census Date that you enter. This function intentionally does not use
+        this setting, so it will guarantee that box is not checked.
+        - The "Make Effective Start Date Match Enrollment Start Date" will give all records the 
+        student's enrollment date for the year as the start date.
+        - The "Start Date" will be the date at which the report looks for enrollments, and it will
+        report data for any student enrolled any time up to the "End Date". The "Effective Start
+        Date" in the final file will be the student's enrollment date for the year, so long as the
+        "Make Effective Start Date Match Enrollment Start Date" box is checked.
+        - The "End Date" cannot be greater than the current date for this report, so this function
+        will enter the report_end_date or the current date, whichever is earlier.
+        - The "Include Students' Preferred Names (If Different From Legal)" will include data in
+        those fields if "Yes" is selected. For student privacy reasons, defaulting to "No" here is 
+        preferred, especially for students whose lived name may differ from their legal name.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Enter specific parameters for this report
+        helper_ensure_checkbox_is_unchecked_by_name(self.driver, 'SubmissionType')
+        time.sleep(1) # Give page time to react
+
+        helper_ensure_checkbox_is_checked_by_name(self.driver, 'effectiveStartDate')
+
+        helper_type_in_element_by_name(self.driver, 'StartDate', 
+            report_parameters['report_start_date'])
+        
+        # If the provided report_end_date is in the future, use today's date instead
+        end_date_string = report_parameters['report_end_date']
+        report_end_date_object = datetime.strptime(end_date_string, '%m/%d/%Y').date()
+        current_date = date.today()
+        if report_end_date_object > current_date:
+            end_date_string = current_date.strftime("%m/%d/%Y")
+        helper_type_in_element_by_name(self.driver, 'EndDate', end_date_string)
+
+        helper_select_visible_text_in_element_by_name(self.driver, 'deltaOff',
+            'Non-submission mode (all records)') # Only 'Non-submission mode' is supported by this tool
+        time.sleep(1) # Give page time to react
+
+        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
+            'No' if validation_only_run else 'Yes')
+        
+        # See note in function definition
+        helper_select_visible_text_in_element_by_name(self.driver, 'includePreferredName', 'No')
+
+        # Submit report
+        helper_click_element_by_id(self.driver, 'btnSubmit')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
+            file_postfix)
+
+
+    # Fall 2 Reports ######################
+
+    def _download_fall_2_report_for_staff_demographics_records_sdem(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        validation_only_run: bool=False):
+        """
+        Switches to the Staff Demographics Records (SDEM) report in PowerSchool and downloads it.
+        Note: This function assumes that the report will be run with data as of Census Day and
+        not using the more general Start Date and End Date parameters.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Check the box to indicate this is a Fall submission
+        ensure_checkbox_is_checked_by_name(self.driver, 'SubmissionType')
+        
+        # Date field needs time to appear
+        time.sleep(1) 
+        type_in_element_by_name(self.driver, 'CensusDate', report_parameters['census_date'])
+        
+        select_visible_text_in_element_by_name(self.driver, 'deltaOff', 'Non-submission mode (all records)')
+        select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
+            'No' if validation_only_run else 'Yes')
+        select_visible_text_in_element_by_name(self.driver, 'schoolGroup', 
+            '[No Group Selected]') 
+
+        # Submit report
+        click_element_by_id(self.driver, 'btnSubmit')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
+            file_postfix)
+
+    def _download_fall_2_report_for_staff_assignment_records_sass(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        validation_only_run: bool=False):
+        """
+        Switches to the Staff Assignment Records (SASS) report in PowerSchool and downloads it.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        type_in_element_by_name(self.driver, 'reportDate', report_parameters['census_date'])
+        
+        select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
+            'No' if validation_only_run else 'Yes')
+        select_visible_text_in_element_by_name(self.driver, 'schoolGroup', 
+            '[No Group Selected]') 
+
+        # Submit report
+        click_element_by_id(self.driver, 'btnSubmit')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
+            file_postfix)
+
+    # TODO: Refactor CRSC/CRSE to be a shared function rather than two totally separate ones
+    def _download_fall2_report_for_course_section_records_crse(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        validation_only_run: bool=False):
+        """
+        Switches to the Course Section Enrollment (CRSE) report in PowerSchool and downloads it.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Enter specific parameters for this report
+        helper_select_visible_text_in_element_by_id(self.driver, 'submission', 
+            report_parameters['submission_type'])
+
+        # Date fields need time to appear
+        time.sleep(1) 
+        helper_select_visible_text_in_element_by_id(self.driver, 'useTracks', 
+            report_parameters['use_tracks'])
+        helper_type_in_element_by_id(self.driver, 'censusDate', 
+            report_parameters['census_date'])
+        helper_select_visible_text_in_element_by_id(self.driver, 'bypassValidation', 
+            'No' if validation_only_run else 'Yes')
+        # The below indicates to not "Include Records For Course Code 1000"
+        helper_select_visible_text_in_element_by_id(self.driver, 'selectCourseCode', 'No') 
+
+        # Submit report
+        helper_click_element_by_id(self.driver, 'submitReportSDKRuntimeParams')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_reportworks(destination_directory_path, 
+            file_postfix)
+
+    # TODO: Make SCSC and SCSE a shared function
+    def _download_fall2_report_for_student_course_section_records_scse(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        ps_school_subdistrict_name:str, validation_only_run: bool=False):
+        """
+        Switches to the Student Course Enrollment (SCSE) report in PowerSchool and downloads it.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Enter specific parameters for this report
+        helper_select_visible_text_in_element_by_name(self.driver, 'submission', 
+            report_parameters['submission_type'])
+        helper_select_visible_text_in_element_by_name(self.driver, 'term', 
+            report_parameters['term'])
+
+        helper_type_in_element_by_name(self.driver, 'censusDate', 
+            report_parameters['census_date'])
+
+        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
+            'No' if validation_only_run else 'Yes')
+        helper_select_visible_text_in_element_by_name(self.driver, 'selectCourseCode', 
+            'No') # Do not "Include Records For Course Code 1000"
+
+        helper_select_visible_text_in_element_by_name(self.driver, 'subDistrict', 
+            ps_school_subdistrict_name)
+
+        # Submit report
+        helper_click_element_by_id(self.driver, 'btnSubmit')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
+            file_postfix)
+    
+    # EOY Reports ######################
+
+    def _download_eoy_report_for_student_incident_records_sinc(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        validation_only_run: bool=False):
+        """
+        Switches to the Student Incident Records (SINC) report in PowerSchool and downloads it.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Enter specific parameters for this report
+        helper_type_in_element_by_id(self.driver, 'reportStartDate', 
+            report_parameters['report_start_date'])
+        helper_type_in_element_by_id(self.driver, 'reportEndDate', 
+            report_parameters['report_end_date'])
+        helper_select_visible_text_in_element_by_id(self.driver, 'reportMode', 
+            'Submission mode') # Only 'Submission mode' is supported by this tool
+        time.sleep(1) # Give page time to react
+        helper_select_visible_text_in_element_by_id(self.driver, 'bypassValidation', 
+            'No' if validation_only_run else 'Yes')
+
+        # Submit report
+        helper_click_element_by_id(self.driver, 'submitReportSDKRuntimeParams')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_reportworks(destination_directory_path, 
+            file_postfix)
+
+    def _download_eoy_report_for_student_incident_results_records_sirs_or_student_offense_records_soff(
+        self, file_postfix: str, destination_directory_path: str, ps_report_link_text: str, 
+        report_parameters: dict, validation_only_run: bool=False):
+        """
+        Switches to the Student Incident Results Records (SIRS) or Student Offense Records (SOFF) 
+        report in PowerSchool and downloads it.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Enter specific parameters for this report
+        helper_type_in_element_by_id(self.driver, 'reportStartDate', 
+            report_parameters['report_start_date'])
+        helper_type_in_element_by_id(self.driver, 'reportEndDate', 
+            report_parameters['report_end_date'])
+        helper_select_visible_text_in_element_by_id(self.driver, 'bypassValidation', 
+            'No' if validation_only_run else 'Yes')
+        
+        # Submit report
+        helper_click_element_by_id(self.driver, 'submitReportSDKRuntimeParams')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_reportworks(destination_directory_path, 
+            file_postfix)
+
+    def _download_eoy_report_for_student_absence_summary_stas(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        validation_only_run: bool=False):
+        """
+        Switches to the Student Absence Summary (STAS) report in PowerSchool and downloads it.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Enter specific parameters for this report
+        helper_type_in_element_by_name(self.driver, 'StartDate', 
+            report_parameters['report_start_date'])
+        helper_type_in_element_by_name(self.driver, 'EndDate', 
+            report_parameters['report_end_date'])
+        # Below 'adaFlag' defaults to 'Yes'
+        helper_select_visible_text_in_element_by_name(self.driver, 'adaFlag', 'Yes') 
+        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
+            'No' if validation_only_run else 'Yes')
+        # Below defaults to "No Group Selected" because school should already be chosen
+        helper_select_visible_text_in_element_by_name(self.driver, 'schoolGroup', 
+            '[No Group Selected]') 
+        
+        # Submit report
+        helper_click_element_by_id(self.driver, 'btnSubmit')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
+            file_postfix)
+
+    def _download_student_program_records_sprg(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        validation_only_run: bool=False):
+        """
+        Switches to the Student Program Records (SPRG) report in PowerSchool and downloads it.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Enter specific parameters for this report
+        helper_type_in_element_by_name(self.driver, 'startDate', 
+            report_parameters['report_start_date'])
+        helper_type_in_element_by_name(self.driver, 'endDate', 
+            report_parameters['report_end_date'])
+        helper_select_visible_text_in_element_by_name(self.driver, 'selectProgs', 
+            report_parameters['submission_type'])
+
+        # I believe 'Non-submission mode (all records)' is the one we want to use for repeated 
+        #   submissions, but there's also 'Replacement Submission Mode' which has a different flow 
+        #   after clicking Submit.
+        helper_select_visible_text_in_element_by_name(self.driver, 'submissionMode', 
+            'Non-submission mode (all records)') 
+
+        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
+            'No' if validation_only_run else 'Yes')
+        # Below defaults to "No Group Selected" because school should already be chosen
+        helper_select_visible_text_in_element_by_name(self.driver, 'schoolGroup', 
+            '[No Group Selected]')
+
+        # Submit report
+        helper_click_element_by_id(self.driver, 'btnSubmit')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
+            file_postfix)
+
+    def _download_eoy_report_for_student_program_records_sprg(self, **kwargs):
+        print("_download_eoy_report_for_student_program_records_sprg deprecated; use _download_student_program_records_sprg")
+        return self._download_student_program_records_sprg(**kwargs)
+    
+    
+    # TODO: Refactor CRSC/CRSE to be a shared function rather than two totally separate ones
+    def _download_eoy_report_for_course_section_records_crsc(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        validation_only_run: bool=False):
+        """
+        Switches to the Course Section Completion (CRSC) report in PowerSchool and downloads it.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Enter specific parameters for this report
+        helper_select_visible_text_in_element_by_id(self.driver, 'submission', 
+            report_parameters['submission_type'])
+
+        # Date fields need time to appear
+        time.sleep(1) 
+        helper_type_in_element_by_id(self.driver, 'startDate', 
+            report_parameters['report_start_date'])
+        helper_type_in_element_by_id(self.driver, 'endDate', 
+            report_parameters['report_end_date'])
+        helper_select_visible_text_in_element_by_id(self.driver, 'bypassValidation', 
+            'No' if validation_only_run else 'Yes')
+        # The below indicates to not "Include Records For Course Code 1000"
+        helper_select_visible_text_in_element_by_id(self.driver, 'selectCourseCode', 'No') 
+
+        # Submit report
+        helper_click_element_by_id(self.driver, 'submitReportSDKRuntimeParams')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_reportworks(destination_directory_path, 
+            file_postfix)
+    
+    # TODO: Make SCSC and SCSE a shared function
+    def _download_eoy_report_for_student_course_section_records_scsc(self, file_postfix: str, 
+        destination_directory_path: str, ps_report_link_text: str, report_parameters: dict, 
+        ps_school_subdistrict_name:str, validation_only_run: bool=False):
+        """
+        Switches to the Student Course Completion (SCSC) report in PowerSchool and downloads it.
+        """
+        self.navigate_to_specific_state_report(ps_report_link_text)
+        
+        # Enter specific parameters for this report
+        helper_select_visible_text_in_element_by_name(self.driver, 'submission', 
+            report_parameters['submission_type'])
+        helper_type_in_element_by_name(self.driver, 'storeCodeList', 
+            report_parameters['eoy_store_code_list'])
+        # Below defaults to 'No' for 'Extract Credits for Grades 7 and 8' 
+        # TODO: Research if this is correct
+        helper_select_visible_text_in_element_by_name(self.driver, 'msExtract', 'No') 
+
+        helper_type_in_element_by_name(self.driver, 'startDate', 
+            report_parameters['report_start_date'])
+        helper_type_in_element_by_name(self.driver, 'endDate', 
+            report_parameters['report_end_date'])
+
+        helper_select_visible_text_in_element_by_name(self.driver, 'bypass_validation', 
+            'No' if validation_only_run else 'Yes')
+        helper_select_visible_text_in_element_by_name(self.driver, 'selectCourseCode', 
+            'No') # Do not "Include Records For Course Code 1000"
+
+        helper_select_visible_text_in_element_by_name(self.driver, 'subDistrict', 
+            ps_school_subdistrict_name)
+
+        # Submit report
+        helper_click_element_by_id(self.driver, 'btnSubmit')
+
+        # Download report zipfile
+        return self.download_latest_report_from_report_queue_system(destination_directory_path, 
+            file_postfix)
+    
+    CALPADS_REPORT_TYPES = {
+        'CRSC': {
+            'ps_title': 'Course Section Records',
+            'function': _download_eoy_report_for_course_section_records_crsc,
+        },
+        'CRSE': {
+            'ps_title': 'Course Section Records',
+            'function': _download_fall2_report_for_course_section_records_crse,
+        },
+        'SASS': {
+            'ps_title': 'Staff Assignment Records',
+            'function': _download_fall_2_report_for_staff_assignment_records_sass,
+        },
+        'SCSC': {
+            'ps_title': 'Student Course Section Records',
+            'function': _download_eoy_report_for_student_course_section_records_scsc,
+        },
+        'SCSE': {
+            'ps_title': 'Student Course Section Records',
+            'function': _download_fall2_report_for_student_course_section_records_scse,
+        },
+        'SDEM': {
+            'ps_title': 'Staff Demographic Records',
+            'function': _download_fall_2_report_for_staff_demographics_records_sdem,
+        },    
+        'SELA': {
+            'ps_title': 'Student EL Acquisition Records',
+            'function': _download_all_year_report_for_student_english_language_acquisition_records_sela,
+        },
+        'SENR': {
+            'ps_title': 'SSID Enrollment Records',
+            'function': _download_all_year_report_for_ssid_enrollment_records_senr,
+        },
+        'SINC': {
+            'ps_title': 'Student Incident Records (SINC)',
+            'function': _download_eoy_report_for_student_incident_records_sinc,
+        },
+        'SINF': {
+            'ps_title': 'Student Information Records',
+            'function': _download_all_year_report_for_student_information_records_sinf,
+        },
+        'SIRS': {
+            'ps_title': 'Student Incident Results Records (SIRS)',
+            'function': _download_eoy_report_for_student_incident_results_records_sirs_or_student_offense_records_soff,
+        },
+        'SOFF': {
+            'ps_title': 'Student Offense Records (SOFF)',
+            'function': _download_eoy_report_for_student_incident_results_records_sirs_or_student_offense_records_soff,
+        },
+        'SPRG': {
+            'ps_title': 'Student Program Records',
+            'function': _download_student_program_records_sprg,
+        },
+        'STAS': {
+            'ps_title': 'Student Absence Summary',
+            'function': _download_eoy_report_for_student_absence_summary_stas,
+        },
+    }
+    
+# Helper Functions #################
+
+#    Note: These functions are intentionally not in the class, because one may want to access
+#    them separately from downloading files from PowerSchool.
+
+def swap_value_in_column_of_calpads_file(file_path: str, column_names_of_file: list, 
+    column_name_for_swap: str, existing_value: str, new_value: str, encoding: str='utf-8'):
+    """
+    Opens a CALPADS upload file, looks for the existing_value in the provided column and replaces it
+    with the new_value. Writes the new file to the same folder but with "_modified" added to the
+    filename. Returns the new file path.
+
+    Parameters:
+    file_path: The path of the file that needs to be modified.
+    column_names_of_file: A list storing the CALPADS column names for the relevant file. Needs to be 
+        in order and exactly matching the number of columns in the file. File specifications available at: https://www.cde.ca.gov/ds/sp/cl/systemdocs.asp
+    column_name_for_swap: The name of the column being modified.
+    existing_value: The existing value in that column that needs to be swapped out.
+    new_value: The value that will replace the existing_value.
+
+    Returns:
+    str: The path of the modified file
+    """
+
+    df_to_edit = pd.read_csv(file_path, sep='^', header=None, names=column_names_of_file, dtype=str, encoding=encoding)
+
+    df_to_edit.loc[df_to_edit[column_name_for_swap] == existing_value, column_name_for_swap] = new_value
+
+    df_to_edit.fillna('', inplace=True)
+
+    updated_file_path = file_path.replace('.txt', '_modified.txt')
+    df_to_edit.to_csv(updated_file_path, sep='^', header=False, index=False, na_rep='')
+
+    return updated_file_path
+
+def remove_sela_records_beginning_before_report_start_date(sela_file_path: str, 
+    report_start_date: str):
+    """
+    Take the SELA file at the provided path, filter so it contains only the
+    records with an ELA status start date greater than or equal to the report
+    start date, and return the path to the modified file.
+    """
+
+    # Load existing upload file
+    df_to_edit = pd.read_csv(sela_file_path, sep='^', header=None, names=SELA_COLUMN_NAMES, dtype=str, encoding='cp1252')
+
+    # Convert report_start_date to a string in the format of 'YYYYMMDD' to match the upload file column
+    report_start_date_object = datetime.strptime(report_start_date, '%m/%d/%Y')
+    reformatted_report_start_date_string = report_start_date_object.strftime('%Y%m%d')
+
+    # Keep only records greater than or equal to the report_start_date
+    filtered_df = df_to_edit[df_to_edit['English Language Acquisition Status Start Date'] >= reformatted_report_start_date_string]
+
+    # Output new upload file
+    updated_file_path = sela_file_path.replace('.txt', '_modified.txt')
+    filtered_df.to_csv(updated_file_path, sep='^', header=False, index=False, na_rep='')
+
     return updated_file_path
```

### Comparing `spswarehouse-0.6.1/spswarehouse/powerschool/student_passwords.py` & `spswarehouse-0.6.2/spswarehouse/powerschool/student_passwords.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import logging
-import time
-import os
-
-try:
-    from spswarehouse.credentials import powerschool_config
-except ModuleNotFoundError:
-    print("No credentials file found in spswarehouse. This could cause issues.")
-
-from ducttape.utils import (
-    DriverBuilder,
-    get_most_recent_file_in_dir,
-)
-    
-from selenium.webdriver import Chrome
-from selenium.webdriver.chrome import webdriver as chrome_webdriver
-from selenium.webdriver.support.ui import WebDriverWait, Select
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.common.action_chains import ActionChains
-from selenium.common.exceptions import NoSuchElementException
-
-STUDENT_URL_PATH = 'public'
-
-class PSStudentPassword:
-    """
-    A class for interacting with the Student UI for PowerSchool in order to reset
-    passwords.
-    """
-    
-    def __init__(self, host: str=None, headless: bool=True, wait_time: int=30,
-        download_location: str='.'):
-        
-        if host is None:
-            self.host = powerschool_config['host']
-        else:
-            self.host = host
-        
-        self.wait_time = wait_time
-
-        self.student_url = self.host + '/' + STUDENT_URL_PATH
-        self.driver = DriverBuilder().get_driver(headless=headless, download_location=download_location)
-        
-    def reset_student(self, username: str, old_password: str, new_password: str):
-        self._login(username, old_password)
-        
-        try:
-            self._wait_by_name("newCredential")
-        except:
-            logging.info(f"Username: {username} - password change screen did not load. Skipping.")
-            try:
-                self._logout()
-            except:
-                pass
-            return False
-        
-        self._find_by_name_and_send("currentCredential", old_password)
-        self._find_by_name_and_send("newCredential", new_password)
-        new_pw_box2 = self._find_by_name_and_send("newCredential1", new_password)
-        new_pw_box2.send_keys(Keys.RETURN)
-        
-        try:
-            self._logout()
-        except:
-            reused_pw_message = self.driver.find_element(By.XPATH, '//*[@id="content"]/ul/li/span')
-            if reused_pw_message.text == 'The password entered was previously used. Please enter a new password':
-                logging.info(f"Username: {username} - repeated password. Skipping.")
-                return False
-            
-        self._login(username, new_password)
-        
-        try:
-            self._logout()
-            return True
-        except:
-            logging.info(f"Username: {username} - new password failed to login.")
-            return False
-            
-    def _login(self, username: str, password: str):
-        self.driver.get(self.student_url)
-        
-        try:
-            username_elem = self._wait_by_id("fieldAccount")
-        except:
-            self._logout()
-            username_elem = self._wait_by_id("fieldAccount")
-        
-        username_elem.send_keys(username)
-        pw_box = self._find_by_id_and_send("fieldPassword", password)
-        pw_box.send_keys(Keys.RETURN)
-            
-    def _logout(self):
-        logout_button = self._wait_by_id("btnLogout")
-        logout_button.click()
-    
-    def _find_by_id_and_send(self, field_id, entry):
-        elem = self.driver.find_element(By.ID, field_id)
-        elem.send_keys(entry)
-        return elem
-    
-    def _find_by_name_and_send(self, field_name, entry):
-        elem = self.driver.find_element(By.NAME, field_name)
-        elem.send_keys(entry)
-        return elem
-    
-    def _wait_by_id(self, elem_id):
-        return WebDriverWait(self.driver, self.wait_time).until(
-            EC.presence_of_element_located((By.ID, elem_id))
-        )
-    
-    def _wait_by_name(self, elem_name):
-        return WebDriverWait(self.driver, self.wait_time).until(
-            EC.presence_of_element_located((By.NAME, elem_name))
+import logging
+import time
+import os
+
+try:
+    from spswarehouse.credentials import powerschool_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
+
+from ducttape.utils import (
+    DriverBuilder,
+    get_most_recent_file_in_dir,
+)
+    
+from selenium.webdriver import Chrome
+from selenium.webdriver.chrome import webdriver as chrome_webdriver
+from selenium.webdriver.support.ui import WebDriverWait, Select
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.common.action_chains import ActionChains
+from selenium.common.exceptions import NoSuchElementException
+
+STUDENT_URL_PATH = 'public'
+
+class PSStudentPassword:
+    """
+    A class for interacting with the Student UI for PowerSchool in order to reset
+    passwords.
+    """
+    
+    def __init__(self, host: str=None, headless: bool=True, wait_time: int=30,
+        download_location: str='.'):
+        
+        if host is None:
+            self.host = powerschool_config['host']
+        else:
+            self.host = host
+        
+        self.wait_time = wait_time
+
+        self.student_url = self.host + '/' + STUDENT_URL_PATH
+        self.driver = DriverBuilder().get_driver(headless=headless, download_location=download_location)
+        
+    def reset_student(self, username: str, old_password: str, new_password: str):
+        self._login(username, old_password)
+        
+        try:
+            self._wait_by_name("newCredential")
+        except:
+            logging.info(f"Username: {username} - password change screen did not load. Skipping.")
+            try:
+                self._logout()
+            except:
+                pass
+            return False
+        
+        self._find_by_name_and_send("currentCredential", old_password)
+        self._find_by_name_and_send("newCredential", new_password)
+        new_pw_box2 = self._find_by_name_and_send("newCredential1", new_password)
+        new_pw_box2.send_keys(Keys.RETURN)
+        
+        try:
+            self._logout()
+        except:
+            reused_pw_message = self.driver.find_element(By.XPATH, '//*[@id="content"]/ul/li/span')
+            if reused_pw_message.text == 'The password entered was previously used. Please enter a new password':
+                logging.info(f"Username: {username} - repeated password. Skipping.")
+                return False
+            
+        self._login(username, new_password)
+        
+        try:
+            self._logout()
+            return True
+        except:
+            logging.info(f"Username: {username} - new password failed to login.")
+            return False
+            
+    def _login(self, username: str, password: str):
+        self.driver.get(self.student_url)
+        
+        try:
+            username_elem = self._wait_by_id("fieldAccount")
+        except:
+            self._logout()
+            username_elem = self._wait_by_id("fieldAccount")
+        
+        username_elem.send_keys(username)
+        pw_box = self._find_by_id_and_send("fieldPassword", password)
+        pw_box.send_keys(Keys.RETURN)
+            
+    def _logout(self):
+        logout_button = self._wait_by_id("btnLogout")
+        logout_button.click()
+    
+    def _find_by_id_and_send(self, field_id, entry):
+        elem = self.driver.find_element(By.ID, field_id)
+        elem.send_keys(entry)
+        return elem
+    
+    def _find_by_name_and_send(self, field_name, entry):
+        elem = self.driver.find_element(By.NAME, field_name)
+        elem.send_keys(entry)
+        return elem
+    
+    def _wait_by_id(self, elem_id):
+        return WebDriverWait(self.driver, self.wait_time).until(
+            EC.presence_of_element_located((By.ID, elem_id))
+        )
+    
+    def _wait_by_name(self, elem_name):
+        return WebDriverWait(self.driver, self.wait_time).until(
+            EC.presence_of_element_located((By.NAME, elem_name))
         )
```

### Comparing `spswarehouse-0.6.1/spswarehouse/table_utils.py` & `spswarehouse-0.6.2/spswarehouse/table_utils.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-import pandas as pd
-from pandas.api.extensions import no_default
-
-import numpy as np
-import os
-import random
-import string
-
-from .warehouse import Warehouse
-from .googledrive import GoogleDrive
-
-DEFAULT_ENCODING='utf-8'
-DEFAULT_BATCH_SIZE=200
-
-# Copied from https://stackoverflow.com/questions/40774787/renaming-columns-in-a-pandas-dataframe-with-duplicate-column-names
-# guess_col_types will break if you have duplicate column names
-class renamer():
-    def __init__(self):
-        self.d = dict()
-
-    def __call__(self, x):
-        if x not in self.d:
-            self.d[x] = 0
-            return x
-        else:
-            self.d[x] += 1
-            return "%s_%d" % (x, self.d[x])
-
-def sanitize_string(name):
-    if name == '':
-        name = 'no_col_name_or_merged_column_header'
-    elif name[0].isdigit():
-        name = '_' + name
-    return name.translate(
-        {ord(c): "_" for c in "'""→!@#$%^&*()[]{};:,./<>?\|`~-=_+ \n"}
-    )
-
-def guess_col_types(df):
-    """
-    guess_col_types: pandas.DataFrame -> {column name: column type}
-
-    You should use only these types (without exceptions!)
-        BOOLEAN
-        DATE
-        FLOAT (this is a double precision floating point number)
-        INTEGER (this is a 64-bit int)
-        VARCHAR (this covers all strings up to 16MB)
-        TIMESTAMP WITHOUT TIME ZONE
-        VARIANT (json type)
-        ARRAY
-        NUMERIC(precision, scale) (you MUST provide both arguments if you use this type)
-    """
-    data_types = {
-        np.dtype('int64'): 'INTEGER',
-        np.dtype('O'): 'VARCHAR',
-        np.dtype('float64'): 'FLOAT',
-        np.dtype('bool'): 'BOOLEAN',
-        np.dtype('<M8[ns]'): 'DATE',
-    }
-
-    col_types = {}
-
-    for col_name in df.columns:
-        guess = 'unknown'
-        if col_name.lower() == 'as_of':
-            guess = 'DATE'
-        elif df.dtypes[col_name] in data_types:
-            guess = data_types[df.dtypes[col_name]]
-        col_types[col_name.lower()] = guess
-
-    return col_types
-
-def create_table_stmt(
-    table_name,
-    schema,
-    comment='',
-    # We'll use "columns" as-is
-    columns=None, # {column name: column type}
-    encoding=DEFAULT_ENCODING, # text encoding, e.g. 'utf-8' or 'latin-1'
-    # We'll try to guess what the column types are if you pass in one of the rest
-    dataframe=None, # pandas.DataFrame
-    csv_filename=None, # string
-    google_sheet=None, # gspread.models.Worksheet
-    google_drive_id=None, #string
-    force_string=False, # boolean
-    sep=no_default, # string - if not using comma as separator
-):
-    # Column names and types explicitly specified, use them as-is
-    if columns is not None:
-        return _create_table_stmt(table_name, schema, columns, comment)
-
-    # Convert everything to a dataframe and try to guess column types
-    df = None
-    if dataframe is not None:
-        if force_string:
-            df = dataframe.astype(str)
-        else:
-            df = dataframe
-    elif google_sheet is not None:
-        if force_string:
-            google_sheet_values = google_sheet.get_all_values()
-            df = pd.DataFrame(google_sheet_values[1:],columns=google_sheet_values[0], dtype=str)
-        else:
-            df = pd.DataFrame(google_sheet.get_all_records())
-    elif csv_filename is not None:
-        if force_string:
-            df = pd.read_csv(csv_filename, encoding=encoding, dtype=str, sep=sep)
-        else:
-            df = pd.read_csv(csv_filename, encoding=encoding, sep=sep)
-    elif google_drive_id is not None:
-        letters = string.ascii_letters
-        filename = ''.join(random.choice(letters) for i in range(10)) + '.csv'
-        tempFile = GoogleDrive.CreateFile({'id': google_drive_id})
-        tempFile.GetContentFile(filename)
-        try:
-            if force_string:
-                df = pd.read_csv(filename, encoding=encoding, dtype=str, sep=sep)
-            else:
-                df = pd.read_csv(filename, encoding=encoding, sep=sep)
-        except Exception as error:
-            raise error
-        finally:
-            os.remove(filename)
-    else:
-        raise
-
-    df = _sanitize_columns_for_upload(df)
-    df = df.rename(columns=renamer())
-    
-    return _create_table_stmt(
-        table_name,
-        schema,
-        guess_col_types(df),
-        comment,
-    )
-
-def _create_table_stmt(table_name, schema, col_types, comment):
-    return "CREATE TABLE {schema}.{table_name} ({cols}) COMMENT = '{comment}'".format(
-        schema=schema,
-        table_name=table_name,
-        cols=', '.join([(name + ' ' + tipe) for name, tipe in col_types.items()]),
-        comment=comment,
-    )
-
-def _sanitize_columns_for_upload(dataframe):
-    '''
-    sanitize_df_for_upload: pandas.DataFrame -> pandas.DataFrame
-
-    Creates a dataframe from a CSV file and sanitizes column names.
-    '''
-    # Overwrite column names with sanitized versions, by substituting _ for
-    # special characters
-    dataframe.columns = list(map(sanitize_string, list(dataframe.columns)))
-    return dataframe
-
-def upload_to_warehouse(
-    reflected_table,
-    # Data
-    dataframe=None,
-    csv_filename=None,
-    google_sheet=None,
-    google_drive_id=None,
-    # Range
-    start_index=0,
-    end_index=None,
-    batch_size=DEFAULT_BATCH_SIZE,
-    force_string=False,
-    encoding=DEFAULT_ENCODING,
-    sep=no_default, # string - if not using comma as separator
-):
-    df = None
-    if dataframe is not None:
-        if force_string:
-            df = dataframe.astype(str)
-        else:
-            df = dataframe
-    elif google_sheet is not None:
-        if force_string:
-            google_sheet_values = google_sheet.get_all_values()
-            df = pd.DataFrame(google_sheet_values[1:], columns=google_sheet_values[0])
-        else:
-            df = pd.DataFrame(google_sheet.get_all_records())
-    elif csv_filename is not None:
-        if force_string:
-            df = pd.read_csv(csv_filename, encoding=encoding, dtype=str, sep=sep)
-        else:
-            df = pd.read_csv(csv_filename, encoding=encoding, sep=sep)
-    elif google_drive_id is not None:
-        letters = string.ascii_letters
-        filename = ''.join(random.choice(letters) for i in range(10)) + '.csv'
-        tempFile = GoogleDrive.CreateFile({'id': google_drive_id})
-        tempFile.GetContentFile(filename)
-        try:
-            if force_string:
-                df = pd.read_csv(filename, encoding=encoding, dtype=str, sep=sep)
-            else:
-                df = pd.read_csv(filename, encoding=encoding, sep=sep)
-        except Exception as error:
-            raise error
-        finally:
-            os.remove(filename)
-    else:
-        raise
-
-    _upload_df(reflected_table, df, start_index, end_index, batch_size)
-
-def _upload_df(
-    reflected_table,
-    df,
-    start_index,
-    end_index,
-    batch_size,
-):
-    '''
-    upload_df: SqlAlchemy Table, pandas Dataframe -> void
-
-    Uploads a pandas.DataFrame to specified table.
-    If specified, uploads the range [start_index, end_index).
-
-    Assumes that the table you're uploading to exists.
-    '''
-    if end_index is None:
-        end_index = len(df)
-
-    df = _sanitize_columns_for_upload(df)
-    df = df.rename(columns=renamer())
-
-    print(str(end_index - start_index) + ' rows to insert')
-
-    while start_index < end_index:
-        end = min(start_index + batch_size, end_index)
-        df_insert = df[start_index:end]
-        values_to_insert = [
-            _build_dict_for_insert(row)
-            for _, row in df_insert.iterrows()
-        ]
-
-        Warehouse.engine.execute(reflected_table.insert(), values_to_insert)
-        print("Inserted {count} rows to {schema}.{table}".format(
-            count=len(df_insert),
-            schema=reflected_table.schema,
-            table=reflected_table.name,
-        ))
-
-        start_index = end
-
-def _build_dict_for_insert(row):
-    ret = {}
-    for col_name in list(row.index):
-        val = row[col_name]
-
-        is_numeric = isinstance(val, float)
-        if is_numeric and np.isnan(val):
-            val = None
-
-        ret[col_name.lower()] = val
-    return ret
+import pandas as pd
+from pandas.api.extensions import no_default
+
+import numpy as np
+import os
+import random
+import string
+
+from .warehouse import Warehouse
+from .googledrive import GoogleDrive
+
+DEFAULT_ENCODING='utf-8'
+DEFAULT_BATCH_SIZE=200
+
+# Copied from https://stackoverflow.com/questions/40774787/renaming-columns-in-a-pandas-dataframe-with-duplicate-column-names
+# guess_col_types will break if you have duplicate column names
+class renamer():
+    def __init__(self):
+        self.d = dict()
+
+    def __call__(self, x):
+        if x not in self.d:
+            self.d[x] = 0
+            return x
+        else:
+            self.d[x] += 1
+            return "%s_%d" % (x, self.d[x])
+
+def sanitize_string(name):
+    if name == '':
+        name = 'no_col_name_or_merged_column_header'
+    elif name[0].isdigit():
+        name = '_' + name
+    return name.translate(
+        {ord(c): "_" for c in "'""→!@#$%^&*()[]{};:,./<>?\|`~-=_+ \n"}
+    )
+
+def guess_col_types(df):
+    """
+    guess_col_types: pandas.DataFrame -> {column name: column type}
+
+    You should use only these types (without exceptions!)
+        BOOLEAN
+        DATE
+        FLOAT (this is a double precision floating point number)
+        INTEGER (this is a 64-bit int)
+        VARCHAR (this covers all strings up to 16MB)
+        TIMESTAMP WITHOUT TIME ZONE
+        VARIANT (json type)
+        ARRAY
+        NUMERIC(precision, scale) (you MUST provide both arguments if you use this type)
+    """
+    data_types = {
+        np.dtype('int64'): 'INTEGER',
+        np.dtype('O'): 'VARCHAR',
+        np.dtype('float64'): 'FLOAT',
+        np.dtype('bool'): 'BOOLEAN',
+        np.dtype('<M8[ns]'): 'DATE',
+    }
+
+    col_types = {}
+
+    for col_name in df.columns:
+        guess = 'unknown'
+        if col_name.lower() == 'as_of':
+            guess = 'DATE'
+        elif df.dtypes[col_name] in data_types:
+            guess = data_types[df.dtypes[col_name]]
+        col_types[col_name.lower()] = guess
+
+    return col_types
+
+def create_table_stmt(
+    table_name,
+    schema,
+    comment='',
+    # We'll use "columns" as-is
+    columns=None, # {column name: column type}
+    encoding=DEFAULT_ENCODING, # text encoding, e.g. 'utf-8' or 'latin-1'
+    # We'll try to guess what the column types are if you pass in one of the rest
+    dataframe=None, # pandas.DataFrame
+    csv_filename=None, # string
+    google_sheet=None, # gspread.models.Worksheet
+    google_drive_id=None, #string
+    force_string=False, # boolean
+    sep=no_default, # string - if not using comma as separator
+):
+    # Column names and types explicitly specified, use them as-is
+    if columns is not None:
+        return _create_table_stmt(table_name, schema, columns, comment)
+
+    # Convert everything to a dataframe and try to guess column types
+    df = None
+    if dataframe is not None:
+        if force_string:
+            df = dataframe.astype(str)
+        else:
+            df = dataframe
+    elif google_sheet is not None:
+        if force_string:
+            google_sheet_values = google_sheet.get_all_values()
+            df = pd.DataFrame(google_sheet_values[1:],columns=google_sheet_values[0], dtype=str)
+        else:
+            df = pd.DataFrame(google_sheet.get_all_records())
+    elif csv_filename is not None:
+        if force_string:
+            df = pd.read_csv(csv_filename, encoding=encoding, dtype=str, sep=sep)
+        else:
+            df = pd.read_csv(csv_filename, encoding=encoding, sep=sep)
+    elif google_drive_id is not None:
+        letters = string.ascii_letters
+        filename = ''.join(random.choice(letters) for i in range(10)) + '.csv'
+        tempFile = GoogleDrive.CreateFile({'id': google_drive_id})
+        tempFile.GetContentFile(filename)
+        try:
+            if force_string:
+                df = pd.read_csv(filename, encoding=encoding, dtype=str, sep=sep)
+            else:
+                df = pd.read_csv(filename, encoding=encoding, sep=sep)
+        except Exception as error:
+            raise error
+        finally:
+            os.remove(filename)
+    else:
+        raise
+
+    df = _sanitize_columns_for_upload(df)
+    df = df.rename(columns=renamer())
+    
+    return _create_table_stmt(
+        table_name,
+        schema,
+        guess_col_types(df),
+        comment,
+    )
+
+def _create_table_stmt(table_name, schema, col_types, comment):
+    return "CREATE TABLE {schema}.{table_name} ({cols}) COMMENT = '{comment}'".format(
+        schema=schema,
+        table_name=table_name,
+        cols=', '.join([(name + ' ' + tipe) for name, tipe in col_types.items()]),
+        comment=comment,
+    )
+
+def _sanitize_columns_for_upload(dataframe):
+    '''
+    sanitize_df_for_upload: pandas.DataFrame -> pandas.DataFrame
+
+    Creates a dataframe from a CSV file and sanitizes column names.
+    '''
+    # Overwrite column names with sanitized versions, by substituting _ for
+    # special characters
+    dataframe.columns = list(map(sanitize_string, list(dataframe.columns)))
+    return dataframe
+
+def upload_to_warehouse(
+    reflected_table,
+    # Data
+    dataframe=None,
+    csv_filename=None,
+    google_sheet=None,
+    google_drive_id=None,
+    # Range
+    start_index=0,
+    end_index=None,
+    batch_size=DEFAULT_BATCH_SIZE,
+    force_string=False,
+    encoding=DEFAULT_ENCODING,
+    sep=no_default, # string - if not using comma as separator
+):
+    df = None
+    if dataframe is not None:
+        if force_string:
+            df = dataframe.astype(str)
+        else:
+            df = dataframe
+    elif google_sheet is not None:
+        if force_string:
+            google_sheet_values = google_sheet.get_all_values()
+            df = pd.DataFrame(google_sheet_values[1:], columns=google_sheet_values[0])
+        else:
+            df = pd.DataFrame(google_sheet.get_all_records())
+    elif csv_filename is not None:
+        if force_string:
+            df = pd.read_csv(csv_filename, encoding=encoding, dtype=str, sep=sep)
+        else:
+            df = pd.read_csv(csv_filename, encoding=encoding, sep=sep)
+    elif google_drive_id is not None:
+        letters = string.ascii_letters
+        filename = ''.join(random.choice(letters) for i in range(10)) + '.csv'
+        tempFile = GoogleDrive.CreateFile({'id': google_drive_id})
+        tempFile.GetContentFile(filename)
+        try:
+            if force_string:
+                df = pd.read_csv(filename, encoding=encoding, dtype=str, sep=sep)
+            else:
+                df = pd.read_csv(filename, encoding=encoding, sep=sep)
+        except Exception as error:
+            raise error
+        finally:
+            os.remove(filename)
+    else:
+        raise
+
+    _upload_df(reflected_table, df, start_index, end_index, batch_size)
+
+def _upload_df(
+    reflected_table,
+    df,
+    start_index,
+    end_index,
+    batch_size,
+):
+    '''
+    upload_df: SqlAlchemy Table, pandas Dataframe -> void
+
+    Uploads a pandas.DataFrame to specified table.
+    If specified, uploads the range [start_index, end_index).
+
+    Assumes that the table you're uploading to exists.
+    '''
+    if end_index is None:
+        end_index = len(df)
+
+    df = _sanitize_columns_for_upload(df)
+    df = df.rename(columns=renamer())
+
+    print(str(end_index - start_index) + ' rows to insert')
+
+    while start_index < end_index:
+        end = min(start_index + batch_size, end_index)
+        df_insert = df[start_index:end]
+        values_to_insert = [
+            _build_dict_for_insert(row)
+            for _, row in df_insert.iterrows()
+        ]
+
+        Warehouse.engine.execute(reflected_table.insert(), values_to_insert)
+        print("Inserted {count} rows to {schema}.{table}".format(
+            count=len(df_insert),
+            schema=reflected_table.schema,
+            table=reflected_table.name,
+        ))
+
+        start_index = end
+
+def _build_dict_for_insert(row):
+    ret = {}
+    for col_name in list(row.index):
+        val = row[col_name]
+
+        is_numeric = isinstance(val, float)
+        if is_numeric and np.isnan(val):
+            val = None
+
+        ret[col_name.lower()] = val
+    return ret
```

### Comparing `spswarehouse-0.6.1/spswarehouse/warehouse.py` & `spswarehouse-0.6.2/spswarehouse/warehouse.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import pandas
-
-try:
-    from .credentials import snowflake_config
-except ModuleNotFoundError:
-    print("No credentials file found in spswarehouse. This could cause issues.")
-    
-from sqlalchemy.engine.url import URL
-from sqlalchemy import create_engine, MetaData, Table
-from sqlalchemy.engine import reflection
-from snowflake.sqlalchemy import VARIANT
-
-from datetime import date
-
-def describe(table):
-    for c in table.columns:
-        tipe = c.type
-        if isinstance(tipe, VARIANT):
-             tipe = 'VARIANT'
-        print('{}: {}'.format(c.name, tipe))
-
-class Warehouse:
-    """
-    This class is an abstraction that allows you to connect to the Snowflake Warehouse.
-    It has several methods that allow for easy access to the warehouse.
-    -- execute: run some arbitrary SQL in the warehouse. totally safe!
-    -- read_sql: execute a SELECT statement and return results as a pandas.DataFrame
-    -- reflect: return a SQLAlchemy Table object containing metadata about the table
-
-    This class also has a couple of SQLAlchemy-based instance variables
-    - engine: contains information about how to connect to the warehouse
-    - insp: a SQLAlchemy inspector object that lets query metadata about the warehouse
-            e.g., Snowflake.insp.get_table_names('wild_west')
-    """
-    def __init__(self, engine):
-        self.engine = engine
-        self.meta = MetaData(bind=engine)
-        self._insp = None
-        self._conn = None
-        self.loaded_tables = {}   # dictionary of Table objects keyed by "schema.table_name"
-
-    @property
-    def insp(self):
-        if self._insp is None:
-            self._insp = reflection.Inspector.from_engine(self.engine)
-        return self._insp
-
-    @property
-    def conn(self):
-        if self._conn is None:
-            self._conn = self.engine.connect()
-        return self._conn
-
-    # caller is responsible for closing the connection when done
-    def execute(self, sql):
-        """
-        execute: SQL statement -> (connection, proxy)
-
-        Running the execute method sends the SQL string to the warehouse using
-        this object's connection object. The return value is a tuple of the
-        connection object and the SQLAlchemy proxy object returned from executing
-        the SQL.
-        """
-        return self.conn, self.conn.execute(sql)
-
-    def read_sql(self, sql):
-        """
-        read_sql: 'SELECT ...' -> pandas.DataFrame
-        read_sql: SQLAlchemy select object -> pandas.DataFrame
-
-        The warehouse read_sql method is a minimalist wrapper around the pandas.read_sql
-        method. The sole argument to this method can either be a string (typically a SELECT statement)
-        or an object constructed using SQLAlchemy's select method.
-        """
-        return pandas.read_sql(sql, self.engine)
-
-    def reflect(self, table_or_view, schema=snowflake_config['schema']):
-        """
-        reflect: table name, schema name (optional) -> SQLAlchemy Table object
-        reflect: view name,  schema name (optional) -> SQLAlchemy Table object
-
-        The reflect method is useful to grab the underlying metadata for a table in the warehouse.
-        Using the returned value, you can print out the column names and types using the describe method.
-
-        Note that if the table or view name has a '.' in it, then this method will try to infer the schema name
-        and ignore the passed in argument
-
-        t_table = Snowflake.reflect('users', schema='staging_scrapes')
-        describe(t_table)
-        """
-        name_with_schema = '{schema}.{table_or_view}'.format(
-            schema=schema,
-            table_or_view=table_or_view
-        )
-
-        # if it's already been loaded, why bother loading it again? just return it
-        table = self.loaded_tables.get(name_with_schema, None)
-        if table is not None:
-            return table
-
-        table = Table(table_or_view, self.meta, autoload=True, schema=schema)
-
-        # sets the column names explicitly on the instance so that tab-completion is easy
-        for c in table.columns:
-            setattr(table, 'c_{}'.format(c.name), c)
-
-        # save so we don't have to load it again later
-        self.loaded_tables[name_with_schema] = table
-
-        return table
-
-Warehouse = Warehouse(
-    create_engine(
-        'snowflake://{user}:{password}@{account}/{db}/{schema}?warehouse={warehouse}'.format(
-            user=snowflake_config['user'],
-            password=snowflake_config['password'],
-            account=snowflake_config['account'],
-            db=snowflake_config['db'],
-            schema=snowflake_config['schema'],
-            warehouse=snowflake_config['warehouse']),
-        pool_size=1
-    )
-)
+import pandas
+
+try:
+    from .credentials import snowflake_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
+    
+from sqlalchemy.engine.url import URL
+from sqlalchemy import create_engine, MetaData, Table
+from sqlalchemy.engine import reflection
+from snowflake.sqlalchemy import VARIANT
+
+from datetime import date
+
+def describe(table):
+    for c in table.columns:
+        tipe = c.type
+        if isinstance(tipe, VARIANT):
+             tipe = 'VARIANT'
+        print('{}: {}'.format(c.name, tipe))
+
+class Warehouse:
+    """
+    This class is an abstraction that allows you to connect to the Snowflake Warehouse.
+    It has several methods that allow for easy access to the warehouse.
+    -- execute: run some arbitrary SQL in the warehouse. totally safe!
+    -- read_sql: execute a SELECT statement and return results as a pandas.DataFrame
+    -- reflect: return a SQLAlchemy Table object containing metadata about the table
+
+    This class also has a couple of SQLAlchemy-based instance variables
+    - engine: contains information about how to connect to the warehouse
+    - insp: a SQLAlchemy inspector object that lets query metadata about the warehouse
+            e.g., Snowflake.insp.get_table_names('wild_west')
+    """
+    def __init__(self, engine):
+        self.engine = engine
+        self.meta = MetaData(bind=engine)
+        self._insp = None
+        self._conn = None
+        self.loaded_tables = {}   # dictionary of Table objects keyed by "schema.table_name"
+
+    @property
+    def insp(self):
+        if self._insp is None:
+            self._insp = reflection.Inspector.from_engine(self.engine)
+        return self._insp
+
+    @property
+    def conn(self):
+        if self._conn is None:
+            self._conn = self.engine.connect()
+        return self._conn
+
+    # caller is responsible for closing the connection when done
+    def execute(self, sql):
+        """
+        execute: SQL statement -> (connection, proxy)
+
+        Running the execute method sends the SQL string to the warehouse using
+        this object's connection object. The return value is a tuple of the
+        connection object and the SQLAlchemy proxy object returned from executing
+        the SQL.
+        """
+        return self.conn, self.conn.execute(sql)
+
+    def read_sql(self, sql):
+        """
+        read_sql: 'SELECT ...' -> pandas.DataFrame
+        read_sql: SQLAlchemy select object -> pandas.DataFrame
+
+        The warehouse read_sql method is a minimalist wrapper around the pandas.read_sql
+        method. The sole argument to this method can either be a string (typically a SELECT statement)
+        or an object constructed using SQLAlchemy's select method.
+        """
+        return pandas.read_sql(sql, self.engine)
+
+    def reflect(self, table_or_view, schema=snowflake_config['schema']):
+        """
+        reflect: table name, schema name (optional) -> SQLAlchemy Table object
+        reflect: view name,  schema name (optional) -> SQLAlchemy Table object
+
+        The reflect method is useful to grab the underlying metadata for a table in the warehouse.
+        Using the returned value, you can print out the column names and types using the describe method.
+
+        Note that if the table or view name has a '.' in it, then this method will try to infer the schema name
+        and ignore the passed in argument
+
+        t_table = Snowflake.reflect('users', schema='staging_scrapes')
+        describe(t_table)
+        """
+        name_with_schema = '{schema}.{table_or_view}'.format(
+            schema=schema,
+            table_or_view=table_or_view
+        )
+
+        # if it's already been loaded, why bother loading it again? just return it
+        table = self.loaded_tables.get(name_with_schema, None)
+        if table is not None:
+            return table
+
+        table = Table(table_or_view, self.meta, autoload=True, schema=schema)
+
+        # sets the column names explicitly on the instance so that tab-completion is easy
+        for c in table.columns:
+            setattr(table, 'c_{}'.format(c.name), c)
+
+        # save so we don't have to load it again later
+        self.loaded_tables[name_with_schema] = table
+
+        return table
+
+Warehouse = Warehouse(
+    create_engine(
+        'snowflake://{user}:{password}@{account}/{db}/{schema}?warehouse={warehouse}'.format(
+            user=snowflake_config['user'],
+            password=snowflake_config['password'],
+            account=snowflake_config['account'],
+            db=snowflake_config['db'],
+            schema=snowflake_config['schema'],
+            warehouse=snowflake_config['warehouse']),
+        pool_size=1
+    )
+)
```

### Comparing `spswarehouse-0.6.1/spswarehouse.egg-info/PKG-INFO` & `spswarehouse-0.6.2/spswarehouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.6.1
+Version: 0.6.2
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.6.1/spswarehouse.egg-info/SOURCES.txt` & `spswarehouse-0.6.2/spswarehouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

