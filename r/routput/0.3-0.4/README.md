# Comparing `tmp/routput-0.3.tar.gz` & `tmp/routput-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.3.tar", last modified: Thu Apr 18 09:25:05 2024, max compression
+gzip compressed data, was "routput-0.4.tar", last modified: Wed May  1 23:49:43 2024, max compression
```

## Comparing `routput-0.3.tar` & `routput-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 09:25:05.280696 routput-0.3/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.3/LICENCE
--rw-rw-rw-   0        0        0     2887 2024-04-18 09:25:05.279613 routput-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 09:25:05.274529 routput-0.3/routput/
--rw-rw-rw-   0        0        0        0 2024-04-18 09:05:49.000000 routput-0.3/routput/__init__.py
--rw-rw-rw-   0        0        0       31 2024-04-18 09:05:31.000000 routput-0.3/routput/__main__.py
--rw-rw-rw-   0        0        0     8179 2024-04-18 09:10:57.000000 routput-0.3/routput/routput.py
-drwxrwxrwx   0        0        0        0 2024-04-18 09:25:05.279613 routput-0.3/routput.egg-info/
--rw-rw-rw-   0        0        0     2887 2024-04-18 09:25:05.000000 routput-0.3/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-18 09:25:05.000000 routput-0.3/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 09:25:05.000000 routput-0.3/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 09:25:05.000000 routput-0.3/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 09:25:05.281703 routput-0.3/setup.cfg
--rw-rw-rw-   0        0        0     4198 2024-04-18 09:22:41.000000 routput-0.3/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-01 23:49:43.156872 routput-0.4/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-04-14 05:51:33.000000 routput-0.4/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2505 2024-05-01 23:49:43.155975 routput-0.4/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2000 2024-05-01 23:41:41.000000 routput-0.4/README.md
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-01 23:49:43.152798 routput-0.4/routput/
+-rw-r--r--   0 joel-watson   (501) staff       (20)        0 2024-05-01 23:41:41.000000 routput-0.4/routput/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)       31 2024-05-01 23:41:41.000000 routput-0.4/routput/__main__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)     7856 2024-05-01 23:41:41.000000 routput-0.4/routput/routput.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-01 23:49:43.155277 routput-0.4/routput.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2505 2024-05-01 23:49:42.000000 routput-0.4/routput.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      209 2024-05-01 23:49:42.000000 routput-0.4/routput.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-01 23:49:42.000000 routput-0.4/routput.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        8 2024-05-01 23:49:42.000000 routput-0.4/routput.egg-info/top_level.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-01 23:49:43.157069 routput-0.4/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      451 2024-05-01 23:47:35.000000 routput-0.4/setup.py
```

### Comparing `routput-0.3/LICENCE` & `routput-0.4/LICENCE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,482 +1,482 @@
-# GNU LIBRARY GENERAL PUBLIC LICENSE
-
-Version 2, June 1991
-
-    Copyright (C) 1991 Free Software Foundation, Inc.
-    51 Franklin St, Fifth Floor, Boston, MA  02110-1301, USA
-    
-    Everyone is permitted to copy and distribute verbatim copies
-    of this license document, but changing it is not allowed.
-
-    [This is the first released version of the library GPL.  It is
-     numbered 2 because it goes with version 2 of the ordinary GPL.]
-
-## Preamble
-
-The licenses for most software are designed to take away your freedom
-to share and change it. By contrast, the GNU General Public Licenses
-are intended to guarantee your freedom to share and change free
-software--to make sure the software is free for all its users.
-
-This license, the Library General Public License, applies to some
-specially designated Free Software Foundation software, and to any
-other libraries whose authors decide to use it. You can use it for
-your libraries, too.
-
-When we speak of free software, we are referring to freedom, not
-price. Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-this service if you wish), that you receive source code or can get it
-if you want it, that you can change the software or use pieces of it
-in new free programs; and that you know you can do these things.
-
-To protect your rights, we need to make restrictions that forbid
-anyone to deny you these rights or to ask you to surrender the rights.
-These restrictions translate to certain responsibilities for you if
-you distribute copies of the library, or if you modify it.
-
-For example, if you distribute copies of the library, whether gratis
-or for a fee, you must give the recipients all the rights that we gave
-you. You must make sure that they, too, receive or can get the source
-code. If you link a program with the library, you must provide
-complete object files to the recipients so that they can relink them
-with the library, after making changes to the library and recompiling
-it. And you must show them these terms so they know their rights.
-
-Our method of protecting your rights has two steps: (1) copyright the
-library, and (2) offer you this license which gives you legal
-permission to copy, distribute and/or modify the library.
-
-Also, for each distributor's protection, we want to make certain that
-everyone understands that there is no warranty for this free library.
-If the library is modified by someone else and passed on, we want its
-recipients to know that what they have is not the original version, so
-that any problems introduced by others will not reflect on the
-original authors' reputations.
-
-Finally, any free program is threatened constantly by software
-patents. We wish to avoid the danger that companies distributing free
-software will individually obtain patent licenses, thus in effect
-transforming the program into proprietary software. To prevent this,
-we have made it clear that any patent must be licensed for everyone's
-free use or not licensed at all.
-
-Most GNU software, including some libraries, is covered by the
-ordinary GNU General Public License, which was designed for utility
-programs. This license, the GNU Library General Public License,
-applies to certain designated libraries. This license is quite
-different from the ordinary one; be sure to read it in full, and don't
-assume that anything in it is the same as in the ordinary license.
-
-The reason we have a separate public license for some libraries is
-that they blur the distinction we usually make between modifying or
-adding to a program and simply using it. Linking a program with a
-library, without changing the library, is in some sense simply using
-the library, and is analogous to running a utility program or
-application program. However, in a textual and legal sense, the linked
-executable is a combined work, a derivative of the original library,
-and the ordinary General Public License treats it as such.
-
-Because of this blurred distinction, using the ordinary General Public
-License for libraries did not effectively promote software sharing,
-because most developers did not use the libraries. We concluded that
-weaker conditions might promote sharing better.
-
-However, unrestricted linking of non-free programs would deprive the
-users of those programs of all benefit from the free status of the
-libraries themselves. This Library General Public License is intended
-to permit developers of non-free programs to use free libraries, while
-preserving your freedom as a user of such programs to change the free
-libraries that are incorporated in them. (We have not seen how to
-achieve this as regards changes in header files, but we have achieved
-it as regards changes in the actual functions of the Library.) The
-hope is that this will lead to faster development of free libraries.
-
-The precise terms and conditions for copying, distribution and
-modification follow. Pay close attention to the difference between a
-"work based on the library" and a "work that uses the library". The
-former contains code derived from the library, while the latter only
-works together with the library.
-
-Note that it is possible for a library to be covered by the ordinary
-General Public License rather than by this special one.
-
-## TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
-
-**0.** This License Agreement applies to any software library which
-contains a notice placed by the copyright holder or other authorized
-party saying it may be distributed under the terms of this Library
-General Public License (also called "this License"). Each licensee is
-addressed as "you".
-
-A "library" means a collection of software functions and/or data
-prepared so as to be conveniently linked with application programs
-(which use some of those functions and data) to form executables.
-
-The "Library", below, refers to any such software library or work
-which has been distributed under these terms. A "work based on the
-Library" means either the Library or any derivative work under
-copyright law: that is to say, a work containing the Library or a
-portion of it, either verbatim or with modifications and/or translated
-straightforwardly into another language. (Hereinafter, translation is
-included without limitation in the term "modification".)
-
-"Source code" for a work means the preferred form of the work for
-making modifications to it. For a library, complete source code means
-all the source code for all modules it contains, plus any associated
-interface definition files, plus the scripts used to control
-compilation and installation of the library.
-
-Activities other than copying, distribution and modification are not
-covered by this License; they are outside its scope. The act of
-running a program using the Library is not restricted, and output from
-such a program is covered only if its contents constitute a work based
-on the Library (independent of the use of the Library in a tool for
-writing it). Whether that is true depends on what the Library does and
-what the program that uses the Library does.
-
-**1.** You may copy and distribute verbatim copies of the Library's
-complete source code as you receive it, in any medium, provided that
-you conspicuously and appropriately publish on each copy an
-appropriate copyright notice and disclaimer of warranty; keep intact
-all the notices that refer to this License and to the absence of any
-warranty; and distribute a copy of this License along with the
-Library.
-
-You may charge a fee for the physical act of transferring a copy, and
-you may at your option offer warranty protection in exchange for a
-fee.
-
-**2.** You may modify your copy or copies of the Library or any
-portion of it, thus forming a work based on the Library, and copy and
-distribute such modifications or work under the terms of Section 1
-above, provided that you also meet all of these conditions:
-
--   **a)** The modified work must itself be a software library.
--   **b)** You must cause the files modified to carry prominent
-    notices stating that you changed the files and the date of
-    any change.
--   **c)** You must cause the whole of the work to be licensed at no
-    charge to all third parties under the terms of this License.
--   **d)** If a facility in the modified Library refers to a function
-    or a table of data to be supplied by an application program that
-    uses the facility, other than as an argument passed when the
-    facility is invoked, then you must make a good faith effort to
-    ensure that, in the event an application does not supply such
-    function or table, the facility still operates, and performs
-    whatever part of its purpose remains meaningful.
-
-    (For example, a function in a library to compute square roots has
-    a purpose that is entirely well-defined independent of
-    the application. Therefore, Subsection 2d requires that any
-    application-supplied function or table used by this function must
-    be optional: if the application does not supply it, the square
-    root function must still compute square roots.)
-
-These requirements apply to the modified work as a whole. If
-identifiable sections of that work are not derived from the Library,
-and can be reasonably considered independent and separate works in
-themselves, then this License, and its terms, do not apply to those
-sections when you distribute them as separate works. But when you
-distribute the same sections as part of a whole which is a work based
-on the Library, the distribution of the whole must be on the terms of
-this License, whose permissions for other licensees extend to the
-entire whole, and thus to each and every part regardless of who wrote
-it.
-
-Thus, it is not the intent of this section to claim rights or contest
-your rights to work written entirely by you; rather, the intent is to
-exercise the right to control the distribution of derivative or
-collective works based on the Library.
-
-In addition, mere aggregation of another work not based on the Library
-with the Library (or with a work based on the Library) on a volume of
-a storage or distribution medium does not bring the other work under
-the scope of this License.
-
-**3.** You may opt to apply the terms of the ordinary GNU General
-Public License instead of this License to a given copy of the Library.
-To do this, you must alter all the notices that refer to this License,
-so that they refer to the ordinary GNU General Public License, version
-2, instead of to this License. (If a newer version than version 2 of
-the ordinary GNU General Public License has appeared, then you can
-specify that version instead if you wish.) Do not make any other
-change in these notices.
-
-Once this change is made in a given copy, it is irreversible for that
-copy, so the ordinary GNU General Public License applies to all
-subsequent copies and derivative works made from that copy.
-
-This option is useful when you wish to copy part of the code of the
-Library into a program that is not a library.
-
-**4.** You may copy and distribute the Library (or a portion or
-derivative of it, under Section 2) in object code or executable form
-under the terms of Sections 1 and 2 above provided that you accompany
-it with the complete corresponding machine-readable source code, which
-must be distributed under the terms of Sections 1 and 2 above on a
-medium customarily used for software interchange.
-
-If distribution of object code is made by offering access to copy from
-a designated place, then offering equivalent access to copy the source
-code from the same place satisfies the requirement to distribute the
-source code, even though third parties are not compelled to copy the
-source along with the object code.
-
-**5.** A program that contains no derivative of any portion of the
-Library, but is designed to work with the Library by being compiled or
-linked with it, is called a "work that uses the Library". Such a work,
-in isolation, is not a derivative work of the Library, and therefore
-falls outside the scope of this License.
-
-However, linking a "work that uses the Library" with the Library
-creates an executable that is a derivative of the Library (because it
-contains portions of the Library), rather than a "work that uses the
-library". The executable is therefore covered by this License. Section
-6 states terms for distribution of such executables.
-
-When a "work that uses the Library" uses material from a header file
-that is part of the Library, the object code for the work may be a
-derivative work of the Library even though the source code is not.
-Whether this is true is especially significant if the work can be
-linked without the Library, or if the work is itself a library. The
-threshold for this to be true is not precisely defined by law.
-
-If such an object file uses only numerical parameters, data structure
-layouts and accessors, and small macros and small inline functions
-(ten lines or less in length), then the use of the object file is
-unrestricted, regardless of whether it is legally a derivative work.
-(Executables containing this object code plus portions of the Library
-will still fall under Section 6.)
-
-Otherwise, if the work is a derivative of the Library, you may
-distribute the object code for the work under the terms of Section 6.
-Any executables containing that work also fall under Section 6,
-whether or not they are linked directly with the Library itself.
-
-**6.** As an exception to the Sections above, you may also compile or
-link a "work that uses the Library" with the Library to produce a work
-containing portions of the Library, and distribute that work under
-terms of your choice, provided that the terms permit modification of
-the work for the customer's own use and reverse engineering for
-debugging such modifications.
-
-You must give prominent notice with each copy of the work that the
-Library is used in it and that the Library and its use are covered by
-this License. You must supply a copy of this License. If the work
-during execution displays copyright notices, you must include the
-copyright notice for the Library among them, as well as a reference
-directing the user to the copy of this License. Also, you must do one
-of these things:
-
--   **a)** Accompany the work with the complete corresponding
-    machine-readable source code for the Library including whatever
-    changes were used in the work (which must be distributed under
-    Sections 1 and 2 above); and, if the work is an executable linked
-    with the Library, with the complete machine-readable "work that
-    uses the Library", as object code and/or source code, so that the
-    user can modify the Library and then relink to produce a modified
-    executable containing the modified Library. (It is understood that
-    the user who changes the contents of definitions files in the
-    Library will not necessarily be able to recompile the application
-    to use the modified definitions.)
--   **b)** Accompany the work with a written offer, valid for at least
-    three years, to give the same user the materials specified in
-    Subsection 6a, above, for a charge no more than the cost of
-    performing this distribution.
--   **c)** If distribution of the work is made by offering access to
-    copy from a designated place, offer equivalent access to copy the
-    above specified materials from the same place.
--   **d)** Verify that the user has already received a copy of these
-    materials or that you have already sent this user a copy.
-
-For an executable, the required form of the "work that uses the
-Library" must include any data and utility programs needed for
-reproducing the executable from it. However, as a special exception,
-the source code distributed need not include anything that is normally
-distributed (in either source or binary form) with the major
-components (compiler, kernel, and so on) of the operating system on
-which the executable runs, unless that component itself accompanies
-the executable.
-
-It may happen that this requirement contradicts the license
-restrictions of other proprietary libraries that do not normally
-accompany the operating system. Such a contradiction means you cannot
-use both them and the Library together in an executable that you
-distribute.
-
-**7.** You may place library facilities that are a work based on the
-Library side-by-side in a single library together with other library
-facilities not covered by this License, and distribute such a combined
-library, provided that the separate distribution of the work based on
-the Library and of the other library facilities is otherwise
-permitted, and provided that you do these two things:
-
--   **a)** Accompany the combined library with a copy of the same work
-    based on the Library, uncombined with any other
-    library facilities. This must be distributed under the terms of
-    the Sections above.
--   **b)** Give prominent notice with the combined library of the fact
-    that part of it is a work based on the Library, and explaining
-    where to find the accompanying uncombined form of the same work.
-
-**8.** You may not copy, modify, sublicense, link with, or distribute
-the Library except as expressly provided under this License. Any
-attempt otherwise to copy, modify, sublicense, link with, or
-distribute the Library is void, and will automatically terminate your
-rights under this License. However, parties who have received copies,
-or rights, from you under this License will not have their licenses
-terminated so long as such parties remain in full compliance.
-
-**9.** You are not required to accept this License, since you have not
-signed it. However, nothing else grants you permission to modify or
-distribute the Library or its derivative works. These actions are
-prohibited by law if you do not accept this License. Therefore, by
-modifying or distributing the Library (or any work based on the
-Library), you indicate your acceptance of this License to do so, and
-all its terms and conditions for copying, distributing or modifying
-the Library or works based on it.
-
-**10.** Each time you redistribute the Library (or any work based on
-the Library), the recipient automatically receives a license from the
-original licensor to copy, distribute, link with or modify the Library
-subject to these terms and conditions. You may not impose any further
-restrictions on the recipients' exercise of the rights granted herein.
-You are not responsible for enforcing compliance by third parties to
-this License.
-
-**11.** If, as a consequence of a court judgment or allegation of
-patent infringement or for any other reason (not limited to patent
-issues), conditions are imposed on you (whether by court order,
-agreement or otherwise) that contradict the conditions of this
-License, they do not excuse you from the conditions of this License.
-If you cannot distribute so as to satisfy simultaneously your
-obligations under this License and any other pertinent obligations,
-then as a consequence you may not distribute the Library at all. For
-example, if a patent license would not permit royalty-free
-redistribution of the Library by all those who receive copies directly
-or indirectly through you, then the only way you could satisfy both it
-and this License would be to refrain entirely from distribution of the
-Library.
-
-If any portion of this section is held invalid or unenforceable under
-any particular circumstance, the balance of the section is intended to
-apply, and the section as a whole is intended to apply in other
-circumstances.
-
-It is not the purpose of this section to induce you to infringe any
-patents or other property right claims or to contest validity of any
-such claims; this section has the sole purpose of protecting the
-integrity of the free software distribution system which is
-implemented by public license practices. Many people have made
-generous contributions to the wide range of software distributed
-through that system in reliance on consistent application of that
-system; it is up to the author/donor to decide if he or she is willing
-to distribute software through any other system and a licensee cannot
-impose that choice.
-
-This section is intended to make thoroughly clear what is believed to
-be a consequence of the rest of this License.
-
-**12.** If the distribution and/or use of the Library is restricted in
-certain countries either by patents or by copyrighted interfaces, the
-original copyright holder who places the Library under this License
-may add an explicit geographical distribution limitation excluding
-those countries, so that distribution is permitted only in or among
-countries not thus excluded. In such case, this License incorporates
-the limitation as if written in the body of this License.
-
-**13.** The Free Software Foundation may publish revised and/or new
-versions of the Library General Public License from time to time. Such
-new versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Library
-specifies a version number of this License which applies to it and
-"any later version", you have the option of following the terms and
-conditions either of that version or of any later version published by
-the Free Software Foundation. If the Library does not specify a
-license version number, you may choose any version ever published by
-the Free Software Foundation.
-
-**14.** If you wish to incorporate parts of the Library into other
-free programs whose distribution conditions are incompatible with
-these, write to the author to ask for permission. For software which
-is copyrighted by the Free Software Foundation, write to the Free
-Software Foundation; we sometimes make exceptions for this. Our
-decision will be guided by the two goals of preserving the free status
-of all derivatives of our free software and of promoting the sharing
-and reuse of software generally.
-
-**NO WARRANTY**
-
-**15.** BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
-WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
-EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
-OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
-KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
-LIBRARY IS WITH YOU. SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
-THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-**16.** IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
-WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
-AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
-FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
-CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
-LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
-RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
-FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
-SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
-DAMAGES.
-
-END OF TERMS AND CONDITIONS
-
-## How to Apply These Terms to Your New Libraries
-
-If you develop a new library, and you want it to be of the greatest
-possible use to the public, we recommend making it free software that
-everyone can redistribute and change. You can do so by permitting
-redistribution under these terms (or, alternatively, under the terms
-of the ordinary General Public License).
-
-To apply these terms, attach the following notices to the library. It
-is safest to attach them to the start of each source file to most
-effectively convey the exclusion of warranty; and each file should
-have at least the "copyright" line and a pointer to where the full
-notice is found.
-
-    one line to give the library's name and an idea of what it does.
-    Copyright (C) year  name of author
-
-    This library is free software; you can redistribute it and/or
-    modify it under the terms of the GNU Library General Public
-    License as published by the Free Software Foundation; either
-    version 2 of the License, or (at your option) any later version.
-
-    This library is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-    Library General Public License for more details.
-
-    You should have received a copy of the GNU Library General Public
-    License along with this library; if not, write to the
-    Free Software Foundation, Inc., 51 Franklin St, Fifth Floor,
-    Boston, MA  02110-1301, USA.
-
-Also add information on how to contact you by electronic and paper
-mail.
-
-You should also get your employer (if you work as a programmer) or
-your school, if any, to sign a "copyright disclaimer" for the library,
-if necessary. Here is a sample; alter the names:
-
-    Yoyodyne, Inc., hereby disclaims all copyright interest in
-    the library `Frob' (a library for tweaking knobs) written
-    by James Random Hacker.
-
-    signature of Ty Coon, 1 April 1990
-    Ty Coon, President of Vice
-
+# GNU LIBRARY GENERAL PUBLIC LICENSE
+
+Version 2, June 1991
+
+    Copyright (C) 1991 Free Software Foundation, Inc.
+    51 Franklin St, Fifth Floor, Boston, MA  02110-1301, USA
+    
+    Everyone is permitted to copy and distribute verbatim copies
+    of this license document, but changing it is not allowed.
+
+    [This is the first released version of the library GPL.  It is
+     numbered 2 because it goes with version 2 of the ordinary GPL.]
+
+## Preamble
+
+The licenses for most software are designed to take away your freedom
+to share and change it. By contrast, the GNU General Public Licenses
+are intended to guarantee your freedom to share and change free
+software--to make sure the software is free for all its users.
+
+This license, the Library General Public License, applies to some
+specially designated Free Software Foundation software, and to any
+other libraries whose authors decide to use it. You can use it for
+your libraries, too.
+
+When we speak of free software, we are referring to freedom, not
+price. Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+this service if you wish), that you receive source code or can get it
+if you want it, that you can change the software or use pieces of it
+in new free programs; and that you know you can do these things.
+
+To protect your rights, we need to make restrictions that forbid
+anyone to deny you these rights or to ask you to surrender the rights.
+These restrictions translate to certain responsibilities for you if
+you distribute copies of the library, or if you modify it.
+
+For example, if you distribute copies of the library, whether gratis
+or for a fee, you must give the recipients all the rights that we gave
+you. You must make sure that they, too, receive or can get the source
+code. If you link a program with the library, you must provide
+complete object files to the recipients so that they can relink them
+with the library, after making changes to the library and recompiling
+it. And you must show them these terms so they know their rights.
+
+Our method of protecting your rights has two steps: (1) copyright the
+library, and (2) offer you this license which gives you legal
+permission to copy, distribute and/or modify the library.
+
+Also, for each distributor's protection, we want to make certain that
+everyone understands that there is no warranty for this free library.
+If the library is modified by someone else and passed on, we want its
+recipients to know that what they have is not the original version, so
+that any problems introduced by others will not reflect on the
+original authors' reputations.
+
+Finally, any free program is threatened constantly by software
+patents. We wish to avoid the danger that companies distributing free
+software will individually obtain patent licenses, thus in effect
+transforming the program into proprietary software. To prevent this,
+we have made it clear that any patent must be licensed for everyone's
+free use or not licensed at all.
+
+Most GNU software, including some libraries, is covered by the
+ordinary GNU General Public License, which was designed for utility
+programs. This license, the GNU Library General Public License,
+applies to certain designated libraries. This license is quite
+different from the ordinary one; be sure to read it in full, and don't
+assume that anything in it is the same as in the ordinary license.
+
+The reason we have a separate public license for some libraries is
+that they blur the distinction we usually make between modifying or
+adding to a program and simply using it. Linking a program with a
+library, without changing the library, is in some sense simply using
+the library, and is analogous to running a utility program or
+application program. However, in a textual and legal sense, the linked
+executable is a combined work, a derivative of the original library,
+and the ordinary General Public License treats it as such.
+
+Because of this blurred distinction, using the ordinary General Public
+License for libraries did not effectively promote software sharing,
+because most developers did not use the libraries. We concluded that
+weaker conditions might promote sharing better.
+
+However, unrestricted linking of non-free programs would deprive the
+users of those programs of all benefit from the free status of the
+libraries themselves. This Library General Public License is intended
+to permit developers of non-free programs to use free libraries, while
+preserving your freedom as a user of such programs to change the free
+libraries that are incorporated in them. (We have not seen how to
+achieve this as regards changes in header files, but we have achieved
+it as regards changes in the actual functions of the Library.) The
+hope is that this will lead to faster development of free libraries.
+
+The precise terms and conditions for copying, distribution and
+modification follow. Pay close attention to the difference between a
+"work based on the library" and a "work that uses the library". The
+former contains code derived from the library, while the latter only
+works together with the library.
+
+Note that it is possible for a library to be covered by the ordinary
+General Public License rather than by this special one.
+
+## TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+**0.** This License Agreement applies to any software library which
+contains a notice placed by the copyright holder or other authorized
+party saying it may be distributed under the terms of this Library
+General Public License (also called "this License"). Each licensee is
+addressed as "you".
+
+A "library" means a collection of software functions and/or data
+prepared so as to be conveniently linked with application programs
+(which use some of those functions and data) to form executables.
+
+The "Library", below, refers to any such software library or work
+which has been distributed under these terms. A "work based on the
+Library" means either the Library or any derivative work under
+copyright law: that is to say, a work containing the Library or a
+portion of it, either verbatim or with modifications and/or translated
+straightforwardly into another language. (Hereinafter, translation is
+included without limitation in the term "modification".)
+
+"Source code" for a work means the preferred form of the work for
+making modifications to it. For a library, complete source code means
+all the source code for all modules it contains, plus any associated
+interface definition files, plus the scripts used to control
+compilation and installation of the library.
+
+Activities other than copying, distribution and modification are not
+covered by this License; they are outside its scope. The act of
+running a program using the Library is not restricted, and output from
+such a program is covered only if its contents constitute a work based
+on the Library (independent of the use of the Library in a tool for
+writing it). Whether that is true depends on what the Library does and
+what the program that uses the Library does.
+
+**1.** You may copy and distribute verbatim copies of the Library's
+complete source code as you receive it, in any medium, provided that
+you conspicuously and appropriately publish on each copy an
+appropriate copyright notice and disclaimer of warranty; keep intact
+all the notices that refer to this License and to the absence of any
+warranty; and distribute a copy of this License along with the
+Library.
+
+You may charge a fee for the physical act of transferring a copy, and
+you may at your option offer warranty protection in exchange for a
+fee.
+
+**2.** You may modify your copy or copies of the Library or any
+portion of it, thus forming a work based on the Library, and copy and
+distribute such modifications or work under the terms of Section 1
+above, provided that you also meet all of these conditions:
+
+-   **a)** The modified work must itself be a software library.
+-   **b)** You must cause the files modified to carry prominent
+    notices stating that you changed the files and the date of
+    any change.
+-   **c)** You must cause the whole of the work to be licensed at no
+    charge to all third parties under the terms of this License.
+-   **d)** If a facility in the modified Library refers to a function
+    or a table of data to be supplied by an application program that
+    uses the facility, other than as an argument passed when the
+    facility is invoked, then you must make a good faith effort to
+    ensure that, in the event an application does not supply such
+    function or table, the facility still operates, and performs
+    whatever part of its purpose remains meaningful.
+
+    (For example, a function in a library to compute square roots has
+    a purpose that is entirely well-defined independent of
+    the application. Therefore, Subsection 2d requires that any
+    application-supplied function or table used by this function must
+    be optional: if the application does not supply it, the square
+    root function must still compute square roots.)
+
+These requirements apply to the modified work as a whole. If
+identifiable sections of that work are not derived from the Library,
+and can be reasonably considered independent and separate works in
+themselves, then this License, and its terms, do not apply to those
+sections when you distribute them as separate works. But when you
+distribute the same sections as part of a whole which is a work based
+on the Library, the distribution of the whole must be on the terms of
+this License, whose permissions for other licensees extend to the
+entire whole, and thus to each and every part regardless of who wrote
+it.
+
+Thus, it is not the intent of this section to claim rights or contest
+your rights to work written entirely by you; rather, the intent is to
+exercise the right to control the distribution of derivative or
+collective works based on the Library.
+
+In addition, mere aggregation of another work not based on the Library
+with the Library (or with a work based on the Library) on a volume of
+a storage or distribution medium does not bring the other work under
+the scope of this License.
+
+**3.** You may opt to apply the terms of the ordinary GNU General
+Public License instead of this License to a given copy of the Library.
+To do this, you must alter all the notices that refer to this License,
+so that they refer to the ordinary GNU General Public License, version
+2, instead of to this License. (If a newer version than version 2 of
+the ordinary GNU General Public License has appeared, then you can
+specify that version instead if you wish.) Do not make any other
+change in these notices.
+
+Once this change is made in a given copy, it is irreversible for that
+copy, so the ordinary GNU General Public License applies to all
+subsequent copies and derivative works made from that copy.
+
+This option is useful when you wish to copy part of the code of the
+Library into a program that is not a library.
+
+**4.** You may copy and distribute the Library (or a portion or
+derivative of it, under Section 2) in object code or executable form
+under the terms of Sections 1 and 2 above provided that you accompany
+it with the complete corresponding machine-readable source code, which
+must be distributed under the terms of Sections 1 and 2 above on a
+medium customarily used for software interchange.
+
+If distribution of object code is made by offering access to copy from
+a designated place, then offering equivalent access to copy the source
+code from the same place satisfies the requirement to distribute the
+source code, even though third parties are not compelled to copy the
+source along with the object code.
+
+**5.** A program that contains no derivative of any portion of the
+Library, but is designed to work with the Library by being compiled or
+linked with it, is called a "work that uses the Library". Such a work,
+in isolation, is not a derivative work of the Library, and therefore
+falls outside the scope of this License.
+
+However, linking a "work that uses the Library" with the Library
+creates an executable that is a derivative of the Library (because it
+contains portions of the Library), rather than a "work that uses the
+library". The executable is therefore covered by this License. Section
+6 states terms for distribution of such executables.
+
+When a "work that uses the Library" uses material from a header file
+that is part of the Library, the object code for the work may be a
+derivative work of the Library even though the source code is not.
+Whether this is true is especially significant if the work can be
+linked without the Library, or if the work is itself a library. The
+threshold for this to be true is not precisely defined by law.
+
+If such an object file uses only numerical parameters, data structure
+layouts and accessors, and small macros and small inline functions
+(ten lines or less in length), then the use of the object file is
+unrestricted, regardless of whether it is legally a derivative work.
+(Executables containing this object code plus portions of the Library
+will still fall under Section 6.)
+
+Otherwise, if the work is a derivative of the Library, you may
+distribute the object code for the work under the terms of Section 6.
+Any executables containing that work also fall under Section 6,
+whether or not they are linked directly with the Library itself.
+
+**6.** As an exception to the Sections above, you may also compile or
+link a "work that uses the Library" with the Library to produce a work
+containing portions of the Library, and distribute that work under
+terms of your choice, provided that the terms permit modification of
+the work for the customer's own use and reverse engineering for
+debugging such modifications.
+
+You must give prominent notice with each copy of the work that the
+Library is used in it and that the Library and its use are covered by
+this License. You must supply a copy of this License. If the work
+during execution displays copyright notices, you must include the
+copyright notice for the Library among them, as well as a reference
+directing the user to the copy of this License. Also, you must do one
+of these things:
+
+-   **a)** Accompany the work with the complete corresponding
+    machine-readable source code for the Library including whatever
+    changes were used in the work (which must be distributed under
+    Sections 1 and 2 above); and, if the work is an executable linked
+    with the Library, with the complete machine-readable "work that
+    uses the Library", as object code and/or source code, so that the
+    user can modify the Library and then relink to produce a modified
+    executable containing the modified Library. (It is understood that
+    the user who changes the contents of definitions files in the
+    Library will not necessarily be able to recompile the application
+    to use the modified definitions.)
+-   **b)** Accompany the work with a written offer, valid for at least
+    three years, to give the same user the materials specified in
+    Subsection 6a, above, for a charge no more than the cost of
+    performing this distribution.
+-   **c)** If distribution of the work is made by offering access to
+    copy from a designated place, offer equivalent access to copy the
+    above specified materials from the same place.
+-   **d)** Verify that the user has already received a copy of these
+    materials or that you have already sent this user a copy.
+
+For an executable, the required form of the "work that uses the
+Library" must include any data and utility programs needed for
+reproducing the executable from it. However, as a special exception,
+the source code distributed need not include anything that is normally
+distributed (in either source or binary form) with the major
+components (compiler, kernel, and so on) of the operating system on
+which the executable runs, unless that component itself accompanies
+the executable.
+
+It may happen that this requirement contradicts the license
+restrictions of other proprietary libraries that do not normally
+accompany the operating system. Such a contradiction means you cannot
+use both them and the Library together in an executable that you
+distribute.
+
+**7.** You may place library facilities that are a work based on the
+Library side-by-side in a single library together with other library
+facilities not covered by this License, and distribute such a combined
+library, provided that the separate distribution of the work based on
+the Library and of the other library facilities is otherwise
+permitted, and provided that you do these two things:
+
+-   **a)** Accompany the combined library with a copy of the same work
+    based on the Library, uncombined with any other
+    library facilities. This must be distributed under the terms of
+    the Sections above.
+-   **b)** Give prominent notice with the combined library of the fact
+    that part of it is a work based on the Library, and explaining
+    where to find the accompanying uncombined form of the same work.
+
+**8.** You may not copy, modify, sublicense, link with, or distribute
+the Library except as expressly provided under this License. Any
+attempt otherwise to copy, modify, sublicense, link with, or
+distribute the Library is void, and will automatically terminate your
+rights under this License. However, parties who have received copies,
+or rights, from you under this License will not have their licenses
+terminated so long as such parties remain in full compliance.
+
+**9.** You are not required to accept this License, since you have not
+signed it. However, nothing else grants you permission to modify or
+distribute the Library or its derivative works. These actions are
+prohibited by law if you do not accept this License. Therefore, by
+modifying or distributing the Library (or any work based on the
+Library), you indicate your acceptance of this License to do so, and
+all its terms and conditions for copying, distributing or modifying
+the Library or works based on it.
+
+**10.** Each time you redistribute the Library (or any work based on
+the Library), the recipient automatically receives a license from the
+original licensor to copy, distribute, link with or modify the Library
+subject to these terms and conditions. You may not impose any further
+restrictions on the recipients' exercise of the rights granted herein.
+You are not responsible for enforcing compliance by third parties to
+this License.
+
+**11.** If, as a consequence of a court judgment or allegation of
+patent infringement or for any other reason (not limited to patent
+issues), conditions are imposed on you (whether by court order,
+agreement or otherwise) that contradict the conditions of this
+License, they do not excuse you from the conditions of this License.
+If you cannot distribute so as to satisfy simultaneously your
+obligations under this License and any other pertinent obligations,
+then as a consequence you may not distribute the Library at all. For
+example, if a patent license would not permit royalty-free
+redistribution of the Library by all those who receive copies directly
+or indirectly through you, then the only way you could satisfy both it
+and this License would be to refrain entirely from distribution of the
+Library.
+
+If any portion of this section is held invalid or unenforceable under
+any particular circumstance, the balance of the section is intended to
+apply, and the section as a whole is intended to apply in other
+circumstances.
+
+It is not the purpose of this section to induce you to infringe any
+patents or other property right claims or to contest validity of any
+such claims; this section has the sole purpose of protecting the
+integrity of the free software distribution system which is
+implemented by public license practices. Many people have made
+generous contributions to the wide range of software distributed
+through that system in reliance on consistent application of that
+system; it is up to the author/donor to decide if he or she is willing
+to distribute software through any other system and a licensee cannot
+impose that choice.
+
+This section is intended to make thoroughly clear what is believed to
+be a consequence of the rest of this License.
+
+**12.** If the distribution and/or use of the Library is restricted in
+certain countries either by patents or by copyrighted interfaces, the
+original copyright holder who places the Library under this License
+may add an explicit geographical distribution limitation excluding
+those countries, so that distribution is permitted only in or among
+countries not thus excluded. In such case, this License incorporates
+the limitation as if written in the body of this License.
+
+**13.** The Free Software Foundation may publish revised and/or new
+versions of the Library General Public License from time to time. Such
+new versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Library
+specifies a version number of this License which applies to it and
+"any later version", you have the option of following the terms and
+conditions either of that version or of any later version published by
+the Free Software Foundation. If the Library does not specify a
+license version number, you may choose any version ever published by
+the Free Software Foundation.
+
+**14.** If you wish to incorporate parts of the Library into other
+free programs whose distribution conditions are incompatible with
+these, write to the author to ask for permission. For software which
+is copyrighted by the Free Software Foundation, write to the Free
+Software Foundation; we sometimes make exceptions for this. Our
+decision will be guided by the two goals of preserving the free status
+of all derivatives of our free software and of promoting the sharing
+and reuse of software generally.
+
+**NO WARRANTY**
+
+**15.** BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
+WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
+EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
+OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
+KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
+LIBRARY IS WITH YOU. SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
+THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+**16.** IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
+WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
+AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
+FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
+CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
+LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
+RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
+FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
+SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
+DAMAGES.
+
+END OF TERMS AND CONDITIONS
+
+## How to Apply These Terms to Your New Libraries
+
+If you develop a new library, and you want it to be of the greatest
+possible use to the public, we recommend making it free software that
+everyone can redistribute and change. You can do so by permitting
+redistribution under these terms (or, alternatively, under the terms
+of the ordinary General Public License).
+
+To apply these terms, attach the following notices to the library. It
+is safest to attach them to the start of each source file to most
+effectively convey the exclusion of warranty; and each file should
+have at least the "copyright" line and a pointer to where the full
+notice is found.
+
+    one line to give the library's name and an idea of what it does.
+    Copyright (C) year  name of author
+
+    This library is free software; you can redistribute it and/or
+    modify it under the terms of the GNU Library General Public
+    License as published by the Free Software Foundation; either
+    version 2 of the License, or (at your option) any later version.
+
+    This library is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+    Library General Public License for more details.
+
+    You should have received a copy of the GNU Library General Public
+    License along with this library; if not, write to the
+    Free Software Foundation, Inc., 51 Franklin St, Fifth Floor,
+    Boston, MA  02110-1301, USA.
+
+Also add information on how to contact you by electronic and paper
+mail.
+
+You should also get your employer (if you work as a programmer) or
+your school, if any, to sign a "copyright disclaimer" for the library,
+if necessary. Here is a sample; alter the names:
+
+    Yoyodyne, Inc., hereby disclaims all copyright interest in
+    the library `Frob' (a library for tweaking knobs) written
+    by James Random Hacker.
+
+    signature of Ty Coon, 1 April 1990
+    Ty Coon, President of Vice
+
 That's all there is to it!
```

### Comparing `routput-0.3/PKG-INFO` & `routput-0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,83 @@
-Metadata-Version: 2.1
-Name: routput
-Version: 0.3
-Summary: Find files recursively and optionally print their contents.
-Author: matrikater (Joel C. Watson)
-Author-email: matrikater@matriko.xyz
-Keywords: python,recursive,find,files,directories,subdirectories,contents,recursive output,routput
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: Natural Language :: English
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-License-File: LICENCE
-
-# Recursive Output Utility
-
-## Overview
-
-This Python script recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
-
-## Requirements
-
-* Python 3.10 or higher,
-* `bat` (optional, for syntax highlighting),
-
-## Installation
-
-### Using pip
-
-```bash
-python -m pip install routput
-```
-
-On some systems, you may need to put the version number of python:
-
-```bash
-python3.12 -m pip install routput
-```
-
-> For the sake of simplicity, whenever I mention `python` in the following sections, you can replace it with `python3.x` version if necessary.
-
-### From source
-
-Clone this repository.
-
-```bash
-git clone https://github.com/nacioboi/routput.git
-```
-
-Navigate to the repository directory.
-
-```bash
-cd routput
-```
-
-And install the package.
-
-```bash
-python -m pip install .
-```
-
-## Usage
-
-```bash
-python -m routput [options]
-```
-
-Options
-
-* -d, --starting-directory: Directory to start the search from (default: current directory).
-* -s, --do-print-structure: Print the directory structure.
-* -e, --extensions: List of file extensions to search for, format [ext1,ext2,...] (default: [c,h]).
-* -p, --do-protect-privacy: Anonymize file paths.
-* -a, --also-include: List of additional filenames to include, format [file1,file2,...].
-* -i, --ignore: List of filenames to ignore, format [file1,file2,dir1,dir2...].
-* -n, --no-print: Don't print the files, just return them.
-* -b, --do-use-bat: Use bat for syntax highlighting.
-* -c, --do-colors: Use different colors for each file type.
-* -h, --help: Show help message and exit.
-
-## Examples
-
-To print the structure of a directory:
-
-```bash
-python -m routput.py -d /path/to/directory -s
-```
-
-To find and print .py files in the current directory, using bat for highlighting:
-
-```bash
-python routput.py -e [py] -b
-```
-
-## License
-
-Open-source software licensed under GPL-2 license.
-
-## V0.3 released on 18th/4/2024
-
-among other small changes, a `--script` option has been added.
-- updated `README.md` to show correct usage,
-- made it so the `__name__` of the module is `routput` when the help is displayed.
-- added an example for the `--script` option.
+# Recursive Output Utility
+
+## Overview
+
+This Python script recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
+
+## Requirements
+
+* Python 3.10 or higher,
+* `bat` (optional, for syntax highlighting),
+
+## Installation
+
+### Using pip
+
+```bash
+python -m pip install routput
+```
+
+On some systems, you may need to put the version number of python:
+
+```bash
+python3.12 -m pip install routput
+```
+
+> For the sake of simplicity, whenever I mention `python` in the following sections, you can replace it with `python3.x` version if necessary.
+
+### From source
+
+Clone this repository.
+
+```bash
+git clone https://github.com/nacioboi/routput.git
+```
+
+Navigate to the repository directory.
+
+```bash
+cd routput
+```
+
+And install the package.
+
+```bash
+python -m pip install .
+```
+
+## Usage
+
+```bash
+python -m routput [options]
+```
+
+Options
+
+* -d, --starting-directory: Directory to start the search from (default: current directory).
+* -s, --do-print-structure: Print the directory structure.
+* -e, --extensions: List of file extensions to search for, format [ext1,ext2,...] (default: [c,h]).
+* -p, --do-protect-privacy: Anonymize file paths.
+* -a, --also-include: List of additional filenames to include, format [file1,file2,...].
+* -i, --ignore: List of filenames to ignore, format [file1,file2,dir1,dir2...].
+* -n, --no-print: Don't print the files, just return them.
+* -b, --do-use-bat: Use bat for syntax highlighting.
+* -c, --do-colors: Use different colors for each file type.
+* -h, --help: Show help message and exit.
+
+## Examples
+
+To print the structure of a directory:
+
+```bash
+python -m routput.py -d /path/to/directory -s
+```
+
+To find and print .py files in the current directory, using bat for highlighting:
+
+```bash
+python routput.py -e [py] -b
+```
+
+## License
+
+Open-source software licensed under GPL-2 license.
```

### Comparing `routput-0.3/README.md` & `routput-0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,94 @@
-# Recursive Output Utility
-
-## Overview
-
-This Python script recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
-
-## Requirements
-
-* Python 3.10 or higher,
-* `bat` (optional, for syntax highlighting),
-
-## Installation
-
-### Using pip
-
-```bash
-python -m pip install routput
-```
-
-On some systems, you may need to put the version number of python:
-
-```bash
-python3.12 -m pip install routput
-```
-
-> For the sake of simplicity, whenever I mention `python` in the following sections, you can replace it with `python3.x` version if necessary.
-
-### From source
-
-Clone this repository.
-
-```bash
-git clone https://github.com/nacioboi/routput.git
-```
-
-Navigate to the repository directory.
-
-```bash
-cd routput
-```
-
-And install the package.
-
-```bash
-python -m pip install .
-```
-
-## Usage
-
-```bash
-python -m routput [options]
-```
-
-Options
-
-* -d, --starting-directory: Directory to start the search from (default: current directory).
-* -s, --do-print-structure: Print the directory structure.
-* -e, --extensions: List of file extensions to search for, format [ext1,ext2,...] (default: [c,h]).
-* -p, --do-protect-privacy: Anonymize file paths.
-* -a, --also-include: List of additional filenames to include, format [file1,file2,...].
-* -i, --ignore: List of filenames to ignore, format [file1,file2,dir1,dir2...].
-* -n, --no-print: Don't print the files, just return them.
-* -b, --do-use-bat: Use bat for syntax highlighting.
-* -c, --do-colors: Use different colors for each file type.
-* -h, --help: Show help message and exit.
-
-## Examples
-
-To print the structure of a directory:
-
-```bash
-python -m routput.py -d /path/to/directory -s
-```
-
-To find and print .py files in the current directory, using bat for highlighting:
-
-```bash
-python routput.py -e [py] -b
-```
-
-## License
-
-Open-source software licensed under GPL-2 license.
+Metadata-Version: 2.1
+Name: routput
+Version: 0.4
+Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
+Author: matrikater (Joel Watson)
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+License-File: LICENCE
+
+# Recursive Output Utility
+
+## Overview
+
+This Python script recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
+
+## Requirements
+
+* Python 3.10 or higher,
+* `bat` (optional, for syntax highlighting),
+
+## Installation
+
+### Using pip
+
+```bash
+python -m pip install routput
+```
+
+On some systems, you may need to put the version number of python:
+
+```bash
+python3.12 -m pip install routput
+```
+
+> For the sake of simplicity, whenever I mention `python` in the following sections, you can replace it with `python3.x` version if necessary.
+
+### From source
+
+Clone this repository.
+
+```bash
+git clone https://github.com/nacioboi/routput.git
+```
+
+Navigate to the repository directory.
+
+```bash
+cd routput
+```
+
+And install the package.
+
+```bash
+python -m pip install .
+```
+
+## Usage
+
+```bash
+python -m routput [options]
+```
+
+Options
+
+* -d, --starting-directory: Directory to start the search from (default: current directory).
+* -s, --do-print-structure: Print the directory structure.
+* -e, --extensions: List of file extensions to search for, format [ext1,ext2,...] (default: [c,h]).
+* -p, --do-protect-privacy: Anonymize file paths.
+* -a, --also-include: List of additional filenames to include, format [file1,file2,...].
+* -i, --ignore: List of filenames to ignore, format [file1,file2,dir1,dir2...].
+* -n, --no-print: Don't print the files, just return them.
+* -b, --do-use-bat: Use bat for syntax highlighting.
+* -c, --do-colors: Use different colors for each file type.
+* -h, --help: Show help message and exit.
+
+## Examples
+
+To print the structure of a directory:
+
+```bash
+python -m routput.py -d /path/to/directory -s
+```
+
+To find and print .py files in the current directory, using bat for highlighting:
+
+```bash
+python routput.py -e [py] -b
+```
+
+## License
+
+Open-source software licensed under GPL-2 license.
+
+## V0.4 released on 2nd/5/2024
+hopefully we will be able to install from pip. :p
```

### Comparing `routput-0.3/routput/routput.py` & `routput-0.4/routput/routput.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,323 +1,323 @@
-#!/usr/bin/env python3
-
-
-
-import os
-import sys
-import argparse
-import subprocess
-from sys import argv as SYS_ARGV
-from dataclasses import dataclass
-
-
-
-@dataclass
-class Validated_Arguments:
-	starting_directory: str
-	extensions_list: list[str]
-	include_list: list[str]
-	ignore_list: list[str]
-	do_print_structure: bool
-	do_protect_privacy: bool
-	do_print: bool
-	do_use_bat: bool
-	do_use_color: bool
-	script: str
-
-
-
-if os.name == "nt":
-	SPLITTER = "\\"
-else:
-	SPLITTER = "/"
-
-
-
-def display_error(err_msg:"str"):
-
-	if os.name != "nt":
-		err_msg = f"\033[31m{err_msg}\033[0m"
-
-	print(err_msg)
-	exit(1)
-
-	return None
-
-	f"END {display_error}"
-
-
-
-def parse_bracket_list(s:"str"):
-
-	return s[1:-1].replace(" ", "").split(",") if s.startswith("[") and s.endswith("]") else []
-
-	f"END {parse_bracket_list}"
-
-
-
-def print_structure(directory:"str"):
-	indent_level = 0
-	for root, _, _ in os.walk(directory):
-
-		indent_level = root[len(directory):].count(os.sep)
-		indent = "\t" * indent_level
-
-		print(f"{indent}+-- {os.path.basename(root)}/", flush=True)
-
-	return None
-
-	f"END {print_structure}"
-
-
-
-def find_children_of_dir(s_dir:"str", extensions:"list[str]", includes:"list[str]", ignores:"list[str]") -> "list[str]":
-	"""
-	Find all the files in the starting_directory that have the extensions in the extensions_list or are in the
-	include_list, while excluding those in the ignore_list.
-	"""
-	# Convert lists to sets for faster checks
-	ignore_set = set(ignores)
-	include_set = set(includes)
-	extensions_tuple = tuple(extensions)  # Prepare a tuple of extensions
-	found_items = []
-	for root, dirs, files in os.walk(s_dir, topdown=True):
-
-		# Modify dirs in-place to prevent os.walk from walking ignored directories
-		dirs[:] = [d for d in dirs if os.path.join(root, d) not in ignore_set]
-
-		for file in files:
-			full_path = os.path.join(root, file)
-			if full_path in ignore_set:
-				continue
-			if file.endswith(extensions_tuple) or full_path in include_set:
-				found_items.append(full_path)
-
-	return found_items
-	f"END {find_children_of_dir}"
-
-
-
-def use_bat_to_print(starting_directory, file_path, i, do_protect_privacy):
-	# TODO: Add support for `do_protect_privacy` in this function.
-	try:
-
-		subprocess.run(["bat", "--paging=never", file_path])
-
-	except Exception as e:
-
-		display_error(f"Could not use bat: {e}")
-
-	return None
-	f"END {use_bat_to_print}"
-
-
-
-def normal_print(starting_directory, item_path, i, do_protect_privacy):
-
-	if os.path.isdir(item_path):
-		return
-	
-	with open(item_path, "r") as f:
-		if do_protect_privacy:
-			item_path = item_path[len(starting_directory):]
-		print(f"[{i}] '{item_path}': ```\n")
-		print(f.read())
-		print("\n```")
-	
-	return None
-	f"END {normal_print}"
-
-
-
-def just_print_paths(item_path:"str", i:"int", args:"Validated_Arguments") -> None:
-
-	path = item_path
-
-	if args.do_protect_privacy:
-		path = "." + path[len(args.starting_directory):]
-		assert os.path.exists(path)
-
-	print(f"[{i}] '{path}'")
-
-	f"END {just_print_paths}"
-
-
-
-def validate_args(args):
-
-	if not os.path.exists(args.starting_directory):
-		err_msg = ""
-		err_msg += f"[[routput.py]]: Invalid `starting_directory`: [{args.starting_directory}]\n"
-		err_msg += "Directory does not exist."
-		display_error(err_msg)
-
-	starting_dir = os.path.abspath(args.starting_directory)
-	extensions_list = [ext if ext.startswith('.') else f".{ext}" for ext in parse_bracket_list(args.extensions)]
-	include_list = parse_bracket_list(args.also_include)
-	ignore_list = parse_bracket_list(args.ignore)
-
-	for i, item in enumerate(ignore_list):
-		if item == "":
-			ignore_list.pop(i)
-			continue
-		if not os.path.exists(item):
-			display_error(f"[[routput.py]]: Invalid `ignore_list` item: [{item}]\nItem does not exist.")
-		ignore_list[i] = os.path.abspath(item)
-
-	for i, item in enumerate(include_list):
-		if item == "":
-			include_list.pop(i)
-			continue
-		if not os.path.exists(item):
-			display_error(f"[[routput.py]]: Invalid `also_include` item: [{item}]\nItem does not exist.")
-		include_list[i] = os.path.abspath(item)
-
-	if args.script != "":
-		file = args.script
-		if not os.path.exists(file):
-			display_error(f"[[routput.py]]: Invalid `script` item: [{file}]\nItem does not exist.")
-		if not os.path.isabs(file):
-			args.script = os.path.abspath(file)
-
-	return Validated_Arguments(
-		starting_directory= 	starting_dir,
-		extensions_list= 	extensions_list,
-		include_list= 		include_list,
-		ignore_list= 		ignore_list,
-		do_print_structure= 	args.do_print_structure,
-		do_protect_privacy= 	args.do_protect_privacy,
-		do_print= 		not args.no_print,
-		do_use_bat= 		args.do_use_bat,
-		do_use_color= 		args.do_colors,
-		script= 		args.script 
-	)
-
-	f"END {validate_args}"
-
-
-
-def main():
-
-	desc = ""
-	desc += "Find files based on their extensions, recursively from a starting directory.\n"
-	appendix_a = ""
-	appendix_a += "Appendix A: Three arguments are passed to your script: "
-	appendix_a += "1) The path to the starting directory. "
-	appendix_a += "2) The path to the file. "
-	appendix_a += "3) The index of the file in the list of found files. "
-	appendix_a += "Also note that if `-p` is used: "
-	appendix_a += "1) the 2nd argument will be the relative path, and "
-	appendix_a += "2) the 1st argument will be the exact string, `HIDDEN`. "
-	appendix_a += "This means it is important to check the 1st argument to determine if the path is hidden. "
-	parser = argparse.ArgumentParser(description=desc, epilog=" | ".join([
-		appendix_a
-	]))
-	
-	parser.add_argument(
-		"-d",
-		"--starting-directory", 
-		type=str, 
-		default=".",
-		help="Directory to start the search from."
-	)
-	parser.add_argument(
-		"-s",
-		"--do-print-structure", 
-		action="store_true",
-		default=False,
-		help="Print the directory structure."
-	)
-	parser.add_argument(
-		"-e",
-		"--extensions", 
-		type=str,
-		required=True,
-		help="List of file extensions to search for, in the format [ext1,ext2,...]."
-	)
-	parser.add_argument(
-		"-p",
-		"--do-protect-privacy", 
-		action="store_true",
-		default=False,
-		help="Anonymize the file paths to be relative to the starting directory."
-	)
-	parser.add_argument(
-		"-a",
-		"--also-include",
-		type=str,
-		default="[]",
-		help="List of additional filenames to include, in the format [file1,file2,...]."
-	)
-	parser.add_argument(
-		"-i",
-		"--ignore",
-		type=str,
-		default="[]",
-		help="List of filenames to ignore, in the format [file1,file2,dir1,dir2...]."
-	)
-	parser.add_argument(
-		"-n",
-		"--no-print",
-		action="store_true",
-		default=False,
-		help="Don't print the files, just return them."
-	)
-	parser.add_argument(
-		"-b",
-		"--do-use-bat",
-		action="store_true",
-		default=False,
-		help="Use `bat` utility for syntax highlighting."
-	)
-	parser.add_argument(
-		"-c",
-		"--do-colors",
-		action="store_true",
-		default=False,
-		help="Use a different color for each file."
-	)
-	parser.add_argument(
-		"--script",
-		type=str,
-		default="",
-		help="Script to run on each file. SEE Appendix A."
-	)
-	
-	if not len(SYS_ARGV) > 1:
-		parser.print_help()
-		exit(0)
-
-	args = parser.parse_args()
-	args = validate_args(args)
-
-	if args.do_print_structure:
-		print("Directory Structure:")
-		print_structure(args.starting_directory)
-	
-	found_items = find_children_of_dir(
-		args.starting_directory,
-		args.extensions_list,
-		args.include_list,
-		args.ignore_list
-	)
-	
-	for i, item_path in enumerate(found_items):
-		if args.script != "":
-			if args.do_protect_privacy:
-				item_path = item_path[len(args.starting_directory):]
-				args.starting_directory = "HIDDEN"
-			subprocess.run([sys.executable, args.script,
-				args.starting_directory, item_path, str(i)
-			])
-		else:
-			if args.do_print:
-				if args.do_use_bat:
-					use_bat_to_print(args.starting_directory, item_path, i, args.do_protect_privacy)
-				else:
-					normal_print(args.starting_directory, item_path, i, args.do_protect_privacy)
-			else:
-				just_print_paths(item_path, i, args)
-
-	return None
-	f"END {main}"
-
+#!/usr/bin/env python3
+
+
+
+import os
+import sys
+import argparse
+import subprocess
+from sys import argv as SYS_ARGV
+from dataclasses import dataclass
+
+
+
+@dataclass
+class Validated_Arguments:
+	starting_directory: str
+	extensions_list: list[str]
+	include_list: list[str]
+	ignore_list: list[str]
+	do_print_structure: bool
+	do_protect_privacy: bool
+	do_print: bool
+	do_use_bat: bool
+	do_use_color: bool
+	script: str
+
+
+
+if os.name == "nt":
+	SPLITTER = "\\"
+else:
+	SPLITTER = "/"
+
+
+
+def display_error(err_msg:"str"):
+
+	if os.name != "nt":
+		err_msg = f"\033[31m{err_msg}\033[0m"
+
+	print(err_msg)
+	exit(1)
+
+	return None
+
+	f"END {display_error}"
+
+
+
+def parse_bracket_list(s:"str"):
+
+	return s[1:-1].replace(" ", "").split(",") if s.startswith("[") and s.endswith("]") else []
+
+	f"END {parse_bracket_list}"
+
+
+
+def print_structure(directory:"str"):
+	indent_level = 0
+	for root, _, _ in os.walk(directory):
+
+		indent_level = root[len(directory):].count(os.sep)
+		indent = "\t" * indent_level
+
+		print(f"{indent}+-- {os.path.basename(root)}/", flush=True)
+
+	return None
+
+	f"END {print_structure}"
+
+
+
+def find_children_of_dir(s_dir:"str", extensions:"list[str]", includes:"list[str]", ignores:"list[str]") -> "list[str]":
+	"""
+	Find all the files in the starting_directory that have the extensions in the extensions_list or are in the
+	include_list, while excluding those in the ignore_list.
+	"""
+	# Convert lists to sets for faster checks
+	ignore_set = set(ignores)
+	include_set = set(includes)
+	extensions_tuple = tuple(extensions)  # Prepare a tuple of extensions
+	found_items = []
+	for root, dirs, files in os.walk(s_dir, topdown=True):
+
+		# Modify dirs in-place to prevent os.walk from walking ignored directories
+		dirs[:] = [d for d in dirs if os.path.join(root, d) not in ignore_set]
+
+		for file in files:
+			full_path = os.path.join(root, file)
+			if full_path in ignore_set:
+				continue
+			if file.endswith(extensions_tuple) or full_path in include_set:
+				found_items.append(full_path)
+
+	return found_items
+	f"END {find_children_of_dir}"
+
+
+
+def use_bat_to_print(starting_directory, file_path, i, do_protect_privacy):
+	# TODO: Add support for `do_protect_privacy` in this function.
+	try:
+
+		subprocess.run(["bat", "--paging=never", file_path])
+
+	except Exception as e:
+
+		display_error(f"Could not use bat: {e}")
+
+	return None
+	f"END {use_bat_to_print}"
+
+
+
+def normal_print(starting_directory, item_path, i, do_protect_privacy):
+
+	if os.path.isdir(item_path):
+		return
+	
+	with open(item_path, "r") as f:
+		if do_protect_privacy:
+			item_path = item_path[len(starting_directory):]
+		print(f"[{i}] '{item_path}': ```\n")
+		print(f.read())
+		print("\n```")
+	
+	return None
+	f"END {normal_print}"
+
+
+
+def just_print_paths(item_path:"str", i:"int", args:"Validated_Arguments") -> None:
+
+	path = item_path
+
+	if args.do_protect_privacy:
+		path = "." + path[len(args.starting_directory):]
+		assert os.path.exists(path)
+
+	print(f"[{i}] '{path}'")
+
+	f"END {just_print_paths}"
+
+
+
+def validate_args(args):
+
+	if not os.path.exists(args.starting_directory):
+		err_msg = ""
+		err_msg += f"[[routput.py]]: Invalid `starting_directory`: [{args.starting_directory}]\n"
+		err_msg += "Directory does not exist."
+		display_error(err_msg)
+
+	starting_dir = os.path.abspath(args.starting_directory)
+	extensions_list = [ext if ext.startswith('.') else f".{ext}" for ext in parse_bracket_list(args.extensions)]
+	include_list = parse_bracket_list(args.also_include)
+	ignore_list = parse_bracket_list(args.ignore)
+
+	for i, item in enumerate(ignore_list):
+		if item == "":
+			ignore_list.pop(i)
+			continue
+		if not os.path.exists(item):
+			display_error(f"[[routput.py]]: Invalid `ignore_list` item: [{item}]\nItem does not exist.")
+		ignore_list[i] = os.path.abspath(item)
+
+	for i, item in enumerate(include_list):
+		if item == "":
+			include_list.pop(i)
+			continue
+		if not os.path.exists(item):
+			display_error(f"[[routput.py]]: Invalid `also_include` item: [{item}]\nItem does not exist.")
+		include_list[i] = os.path.abspath(item)
+
+	if args.script != "":
+		file = args.script
+		if not os.path.exists(file):
+			display_error(f"[[routput.py]]: Invalid `script` item: [{file}]\nItem does not exist.")
+		if not os.path.isabs(file):
+			args.script = os.path.abspath(file)
+
+	return Validated_Arguments(
+		starting_directory= 	starting_dir,
+		extensions_list= 	extensions_list,
+		include_list= 		include_list,
+		ignore_list= 		ignore_list,
+		do_print_structure= 	args.do_print_structure,
+		do_protect_privacy= 	args.do_protect_privacy,
+		do_print= 		not args.no_print,
+		do_use_bat= 		args.do_use_bat,
+		do_use_color= 		args.do_colors,
+		script= 		args.script 
+	)
+
+	f"END {validate_args}"
+
+
+
+def main():
+
+	desc = ""
+	desc += "Find files based on their extensions, recursively from a starting directory.\n"
+	appendix_a = ""
+	appendix_a += "Appendix A: Three arguments are passed to your script: "
+	appendix_a += "1) The path to the starting directory. "
+	appendix_a += "2) The path to the file. "
+	appendix_a += "3) The index of the file in the list of found files. "
+	appendix_a += "Also note that if `-p` is used: "
+	appendix_a += "1) the 2nd argument will be the relative path, and "
+	appendix_a += "2) the 1st argument will be the exact string, `HIDDEN`. "
+	appendix_a += "This means it is important to check the 1st argument to determine if the path is hidden. "
+	parser = argparse.ArgumentParser(description=desc, epilog=" | ".join([
+		appendix_a
+	]))
+	
+	parser.add_argument(
+		"-d",
+		"--starting-directory", 
+		type=str, 
+		default=".",
+		help="Directory to start the search from."
+	)
+	parser.add_argument(
+		"-s",
+		"--do-print-structure", 
+		action="store_true",
+		default=False,
+		help="Print the directory structure."
+	)
+	parser.add_argument(
+		"-e",
+		"--extensions", 
+		type=str,
+		required=True,
+		help="List of file extensions to search for, in the format [ext1,ext2,...]."
+	)
+	parser.add_argument(
+		"-p",
+		"--do-protect-privacy", 
+		action="store_true",
+		default=False,
+		help="Anonymize the file paths to be relative to the starting directory."
+	)
+	parser.add_argument(
+		"-a",
+		"--also-include",
+		type=str,
+		default="[]",
+		help="List of additional filenames to include, in the format [file1,file2,...]."
+	)
+	parser.add_argument(
+		"-i",
+		"--ignore",
+		type=str,
+		default="[]",
+		help="List of filenames to ignore, in the format [file1,file2,dir1,dir2...]."
+	)
+	parser.add_argument(
+		"-n",
+		"--no-print",
+		action="store_true",
+		default=False,
+		help="Don't print the files, just return them."
+	)
+	parser.add_argument(
+		"-b",
+		"--do-use-bat",
+		action="store_true",
+		default=False,
+		help="Use `bat` utility for syntax highlighting."
+	)
+	parser.add_argument(
+		"-c",
+		"--do-colors",
+		action="store_true",
+		default=False,
+		help="Use a different color for each file."
+	)
+	parser.add_argument(
+		"--script",
+		type=str,
+		default="",
+		help="Script to run on each file. SEE Appendix A."
+	)
+	
+	if not len(SYS_ARGV) > 1:
+		parser.print_help()
+		exit(0)
+
+	args = parser.parse_args()
+	args = validate_args(args)
+
+	if args.do_print_structure:
+		print("Directory Structure:")
+		print_structure(args.starting_directory)
+	
+	found_items = find_children_of_dir(
+		args.starting_directory,
+		args.extensions_list,
+		args.include_list,
+		args.ignore_list
+	)
+	
+	for i, item_path in enumerate(found_items):
+		if args.script != "":
+			if args.do_protect_privacy:
+				item_path = item_path[len(args.starting_directory):]
+				args.starting_directory = "HIDDEN"
+			subprocess.run([sys.executable, args.script,
+				args.starting_directory, item_path, str(i)
+			])
+		else:
+			if args.do_print:
+				if args.do_use_bat:
+					use_bat_to_print(args.starting_directory, item_path, i, args.do_protect_privacy)
+				else:
+					normal_print(args.starting_directory, item_path, i, args.do_protect_privacy)
+			else:
+				just_print_paths(item_path, i, args)
+
+	return None
+	f"END {main}"
+
```

