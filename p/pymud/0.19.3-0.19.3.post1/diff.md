# Comparing `tmp/pymud-0.19.3.tar.gz` & `tmp/pymud-0.19.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymud-0.19.3.tar", last modified: Wed Mar 27 01:46:46 2024, max compression
+gzip compressed data, was "pymud-0.19.3.post1.tar", last modified: Wed Apr  3 08:33:43 2024, max compression
```

## Comparing `pymud-0.19.3.tar` & `pymud-0.19.3.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 01:46:46.453309 pymud-0.19.3/
--rw-rw-rw-   0        0        0    35149 2023-12-05 01:41:48.000000 pymud-0.19.3/LICENSE.txt
--rw-rw-rw-   0        0        0    66716 2024-03-27 01:46:46.450590 pymud-0.19.3/PKG-INFO
--rw-rw-rw-   0        0        0    24192 2024-03-27 01:45:00.000000 pymud-0.19.3/README.md
--rw-rw-rw-   0        0        0     2070 2024-03-27 01:45:57.000000 pymud-0.19.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 01:46:46.453309 pymud-0.19.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-27 01:46:46.392543 pymud-0.19.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-27 01:46:46.428541 pymud-0.19.3/src/pymud/
--rw-rw-rw-   0        0        0      451 2024-02-26 08:13:30.000000 pymud-0.19.3/src/pymud/__init__.py
--rw-rw-rw-   0        0        0     4636 2024-03-25 12:29:31.000000 pymud-0.19.3/src/pymud/__main__.py
--rw-rw-rw-   0        0        0     5596 2024-02-23 09:37:07.000000 pymud-0.19.3/src/pymud/dialogs.py
--rw-rw-rw-   0        0        0    42062 2024-02-27 13:15:27.000000 pymud-0.19.3/src/pymud/extras.py
--rw-rw-rw-   0        0        0    29117 2024-03-24 00:49:44.000000 pymud-0.19.3/src/pymud/objects.py
--rw-rw-rw-   0        0        0    11496 2024-02-23 00:24:07.000000 pymud-0.19.3/src/pymud/pkuxkx.py
--rw-rw-rw-   0        0        0    49120 2023-12-18 05:29:21.000000 pymud-0.19.3/src/pymud/protocol.py
--rw-rw-rw-   0        0        0    39526 2024-03-23 13:05:21.000000 pymud-0.19.3/src/pymud/pymud.py
--rw-rw-rw-   0        0        0    89540 2024-03-27 01:45:03.000000 pymud-0.19.3/src/pymud/session.py
--rw-rw-rw-   0        0        0     7092 2024-03-27 01:46:12.000000 pymud-0.19.3/src/pymud/settings.py
-drwxrwxrwx   0        0        0        0 2024-03-27 01:46:46.447544 pymud-0.19.3/src/pymud.egg-info/
--rw-rw-rw-   0        0        0    66716 2024-03-27 01:46:46.000000 pymud-0.19.3/src/pymud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-03-27 01:46:46.000000 pymud-0.19.3/src/pymud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 01:46:46.000000 pymud-0.19.3/src/pymud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-27 01:46:46.000000 pymud-0.19.3/src/pymud.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 01:46:46.000000 pymud-0.19.3/src/pymud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-27 01:46:46.000000 pymud-0.19.3/src/pymud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 08:33:43.062746 pymud-0.19.3.post1/
+-rw-rw-rw-   0        0        0    35823 2024-03-10 00:23:03.000000 pymud-0.19.3.post1/LICENSE.txt
+-rw-rw-rw-   0        0        0    67187 2024-04-03 08:33:43.059456 pymud-0.19.3.post1/PKG-INFO
+-rw-rw-rw-   0        0        0    24657 2024-04-03 08:31:09.000000 pymud-0.19.3.post1/README.md
+-rw-rw-rw-   0        0        0     2075 2024-04-03 08:31:15.000000 pymud-0.19.3.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:33:43.062746 pymud-0.19.3.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 08:33:42.872724 pymud-0.19.3.post1/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 08:33:42.945031 pymud-0.19.3.post1/src/pymud/
+-rw-rw-rw-   0        0        0      422 2024-04-03 05:54:50.000000 pymud-0.19.3.post1/src/pymud/__init__.py
+-rw-rw-rw-   0        0        0     4636 2024-03-25 06:44:52.000000 pymud-0.19.3.post1/src/pymud/__main__.py
+-rw-rw-rw-   0        0        0     5596 2024-03-10 00:23:03.000000 pymud-0.19.3.post1/src/pymud/dialogs.py
+-rw-rw-rw-   0        0        0    42400 2024-04-03 08:16:37.000000 pymud-0.19.3.post1/src/pymud/extras.py
+-rw-rw-rw-   0        0        0    38063 2024-04-03 07:08:32.000000 pymud-0.19.3.post1/src/pymud/objects.py
+-rw-rw-rw-   0        0        0    11496 2024-03-10 00:23:03.000000 pymud-0.19.3.post1/src/pymud/pkuxkx.py
+-rw-rw-rw-   0        0        0    49106 2024-04-03 03:07:55.000000 pymud-0.19.3.post1/src/pymud/protocol.py
+-rw-rw-rw-   0        0        0    42936 2024-04-03 06:09:53.000000 pymud-0.19.3.post1/src/pymud/pymud.py
+-rw-rw-rw-   0        0        0   114021 2024-04-02 10:44:13.000000 pymud-0.19.3.post1/src/pymud/session.py
+-rw-rw-rw-   0        0        0     7092 2024-04-03 08:31:32.000000 pymud-0.19.3.post1/src/pymud/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:33:43.045133 pymud-0.19.3.post1/src/pymud.egg-info/
+-rw-rw-rw-   0        0        0    67187 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/top_level.txt
```

### Comparing `pymud-0.19.3/LICENSE.txt` & `pymud-0.19.3.post1/LICENSE.txt`

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

### Comparing `pymud-0.19.3/PKG-INFO` & `pymud-0.19.3.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymud
-Version: 0.19.3
+Version: 0.19.3.post1
 Summary: a MUD Client written in Python
 Author-email: "newstart@pkuxkx" <crapex@crapex.cc>
 Maintainer-email: "newstart@pkuxkx" <crapex@crapex.cc>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -949,9 +949,14 @@
 + 实现调整: 在清除task的列表推导过程中去掉了类型判断以减少任务时间占用
 + 其他调整: 从包中删除了拷贝过来作为参考的文件
 + 帮助完善: 帮助文档逻辑完善
 
 ### 0.19.2post2 （2024-03-24）
 + 实现调整: 改用官方示例的task清除方式，每个任务结束后清除
 
-### 0.19.3 (2024-XX-XX)
+### 0.19.3 (2024-03-27)
 + 问题修复: 一次发送多个命令时，发送顺序可能不正确的情况
+
+### 0.19.3post1 (2024-04-03)
++ 功能增加: 新增一个exec_async函数，是exec函数的异步形式。可以在其他会话中异步执行一段代码
++ 帮助完善: 帮助文档逻辑完善，已完成整个包的内置文档的编写和修改
++ 注: 由于我没弄太明白 readthedocs.io 网站对于读取github源代码的逻辑，目前只能通过新发布正式版本的形式来使 readthedocs.io 网站的文档中的类参考自动更新。
```

### Comparing `pymud-0.19.3/README.md` & `pymud-0.19.3.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -244,9 +244,14 @@
 + 实现调整: 在清除task的列表推导过程中去掉了类型判断以减少任务时间占用
 + 其他调整: 从包中删除了拷贝过来作为参考的文件
 + 帮助完善: 帮助文档逻辑完善
 
 ### 0.19.2post2 （2024-03-24）
 + 实现调整: 改用官方示例的task清除方式，每个任务结束后清除
 
-### 0.19.3 (2024-XX-XX)
-+ 问题修复: 一次发送多个命令时，发送顺序可能不正确的情况
+### 0.19.3 (2024-03-27)
++ 问题修复: 一次发送多个命令时，发送顺序可能不正确的情况
+
+### 0.19.3post1 (2024-04-03)
++ 功能增加: 新增一个exec_async函数，是exec函数的异步形式。可以在其他会话中异步执行一段代码
++ 帮助完善: 帮助文档逻辑完善，已完成整个包的内置文档的编写和修改
++ 注: 由于我没弄太明白 readthedocs.io 网站对于读取github源代码的逻辑，目前只能通过新发布正式版本的形式来使 readthedocs.io 网站的文档中的类参考自动更新。
```

### Comparing `pymud-0.19.3/pyproject.toml` & `pymud-0.19.3.post1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "pymud"  # Required
-version = "0.19.3"  # Required
+version = "0.19.3post1"  # Required
 description = "a MUD Client written in Python"  # Optional
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["MUD", "multi-user dungeon", "client"]  # Optional
 authors = [
   {name = "newstart@pkuxkx", email = "crapex@crapex.cc" } # Optional
```

### Comparing `pymud-0.19.3/src/pymud/__main__.py` & `pymud-0.19.3.post1/src/pymud/__main__.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3/src/pymud/dialogs.py` & `pymud-0.19.3.post1/src/pymud/dialogs.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3/src/pymud/extras.py` & `pymud-0.19.3.post1/src/pymud/extras.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,103 +1,63 @@
 # External Libraries
 from unicodedata import east_asian_width
 from wcwidth import wcwidth
-from typing import TYPE_CHECKING, Any
+from typing import Any
 import time
 
-from typing import Callable, Iterable, List, Optional, Sequence, Union
+from typing import Iterable
 from prompt_toolkit import ANSI
 from prompt_toolkit.application import get_app
 from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.formatted_text import to_formatted_text, fragment_list_to_text
 from prompt_toolkit.formatted_text.base import OneStyleAndTextTuple
 from prompt_toolkit.layout.processors import Processor, Transformation
 from prompt_toolkit.application.current import get_app
-from prompt_toolkit.auto_suggest import AutoSuggest, DynamicAutoSuggest
-from prompt_toolkit.buffer import Buffer, BufferAcceptHandler
-from prompt_toolkit.completion import Completer, DynamicCompleter
+from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.document import Document
 from prompt_toolkit.data_structures import Point
-from prompt_toolkit.layout.controls import SearchBufferControl, UIContent, UIControl
-from prompt_toolkit.lexers import Lexer, SimpleLexer
+from prompt_toolkit.layout.controls import UIContent
+from prompt_toolkit.lexers import Lexer
 from prompt_toolkit.mouse_events import MouseButton, MouseEvent, MouseEventType
-from prompt_toolkit.search import SearchState
-from prompt_toolkit.selection import SelectionType, SelectionState
-from prompt_toolkit.buffer import Buffer, BufferAcceptHandler, BufferEventHandler, ValidationState, CompletionState, YankNthArgState
+from prompt_toolkit.selection import SelectionType
+from prompt_toolkit.buffer import Buffer, ValidationState
 
 from prompt_toolkit.filters import (
-    Condition,
     FilterOrBool,
-    has_focus,
-    is_done,
-    is_true,
-    to_filter,
 )
 from prompt_toolkit.formatted_text import (
-    AnyFormattedText,
     StyleAndTextTuples,
-    Template,
     to_formatted_text,
 )
 from prompt_toolkit.formatted_text.utils import fragment_list_to_text
-from prompt_toolkit.history import History, InMemoryHistory
-from prompt_toolkit.key_binding.key_bindings import KeyBindings, KeyBindingsBase
-from prompt_toolkit.key_binding.key_processor import KeyPressEvent
-from prompt_toolkit.keys import Keys
-from prompt_toolkit.search import SearchState
+from prompt_toolkit.history import InMemoryHistory
+from prompt_toolkit.key_binding.key_bindings import KeyBindingsBase
 from prompt_toolkit.layout.containers import (
-    AnyContainer,
-    ColorColumn,
-    ConditionalContainer,
-    Container,
-    DynamicContainer,
-    Float,
-    FloatContainer,
-    HSplit,
-    ScrollOffsets,
-    VSplit,
     Window,
     WindowAlign,
 )
 from prompt_toolkit.layout.controls import (
     BufferControl,
     FormattedTextControl,
-    GetLinePrefixCallable,
-)
-from prompt_toolkit.layout.dimension import AnyDimension
-from prompt_toolkit.layout.dimension import Dimension as D
-from prompt_toolkit.layout.dimension import to_dimension
-from prompt_toolkit.layout.margins import (
-    ConditionalMargin,
-    Margin,
-    NumberedMargin,
-    ScrollbarMargin,
 )
 from prompt_toolkit.layout.processors import (
-    AppendAutoSuggestion,
-    BeforeInput,
-    ConditionalProcessor,
-    PasswordProcessor,
     Processor,
-    TabsProcessor,
 )
-from prompt_toolkit.lexers import DynamicLexer, Lexer
+from prompt_toolkit.lexers import Lexer
 from prompt_toolkit.mouse_events import MouseEvent, MouseEventType
 from prompt_toolkit.utils import get_cwidth
-from prompt_toolkit.validation import DynamicValidator, Validator
-from prompt_toolkit.widgets import Button, Dialog, Label, MenuContainer, MenuItem, TextArea, SystemToolbar, Frame
+from prompt_toolkit.widgets import Button, MenuContainer, MenuItem
 from prompt_toolkit.widgets.base import Border
 
 from prompt_toolkit.layout.screen import _CHAR_CACHE, Screen, WritePosition
 from prompt_toolkit.layout.utils import explode_text_fragments
 from prompt_toolkit.formatted_text.utils import (
     fragment_list_to_text,
     fragment_list_width,
 )
-from prompt_toolkit.utils import Event
 
 from .settings import Settings
 
 class MudFormatProcessor(Processor):
     "在BufferControl中显示ANSI格式的处理器"
 
     def __init__(self) -> None:
@@ -1007,14 +967,34 @@
         if self.children:
             return max(get_cwidth(c.text) for c in self.children)
         else:
             return 0
 
 
 class DotDict(dict):
+    """
+    可以通过点.访问内部key-value对的字典。此类型继承自dict。
+
+    - 由于继承关系，此类型可以使用所有dict可以使用的方法
+    - 额外增加的点.访问方法使用示例如下
+
+    示例:
+        .. code:: Python
+
+            mydict = DotDict()
+            
+            # 以下写内容访问等价
+            mydict["key1"] = "value1"
+            mydict.key1 = "value1"
+
+            # 以下读访问等价
+            val = mydict["key1"]
+            val = mydict.key1
+    """
+
     def __getattr__(self, __key):
         if (not __key in self.__dict__) and (not __key.startswith("__")):
             return self.__getitem__(__key)
 
     def __setattr__(self, __name: str, __value):
         if __name in self.__dict__:
             object.__setattr__(self, __name, __value)
@@ -1027,47 +1007,75 @@
     def __setstate__(self, state):
         self.update(state)
 
 import importlib
 import importlib.util
 
 class Plugin:
+    """
+    插件管理类。对加载的插件文件进行管理。该类型由PyMudApp进行管理，无需人工创建。
+
+    有关插件的详细信息，请参见 `插件 <plugins.html>`_
+
+    :param name: 插件的文件名, 如'myplugin.py'
+    :param location: 插件所在的目录。自动加载的插件包括PyMUD包目录下的plugins目录以及当前目录下的plugins目录
+
+    """
     def __init__(self, name, location):
         self._plugin_file = name
         self._plugin_loc  = location
 
         self.reload()
 
     def reload(self):
+        "加载/重新加载插件对象"
         #del self.modspec, self.mod
         self.modspec = importlib.util.spec_from_file_location(self._plugin_file[:-3], self._plugin_loc)
         self.mod     = importlib.util.module_from_spec(self.modspec)
         self.modspec.loader.exec_module(self.mod)
 
         self._app_init = self.mod.__dict__["PLUGIN_PYMUD_START"]
         self._session_create = self.mod.__dict__["PLUGIN_SESSION_CREATE"]
         self._session_destroy = self.mod.__dict__["PLUGIN_SESSION_DESTROY"]
         
     @property
     def name(self):
+        "插件名称，由插件文件中的 PLUGIN_NAME 常量定义"
         return self.mod.__dict__["PLUGIN_NAME"]
     
     @property
     def desc(self):
+        "插件描述，由插件文件中的 PLUGIN_DESC 常量定义"
         return self.mod.__dict__["PLUGIN_DESC"]
     
     @property
     def help(self):
+        "插件帮助，由插件文件中的文档字符串定义"
         return self.mod.__doc__
     
     def onAppInit(self, app):
+        """
+        PyMUD应用启动时对插件执行的操作，由插件文件中的 PLUGIN_PYMUD_START 函数定义
+
+        :param app: 启动的 PyMudApp 对象实例
+        """
         self._app_init(app)
 
     def onSessionCreate(self, session):
+        """
+        新会话创建时对插件执行的操作，由插件文件中的 PLUGIN_SESSION_CREATE 函数定义
+
+        :param session: 新创建的会话对象实例
+        """
         self._session_create(session)
 
     def onSessionDestroy(self, session):
+        """
+        会话关闭时（注意不是断开）对插件执行的操作，由插件文件中的 PLUGIN_SESSION_DESTROY 函数定义
+
+        :param session: 所关闭的会话对象实例
+        """
         self._session_destroy(session)
 
     def __getattr__(self, __name: str) -> Any:
         if hasattr(self.mod, __name):
             return self.mod.__getattribute__(__name)
```

### Comparing `pymud-0.19.3/src/pymud/pkuxkx.py` & `pymud-0.19.3.post1/src/pymud/pkuxkx.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3/src/pymud/protocol.py` & `pymud-0.19.3.post1/src/pymud/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,18 +123,18 @@
     适用于MUD客户端的asyncio的协议实现
     基本协议： TELNET
     扩展协议： GMCP, MCDP, MSP, MXP等等
     """
 
     def __init__(self, session, *args, **kwargs) -> None:
         """
-        MUD客户端协议实现, 参数包括：       \n
-          + session: 管理protocol的会话     \n
-        除此之外，还可以接受的命名参数包括： \n
-          + onConnected:    当连接建立时的回调，包含2个参数： MudClientProtocol本身，以及生成的传输Transport对象  \n
+        MUD客户端协议实现, 参数包括：     
+          + session: 管理protocol的会话   
+        除此之外，还可以接受的命名参数包括：
+          + onConnected:    当连接建立时的回调，包含2个参数： MudClientProtocol本身，以及生成的传输Transport对象 
           + onDisconnected: 当连接断开时的回调，包含1个参数： MudClientProtocol本身
         """
 
         self.log = logging.getLogger("pymud.MudClientProtocol")
         self.session = session                                              # 数据处理的会话
         self.connected = False                                              # 连接状态标识                              
         self._iac_handlers = dict()                                         # 支持选项协商处理函数
```

### Comparing `pymud-0.19.3/src/pymud/pymud.py` & `pymud-0.19.3.post1/src/pymud/pymud.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 class PyMudApp:
     """
     PYMUD程序管理主对象，对窗体、操作及所有会话进行管理。
 
     PyMudApp对象不需要手动创建，在命令行中执行 ``python -m pymud`` 时会自动创建对象实例。
 
-    构造函数参数： 
+    参数： 
         - ``cfg_data``: 替代配置数据，由本地pymud.cfg文件读取，用于覆盖settings.py中的默认Settings数据
 
     可替代字典: 含义请查阅 `应用配置及本地化 <settings.html>`_
         - sessions: 用于创建菜单栏会话的字典
         - client: 用于配置客户端属性的字典
         - text: 用于各默认显示文字内容的字典
         - server: 用于服务器选项的配置字典
@@ -139,14 +139,15 @@
 
         set_title("{} {}".format(Settings.__appname__, Settings.__version__))
         self.set_status(Settings.text["welcome"])
 
         self.load_plugins()
 
     def initUI(self):
+        """初始化UI界面"""
         self.style = Style.from_dict(Settings.styles)
         self.status_message = ""
         self.showHistory = False
         self.wrap_lines  = True
 
         self.commandLine = TextArea(
             prompt=self.get_input_prompt, 
@@ -319,15 +320,15 @@
                     ycursor=True,
                     content=CompletionsMenu(max_height=16, scroll_offset=1)
                 )
             ],
         )
 
     def create_world_menus(self):
-        "创建世界子菜单"
+        "创建世界子菜单，其中根据本地pymud.cfg中的有关配置创建会话有关子菜单"
         menus = []
         menus.append(MenuItem(Settings.text["new_session"], handler = self.act_new))
         menus.append(MenuItem("-", disabled=True))
 
         ss = Settings.sessions
 
         for key, site in ss.items():
@@ -374,58 +375,63 @@
             b = s.buffer
             if lines < 0:
                 b.cursor_up(-1 * lines)
             elif lines > 0:
                 b.cursor_down(lines)
 
     def page_up(self, event: KeyPressEvent) -> None:
+        "快捷键PageUp: 用于向上翻页。翻页页数为显示窗口行数的一半减去一行。"
         #lines = (self.app.output.get_size().rows - 5) // 2 - 1
         lines = self.get_height() // 2 - 1
         self.scroll(-1 * lines)
 
     def page_down(self, event: KeyPressEvent) -> None:
+        "快捷键PageDown: 用于向下翻页。翻页页数为显示窗口行数的一半减去一行。"
         #lines = (self.app.output.get_size().rows - 5) // 2 - 1
         lines = self.get_height() // 2 - 1
         self.scroll(lines)
 
     def custom_key_press(self, event: KeyPressEvent):
+        "自定义快捷键功能实现，根据keys字典配置在当前会话执行指定指令"
         if (len(event.key_sequence) == 1) and (event.key_sequence[-1].key in Settings.keys.keys()):
             cmd = Settings.keys[event.key_sequence[-1].key]
             if self.current_session:
                 self.current_session.exec_command(cmd)
 
     def hide_history(self, event: KeyPressEvent) -> None:
-        """关闭历史行显示"""
+        """快捷键Ctrl+Z: 关闭历史行显示"""
         self.act_nosplit()
 
     def copy_selection(self, event: KeyPressEvent)-> None:
+        """快捷键Ctrl+C/Ctrl+R: 复制选择内容。根据按键不同选择文本复制方式和RAW复制方式"""
         if event.key_sequence[-1].key == Keys.ControlC:
             self.copy()
         elif event.key_sequence[-1].key == Keys.ControlR:
             self.copy(raw = True)
 
     def delete_selection(self, event: KeyPressEvent):
         event.key_sequence
         b = event.current_buffer
         if b.selection_state:
             event.key_processor.feed(KeyPress(Keys.Delete), first=True)
         else:
             b.delete_before_cursor(1)
 
     def complete_autosuggest(self, event: KeyPressEvent):
-        """自动完成建议"""
+        """快捷键右箭头→: 自动完成建议"""
         b = event.current_buffer
         if b.cursor_position == len(b.text):
             s = b.auto_suggest.get_suggestion(b, b.document)
             if s:
                 b.insert_text(s.text, fire_event=False)
         else:
             b.cursor_right()
 
     def change_session(self, event: KeyPressEvent):
+        """快捷键Ctrl+左右箭头: 切换会话"""
         if self.current_session:
             current = self.current_session.name
             keys = list(self.sessions.keys())
             idx = keys.index(current)
             count = len(keys)
 
             if event.key_sequence[-1].key == Keys.ControlRight:
@@ -435,21 +441,29 @@
 
             elif event.key_sequence[-1].key == Keys.ControlLeft:
                 if idx > 0:
                     new_key = keys[idx-1]
                     self.activate_session(new_key)
 
     def toggle_mousesupport(self, event: KeyPressEvent):
+        """快捷键F2: 切换鼠标支持状态。用于远程连接时本地复制命令执行操作"""
         self._mouse_support = not self._mouse_support
         if self._mouse_support:
             self.app.renderer.output.enable_mouse_support()
         else:
             self.app.renderer.output.disable_mouse_support()
 
     def copy(self, raw = False):
+        """
+        复制会话中的选中内容
+
+        :param raw: 指定采取文本模式还是ANSI格式模式
+
+        ``注意: 复制的内容仅存在于运行环境的剪贴板中。若使用ssh远程，该复制命令不能访问本地剪贴板。``
+        """
         b = self.consoleView.buffer
         if b.selection_state:
             srow, scol = b.document.translate_index_to_position(b.selection_state.original_cursor_position)
             erow, ecol = b.document.translate_index_to_position(b.document.cursor_position)
 
             if not raw:
                 # Control-C 复制纯文本
@@ -500,14 +514,25 @@
                 # self.set_status("已复制：{}".format(data.text))
 
                 # self.current_session.setVariable("%copy", data.text)
         else:
             self.set_status("未选中任何内容...")
 
     def create_session(self, name, host, port, encoding = None, after_connect = None, scripts = None, userid = None):
+        """
+        创建一个会话。菜单或者#session命令均调用本函数执行创建会话。
+
+        :param name: 会话名称
+        :param host: 服务器域名或IP地址
+        :param port: 端口号
+        :param encoding: 服务器编码
+        :param after_connect: 连接后要向服务器发送的内容，用来实现自动登录功能
+        :param scripts: 要加载的脚本清单
+        :param userid: 自动登录的ID(获取自cfg文件中的定义，绑定到菜单)，将以该值在该会话中创建一个名为id的变量
+        """
         result = False
         encoding = encoding or Settings.server["default_encoding"]
 
         if name not in self.sessions.keys():
             session = Session(self, name, host, port, encoding, after_connect, scripts = scripts)
             session.setVariable("id", userid)
             self.sessions[name] = session
@@ -530,15 +555,15 @@
         if isinstance(session, Session):
             self.current_session = session
             self.consoleView.buffer = session.buffer
             #self.set_status(Settings.text["session_changed"].format(session.name))
             self.app.invalidate()
 
     def close_session(self):
-        "关闭当前会话"
+        "关闭当前会话。若当前会话处于连接状态，将弹出对话框以确认。"
         async def coroutine():
             if self.current_session:
                 if self.current_session.connected:
                     dlgQuery = QueryDialog(HTML('<b fg="red">警告</b>'), HTML('<style fg="red">当前会话 {0} 还处于连接状态，确认要关闭？</style>'.format(self.current_session.name)))
                     result = await self.show_dialog_as_float(dlgQuery)
                     if result:
                         self.current_session.disconnect()
@@ -566,125 +591,141 @@
                     #self.set_status(f"当前会话已切换为 {self.current_session.name}")
 
         asyncio.ensure_future(coroutine())
 
     # 菜单选项操作 - 开始
 
     def act_new(self):
+        "菜单: 创建新会话"
         async def coroutine():
             dlgNew = NewSessionDialog()
             result = await self.show_dialog_as_float(dlgNew)
             if result:
                 self.create_session(*result)
             return result
         
         asyncio.ensure_future(coroutine())
 
     def act_connect(self):
+        "菜单: 连接/重新连接"
         if self.current_session:
             self.current_session.handle_connect()
 
     def act_discon(self):
+        "菜单: 断开连接"
         if self.current_session:
             self.current_session.disconnect()
 
     def act_nosplit(self):
+        "菜单: 取消分屏"
         if self.current_session:
             s = self.current_session
             b = s.buffer
             b.exit_selection()
             b.cursor_position = len(b.text)
 
     def act_close_session(self):
+        "菜单: 关闭当前会话"
         self.close_session()
 
     def act_echoinput(self):
+        "菜单: 显示/隐藏输入指令"
         val = not Settings.client["echo_input"]
         Settings.client["echo_input"] = val
         if self.current_session:
             self.current_session.info(f"回显输入命令被设置为：{'打开' if val else '关闭'}")
 
     def act_autoreconnect(self):
+        "菜单: 打开/关闭自动重连"
         val = not Settings.client["auto_reconnect"]
         Settings.client["auto_reconnect"] = val
         if self.current_session:
             self.current_session.info(f"自动重连被设置为：{'打开' if val else '关闭'}")
 
     def act_copy(self):
-        "复制菜单"
+        "菜单: 复制纯文本"
         self.copy()
 
     def act_copyraw(self):
-        "复制ANSI菜单"
+        "菜单: 复制(ANSI)"
         self.copy(raw = True)
 
     def act_clearsession(self):
-        "清空当前会话缓存的文本内容"
+        "菜单: 清空会话内容"
         self.consoleView.buffer.text = ""
 
     def act_reload(self):
-        "重新加载配置文件菜单"
+        "菜单: 重新加载脚本配置"
         if self.current_session:
             self.current_session.handle_reload()
 
+    # 暂未实现该功能
     def act_change_layout(self, layout):
-        "更改状态窗口显示"
         #if isinstance(layout, STATUS_DISPLAY):
         self.status_display = layout
         #self.console_frame.body.reset()
         # if layout == STATUS_DISPLAY.HORIZON:
         #     self.console_frame.body = self.console_with_horizon_status
         # elif layout == STATUS_DISPLAY.VERTICAL:
         #     self.console_frame.body = self.console_with_vertical_status
         # elif layout == STATUS_DISPLAY.NONE:
         #     self.console_frame.body = self.console_without_status
 
         #self.show_message("布局调整", f"已将布局设置为{layout}")
         self.app.invalidate()
 
     def act_exit(self):
-        "退出菜单"
+        """菜单: 退出"""
         async def coroutine():
+            con_sessions = list()
             for session in self.sessions.values():
                 if session.connected:
-                    dlgQuery = QueryDialog(HTML('<b fg="red">程序退出警告</b>'), HTML('<style fg="red">会话 {0} 还处于连接状态，确认要关闭？</style>'.format(session.name)))
-                    result = await self.show_dialog_as_float(dlgQuery)
-                    if result:
-                        session.disconnect()
+                    con_sessions.append(session.name)
+
+            if len(con_sessions) > 0:
+                dlgQuery = QueryDialog(HTML('<b fg="red">程序退出警告</b>'), HTML('<style fg="red">尚有 {0} 个会话 {1} 还处于连接状态，确认要关闭？</style>'.format(len(con_sessions), ", ".join(con_sessions))))
+                result = await self.show_dialog_as_float(dlgQuery)
+                if result:
+                    for ss_name in con_sessions:
+                        ss = self.sessions[ss_name]
+                        ss.disconnect()
 
                         # 增加延时等待确保会话关闭
-                        while session.connected:
+                        while ss.connected:
                             await asyncio.sleep(0.1)
 
                         for plugin in self._plugins.values():
                             if isinstance(plugin, Plugin):
-                                plugin.onSessionDestroy(self.current_session)
+                                plugin.onSessionDestroy(ss)
 
                     else:
                         return
                 
             self.app.exit()
 
         asyncio.ensure_future(coroutine())
 
     def act_about(self):
-        "关于菜单"
+        "菜单: 关于"
         dialog_about = WelcomeDialog(True)
         self.show_dialog(dialog_about)
 
     # 菜单选项操作 - 完成
 
     def get_input_prompt(self):
+        "命令输入行提示符"
         return HTML(Settings.text["input_prompt"])
 
     def btn_title_clicked(self, name, mouse_event: MouseEvent):
+        "顶部会话标签点击切换鼠标事件"
         if mouse_event.event_type == MouseEventType.MOUSE_UP:
             self.activate_session(name)
 
     def get_frame_title(self):
+        "顶部会话标题选项卡"
         if len(self.sessions.keys()) == 0:
             return Settings.__appname__ + " " + Settings.__version__
         
         title_formatted_list = []
         for key, session in self.sessions.items():
             if session == self.current_session:
                 if session.connected:
@@ -700,20 +741,22 @@
 
             title_formatted_list.append((style, key, functools.partial(self.btn_title_clicked, key)))
             title_formatted_list.append(("", " | "))
 
         return title_formatted_list[:-1]
 
     def get_statusbar_text(self):
+        "状态栏内容"
         return [
             ("class:status", " "),
             ("class:status", self.status_message),
         ]
     
     def get_statusbar_right_text(self):
+        "状态栏右侧内容"
         con_str, mouse_support, tri_status = "", "", ""
         if not self._mouse_support:
             mouse_support = "鼠标已禁用 "
 
         if self.current_session:
             if self.current_session._ignore:
                 tri_status = "全局禁用 "
@@ -739,39 +782,45 @@
                     con_str = "已连接：{:.0f}分{:.0f}秒".format(mins, sec)
                 else:
                     con_str = "已连接：{:.0f}秒".format(sec)
 
         return "{}{}{} {} {} ".format(mouse_support, tri_status, con_str, Settings.__appname__, Settings.__version__)
 
     def get_statuswindow_text(self):
+        "状态窗口: status_maker 的内容"
         text = ""
         if self.current_session:
             text = self.current_session.get_status()
 
         return text
 
     def set_status(self, msg):
+        """
+        在状态栏中上显示消息。可在代码中调用
+        
+        :param msg: 要显示的消息
+        """
         self.status_message = msg
         self.app.invalidate()
 
     def handle_session(self, *args):
         '''
         嵌入命令 #session 的执行函数，创建一个远程连接会话。
         该函数不应该在代码中直接调用。
 
         使用:
-            - #session {Name} {Host} {Port} {Encoding}
+            - #session {name} {host} {port} {encoding}
             - 当不指定 Encoding: 时, 默认使用utf-8编码
             - 可以直接使用 #{名称} 切换会话和操作会话命令
 
         参数:
-            :Name: 会话名称
-            :Host: 服务器域名或IP地址
-            :Port: 端口号
-            :Encoding: 编码格式，不指定时默认为 utf8
+            :name: 会话名称
+            :host: 服务器域名或IP地址
+            :port: 端口号
+            :encoding: 编码格式，不指定时默认为 utf8
     
         示例:
             ``#session {名称} {宿主机} {端口} {编码}`` 
                 创建一个远程连接会话，使用指定编码格式连接到远程宿主机的指定端口并保存为 {名称} 。其中，编码可以省略，此时使用Settings.server["default_encoding"]的值，默认为utf8
             ``#session newstart mud.pkuxkx.net 8080 GBK`` 
                 使用GBK编码连接到mud.pkuxkx.net的8080端口，并将该会话命名为newstart
             ``#session newstart mud.pkuxkx.net 8081`` 
@@ -801,14 +850,15 @@
             self.create_session(session_name, session_host, session_port, session_encoding)
             nothandle = False
         
         if nothandle:
             self.set_status("错误的#session命令")
 
     def enter_pressed(self, buffer: Buffer):
+        "命令行回车按键处理"
         cmd_line = buffer.text
         space_index = cmd_line.find(" ")
         
         if len(cmd_line) == 0:
             if self.current_session:
                 self.current_session.writeline("")
         
@@ -842,34 +892,54 @@
             return True
         
         else:
             return False
 
     @property
     def globals(self):
+        """
+        全局变量，快捷点访问器
+        用于替代get_globals与set_globals函数的调用
+        """
         return self._globals
 
     def get_globals(self, name, default = None):
-        "获取PYMUD全局变量"
+        """
+        获取PYMUD全局变量
+        
+        :param name: 全局变量名称
+        :param default: 当全局变量不存在时的返回值
+        """
         if name in self._globals.keys():
             return self._globals[name]
         else:
             return default
 
     def set_globals(self, name, value):
-        "设置PYMUD全局变量"
+        """
+        设置PYMUD全局变量
+
+        :param name: 全局变量名称
+        :param value: 全局变量值。值可以为任何类型。
+        """
         self._globals[name] = value
 
     def del_globals(self, name):
-        "移除一个PYMUD全局变量"
+        """
+        移除一个PYMUD全局变量
+        移除全局变量是从字典中删除该变量，而不是将其设置为None
+
+        :param name: 全局变量名称
+        """
         if name in self._globals.keys():
             self._globals.pop(name)
 
     @property
     def plugins(self):
+        "所有已加载的插件列表，快捷点访问器"
         return self._plugins
 
     def show_message(self, title, text, modal = True):
         "显示一个消息对话框"
         async def coroutine():
             dialog = MessageDialog(title, text, modal)
             await self.show_dialog_as_float(dialog)
@@ -894,17 +964,19 @@
 
         if float_ in self.root_container.floats:
             self.root_container.floats.remove(float_)
 
         return result
 
     async def run_async(self):
+        "以异步方式运行本程序"
         await self.app.run_async()
 
     def run(self):
+        "运行本程序"
         self.app.run()
         #asyncio.run(self.run_async())
 
     def get_width(self):
         "获取ConsoleView的实际宽度，等于输出宽度-4,（左右线条宽度, 滚动条宽度，右边让出的1列）"
         size = self.app.output.get_size().columns - 4
         if Settings.client["status_display"] == 2:
@@ -919,14 +991,15 @@
             size = size - Settings.client["status_height"] - 1
         return size
 
     #####################################
     # plugins 处理
     #####################################
     def load_plugins(self):
+        "加载插件。将加载pymud包的plugins目录下插件，以及当前目录的plugins目录下插件"
         # 首先加载系统目录下的插件
         current_dir = os.path.dirname(__file__)
         plugins_dir = os.path.join(current_dir, "plugins")
         if os.path.exists(plugins_dir):
             for file in os.listdir(plugins_dir):
                 if file.endswith(".py"):
                     try:
```

### Comparing `pymud-0.19.3/src/pymud/settings.py` & `pymud-0.19.3.post1/src/pymud/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     # 下列内容为APP的常量定义，请勿修改
     __appname__   = "PYMUD"
     "APP 名称, 默认PYMUD"
     __appdesc__   = "a MUD client written in Python"
     "APP 简要描述"
     __version__   = "0.19.3"
     "APP 当前版本"
-    __release__   = "2024-03-22"
+    __release__   = "2024-04-03"
     "APP 当前版本发布日期"
     __author__    = "本牛(newstart)@北侠"
     "APP 作者"
     __email__     = "crapex@crapex.cc"
     "APP 作者邮箱"
     __website__     = "https://pymud.readthedocs.org/"
     "帮助文档发布网址"
```

### Comparing `pymud-0.19.3/src/pymud.egg-info/PKG-INFO` & `pymud-0.19.3.post1/src/pymud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymud
-Version: 0.19.3
+Version: 0.19.3.post1
 Summary: a MUD Client written in Python
 Author-email: "newstart@pkuxkx" <crapex@crapex.cc>
 Maintainer-email: "newstart@pkuxkx" <crapex@crapex.cc>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -949,9 +949,14 @@
 + 实现调整: 在清除task的列表推导过程中去掉了类型判断以减少任务时间占用
 + 其他调整: 从包中删除了拷贝过来作为参考的文件
 + 帮助完善: 帮助文档逻辑完善
 
 ### 0.19.2post2 （2024-03-24）
 + 实现调整: 改用官方示例的task清除方式，每个任务结束后清除
 
-### 0.19.3 (2024-XX-XX)
+### 0.19.3 (2024-03-27)
 + 问题修复: 一次发送多个命令时，发送顺序可能不正确的情况
+
+### 0.19.3post1 (2024-04-03)
++ 功能增加: 新增一个exec_async函数，是exec函数的异步形式。可以在其他会话中异步执行一段代码
++ 帮助完善: 帮助文档逻辑完善，已完成整个包的内置文档的编写和修改
++ 注: 由于我没弄太明白 readthedocs.io 网站对于读取github源代码的逻辑，目前只能通过新发布正式版本的形式来使 readthedocs.io 网站的文档中的类参考自动更新。
```

