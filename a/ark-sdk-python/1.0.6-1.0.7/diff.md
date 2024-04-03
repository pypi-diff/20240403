# Comparing `tmp/ark_sdk_python-1.0.6-py3-none-any.whl.zip` & `tmp/ark_sdk_python-1.0.7-py3-none-any.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    248042 (000000000003C8EAh)
-  Actual end-cent-dir record offset:        248020 (000000000003C8D4h)
-  Expected end-cent-dir record offset:      248020 (000000000003C8D4h)
+  Zip archive file size:                    250521 (000000000003D299h)
+  Actual end-cent-dir record offset:        250499 (000000000003D283h)
+  Expected end-cent-dir record offset:      250499 (000000000003D283h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 310 entries.
-  The central directory is 39005 (000000000000985Dh) bytes long,
+  central directory contains 313 entries.
+  The central directory is 39427 (0000000000009A03h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 209015 (0000000000033077h).
+  is 211072 (0000000000033880h).
 
 
 Central directory entry #1:
 ---------------------------
 
   ark_sdk_python/
 
@@ -25,17 +25,17 @@
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             15 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -50,69 +50,32 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  ark_sdk_python/ark_api.py
+  ark_sdk_python/examples/
 
   offset of local header from start of archive:   73
                                                   (0000000000000049h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         8149ce2b
-  compressed size:                                1220 bytes
-  uncompressed size:                              6836 bytes
-  length of filename:                             25 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e9 03 00 00 04 7f 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #3:
----------------------------
-
-  ark_sdk_python/auth/
-
-  offset of local header from start of archive:   1376
-                                                  (0000000000000560h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             20 characters
+  length of filename:                             24 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -120,36 +83,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #4:
+Central directory entry #3:
 ---------------------------
 
-  ark_sdk_python/auth/__init__.py
+  ark_sdk_python/examples/session_monitoring_activites.py
 
-  offset of local header from start of archive:   1454
-                                                  (00000000000005AEh) bytes
+  offset of local header from start of archive:   155
+                                                  (000000000000009Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c6fe8fd3
-  compressed size:                                281 bytes
-  uncompressed size:                              620 bytes
-  length of filename:                             31 characters
+  32-bit CRC value (hex):                         9a41daa0
+  compressed size:                                578 bytes
+  uncompressed size:                              1632 bytes
+  length of filename:                             55 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -157,36 +120,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #5:
+Central directory entry #4:
 ---------------------------
 
-  ark_sdk_python/auth/ark_isp_auth.py
+  ark_sdk_python/examples/create_dpa_db_environment.py
 
-  offset of local header from start of archive:   1824
-                                                  (0000000000000720h) bytes
+  offset of local header from start of archive:   846
+                                                  (000000000000034Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c4cc674b
-  compressed size:                                1794 bytes
-  uncompressed size:                              9572 bytes
-  length of filename:                             35 characters
+  32-bit CRC value (hex):                         42e1fc46
+  compressed size:                                1110 bytes
+  uncompressed size:                              3744 bytes
+  length of filename:                             52 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -194,36 +157,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #6:
+Central directory entry #5:
 ---------------------------
 
-  ark_sdk_python/auth/ark_auth.py
+  ark_sdk_python/ark_api.py
 
-  offset of local header from start of archive:   3711
-                                                  (0000000000000E7Fh) bytes
+  offset of local header from start of archive:   2066
+                                                  (0000000000000812h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         fce55146
-  compressed size:                                2570 bytes
-  uncompressed size:                              12740 bytes
-  length of filename:                             31 characters
+  32-bit CRC value (hex):                         8149ce2b
+  compressed size:                                1220 bytes
+  uncompressed size:                              6836 bytes
+  length of filename:                             25 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -231,35 +194,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #6:
 ---------------------------
 
-  ark_sdk_python/auth/identity/
+  ark_sdk_python/auth/
 
-  offset of local header from start of archive:   6370
-                                                  (00000000000018E2h) bytes
+  offset of local header from start of archive:   3369
+                                                  (0000000000000D29h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             29 characters
+  length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -267,36 +230,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #8:
+Central directory entry #7:
 ---------------------------
 
-  ark_sdk_python/auth/identity/__init__.py
+  ark_sdk_python/auth/__init__.py
 
-  offset of local header from start of archive:   6457
-                                                  (0000000000001939h) bytes
+  offset of local header from start of archive:   3447
+                                                  (0000000000000D77h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         8a15262f
-  compressed size:                                130 bytes
-  uncompressed size:                              328 bytes
-  length of filename:                             40 characters
+  32-bit CRC value (hex):                         c6fe8fd3
+  compressed size:                                281 bytes
+  uncompressed size:                              620 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -304,36 +267,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #9:
+Central directory entry #8:
 ---------------------------
 
-  ark_sdk_python/auth/identity/ark_identity.py
+  ark_sdk_python/auth/ark_isp_auth.py
 
-  offset of local header from start of archive:   6685
-                                                  (0000000000001A1Dh) bytes
+  offset of local header from start of archive:   3817
+                                                  (0000000000000EE9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         6727459a
-  compressed size:                                6074 bytes
-  uncompressed size:                              28247 bytes
-  length of filename:                             44 characters
+  32-bit CRC value (hex):                         c4cc674b
+  compressed size:                                1794 bytes
+  uncompressed size:                              9572 bytes
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -341,73 +304,72 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #10:
+Central directory entry #9:
 ---------------------------
 
-  ark_sdk_python/auth/identity/ark_identity_fqdn_resolver.py
+  ark_sdk_python/auth/identity/
 
-  offset of local header from start of archive:   12861
-                                                  (000000000000323Dh) bytes
+  offset of local header from start of archive:   5704
+                                                  (0000000000001648h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         934daef9
-  compressed size:                                1511 bytes
-  uncompressed size:                              4777 bytes
-  length of filename:                             58 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #11:
+Central directory entry #10:
 ---------------------------
 
-  ark_sdk_python/auth/identity/ark_identity_service_user.py
+  ark_sdk_python/auth/identity/ark_identity_fqdn_resolver.py
 
-  offset of local header from start of archive:   14488
-                                                  (0000000000003898h) bytes
+  offset of local header from start of archive:   5791
+                                                  (000000000000169Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7baeca7f
-  compressed size:                                2106 bytes
-  uncompressed size:                              7495 bytes
-  length of filename:                             57 characters
+  32-bit CRC value (hex):                         934daef9
+  compressed size:                                1511 bytes
+  uncompressed size:                              4777 bytes
+  length of filename:                             58 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -415,36 +377,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #12:
+Central directory entry #11:
 ---------------------------
 
-  ark_sdk_python/__init__.py
+  ark_sdk_python/auth/identity/__init__.py
 
-  offset of local header from start of archive:   16709
-                                                  (0000000000004145h) bytes
+  offset of local header from start of archive:   7418
+                                                  (0000000000001CFAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         ebba75f7
-  compressed size:                                118 bytes
-  uncompressed size:                              226 bytes
-  length of filename:                             26 characters
+  32-bit CRC value (hex):                         8a15262f
+  compressed size:                                130 bytes
+  uncompressed size:                              328 bytes
+  length of filename:                             40 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -452,71 +414,73 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #13:
+Central directory entry #12:
 ---------------------------
 
-  ark_sdk_python/services/
+  ark_sdk_python/auth/identity/ark_identity_service_user.py
 
-  offset of local header from start of archive:   16911
-                                                  (000000000000420Fh) bytes
+  offset of local header from start of archive:   7646
+                                                  (0000000000001DDEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             24 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         7baeca7f
+  compressed size:                                2106 bytes
+  uncompressed size:                              7495 bytes
+  length of filename:                             57 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #14:
+Central directory entry #13:
 ---------------------------
 
-  ark_sdk_python/services/__init__.py
+  ark_sdk_python/auth/identity/ark_identity.py
 
-  offset of local header from start of archive:   16993
-                                                  (0000000000004261h) bytes
+  offset of local header from start of archive:   9867
+                                                  (000000000000268Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         32d70693
-  compressed size:                                1 bytes
-  uncompressed size:                              1 bytes
-  length of filename:                             35 characters
+  32-bit CRC value (hex):                         6727459a
+  compressed size:                                6074 bytes
+  uncompressed size:                              28247 bytes
+  length of filename:                             44 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -524,36 +488,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #15:
+Central directory entry #14:
 ---------------------------
 
-  ark_sdk_python/services/ark_service.py
+  ark_sdk_python/auth/ark_auth.py
 
-  offset of local header from start of archive:   17087
-                                                  (00000000000042BFh) bytes
+  offset of local header from start of archive:   16043
+                                                  (0000000000003EABh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         6c78ace9
-  compressed size:                                683 bytes
-  uncompressed size:                              2314 bytes
-  length of filename:                             38 characters
+  32-bit CRC value (hex):                         677d4166
+  compressed size:                                2626 bytes
+  uncompressed size:                              12947 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -561,31 +525,31 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #16:
+Central directory entry #15:
 ---------------------------
 
-  ark_sdk_python/services/dpa/
+  ark_sdk_python/cli_services/
 
-  offset of local header from start of archive:   17866
-                                                  (00000000000045CAh) bytes
+  offset of local header from start of archive:   18758
+                                                  (0000000000004946h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -597,31 +561,31 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #17:
+Central directory entry #16:
 ---------------------------
 
-  ark_sdk_python/services/dpa/sso/
+  ark_sdk_python/cli_services/dpa/
 
-  offset of local header from start of archive:   17952
-                                                  (0000000000004620h) bytes
+  offset of local header from start of archive:   18844
+                                                  (000000000000499Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -633,73 +597,72 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #18:
+Central directory entry #17:
 ---------------------------
 
-  ark_sdk_python/services/dpa/sso/__init__.py
+  ark_sdk_python/cli_services/dpa/vm/
 
-  offset of local header from start of archive:   18042
-                                                  (000000000000467Ah) bytes
+  offset of local header from start of archive:   18934
+                                                  (00000000000049F6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c7961b71
-  compressed size:                                92 bytes
-  uncompressed size:                              120 bytes
-  length of filename:                             43 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #19:
+Central directory entry #18:
 ---------------------------
 
-  ark_sdk_python/services/dpa/sso/ark_dpa_sso_service.py
+  ark_sdk_python/cli_services/dpa/vm/__init__.py
 
-  offset of local header from start of archive:   18235
-                                                  (000000000000473Bh) bytes
+  offset of local header from start of archive:   19027
+                                                  (0000000000004A53h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         b72eea43
-  compressed size:                                2696 bytes
-  uncompressed size:                              15817 bytes
-  length of filename:                             54 characters
+  32-bit CRC value (hex):                         1a2ea348
+  compressed size:                                109 bytes
+  uncompressed size:                              157 bytes
+  length of filename:                             46 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -707,36 +670,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #20:
+Central directory entry #19:
 ---------------------------
 
-  ark_sdk_python/services/dpa/__init__.py
+  ark_sdk_python/cli_services/dpa/vm/ark_dpa_vm_policies_editor_service.py
 
-  offset of local header from start of archive:   21043
-                                                  (0000000000005233h) bytes
+  offset of local header from start of archive:   19240
+                                                  (0000000000004B28h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         371d7e9e
-  compressed size:                                78 bytes
-  uncompressed size:                              87 bytes
-  length of filename:                             39 characters
+  32-bit CRC value (hex):                         ceb6cbf1
+  compressed size:                                2177 bytes
+  uncompressed size:                              8709 bytes
+  length of filename:                             72 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -744,72 +707,71 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #21:
+Central directory entry #20:
 ---------------------------
 
-  ark_sdk_python/services/dpa/ark_dpa_api.py
+  ark_sdk_python/cli_services/dpa/__init__.py
 
-  offset of local header from start of archive:   21218
-                                                  (00000000000052E2h) bytes
+  offset of local header from start of archive:   21547
+                                                  (000000000000542Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         e142e33a
-  compressed size:                                512 bytes
-  uncompressed size:                              3077 bytes
-  length of filename:                             42 characters
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             43 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #22:
+Central directory entry #21:
 ---------------------------
 
-  ark_sdk_python/services/dpa/db/
+  ark_sdk_python/cli_services/dpa/common/
 
-  offset of local header from start of archive:   21830
-                                                  (0000000000005546h) bytes
+  offset of local header from start of archive:   21648
+                                                  (0000000000005490h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             31 characters
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -817,36 +779,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #23:
+Central directory entry #22:
 ---------------------------
 
-  ark_sdk_python/services/dpa/db/__init__.py
+  ark_sdk_python/cli_services/dpa/common/ark_dpa_base_policies_editor_service.py
 
-  offset of local header from start of archive:   21919
-                                                  (000000000000559Fh) bytes
+  offset of local header from start of archive:   21745
+                                                  (00000000000054F1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         40fa751f
-  compressed size:                                91 bytes
-  uncompressed size:                              116 bytes
-  length of filename:                             42 characters
+  32-bit CRC value (hex):                         ce4aecda
+  compressed size:                                4913 bytes
+  uncompressed size:                              27869 bytes
+  length of filename:                             78 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -854,72 +816,71 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #24:
+Central directory entry #23:
 ---------------------------
 
-  ark_sdk_python/services/dpa/db/ark_dpa_db_service.py
+  ark_sdk_python/cli_services/dpa/common/__init__.py
 
-  offset of local header from start of archive:   22110
-                                                  (000000000000565Eh) bytes
+  offset of local header from start of archive:   26794
+                                                  (00000000000068AAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         baf62c49
-  compressed size:                                2389 bytes
-  uncompressed size:                              9080 bytes
-  length of filename:                             52 characters
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #25:
+Central directory entry #24:
 ---------------------------
 
-  ark_sdk_python/services/dpa/policies/
+  ark_sdk_python/cli_services/dpa/db/
 
-  offset of local header from start of archive:   24609
-                                                  (0000000000006021h) bytes
+  offset of local header from start of archive:   26902
+                                                  (0000000000006916h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             37 characters
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -927,72 +888,73 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #26:
+Central directory entry #25:
 ---------------------------
 
-  ark_sdk_python/services/dpa/policies/vm/
+  ark_sdk_python/cli_services/dpa/db/__init__.py
 
-  offset of local header from start of archive:   24704
-                                                  (0000000000006080h) bytes
+  offset of local header from start of archive:   26995
+                                                  (0000000000006973h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             40 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         0df547f0
+  compressed size:                                108 bytes
+  uncompressed size:                              157 bytes
+  length of filename:                             46 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #27:
+Central directory entry #26:
 ---------------------------
 
-  ark_sdk_python/services/dpa/policies/vm/ark_dpa_vm_policies_service.py
+  ark_sdk_python/cli_services/dpa/db/ark_dpa_db_policies_editor_service.py
 
-  offset of local header from start of archive:   24802
-                                                  (00000000000060E2h) bytes
+  offset of local header from start of archive:   27207
+                                                  (0000000000006A47h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         2100f2ae
-  compressed size:                                2466 bytes
-  uncompressed size:                              12681 bytes
-  length of filename:                             70 characters
+  32-bit CRC value (hex):                         18357480
+  compressed size:                                2356 bytes
+  uncompressed size:                              10620 bytes
+  length of filename:                             72 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1000,36 +962,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #28:
+Central directory entry #27:
 ---------------------------
 
-  ark_sdk_python/services/dpa/policies/vm/__init__.py
+  ark_sdk_python/cli_services/__init__.py
 
-  offset of local header from start of archive:   27396
-                                                  (0000000000006B04h) bytes
+  offset of local header from start of archive:   29693
+                                                  (00000000000073FDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         a29a2454
-  compressed size:                                99 bytes
-  uncompressed size:                              143 bytes
-  length of filename:                             51 characters
+  32-bit CRC value (hex):                         9c432aca
+  compressed size:                                77 bytes
+  uncompressed size:                              87 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1037,71 +999,72 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #29:
+Central directory entry #28:
 ---------------------------
 
-  ark_sdk_python/services/dpa/policies/__init__.py
+  ark_sdk_python/cli_services/ark_cli_api.py
 
-  offset of local header from start of archive:   27604
-                                                  (0000000000006BD4h) bytes
+  offset of local header from start of archive:   29867
+                                                  (00000000000074ABh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             48 characters
+  32-bit CRC value (hex):                         9e30d8a1
+  compressed size:                                288 bytes
+  uncompressed size:                              912 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #30:
+Central directory entry #29:
 ---------------------------
 
-  ark_sdk_python/services/dpa/policies/db/
+  ark_sdk_python/actions/
 
-  offset of local header from start of archive:   27710
-                                                  (0000000000006C3Eh) bytes
+  offset of local header from start of archive:   30255
+                                                  (000000000000762Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             40 characters
+  length of filename:                             23 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -1109,36 +1072,73 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
+Central directory entry #30:
+---------------------------
+
+  ark_sdk_python/actions/ark_action.py
+
+  offset of local header from start of archive:   30336
+                                                  (0000000000007680h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         50be69ae
+  compressed size:                                1049 bytes
+  uncompressed size:                              3546 bytes
+  length of filename:                             36 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 7f 00 00 00.
+
+  There is no file comment.
+
 Central directory entry #31:
 ---------------------------
 
-  ark_sdk_python/services/dpa/policies/db/__init__.py
+  ark_sdk_python/actions/ark_service_exec_action.py
 
-  offset of local header from start of archive:   27808
-                                                  (0000000000006CA0h) bytes
+  offset of local header from start of archive:   31479
+                                                  (0000000000007AF7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         5f59e261
-  compressed size:                                98 bytes
-  uncompressed size:                              143 bytes
-  length of filename:                             51 characters
+  32-bit CRC value (hex):                         bae7a058
+  compressed size:                                1152 bytes
+  uncompressed size:                              5109 bytes
+  length of filename:                             49 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1149,33 +1149,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #32:
 ---------------------------
 
-  ark_sdk_python/services/dpa/policies/db/ark_dpa_db_policies_service.py
+  ark_sdk_python/actions/__init__.py
 
-  offset of local header from start of archive:   28015
-                                                  (0000000000006D6Fh) bytes
+  offset of local header from start of archive:   32738
+                                                  (0000000000007FE2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7f980b15
-  compressed size:                                2149 bytes
-  uncompressed size:                              10943 bytes
-  length of filename:                             70 characters
+  32-bit CRC value (hex):                         98b326d0
+  compressed size:                                175 bytes
+  uncompressed size:                              659 bytes
+  length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1186,141 +1186,144 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #33:
 ---------------------------
 
-  ark_sdk_python/services/dpa/secrets/
+  ark_sdk_python/actions/ark_configure_action.py
 
-  offset of local header from start of archive:   30292
-                                                  (0000000000007654h) bytes
+  offset of local header from start of archive:   33005
+                                                  (00000000000080EDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         fbbc9923
+  compressed size:                                2981 bytes
+  uncompressed size:                              15926 bytes
+  length of filename:                             46 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #34:
 ---------------------------
 
-  ark_sdk_python/services/dpa/secrets/__init__.py
+  ark_sdk_python/actions/ark_profiles_action.py
 
-  offset of local header from start of archive:   30386
-                                                  (00000000000076B2h) bytes
+  offset of local header from start of archive:   36090
+                                                  (0000000000008CFAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             47 characters
+  32-bit CRC value (hex):                         79e016a0
+  compressed size:                                1995 bytes
+  uncompressed size:                              9638 bytes
+  length of filename:                             45 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #35:
 ---------------------------
 
-  ark_sdk_python/services/dpa/secrets/db/
+  ark_sdk_python/actions/ark_cache_action.py
 
-  offset of local header from start of archive:   30491
-                                                  (000000000000771Bh) bytes
+  offset of local header from start of archive:   38188
+                                                  (000000000000952Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             39 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         f5d8dbab
+  compressed size:                                790 bytes
+  uncompressed size:                              2392 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #36:
 ---------------------------
 
-  ark_sdk_python/services/dpa/secrets/db/__init__.py
+  ark_sdk_python/actions/ark_exec_action.py
 
-  offset of local header from start of archive:   30588
-                                                  (000000000000777Ch) bytes
+  offset of local header from start of archive:   39078
+                                                  (00000000000098A6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         6066091e
-  compressed size:                                97 bytes
-  uncompressed size:                              139 bytes
-  length of filename:                             50 characters
+  32-bit CRC value (hex):                         dc6fe184
+  compressed size:                                3117 bytes
+  uncompressed size:                              14323 bytes
+  length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1331,33 +1334,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #37:
 ---------------------------
 
-  ark_sdk_python/services/dpa/secrets/db/ark_dpa_db_secrets_service.py
+  ark_sdk_python/actions/ark_login_action.py
 
-  offset of local header from start of archive:   30793
-                                                  (0000000000007849h) bytes
+  offset of local header from start of archive:   42294
+                                                  (000000000000A536h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         50bcf558
-  compressed size:                                2590 bytes
-  uncompressed size:                              15607 bytes
-  length of filename:                             68 characters
+  32-bit CRC value (hex):                         755a6417
+  compressed size:                                2399 bytes
+  uncompressed size:                              10357 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1368,32 +1371,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #38:
 ---------------------------
 
-  ark_sdk_python/services/dpa/certificates/
+  ark_sdk_python/__init__.py
+
+  offset of local header from start of archive:   44793
+                                                  (000000000000AEF9h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         ebba75f7
+  compressed size:                                118 bytes
+  uncompressed size:                              226 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 7f 00 00 00.
 
-  offset of local header from start of archive:   33509
-                                                  (00000000000082E5h) bytes
+  There is no file comment.
+
+Central directory entry #39:
+---------------------------
+
+  ark_sdk_python/common/
+
+  offset of local header from start of archive:   44995
+                                                  (000000000000AFC3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             41 characters
+  length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -1401,36 +1441,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #39:
+Central directory entry #40:
 ---------------------------
 
-  ark_sdk_python/services/dpa/certificates/__init__.py
+  ark_sdk_python/common/ark_system_config.py
 
-  offset of local header from start of archive:   33608
-                                                  (0000000000008348h) bytes
+  offset of local header from start of archive:   45075
+                                                  (000000000000B013h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         b768beed
-  compressed size:                                96 bytes
-  uncompressed size:                              149 bytes
-  length of filename:                             52 characters
+  32-bit CRC value (hex):                         70cb4a96
+  compressed size:                                600 bytes
+  uncompressed size:                              2436 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1438,36 +1478,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #40:
+Central directory entry #41:
 ---------------------------
 
-  ark_sdk_python/services/dpa/certificates/ark_dpa_certificates_service.py
+  ark_sdk_python/common/ark_random_utils.py
 
-  offset of local header from start of archive:   33814
-                                                  (0000000000008416h) bytes
+  offset of local header from start of archive:   45775
+                                                  (000000000000B2CFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         1b597d2a
-  compressed size:                                1662 bytes
-  uncompressed size:                              7989 bytes
-  length of filename:                             72 characters
+  32-bit CRC value (hex):                         11c04bfb
+  compressed size:                                255 bytes
+  uncompressed size:                              671 bytes
+  length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1475,35 +1515,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #41:
+Central directory entry #42:
 ---------------------------
 
-  ark_sdk_python/services/dpa/k8s/
+  ark_sdk_python/common/env/
 
-  offset of local header from start of archive:   35606
-                                                  (0000000000008B16h) bytes
+  offset of local header from start of archive:   46129
+                                                  (000000000000B431h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             32 characters
+  length of filename:                             26 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -1511,36 +1551,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #42:
+Central directory entry #43:
 ---------------------------
 
-  ark_sdk_python/services/dpa/k8s/__init__.py
+  ark_sdk_python/common/env/ark_env_mapping.py
 
-  offset of local header from start of archive:   35696
-                                                  (0000000000008B70h) bytes
+  offset of local header from start of archive:   46213
+                                                  (000000000000B485h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         b0460af6
-  compressed size:                                87 bytes
-  uncompressed size:                              113 bytes
-  length of filename:                             43 characters
+  32-bit CRC value (hex):                         99fe050b
+  compressed size:                                520 bytes
+  uncompressed size:                              1132 bytes
+  length of filename:                             44 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1548,36 +1588,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #43:
+Central directory entry #44:
 ---------------------------
 
-  ark_sdk_python/services/dpa/k8s/ark_dpa_k8s_service.py
+  ark_sdk_python/common/env/__init__.py
 
-  offset of local header from start of archive:   35884
-                                                  (0000000000008C2Ch) bytes
+  offset of local header from start of archive:   46835
+                                                  (000000000000B6F3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         5be6c6ad
-  compressed size:                                825 bytes
-  uncompressed size:                              2286 bytes
-  length of filename:                             54 characters
+  32-bit CRC value (hex):                         e6879f05
+  compressed size:                                257 bytes
+  uncompressed size:                              583 bytes
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1585,144 +1625,110 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #44:
----------------------------
-
-  ark_sdk_python/services/dpa/workspaces/
-
-  offset of local header from start of archive:   36821
-                                                  (0000000000008FD5h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             39 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e9 03 00 00 04 7f 00 00 00.
-
-  There is no file comment.
-
 Central directory entry #45:
 ---------------------------
 
-  ark_sdk_python/services/dpa/workspaces/__init__.py
+  ark_sdk_python/common/ark_keyring.py
 
-  offset of local header from start of archive:   36918
-                                                  (0000000000009036h) bytes
+  offset of local header from start of archive:   47187
+                                                  (000000000000B853h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             50 characters
+  32-bit CRC value (hex):                         11b07f4e
+  compressed size:                                2656 bytes
+  uncompressed size:                              11252 bytes
+  length of filename:                             36 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #46:
 ---------------------------
 
-  ark_sdk_python/services/dpa/workspaces/db/
+  ark_sdk_python/common/__init__.py
 
-  offset of local header from start of archive:   37026
-                                                  (00000000000090A2h) bytes
+  offset of local header from start of archive:   49937
+                                                  (000000000000C311h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             42 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         d13625c1
+  compressed size:                                223 bytes
+  uncompressed size:                              763 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #47:
 ---------------------------
 
-  ark_sdk_python/services/dpa/workspaces/db/__init__.py
+  ark_sdk_python/common/ark_logger.py
 
-  offset of local header from start of archive:   37126
-                                                  (0000000000009106h) bytes
+  offset of local header from start of archive:   50251
+                                                  (000000000000C44Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         4539deab
-  compressed size:                                99 bytes
-  uncompressed size:                              148 bytes
-  length of filename:                             53 characters
+  32-bit CRC value (hex):                         853fc624
+  compressed size:                                687 bytes
+  uncompressed size:                              2445 bytes
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1733,33 +1739,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #48:
 ---------------------------
 
-  ark_sdk_python/services/dpa/workspaces/db/ark_dpa_db_workspace_service.py
+  ark_sdk_python/common/ark_client.py
 
-  offset of local header from start of archive:   37336
-                                                  (00000000000091D8h) bytes
+  offset of local header from start of archive:   51031
+                                                  (000000000000C757h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         3ce5ee95
-  compressed size:                                2183 bytes
-  uncompressed size:                              11192 bytes
-  length of filename:                             73 characters
+  32-bit CRC value (hex):                         0aa3d2d9
+  compressed size:                                1416 bytes
+  uncompressed size:                              6606 bytes
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1770,32 +1776,32 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #49:
 ---------------------------
 
-  ark_sdk_python/services/sm/
+  ark_sdk_python/common/isp/
 
-  offset of local header from start of archive:   39650
-                                                  (0000000000009AE2h) bytes
+  offset of local header from start of archive:   52540
+                                                  (000000000000CD3Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             27 characters
+  length of filename:                             26 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -1806,33 +1812,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #50:
 ---------------------------
 
-  ark_sdk_python/services/sm/__init__.py
+  ark_sdk_python/common/isp/__init__.py
 
-  offset of local header from start of archive:   39735
-                                                  (0000000000009B37h) bytes
+  offset of local header from start of archive:   52624
+                                                  (000000000000CD90h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         6d6bd50b
-  compressed size:                                74 bytes
-  uncompressed size:                              95 bytes
-  length of filename:                             38 characters
+  32-bit CRC value (hex):                         19166ab9
+  compressed size:                                89 bytes
+  uncompressed size:                              116 bytes
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1843,33 +1849,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #51:
 ---------------------------
 
-  ark_sdk_python/services/sm/ark_sm_service.py
+  ark_sdk_python/common/isp/ark_isp_service_client.py
 
-  offset of local header from start of archive:   39905
-                                                  (0000000000009BE1h) bytes
+  offset of local header from start of archive:   52808
+                                                  (000000000000CE48h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         d54311c7
-  compressed size:                                2321 bytes
-  uncompressed size:                              11400 bytes
-  length of filename:                             44 characters
+  32-bit CRC value (hex):                         ab2c79dc
+  compressed size:                                1479 bytes
+  uncompressed size:                              6261 bytes
+  length of filename:                             51 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -1880,54 +1886,55 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #52:
 ---------------------------
 
-  ark_sdk_python/common/
+  ark_sdk_python/common/ark_pollers.py
 
-  offset of local header from start of archive:   42328
-                                                  (000000000000A558h) bytes
+  offset of local header from start of archive:   54396
+                                                  (000000000000D47Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             22 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         eb20d9b3
+  compressed size:                                739 bytes
+  uncompressed size:                              3987 bytes
+  length of filename:                             36 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #53:
 ---------------------------
 
   ark_sdk_python/common/ark_async_client.py
 
-  offset of local header from start of archive:   42408
-                                                  (000000000000A5A8h) bytes
+  offset of local header from start of archive:   55229
+                                                  (000000000000D7BDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1953,32 +1960,32 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #54:
 ---------------------------
 
-  ark_sdk_python/common/__init__.py
+  ark_sdk_python/common/ark_page.py
 
-  offset of local header from start of archive:   43161
-                                                  (000000000000A899h) bytes
+  offset of local header from start of archive:   55982
+                                                  (000000000000DAAEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         d13625c1
-  compressed size:                                223 bytes
-  uncompressed size:                              763 bytes
+  32-bit CRC value (hex):                         12494359
+  compressed size:                                186 bytes
+  uncompressed size:                              358 bytes
   length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -1992,16 +1999,16 @@
   There is no file comment.
 
 Central directory entry #55:
 ---------------------------
 
   ark_sdk_python/common/ark_async_request.py
 
-  offset of local header from start of archive:   43475
-                                                  (000000000000A9D3h) bytes
+  offset of local header from start of archive:   56259
+                                                  (000000000000DBC3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2027,106 +2034,104 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #56:
 ---------------------------
 
-  ark_sdk_python/common/ark_page.py
+  ark_sdk_python/services/
 
-  offset of local header from start of archive:   44109
-                                                  (000000000000AC4Dh) bytes
+  offset of local header from start of archive:   56893
+                                                  (000000000000DE3Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         12494359
-  compressed size:                                186 bytes
-  uncompressed size:                              358 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             24 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #57:
 ---------------------------
 
-  ark_sdk_python/common/ark_logger.py
+  ark_sdk_python/services/dpa/
 
-  offset of local header from start of archive:   44386
-                                                  (000000000000AD62h) bytes
+  offset of local header from start of archive:   56975
+                                                  (000000000000DE8Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         853fc624
-  compressed size:                                687 bytes
-  uncompressed size:                              2445 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #58:
 ---------------------------
 
-  ark_sdk_python/common/env/
+  ark_sdk_python/services/dpa/policies/
 
-  offset of local header from start of archive:   45166
-                                                  (000000000000B06Eh) bytes
+  offset of local header from start of archive:   57061
+                                                  (000000000000DEE5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             26 characters
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -2137,70 +2142,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #59:
 ---------------------------
 
-  ark_sdk_python/common/env/__init__.py
+  ark_sdk_python/services/dpa/policies/vm/
 
-  offset of local header from start of archive:   45250
-                                                  (000000000000B0C2h) bytes
+  offset of local header from start of archive:   57156
+                                                  (000000000000DF44h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         e6879f05
-  compressed size:                                257 bytes
-  uncompressed size:                              583 bytes
-  length of filename:                             37 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             40 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #60:
 ---------------------------
 
-  ark_sdk_python/common/env/ark_env_mapping.py
+  ark_sdk_python/services/dpa/policies/vm/ark_dpa_vm_policies_service.py
 
-  offset of local header from start of archive:   45602
-                                                  (000000000000B222h) bytes
+  offset of local header from start of archive:   57254
+                                                  (000000000000DFA6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         99fe050b
-  compressed size:                                520 bytes
-  uncompressed size:                              1132 bytes
-  length of filename:                             44 characters
+  32-bit CRC value (hex):                         2100f2ae
+  compressed size:                                2466 bytes
+  uncompressed size:                              12681 bytes
+  length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2211,33 +2215,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #61:
 ---------------------------
 
-  ark_sdk_python/common/ark_client.py
+  ark_sdk_python/services/dpa/policies/vm/__init__.py
 
-  offset of local header from start of archive:   46224
-                                                  (000000000000B490h) bytes
+  offset of local header from start of archive:   59848
+                                                  (000000000000E9C8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         0aa3d2d9
-  compressed size:                                1416 bytes
-  uncompressed size:                              6606 bytes
-  length of filename:                             35 characters
+  32-bit CRC value (hex):                         a29a2454
+  compressed size:                                99 bytes
+  uncompressed size:                              143 bytes
+  length of filename:                             51 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2248,107 +2252,105 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #62:
 ---------------------------
 
-  ark_sdk_python/common/ark_random_utils.py
+  ark_sdk_python/services/dpa/policies/__init__.py
 
-  offset of local header from start of archive:   47733
-                                                  (000000000000BA75h) bytes
+  offset of local header from start of archive:   60056
+                                                  (000000000000EA98h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         11c04bfb
-  compressed size:                                255 bytes
-  uncompressed size:                              671 bytes
-  length of filename:                             41 characters
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             48 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #63:
 ---------------------------
 
-  ark_sdk_python/common/ark_keyring.py
+  ark_sdk_python/services/dpa/policies/db/
 
-  offset of local header from start of archive:   48087
-                                                  (000000000000BBD7h) bytes
+  offset of local header from start of archive:   60162
+                                                  (000000000000EB02h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         11b07f4e
-  compressed size:                                2656 bytes
-  uncompressed size:                              11252 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             40 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #64:
 ---------------------------
 
-  ark_sdk_python/common/ark_pollers.py
+  ark_sdk_python/services/dpa/policies/db/ark_dpa_db_policies_service.py
 
-  offset of local header from start of archive:   50837
-                                                  (000000000000C695h) bytes
+  offset of local header from start of archive:   60260
+                                                  (000000000000EB64h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         eb20d9b3
-  compressed size:                                739 bytes
-  uncompressed size:                              3987 bytes
-  length of filename:                             36 characters
+  32-bit CRC value (hex):                         7f980b15
+  compressed size:                                2149 bytes
+  uncompressed size:                              10943 bytes
+  length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2359,33 +2361,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #65:
 ---------------------------
 
-  ark_sdk_python/common/ark_system_config.py
+  ark_sdk_python/services/dpa/policies/db/__init__.py
 
-  offset of local header from start of archive:   51670
-                                                  (000000000000C9D6h) bytes
+  offset of local header from start of archive:   62537
+                                                  (000000000000F449h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         70cb4a96
-  compressed size:                                600 bytes
-  uncompressed size:                              2436 bytes
-  length of filename:                             42 characters
+  32-bit CRC value (hex):                         5f59e261
+  compressed size:                                98 bytes
+  uncompressed size:                              143 bytes
+  length of filename:                             51 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2396,32 +2398,32 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #66:
 ---------------------------
 
-  ark_sdk_python/common/isp/
+  ark_sdk_python/services/dpa/certificates/
 
-  offset of local header from start of archive:   52370
-                                                  (000000000000CC92h) bytes
+  offset of local header from start of archive:   62744
+                                                  (000000000000F518h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             26 characters
+  length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -2432,33 +2434,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #67:
 ---------------------------
 
-  ark_sdk_python/common/isp/__init__.py
+  ark_sdk_python/services/dpa/certificates/__init__.py
 
-  offset of local header from start of archive:   52454
-                                                  (000000000000CCE6h) bytes
+  offset of local header from start of archive:   62843
+                                                  (000000000000F57Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         19166ab9
-  compressed size:                                89 bytes
-  uncompressed size:                              116 bytes
-  length of filename:                             37 characters
+  32-bit CRC value (hex):                         b768beed
+  compressed size:                                96 bytes
+  uncompressed size:                              149 bytes
+  length of filename:                             52 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2469,33 +2471,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #68:
 ---------------------------
 
-  ark_sdk_python/common/isp/ark_isp_service_client.py
+  ark_sdk_python/services/dpa/certificates/ark_dpa_certificates_service.py
 
-  offset of local header from start of archive:   52638
-                                                  (000000000000CD9Eh) bytes
+  offset of local header from start of archive:   63049
+                                                  (000000000000F649h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         ab2c79dc
-  compressed size:                                1479 bytes
-  uncompressed size:                              6261 bytes
-  length of filename:                             51 characters
+  32-bit CRC value (hex):                         1b597d2a
+  compressed size:                                1662 bytes
+  uncompressed size:                              7989 bytes
+  length of filename:                             72 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2506,32 +2508,32 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #69:
 ---------------------------
 
-  ark_sdk_python/models/
+  ark_sdk_python/services/dpa/workspaces/
 
-  offset of local header from start of archive:   54226
-                                                  (000000000000D3D2h) bytes
+  offset of local header from start of archive:   64841
+                                                  (000000000000FD49h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             22 characters
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -2542,106 +2544,105 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #70:
 ---------------------------
 
-  ark_sdk_python/models/auth/
+  ark_sdk_python/services/dpa/workspaces/__init__.py
 
-  offset of local header from start of archive:   54306
-                                                  (000000000000D422h) bytes
+  offset of local header from start of archive:   64938
+                                                  (000000000000FDAAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             27 characters
+  length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #71:
 ---------------------------
 
-  ark_sdk_python/models/auth/__init__.py
+  ark_sdk_python/services/dpa/workspaces/db/
 
-  offset of local header from start of archive:   54391
-                                                  (000000000000D477h) bytes
+  offset of local header from start of archive:   65046
+                                                  (000000000000FE16h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         5bf34bd3
-  compressed size:                                271 bytes
-  uncompressed size:                              1065 bytes
-  length of filename:                             38 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #72:
 ---------------------------
 
-  ark_sdk_python/models/auth/ark_secret.py
+  ark_sdk_python/services/dpa/workspaces/db/ark_dpa_db_workspace_service.py
 
-  offset of local header from start of archive:   54758
-                                                  (000000000000D5E6h) bytes
+  offset of local header from start of archive:   65146
+                                                  (000000000000FE7Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         082a3f1b
-  compressed size:                                204 bytes
-  uncompressed size:                              326 bytes
-  length of filename:                             40 characters
+  32-bit CRC value (hex):                         3ce5ee95
+  compressed size:                                2183 bytes
+  uncompressed size:                              11192 bytes
+  length of filename:                             73 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2652,33 +2653,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #73:
 ---------------------------
 
-  ark_sdk_python/models/auth/ark_auth_profile.py
+  ark_sdk_python/services/dpa/workspaces/db/__init__.py
 
-  offset of local header from start of archive:   55060
-                                                  (000000000000D714h) bytes
+  offset of local header from start of archive:   67460
+                                                  (0000000000010784h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         fdcd290a
-  compressed size:                                474 bytes
-  uncompressed size:                              1289 bytes
-  length of filename:                             46 characters
+  32-bit CRC value (hex):                         4539deab
+  compressed size:                                99 bytes
+  uncompressed size:                              148 bytes
+  length of filename:                             53 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2689,33 +2690,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #74:
 ---------------------------
 
-  ark_sdk_python/models/auth/ark_token.py
+  ark_sdk_python/services/dpa/ark_dpa_api.py
 
-  offset of local header from start of archive:   55638
-                                                  (000000000000D956h) bytes
+  offset of local header from start of archive:   67670
+                                                  (0000000000010856h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         256488d4
-  compressed size:                                574 bytes
-  uncompressed size:                              1438 bytes
-  length of filename:                             39 characters
+  32-bit CRC value (hex):                         e142e33a
+  compressed size:                                512 bytes
+  uncompressed size:                              3077 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2726,33 +2727,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #75:
 ---------------------------
 
-  ark_sdk_python/models/auth/ark_auth_method.py
+  ark_sdk_python/services/dpa/__init__.py
 
-  offset of local header from start of archive:   56309
-                                                  (000000000000DBF5h) bytes
+  offset of local header from start of archive:   68282
+                                                  (0000000000010ABAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         d2047f12
-  compressed size:                                898 bytes
-  uncompressed size:                              3150 bytes
-  length of filename:                             45 characters
+  32-bit CRC value (hex):                         371d7e9e
+  compressed size:                                78 bytes
+  uncompressed size:                              87 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2763,33 +2764,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #76:
 ---------------------------
 
-  ark_sdk_python/models/__init__.py
+  ark_sdk_python/services/dpa/k8s/
 
-  offset of local header from start of archive:   57310
-                                                  (000000000000DFDEh) bytes
+  offset of local header from start of archive:   68457
+                                                  (0000000000010B69h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             32 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 7f 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #77:
+---------------------------
+
+  ark_sdk_python/services/dpa/k8s/ark_dpa_k8s_service.py
+
+  offset of local header from start of archive:   68547
+                                                  (0000000000010BC3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         f7d23e44
-  compressed size:                                284 bytes
-  uncompressed size:                              956 bytes
-  length of filename:                             33 characters
+  32-bit CRC value (hex):                         5be6c6ad
+  compressed size:                                825 bytes
+  uncompressed size:                              2286 bytes
+  length of filename:                             54 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2797,36 +2834,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #77:
+Central directory entry #78:
 ---------------------------
 
-  ark_sdk_python/models/ark_exceptions.py
+  ark_sdk_python/services/dpa/k8s/__init__.py
 
-  offset of local header from start of archive:   57685
-                                                  (000000000000E155h) bytes
+  offset of local header from start of archive:   69484
+                                                  (0000000000010F6Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         4d4f63cf
-  compressed size:                                195 bytes
-  uncompressed size:                              562 bytes
-  length of filename:                             39 characters
+  32-bit CRC value (hex):                         b0460af6
+  compressed size:                                87 bytes
+  uncompressed size:                              113 bytes
+  length of filename:                             43 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -2834,31 +2871,31 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #78:
+Central directory entry #79:
 ---------------------------
 
-  ark_sdk_python/models/services/
+  ark_sdk_python/services/dpa/db/
 
-  offset of local header from start of archive:   57977
-                                                  (000000000000E279h) bytes
+  offset of local header from start of archive:   69672
+                                                  (0000000000011028h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -2870,35 +2907,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #79:
+Central directory entry #80:
 ---------------------------
 
-  ark_sdk_python/models/services/__init__.py
+  ark_sdk_python/services/dpa/db/__init__.py
 
-  offset of local header from start of archive:   58066
-                                                  (000000000000E2D2h) bytes
+  offset of local header from start of archive:   69761
+                                                  (0000000000011081h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         9bf17704
-  compressed size:                                84 bytes
-  uncompressed size:                              111 bytes
+  32-bit CRC value (hex):                         40fa751f
+  compressed size:                                91 bytes
+  uncompressed size:                              116 bytes
   length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -2907,71 +2944,72 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #80:
+Central directory entry #81:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/
+  ark_sdk_python/services/dpa/db/ark_dpa_db_service.py
 
-  offset of local header from start of archive:   58250
-                                                  (000000000000E38Ah) bytes
+  offset of local header from start of archive:   69952
+                                                  (0000000000011140h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         b5469f45
+  compressed size:                                2619 bytes
+  uncompressed size:                              10634 bytes
+  length of filename:                             52 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #81:
+Central directory entry #82:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/sso/
+  ark_sdk_python/services/dpa/secrets/
 
-  offset of local header from start of archive:   58343
-                                                  (000000000000E3E7h) bytes
+  offset of local header from start of archive:   72681
+                                                  (0000000000011BE9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             39 characters
+  length of filename:                             36 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -2979,109 +3017,107 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #82:
+Central directory entry #83:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_oracle_wallet.py
+  ark_sdk_python/services/dpa/secrets/__init__.py
 
-  offset of local header from start of archive:   58440
-                                                  (000000000000E448h) bytes
+  offset of local header from start of archive:   72775
+                                                  (0000000000011C47h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         4868e5cb
-  compressed size:                                345 bytes
-  uncompressed size:                              731 bytes
-  length of filename:                             83 characters
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             47 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #83:
+Central directory entry #84:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_rdp_file.py
+  ark_sdk_python/services/dpa/secrets/db/
 
-  offset of local header from start of archive:   58926
-                                                  (000000000000E62Eh) bytes
+  offset of local header from start of archive:   72880
+                                                  (0000000000011CB0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         fe31df39
-  compressed size:                                326 bytes
-  uncompressed size:                              703 bytes
-  length of filename:                             78 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #84:
+Central directory entry #85:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/sso/__init__.py
+  ark_sdk_python/services/dpa/secrets/db/__init__.py
 
-  offset of local header from start of archive:   59388
-                                                  (000000000000E7FCh) bytes
+  offset of local header from start of archive:   72977
+                                                  (0000000000011D11h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         2bfbaea4
-  compressed size:                                255 bytes
-  uncompressed size:                              928 bytes
+  32-bit CRC value (hex):                         6066091e
+  compressed size:                                97 bytes
+  uncompressed size:                              139 bytes
   length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -3090,36 +3126,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #85:
+Central directory entry #86:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_acquire_token_response.py
+  ark_sdk_python/services/dpa/secrets/db/ark_dpa_db_secrets_service.py
 
-  offset of local header from start of archive:   59751
-                                                  (000000000000E967h) bytes
+  offset of local header from start of archive:   73182
+                                                  (0000000000011DDEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         833f0d09
-  compressed size:                                167 bytes
-  uncompressed size:                              277 bytes
-  length of filename:                             76 characters
+  32-bit CRC value (hex):                         50bcf558
+  compressed size:                                2590 bytes
+  uncompressed size:                              15607 bytes
+  length of filename:                             68 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3127,73 +3163,72 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #86:
+Central directory entry #87:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_client_certificate.py
+  ark_sdk_python/services/dpa/sso/
 
-  offset of local header from start of archive:   60052
-                                                  (000000000000EA94h) bytes
+  offset of local header from start of archive:   75898
+                                                  (000000000001287Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c03bb310
-  compressed size:                                454 bytes
-  uncompressed size:                              942 bytes
-  length of filename:                             88 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #87:
+Central directory entry #88:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_password.py
+  ark_sdk_python/services/dpa/sso/__init__.py
 
-  offset of local header from start of archive:   60652
-                                                  (000000000000ECECh) bytes
+  offset of local header from start of archive:   75988
+                                                  (00000000000128D4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         18247993
-  compressed size:                                161 bytes
-  uncompressed size:                              215 bytes
-  length of filename:                             78 characters
+  32-bit CRC value (hex):                         c7961b71
+  compressed size:                                92 bytes
+  uncompressed size:                              120 bytes
+  length of filename:                             43 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3201,108 +3236,72 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #88:
+Central directory entry #89:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/__init__.py
+  ark_sdk_python/services/dpa/sso/ark_dpa_sso_service.py
 
-  offset of local header from start of archive:   60949
-                                                  (000000000000EE15h) bytes
+  offset of local header from start of archive:   76181
+                                                  (0000000000012995h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             46 characters
+  32-bit CRC value (hex):                         b72eea43
+  compressed size:                                2696 bytes
+  uncompressed size:                              15817 bytes
+  length of filename:                             54 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #89:
+Central directory entry #90:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/db/
+  ark_sdk_python/services/__init__.py
 
-  offset of local header from start of archive:   61053
-                                                  (000000000000EE7Dh) bytes
+  offset of local header from start of archive:   78989
+                                                  (000000000001348Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             38 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e9 03 00 00 04 7f 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #90:
----------------------------
-
-  ark_sdk_python/models/services/dpa/db/__init__.py
-
-  offset of local header from start of archive:   61149
-                                                  (000000000000EEDDh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         a7a770aa
-  compressed size:                                219 bytes
-  uncompressed size:                              890 bytes
-  length of filename:                             49 characters
+  32-bit CRC value (hex):                         32d70693
+  compressed size:                                1 bytes
+  uncompressed size:                              1 bytes
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3313,70 +3312,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #91:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/db/ark_dpa_db_generated_assets.py
+  ark_sdk_python/services/sm/
 
-  offset of local header from start of archive:   61475
-                                                  (000000000000F023h) bytes
+  offset of local header from start of archive:   79083
+                                                  (00000000000134EBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         3146e552
-  compressed size:                                159 bytes
-  uncompressed size:                              227 bytes
-  length of filename:                             68 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #92:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_generate_assets.py
+  ark_sdk_python/services/sm/__init__.py
 
-  offset of local header from start of archive:   61760
-                                                  (000000000000F140h) bytes
+  offset of local header from start of archive:   79168
+                                                  (0000000000013540h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         47a5417c
-  compressed size:                                338 bytes
-  uncompressed size:                              764 bytes
-  length of filename:                             72 characters
+  32-bit CRC value (hex):                         6d6bd50b
+  compressed size:                                74 bytes
+  uncompressed size:                              95 bytes
+  length of filename:                             38 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3387,33 +3385,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #93:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/db/ark_dpa_db_psql_execution.py
+  ark_sdk_python/services/sm/ark_sm_service.py
 
-  offset of local header from start of archive:   62228
-                                                  (000000000000F314h) bytes
+  offset of local header from start of archive:   79338
+                                                  (00000000000135EAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         4b5337c4
-  compressed size:                                174 bytes
-  uncompressed size:                              266 bytes
-  length of filename:                             66 characters
+  32-bit CRC value (hex):                         d54311c7
+  compressed size:                                2321 bytes
+  uncompressed size:                              11400 bytes
+  length of filename:                             44 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3424,33 +3422,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #94:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/db/ark_dpa_db_mysql_execution.py
+  ark_sdk_python/services/ark_service.py
 
-  offset of local header from start of archive:   62526
-                                                  (000000000000F43Eh) bytes
+  offset of local header from start of archive:   81761
+                                                  (0000000000013F61h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         910ccef9
-  compressed size:                                177 bytes
-  uncompressed size:                              269 bytes
-  length of filename:                             67 characters
+  32-bit CRC value (hex):                         6c78ace9
+  compressed size:                                683 bytes
+  uncompressed size:                              2314 bytes
+  length of filename:                             38 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3461,106 +3459,105 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #95:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/db/ark_dpa_db_oracle_generate_assets.py
+  ark_sdk_python/ark.py
 
-  offset of local header from start of archive:   62828
-                                                  (000000000000F56Ch) bytes
+  offset of local header from start of archive:   82540
+                                                  (000000000001426Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         d6bd2b47
-  compressed size:                                213 bytes
-  uncompressed size:                              352 bytes
-  length of filename:                             74 characters
+  32-bit CRC value (hex):                         c6ad48cf
+  compressed size:                                542 bytes
+  uncompressed size:                              1280 bytes
+  length of filename:                             21 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #96:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_execution.py
+  ark_sdk_python/models/
 
-  offset of local header from start of archive:   63173
-                                                  (000000000000F6C5h) bytes
+  offset of local header from start of archive:   83161
+                                                  (00000000000144D9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7e2779cb
-  compressed size:                                183 bytes
-  uncompressed size:                              306 bytes
-  length of filename:                             66 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #97:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/
+  ark_sdk_python/models/auth/
 
-  offset of local header from start of archive:   63480
-                                                  (000000000000F7F8h) bytes
+  offset of local header from start of archive:   83241
+                                                  (0000000000014529h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             44 characters
+  length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -3571,69 +3568,70 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #98:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/
+  ark_sdk_python/models/auth/ark_auth_profile.py
 
-  offset of local header from start of archive:   63582
-                                                  (000000000000F85Eh) bytes
+  offset of local header from start of archive:   83326
+                                                  (000000000001457Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             47 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         fdcd290a
+  compressed size:                                474 bytes
+  uncompressed size:                              1289 bytes
+  length of filename:                             46 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #99:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_providers.py
+  ark_sdk_python/models/auth/__init__.py
 
-  offset of local header from start of archive:   63687
-                                                  (000000000000F8C7h) bytes
+  offset of local header from start of archive:   83904
+                                                  (00000000000147C0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         1c3a4ea5
-  compressed size:                                800 bytes
-  uncompressed size:                              3056 bytes
-  length of filename:                             70 characters
+  32-bit CRC value (hex):                         5bf34bd3
+  compressed size:                                271 bytes
+  uncompressed size:                              1065 bytes
+  length of filename:                             38 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3644,33 +3642,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #100:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_add_policy.py
+  ark_sdk_python/models/auth/ark_token.py
 
-  offset of local header from start of archive:   64615
-                                                  (000000000000FC67h) bytes
+  offset of local header from start of archive:   84271
+                                                  (000000000001492Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7b7128ee
-  compressed size:                                617 bytes
-  uncompressed size:                              1650 bytes
-  length of filename:                             71 characters
+  32-bit CRC value (hex):                         256488d4
+  compressed size:                                574 bytes
+  uncompressed size:                              1438 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3681,33 +3679,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #101:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/__init__.py
+  ark_sdk_python/models/auth/ark_auth_method.py
 
-  offset of local header from start of archive:   65361
-                                                  (000000000000FF51h) bytes
+  offset of local header from start of archive:   84942
+                                                  (0000000000014BCEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         17753273
-  compressed size:                                513 bytes
-  uncompressed size:                              2669 bytes
-  length of filename:                             58 characters
+  32-bit CRC value (hex):                         d2047f12
+  compressed size:                                898 bytes
+  uncompressed size:                              3150 bytes
+  length of filename:                             45 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3718,33 +3716,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #102:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy_list_item.py
+  ark_sdk_python/models/auth/ark_secret.py
 
-  offset of local header from start of archive:   65990
-                                                  (00000000000101C6h) bytes
+  offset of local header from start of archive:   85943
+                                                  (0000000000014FB7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         79f5ddda
-  compressed size:                                395 bytes
-  uncompressed size:                              927 bytes
-  length of filename:                             77 characters
+  32-bit CRC value (hex):                         082a3f1b
+  compressed size:                                204 bytes
+  uncompressed size:                              326 bytes
+  length of filename:                             40 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3755,181 +3753,177 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #103:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_authorization_rule.py
+  ark_sdk_python/models/cli_services/
 
-  offset of local header from start of archive:   66520
-                                                  (00000000000103D8h) bytes
+  offset of local header from start of archive:   86245
+                                                  (00000000000150E5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         8dcbb607
-  compressed size:                                537 bytes
-  uncompressed size:                              1662 bytes
-  length of filename:                             79 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #104:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_protocol_type_serializer.py
+  ark_sdk_python/models/cli_services/dpa/
 
-  offset of local header from start of archive:   67194
-                                                  (000000000001067Ah) bytes
+  offset of local header from start of archive:   86338
+                                                  (0000000000015142h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         51ced9d0
-  compressed size:                                240 bytes
-  uncompressed size:                              679 bytes
-  length of filename:                             94 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #105:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_stats.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/
 
-  offset of local header from start of archive:   67586
-                                                  (0000000000010802h) bytes
+  offset of local header from start of archive:   86435
+                                                  (00000000000151A3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         b4482d6a
-  compressed size:                                384 bytes
-  uncompressed size:                              896 bytes
-  length of filename:                             75 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             55 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #106:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_update_policy.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/vm/
 
-  offset of local header from start of archive:   68103
-                                                  (0000000000010A07h) bytes
+  offset of local header from start of archive:   86548
+                                                  (0000000000015214h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         a9e8f593
-  compressed size:                                524 bytes
-  uncompressed size:                              1427 bytes
-  length of filename:                             74 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             58 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #107:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_filter.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/vm/__init__.py
 
-  offset of local header from start of archive:   68759
-                                                  (0000000000010C97h) bytes
+  offset of local header from start of archive:   86664
+                                                  (0000000000015288h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         557b1ab3
-  compressed size:                                401 bytes
-  uncompressed size:                              935 bytes
-  length of filename:                             76 characters
+  32-bit CRC value (hex):                         2b290ee1
+  compressed size:                                118 bytes
+  uncompressed size:                              158 bytes
+  length of filename:                             69 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3940,33 +3934,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #108:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_workspace_type_serializer.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/vm/ark_dpa_vm_generate_policy.py
 
-  offset of local header from start of archive:   69294
-                                                  (0000000000010EAEh) bytes
+  offset of local header from start of archive:   86909
+                                                  (000000000001537Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7efc9af0
-  compressed size:                                235 bytes
+  32-bit CRC value (hex):                         7ac6e730
+  compressed size:                                266 bytes
   uncompressed size:                              522 bytes
-  length of filename:                             95 characters
+  length of filename:                             87 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -3977,179 +3971,179 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #109:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/__init__.py
 
-  offset of local header from start of archive:   69682
-                                                  (0000000000011032h) bytes
+  offset of local header from start of archive:   87320
+                                                  (0000000000015518h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c6ac959d
-  compressed size:                                521 bytes
-  uncompressed size:                              1414 bytes
-  length of filename:                             67 characters
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             66 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #110:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_connection_data.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/
 
-  offset of local header from start of archive:   70328
-                                                  (00000000000112B8h) bytes
+  offset of local header from start of archive:   87444
+                                                  (0000000000015594h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         e781c633
-  compressed size:                                350 bytes
-  uncompressed size:                              926 bytes
-  length of filename:                             76 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             62 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #111:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/__init__.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_base_generate_policy.py
 
-  offset of local header from start of archive:   70812
-                                                  (000000000001149Ch) bytes
+  offset of local header from start of archive:   87564
+                                                  (000000000001560Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             55 characters
+  32-bit CRC value (hex):                         1930969b
+  compressed size:                                219 bytes
+  uncompressed size:                              342 bytes
+  length of filename:                             93 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #112:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_edit_policies.py
 
-  offset of local header from start of archive:   70925
-                                                  (000000000001150Dh) bytes
+  offset of local header from start of archive:   87934
+                                                  (000000000001577Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             51 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         5018b9a2
+  compressed size:                                185 bytes
+  uncompressed size:                              274 bytes
+  length of filename:                             86 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #113:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policies_stats.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/__init__.py
 
-  offset of local header from start of archive:   71034
-                                                  (000000000001157Ah) bytes
+  offset of local header from start of archive:   88263
+                                                  (00000000000158C7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         3876d342
-  compressed size:                                220 bytes
-  uncompressed size:                              425 bytes
-  length of filename:                             81 characters
+  32-bit CRC value (hex):                         54b23c2a
+  compressed size:                                283 bytes
+  uncompressed size:                              1628 bytes
+  length of filename:                             73 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4160,33 +4154,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #114:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/__init__.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_policies_status.py
 
-  offset of local header from start of archive:   71393
-                                                  (00000000000116E1h) bytes
+  offset of local header from start of archive:   88677
+                                                  (0000000000015A65h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         736492e1
-  compressed size:                                367 bytes
-  uncompressed size:                              1942 bytes
-  length of filename:                             62 characters
+  32-bit CRC value (hex):                         c2f1dd97
+  compressed size:                                175 bytes
+  uncompressed size:                              398 bytes
+  length of filename:                             88 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4197,33 +4191,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #115:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_user_data.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_load_policies.py
 
-  offset of local header from start of archive:   71880
-                                                  (00000000000118C8h) bytes
+  offset of local header from start of archive:   88998
+                                                  (0000000000015BA6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c749a8eb
-  compressed size:                                273 bytes
-  uncompressed size:                              769 bytes
-  length of filename:                             71 characters
+  32-bit CRC value (hex):                         840981f9
+  compressed size:                                151 bytes
+  uncompressed size:                              204 bytes
+  length of filename:                             86 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4234,33 +4228,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #116:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policy.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_get_policies_status.py
 
-  offset of local header from start of archive:   72282
-                                                  (0000000000011A5Ah) bytes
+  offset of local header from start of archive:   89293
+                                                  (0000000000015CCDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         04cb14f9
-  compressed size:                                252 bytes
-  uncompressed size:                              691 bytes
-  length of filename:                             73 characters
+  32-bit CRC value (hex):                         e5bff3c0
+  compressed size:                                183 bytes
+  uncompressed size:                              278 bytes
+  length of filename:                             92 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4271,33 +4265,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #117:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policy_list_item.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_commit_policies.py
 
-  offset of local header from start of archive:   72665
-                                                  (0000000000011BD9h) bytes
+  offset of local header from start of archive:   89626
+                                                  (0000000000015E1Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         b81435bb
-  compressed size:                                288 bytes
-  uncompressed size:                              723 bytes
-  length of filename:                             83 characters
+  32-bit CRC value (hex):                         ce252390
+  compressed size:                                249 bytes
+  uncompressed size:                              408 bytes
+  length of filename:                             88 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4308,33 +4302,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #118:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_connection_information.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_view_policies.py
 
-  offset of local header from start of archive:   73094
-                                                  (0000000000011D86h) bytes
+  offset of local header from start of archive:   90021
+                                                  (0000000000015FA5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         36818b67
-  compressed size:                                557 bytes
-  uncompressed size:                              1272 bytes
-  length of filename:                             89 characters
+  32-bit CRC value (hex):                         0382245b
+  compressed size:                                239 bytes
+  uncompressed size:                              371 bytes
+  length of filename:                             86 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4345,33 +4339,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #119:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_get_policy.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_policies_diff.py
 
-  offset of local header from start of archive:   73798
-                                                  (0000000000012046h) bytes
+  offset of local header from start of archive:   90404
+                                                  (0000000000016124h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         d0fc88bb
-  compressed size:                                290 bytes
-  uncompressed size:                              580 bytes
-  length of filename:                             72 characters
+  32-bit CRC value (hex):                         1be3547a
+  compressed size:                                218 bytes
+  uncompressed size:                              349 bytes
+  length of filename:                             86 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4382,33 +4376,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #120:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_delete_policy.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_loaded_policies.py
 
-  offset of local header from start of archive:   74218
-                                                  (00000000000121EAh) bytes
+  offset of local header from start of archive:   90766
+                                                  (000000000001628Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         76dd9763
-  compressed size:                                293 bytes
-  uncompressed size:                              589 bytes
-  length of filename:                             75 characters
+  32-bit CRC value (hex):                         5cea6949
+  compressed size:                                229 bytes
+  uncompressed size:                              559 bytes
+  length of filename:                             88 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4419,33 +4413,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #121:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_update_policy.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_reset_policies.py
 
-  offset of local header from start of archive:   74644
-                                                  (0000000000012394h) bytes
+  offset of local header from start of archive:   91141
+                                                  (0000000000016405h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         8ddfdc21
-  compressed size:                                421 bytes
-  uncompressed size:                              1137 bytes
-  length of filename:                             80 characters
+  32-bit CRC value (hex):                         bbacfaaf
+  compressed size:                                232 bytes
+  uncompressed size:                              376 bytes
+  length of filename:                             87 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4456,33 +4450,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #122:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_update_policy_status.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_remove_policies.py
 
-  offset of local header from start of archive:   75203
-                                                  (00000000000125C3h) bytes
+  offset of local header from start of archive:   91518
+                                                  (000000000001657Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         57334be9
-  compressed size:                                360 bytes
-  uncompressed size:                              798 bytes
-  length of filename:                             82 characters
+  32-bit CRC value (hex):                         7566ada9
+  compressed size:                                187 bytes
+  uncompressed size:                              278 bytes
+  length of filename:                             88 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4493,70 +4487,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #123:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_rule_status.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/db/
 
-  offset of local header from start of archive:   75703
-                                                  (00000000000127B7h) bytes
+  offset of local header from start of archive:   91851
+                                                  (00000000000166CBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         4a6a3dd3
-  compressed size:                                103 bytes
-  uncompressed size:                              153 bytes
-  length of filename:                             73 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             58 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #124:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policies_filter.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/db/ark_dpa_db_generate_policy.py
 
-  offset of local header from start of archive:   75937
-                                                  (00000000000128A1h) bytes
+  offset of local header from start of archive:   91967
+                                                  (000000000001673Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7d5dc2d4
-  compressed size:                                229 bytes
-  uncompressed size:                              437 bytes
-  length of filename:                             82 characters
+  32-bit CRC value (hex):                         2b26d447
+  compressed size:                                261 bytes
+  uncompressed size:                              449 bytes
+  length of filename:                             87 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4567,33 +4560,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #125:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_add_policy.py
+  ark_sdk_python/models/cli_services/dpa/policies_editor/db/__init__.py
 
-  offset of local header from start of archive:   76306
-                                                  (0000000000012A12h) bytes
+  offset of local header from start of archive:   92373
+                                                  (00000000000168D5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         8d7ce2ec
-  compressed size:                                328 bytes
-  uncompressed size:                              807 bytes
-  length of filename:                             77 characters
+  32-bit CRC value (hex):                         df9469a1
+  compressed size:                                116 bytes
+  uncompressed size:                              158 bytes
+  length of filename:                             69 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4604,143 +4597,141 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #126:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_authorization_rule.py
+  ark_sdk_python/models/cli_services/dpa/__init__.py
 
-  offset of local header from start of archive:   76769
-                                                  (0000000000012BE1h) bytes
+  offset of local header from start of archive:   92616
+                                                  (00000000000169C8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         9f887eef
-  compressed size:                                211 bytes
-  uncompressed size:                              386 bytes
-  length of filename:                             85 characters
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #127:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/
+  ark_sdk_python/models/cli_services/__init__.py
 
-  offset of local header from start of archive:   77123
-                                                  (0000000000012D43h) bytes
+  offset of local header from start of archive:   92724
+                                                  (0000000000016A34h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             47 characters
+  length of filename:                             46 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #128:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_stats.py
+  ark_sdk_python/models/actions/
 
-  offset of local header from start of archive:   77228
-                                                  (0000000000012DACh) bytes
+  offset of local header from start of archive:   92828
+                                                  (0000000000016A9Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         1afef5d8
-  compressed size:                                391 bytes
-  uncompressed size:                              933 bytes
-  length of filename:                             75 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #129:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy_list_item.py
+  ark_sdk_python/models/actions/ark_service_action_definition.py
 
-  offset of local header from start of archive:   77752
-                                                  (0000000000012FB8h) bytes
+  offset of local header from start of archive:   92916
+                                                  (0000000000016AF4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         ff1ee095
-  compressed size:                                446 bytes
-  uncompressed size:                              1071 bytes
-  length of filename:                             77 characters
+  32-bit CRC value (hex):                         52c2076c
+  compressed size:                                336 bytes
+  uncompressed size:                              785 bytes
+  length of filename:                             62 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4751,33 +4742,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #130:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/__init__.py
+  ark_sdk_python/models/actions/__init__.py
 
-  offset of local header from start of archive:   78333
-                                                  (00000000000131FDh) bytes
+  offset of local header from start of archive:   93372
+                                                  (0000000000016CBCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         647e6a01
-  compressed size:                                463 bytes
-  uncompressed size:                              2183 bytes
-  length of filename:                             58 characters
+  32-bit CRC value (hex):                         46ad05f9
+  compressed size:                                228 bytes
+  uncompressed size:                              743 bytes
+  length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4788,70 +4779,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #131:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_add_policy.py
+  ark_sdk_python/models/actions/services/
 
-  offset of local header from start of archive:   78912
-                                                  (0000000000013440h) bytes
+  offset of local header from start of archive:   93699
+                                                  (0000000000016E03h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         f55c07bd
-  compressed size:                                371 bytes
-  uncompressed size:                              906 bytes
-  length of filename:                             71 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #132:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_authorization_rule.py
+  ark_sdk_python/models/actions/services/ark_sm_exec_action_consts.py
 
-  offset of local header from start of archive:   79412
-                                                  (0000000000013634h) bytes
+  offset of local header from start of archive:   93796
+                                                  (0000000000016E64h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         d7b8567b
-  compressed size:                                262 bytes
-  uncompressed size:                              739 bytes
-  length of filename:                             79 characters
+  32-bit CRC value (hex):                         28612258
+  compressed size:                                379 bytes
+  uncompressed size:                              1161 bytes
+  length of filename:                             67 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4862,33 +4852,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #133:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy.py
+  ark_sdk_python/models/actions/services/__init__.py
 
-  offset of local header from start of archive:   79811
-                                                  (00000000000137C3h) bytes
+  offset of local header from start of archive:   94300
+                                                  (000000000001705Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         54792f18
-  compressed size:                                292 bytes
-  uncompressed size:                              718 bytes
-  length of filename:                             67 characters
+  32-bit CRC value (hex):                         fc8496dd
+  compressed size:                                182 bytes
+  uncompressed size:                              370 bytes
+  length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4899,33 +4889,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #134:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_workspace_type_serializer.py
+  ark_sdk_python/models/actions/services/ark_dpa_exec_action_consts.py
 
-  offset of local header from start of archive:   80228
-                                                  (0000000000013964h) bytes
+  offset of local header from start of archive:   94590
+                                                  (000000000001717Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         96fdb092
-  compressed size:                                264 bytes
-  uncompressed size:                              670 bytes
-  length of filename:                             95 characters
+  32-bit CRC value (hex):                         52f67a81
+  compressed size:                                1359 bytes
+  uncompressed size:                              7892 bytes
+  length of filename:                             68 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4936,33 +4926,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #135:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_providers.py
+  ark_sdk_python/models/actions/ark_configure_action_consts.py
 
-  offset of local header from start of archive:   80645
-                                                  (0000000000013B05h) bytes
+  offset of local header from start of archive:   96075
+                                                  (000000000001774Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         58d7e2fa
-  compressed size:                                558 bytes
-  uncompressed size:                              1696 bytes
-  length of filename:                             70 characters
+  32-bit CRC value (hex):                         6cbaf971
+  compressed size:                                414 bytes
+  uncompressed size:                              1143 bytes
+  length of filename:                             60 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -4973,33 +4963,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #136:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_connection_data.py
+  ark_sdk_python/models/__init__.py
 
-  offset of local header from start of archive:   81331
-                                                  (0000000000013DB3h) bytes
+  offset of local header from start of archive:   96607
+                                                  (000000000001795Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         24e3cca4
-  compressed size:                                543 bytes
-  uncompressed size:                              2032 bytes
-  length of filename:                             76 characters
+  32-bit CRC value (hex):                         f7d23e44
+  compressed size:                                284 bytes
+  uncompressed size:                              956 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5010,70 +5000,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #137:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_filter.py
+  ark_sdk_python/models/common/
 
-  offset of local header from start of archive:   82008
-                                                  (0000000000014058h) bytes
+  offset of local header from start of archive:   96982
+                                                  (0000000000017AD6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         f248fac2
-  compressed size:                                405 bytes
-  uncompressed size:                              979 bytes
-  length of filename:                             76 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #138:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_update_policy.py
+  ark_sdk_python/models/common/ark_application_code.py
 
-  offset of local header from start of archive:   82547
-                                                  (0000000000014273h) bytes
+  offset of local header from start of archive:   97069
+                                                  (0000000000017B2Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         883fc8b2
-  compressed size:                                359 bytes
-  uncompressed size:                              906 bytes
-  length of filename:                             74 characters
+  32-bit CRC value (hex):                         45bccf01
+  compressed size:                                166 bytes
+  uncompressed size:                              319 bytes
+  length of filename:                             52 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5084,32 +5073,32 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #139:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/
+  ark_sdk_python/models/common/connections/
 
-  offset of local header from start of archive:   83038
-                                                  (000000000001445Eh) bytes
+  offset of local header from start of archive:   97345
+                                                  (0000000000017C41h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             43 characters
+  length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -5120,68 +5109,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #140:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/__init__.py
+  ark_sdk_python/models/common/connections/ark_connection_command.py
 
-  offset of local header from start of archive:   83139
-                                                  (00000000000144C3h) bytes
+  offset of local header from start of archive:   97444
+                                                  (0000000000017CA4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             54 characters
+  32-bit CRC value (hex):                         786ba61f
+  compressed size:                                205 bytes
+  uncompressed size:                              352 bytes
+  length of filename:                             66 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #141:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/
+  ark_sdk_python/models/common/connections/connection_data/
 
-  offset of local header from start of archive:   83251
-                                                  (0000000000014533h) bytes
+  offset of local header from start of archive:   97773
+                                                  (0000000000017DEDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             46 characters
+  length of filename:                             57 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -5192,33 +5182,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #142:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secrets_stats.py
+  ark_sdk_python/models/common/connections/connection_data/ark_winrm_connection_data.py
 
-  offset of local header from start of archive:   83355
-                                                  (000000000001459Bh) bytes
+  offset of local header from start of archive:   97888
+                                                  (0000000000017E60h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         fc4f0e5f
-  compressed size:                                259 bytes
-  uncompressed size:                              799 bytes
-  length of filename:                             73 characters
+  32-bit CRC value (hex):                         5e80c9fa
+  compressed size:                                160 bytes
+  uncompressed size:                              240 bytes
+  length of filename:                             85 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5229,33 +5219,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #143:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/__init__.py
+  ark_sdk_python/models/common/connections/connection_data/__init__.py
 
-  offset of local header from start of archive:   83745
-                                                  (0000000000014721h) bytes
+  offset of local header from start of archive:   98191
+                                                  (0000000000017F8Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         27fcacbc
-  compressed size:                                320 bytes
-  uncompressed size:                              1709 bytes
-  length of filename:                             57 characters
+  32-bit CRC value (hex):                         b4dd4d81
+  compressed size:                                124 bytes
+  uncompressed size:                              294 bytes
+  length of filename:                             68 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5266,33 +5256,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #144:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_update_secret.py
+  ark_sdk_python/models/common/connections/connection_data/ark_ssh_connection_data.py
 
-  offset of local header from start of archive:   84180
-                                                  (00000000000148D4h) bytes
+  offset of local header from start of archive:   98441
+                                                  (0000000000018089h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         29b72961
-  compressed size:                                581 bytes
-  uncompressed size:                              1629 bytes
-  length of filename:                             73 characters
+  32-bit CRC value (hex):                         b674b469
+  compressed size:                                81 bytes
+  uncompressed size:                              92 bytes
+  length of filename:                             83 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5303,33 +5293,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #145:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secret_type.py
+  ark_sdk_python/models/common/connections/__init__.py
 
-  offset of local header from start of archive:   84892
-                                                  (0000000000014B9Ch) bytes
+  offset of local header from start of archive:   98663
+                                                  (0000000000018167h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         af15e4ea
-  compressed size:                                135 bytes
-  uncompressed size:                              168 bytes
-  length of filename:                             71 characters
+  32-bit CRC value (hex):                         80c93fa6
+  compressed size:                                158 bytes
+  uncompressed size:                              545 bytes
+  length of filename:                             52 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5340,68 +5330,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #146:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/secret_links/
+  ark_sdk_python/models/common/connections/ark_connection_result.py
 
-  offset of local header from start of archive:   85156
-                                                  (0000000000014CA4h) bytes
+  offset of local header from start of archive:   98931
+                                                  (0000000000018273h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             59 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         1bc99a8d
+  compressed size:                                172 bytes
+  uncompressed size:                              344 bytes
+  length of filename:                             65 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #147:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/secret_links/__init__.py
+  ark_sdk_python/models/common/connections/ark_connection_credentials.py
 
-  offset of local header from start of archive:   85273
-                                                  (0000000000014D19h) bytes
+  offset of local header from start of archive:   99226
+                                                  (000000000001839Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         9efed661
-  compressed size:                                138 bytes
-  uncompressed size:                              220 bytes
+  32-bit CRC value (hex):                         905c9662
+  compressed size:                                233 bytes
+  uncompressed size:                              536 bytes
   length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -5413,33 +5404,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #148:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/secret_links/ark_dpa_db_pam_account_secret_link.py
+  ark_sdk_python/models/common/connections/ark_connection_details.py
 
-  offset of local header from start of archive:   85539
-                                                  (0000000000014E23h) bytes
+  offset of local header from start of archive:   99587
+                                                  (0000000000018503h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         25434eb9
-  compressed size:                                171 bytes
-  uncompressed size:                              293 bytes
-  length of filename:                             96 characters
+  32-bit CRC value (hex):                         f4e88e30
+  compressed size:                                541 bytes
+  uncompressed size:                              1508 bytes
+  length of filename:                             66 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5450,33 +5441,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #149:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_disable_secret.py
+  ark_sdk_python/models/common/ark_validations.py
 
-  offset of local header from start of archive:   85864
-                                                  (0000000000014F68h) bytes
+  offset of local header from start of archive:   100252
+                                                  (000000000001879Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         6e69a5c9
-  compressed size:                                305 bytes
-  uncompressed size:                              618 bytes
-  length of filename:                             74 characters
+  32-bit CRC value (hex):                         e65b560d
+  compressed size:                                138 bytes
+  uncompressed size:                              184 bytes
+  length of filename:                             47 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5487,33 +5478,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #150:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secret_metadata.py
+  ark_sdk_python/models/common/ark_os_type.py
 
-  offset of local header from start of archive:   86301
-                                                  (000000000001511Dh) bytes
+  offset of local header from start of archive:   100495
+                                                  (000000000001888Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         5bc8dca5
-  compressed size:                                586 bytes
-  uncompressed size:                              2091 bytes
-  length of filename:                             75 characters
+  32-bit CRC value (hex):                         4be765ae
+  compressed size:                                202 bytes
+  uncompressed size:                              452 bytes
+  length of filename:                             43 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5524,33 +5515,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #151:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_delete_secret.py
+  ark_sdk_python/models/common/ark_region.py
 
-  offset of local header from start of archive:   87020
-                                                  (00000000000153ECh) bytes
+  offset of local header from start of archive:   100798
+                                                  (00000000000189BEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         cd19d8e4
-  compressed size:                                307 bytes
-  uncompressed size:                              615 bytes
-  length of filename:                             73 characters
+  32-bit CRC value (hex):                         bb2af7a6
+  compressed size:                                1077 bytes
+  uncompressed size:                              3711 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5561,33 +5552,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #152:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_store_descriptor.py
+  ark_sdk_python/models/common/ark_async_status.py
 
-  offset of local header from start of archive:   87458
-                                                  (00000000000155A2h) bytes
+  offset of local header from start of archive:   101975
+                                                  (0000000000018E57h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         591c5d18
-  compressed size:                                200 bytes
-  uncompressed size:                              403 bytes
-  length of filename:                             76 characters
+  32-bit CRC value (hex):                         5e6b5fab
+  compressed size:                                129 bytes
+  uncompressed size:                              178 bytes
+  length of filename:                             48 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5598,33 +5589,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #153:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_store_type.py
+  ark_sdk_python/models/common/ark_access_method.py
 
-  offset of local header from start of archive:   87792
-                                                  (00000000000156F0h) bytes
+  offset of local header from start of archive:   102210
+                                                  (0000000000018F42h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         b2585378
-  compressed size:                                267 bytes
-  uncompressed size:                              476 bytes
-  length of filename:                             70 characters
+  32-bit CRC value (hex):                         7a1acb83
+  compressed size:                                87 bytes
+  uncompressed size:                              98 bytes
+  length of filename:                             49 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5635,33 +5626,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #154:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secrets_filter.py
+  ark_sdk_python/models/common/__init__.py
 
-  offset of local header from start of archive:   88187
-                                                  (000000000001587Bh) bytes
+  offset of local header from start of archive:   102404
+                                                  (0000000000019004h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         03ba2ead
-  compressed size:                                287 bytes
-  uncompressed size:                              850 bytes
-  length of filename:                             74 characters
+  32-bit CRC value (hex):                         d361b870
+  compressed size:                                459 bytes
+  uncompressed size:                              1877 bytes
+  length of filename:                             40 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5672,33 +5663,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #155:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_enable_secret.py
+  ark_sdk_python/models/common/ark_connection_method.py
 
-  offset of local header from start of archive:   88606
-                                                  (0000000000015A1Eh) bytes
+  offset of local header from start of archive:   102961
+                                                  (0000000000019231h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         25cb0188
-  compressed size:                                306 bytes
-  uncompressed size:                              615 bytes
-  length of filename:                             73 characters
+  32-bit CRC value (hex):                         28d71508
+  compressed size:                                118 bytes
+  uncompressed size:                              143 bytes
+  length of filename:                             53 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5709,33 +5700,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #156:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_get_secret.py
+  ark_sdk_python/models/common/ark_status_stats.py
 
-  offset of local header from start of archive:   89043
-                                                  (0000000000015BD3h) bytes
+  offset of local header from start of archive:   103190
+                                                  (0000000000019316h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         938f2846
-  compressed size:                                304 bytes
-  uncompressed size:                              606 bytes
-  length of filename:                             70 characters
+  32-bit CRC value (hex):                         6c5bf307
+  compressed size:                                170 bytes
+  uncompressed size:                              271 bytes
+  length of filename:                             48 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5746,33 +5737,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #157:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_add_secret.py
+  ark_sdk_python/models/common/ark_network_entity_type.py
 
-  offset of local header from start of archive:   89475
-                                                  (0000000000015D83h) bytes
+  offset of local header from start of archive:   103466
+                                                  (000000000001942Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         20ad8b65
-  compressed size:                                528 bytes
-  uncompressed size:                              1572 bytes
-  length of filename:                             70 characters
+  32-bit CRC value (hex):                         89839e5a
+  compressed size:                                192 bytes
+  uncompressed size:                              391 bytes
+  length of filename:                             55 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5783,32 +5774,32 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #158:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/secrets_data/
+  ark_sdk_python/models/common/isp/
 
-  offset of local header from start of archive:   90131
-                                                  (0000000000016013h) bytes
+  offset of local header from start of archive:   103771
+                                                  (000000000001955Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             59 characters
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -5819,33 +5810,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #159:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/secrets_data/__init__.py
+  ark_sdk_python/models/common/isp/__init__.py
 
-  offset of local header from start of archive:   90248
-                                                  (0000000000016088h) bytes
+  offset of local header from start of archive:   103862
+                                                  (00000000000195B6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         407a0f5d
-  compressed size:                                168 bytes
-  uncompressed size:                              360 bytes
-  length of filename:                             70 characters
+  32-bit CRC value (hex):                         199b0474
+  compressed size:                                106 bytes
+  uncompressed size:                              141 bytes
+  length of filename:                             44 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5856,33 +5847,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #160:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/secrets/db/secrets_data/ark_dpa_db_user_password_secret_data.py
+  ark_sdk_python/models/common/isp/ark_platform_discovery_schemas.py
 
-  offset of local header from start of archive:   90544
-                                                  (00000000000161B0h) bytes
+  offset of local header from start of archive:   104070
+                                                  (0000000000019686h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         8bc6c55a
-  compressed size:                                297 bytes
-  uncompressed size:                              650 bytes
-  length of filename:                             98 characters
+  32-bit CRC value (hex):                         87d5f682
+  compressed size:                                109 bytes
+  uncompressed size:                              139 bytes
+  length of filename:                             66 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5893,32 +5884,32 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #161:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/certificates/
+  ark_sdk_python/models/common/identity/
 
-  offset of local header from start of archive:   90997
-                                                  (0000000000016375h) bytes
+  offset of local header from start of archive:   104303
+                                                  (000000000001976Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             48 characters
+  length of filename:                             38 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -5929,33 +5920,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #162:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_update_certificate.py
+  ark_sdk_python/models/common/identity/ark_identity_common_schemas.py
 
-  offset of local header from start of archive:   91103
-                                                  (00000000000163DFh) bytes
+  offset of local header from start of archive:   104399
+                                                  (00000000000197CFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         17537990
-  compressed size:                                238 bytes
-  uncompressed size:                              547 bytes
-  length of filename:                             90 characters
+  32-bit CRC value (hex):                         2b244a35
+  compressed size:                                212 bytes
+  uncompressed size:                              442 bytes
+  length of filename:                             68 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -5966,33 +5957,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #163:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/certificates/__init__.py
+  ark_sdk_python/models/common/identity/ark_identity_auth_schemas.py
 
-  offset of local header from start of archive:   91489
-                                                  (0000000000016561h) bytes
+  offset of local header from start of archive:   104737
+                                                  (0000000000019921h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         a0ccd7f1
-  compressed size:                                227 bytes
-  uncompressed size:                              1036 bytes
-  length of filename:                             59 characters
+  32-bit CRC value (hex):                         c5dc718c
+  compressed size:                                748 bytes
+  uncompressed size:                              3077 bytes
+  length of filename:                             66 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6003,33 +5994,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #164:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_certificate.py
+  ark_sdk_python/models/common/identity/__init__.py
 
-  offset of local header from start of archive:   91833
-                                                  (00000000000166B9h) bytes
+  offset of local header from start of archive:   105609
+                                                  (0000000000019C89h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         cf550e80
-  compressed size:                                754 bytes
-  uncompressed size:                              3706 bytes
-  length of filename:                             83 characters
+  32-bit CRC value (hex):                         233cb730
+  compressed size:                                455 bytes
+  uncompressed size:                              1945 bytes
+  length of filename:                             49 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6040,33 +6031,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #165:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_delete_certificate.py
+  ark_sdk_python/models/common/identity/ark_identity_directory_schemas.py
 
-  offset of local header from start of archive:   92728
-                                                  (0000000000016A38h) bytes
+  offset of local header from start of archive:   106171
+                                                  (0000000000019EBBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         ebda57cb
-  compressed size:                                148 bytes
-  uncompressed size:                              207 bytes
-  length of filename:                             90 characters
+  32-bit CRC value (hex):                         913b540a
+  compressed size:                                1176 bytes
+  uncompressed size:                              4706 bytes
+  length of filename:                             71 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6077,70 +6068,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #166:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_filter.py
+  ark_sdk_python/models/common/aws/
 
-  offset of local header from start of archive:   93024
-                                                  (0000000000016B60h) bytes
+  offset of local header from start of archive:   107476
+                                                  (000000000001A3D4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         1b244466
-  compressed size:                                179 bytes
-  uncompressed size:                              337 bytes
-  length of filename:                             78 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #167:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_get_certificate.py
+  ark_sdk_python/models/common/aws/ark_cfn_async_task.py
 
-  offset of local header from start of archive:   93339
-                                                  (0000000000016C9Bh) bytes
+  offset of local header from start of archive:   107567
+                                                  (000000000001A42Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         73d15338
-  compressed size:                                144 bytes
-  uncompressed size:                              204 bytes
-  length of filename:                             87 characters
+  32-bit CRC value (hex):                         cf8384fc
+  compressed size:                                269 bytes
+  uncompressed size:                              566 bytes
+  length of filename:                             54 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6151,69 +6141,70 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #168:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/k8s/
+  ark_sdk_python/models/common/aws/__init__.py
 
-  offset of local header from start of archive:   93628
-                                                  (0000000000016DBCh) bytes
+  offset of local header from start of archive:   107948
+                                                  (000000000001A5ACh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             39 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         0748bece
+  compressed size:                                92 bytes
+  uncompressed size:                              111 bytes
+  length of filename:                             44 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #169:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/k8s/__init__.py
+  ark_sdk_python/models/common/ark_status.py
 
-  offset of local header from start of archive:   93725
-                                                  (0000000000016E1Dh) bytes
+  offset of local header from start of archive:   108142
+                                                  (000000000001A66Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         55723d6e
-  compressed size:                                114 bytes
-  uncompressed size:                              154 bytes
-  length of filename:                             50 characters
+  32-bit CRC value (hex):                         f9a9b887
+  compressed size:                                724 bytes
+  uncompressed size:                              2504 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6224,33 +6215,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #170:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/k8s/ark_dpa_k8s_generate_kubeconfig.py
+  ark_sdk_python/models/common/ark_protocol_type.py
 
-  offset of local header from start of archive:   93947
-                                                  (0000000000016EFBh) bytes
+  offset of local header from start of archive:   108966
+                                                  (000000000001A9A6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         df72a0f4
-  compressed size:                                165 bytes
-  uncompressed size:                              218 bytes
-  length of filename:                             73 characters
+  32-bit CRC value (hex):                         fca4a933
+  compressed size:                                190 bytes
+  uncompressed size:                              328 bytes
+  length of filename:                             49 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6261,141 +6252,144 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #171:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/
+  ark_sdk_python/models/common/ark_connector_type.py
 
-  offset of local header from start of archive:   94243
-                                                  (0000000000017023h) bytes
+  offset of local header from start of archive:   109263
+                                                  (000000000001AACFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             46 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         880a652a
+  compressed size:                                82 bytes
+  uncompressed size:                              94 bytes
+  length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #172:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/__init__.py
+  ark_sdk_python/models/common/ark_async_task.py
 
-  offset of local header from start of archive:   94347
-                                                  (000000000001708Bh) bytes
+  offset of local header from start of archive:   109453
+                                                  (000000000001AB8Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             57 characters
+  32-bit CRC value (hex):                         d313e9dc
+  compressed size:                                271 bytes
+  uncompressed size:                              525 bytes
+  length of filename:                             46 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #173:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/
+  ark_sdk_python/models/common/ark_workspace_type.py
 
-  offset of local header from start of archive:   94462
-                                                  (00000000000170FEh) bytes
+  offset of local header from start of archive:   109828
+                                                  (000000000001AD04h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             49 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         52e02a70
+  compressed size:                                301 bytes
+  uncompressed size:                              547 bytes
+  length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #174:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_tag.py
+  ark_sdk_python/models/common/ark_async_request_settings.py
 
-  offset of local header from start of archive:   94569
-                                                  (0000000000017169h) bytes
+  offset of local header from start of archive:   110237
+                                                  (000000000001AE9Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         2e0eb04c
-  compressed size:                                241 bytes
-  uncompressed size:                              490 bytes
-  length of filename:                             66 characters
+  32-bit CRC value (hex):                         e4d10a5d
+  compressed size:                                406 bytes
+  uncompressed size:                              924 bytes
+  length of filename:                             58 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6406,33 +6400,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #175:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_databases_filter.py
+  ark_sdk_python/models/common/ark_counted_values.py
 
-  offset of local header from start of archive:   94934
-                                                  (00000000000172D6h) bytes
+  offset of local header from start of archive:   110759
+                                                  (000000000001B0A7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         ca199899
-  compressed size:                                361 bytes
-  uncompressed size:                              1135 bytes
-  length of filename:                             79 characters
+  32-bit CRC value (hex):                         eb570195
+  compressed size:                                170 bytes
+  uncompressed size:                              272 bytes
+  length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6443,33 +6437,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #176:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/__init__.py
+  ark_sdk_python/models/ark_exceptions.py
 
-  offset of local header from start of archive:   95432
-                                                  (00000000000174C8h) bytes
+  offset of local header from start of archive:   111037
+                                                  (000000000001B1BDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         64dd8afe
-  compressed size:                                406 bytes
-  uncompressed size:                              2080 bytes
-  length of filename:                             60 characters
+  32-bit CRC value (hex):                         4d4f63cf
+  compressed size:                                195 bytes
+  uncompressed size:                              562 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6480,33 +6474,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #177:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_delete_database.py
+  ark_sdk_python/models/ark_profile.py
 
-  offset of local header from start of archive:   95956
-                                                  (00000000000176D4h) bytes
+  offset of local header from start of archive:   111329
+                                                  (000000000001B2E1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         b99a8d79
-  compressed size:                                304 bytes
-  uncompressed size:                              583 bytes
-  length of filename:                             78 characters
+  32-bit CRC value (hex):                         c80c5ecd
+  compressed size:                                1492 bytes
+  uncompressed size:                              6300 bytes
+  length of filename:                             36 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6517,181 +6511,177 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #178:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_provider.py
+  ark_sdk_python/models/services/
 
-  offset of local header from start of archive:   96396
-                                                  (000000000001788Ch) bytes
+  offset of local header from start of archive:   112915
+                                                  (000000000001B913h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         e6d02035
-  compressed size:                                789 bytes
-  uncompressed size:                              3785 bytes
-  length of filename:                             71 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #179:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_get_database.py
+  ark_sdk_python/models/services/dpa/
 
-  offset of local header from start of archive:   97314
-                                                  (0000000000017C22h) bytes
+  offset of local header from start of archive:   113004
+                                                  (000000000001B96Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         8f59dea0
-  compressed size:                                302 bytes
-  uncompressed size:                              574 bytes
-  length of filename:                             75 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #180:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_warning.py
+  ark_sdk_python/models/services/dpa/policies/
 
-  offset of local header from start of archive:   97749
-                                                  (0000000000017DD5h) bytes
+  offset of local header from start of archive:   113097
+                                                  (000000000001B9C9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         edf3a6c9
-  compressed size:                                116 bytes
-  uncompressed size:                              153 bytes
-  length of filename:                             70 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             44 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #181:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_databases_stats.py
+  ark_sdk_python/models/services/dpa/policies/vm/
 
-  offset of local header from start of archive:   97993
-                                                  (0000000000017EC9h) bytes
+  offset of local header from start of archive:   113199
+                                                  (000000000001BA2Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         b48a7e63
-  compressed size:                                361 bytes
-  uncompressed size:                              1246 bytes
-  length of filename:                             78 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             47 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #182:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_update_database.py
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy.py
 
-  offset of local header from start of archive:   98490
-                                                  (00000000000180BAh) bytes
+  offset of local header from start of archive:   113304
+                                                  (000000000001BA98h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         de63733e
-  compressed size:                                914 bytes
-  uncompressed size:                              2989 bytes
-  length of filename:                             78 characters
+  32-bit CRC value (hex):                         f763cc9d
+  compressed size:                                552 bytes
+  uncompressed size:                              1590 bytes
+  length of filename:                             67 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6702,33 +6692,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #183:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_add_database.py
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_connection_data.py
 
-  offset of local header from start of archive:   99540
-                                                  (00000000000184D4h) bytes
+  offset of local header from start of archive:   113981
+                                                  (000000000001BD3Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c9fb8f08
-  compressed size:                                872 bytes
-  uncompressed size:                              2658 bytes
-  length of filename:                             75 characters
+  32-bit CRC value (hex):                         e781c633
+  compressed size:                                350 bytes
+  uncompressed size:                              926 bytes
+  length of filename:                             76 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6739,33 +6729,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #184:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_platform_type_serializer.py
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_workspace_type_serializer.py
 
-  offset of local header from start of archive:   100545
-                                                  (00000000000188C1h) bytes
+  offset of local header from start of archive:   114465
+                                                  (000000000001BF21h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         e78da1af
-  compressed size:                                232 bytes
-  uncompressed size:                              558 bytes
-  length of filename:                             87 characters
+  32-bit CRC value (hex):                         2d319afb
+  compressed size:                                243 bytes
+  uncompressed size:                              585 bytes
+  length of filename:                             95 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6776,32 +6766,32 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #185:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_database_info.py
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_filter.py
 
-  offset of local header from start of archive:   100922
-                                                  (0000000000018A3Ah) bytes
+  offset of local header from start of archive:   114861
+                                                  (000000000001C0ADh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c86caf7a
-  compressed size:                                687 bytes
-  uncompressed size:                              1835 bytes
+  32-bit CRC value (hex):                         557b1ab3
+  compressed size:                                401 bytes
+  uncompressed size:                              935 bytes
   length of filename:                             76 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -6813,33 +6803,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #186:
 ---------------------------
 
-  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_database.py
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_stats.py
 
-  offset of local header from start of archive:   101743
-                                                  (0000000000018D6Fh) bytes
+  offset of local header from start of archive:   115396
+                                                  (000000000001C2C4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         3732c6c4
-  compressed size:                                862 bytes
-  uncompressed size:                              2644 bytes
-  length of filename:                             71 characters
+  32-bit CRC value (hex):                         b4482d6a
+  compressed size:                                384 bytes
+  uncompressed size:                              896 bytes
+  length of filename:                             75 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6850,33 +6840,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #187:
 ---------------------------
 
-  ark_sdk_python/models/services/ark_service_config.py
+  ark_sdk_python/models/services/dpa/policies/vm/__init__.py
 
-  offset of local header from start of archive:   102734
-                                                  (000000000001914Eh) bytes
+  offset of local header from start of archive:   115913
+                                                  (000000000001C4C9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         1bbe4d36
-  compressed size:                                245 bytes
-  uncompressed size:                              487 bytes
-  length of filename:                             52 characters
+  32-bit CRC value (hex):                         d780bf77
+  compressed size:                                494 bytes
+  uncompressed size:                              2599 bytes
+  length of filename:                             58 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6887,69 +6877,70 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #188:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_protocol_type_serializer.py
 
-  offset of local header from start of archive:   103089
-                                                  (00000000000192B1h) bytes
+  offset of local header from start of archive:   116523
+                                                  (000000000001C72Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             34 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         51ced9d0
+  compressed size:                                240 bytes
+  uncompressed size:                              679 bytes
+  length of filename:                             94 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #189:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/ark_sm_session.py
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_update_policy.py
 
-  offset of local header from start of archive:   103181
-                                                  (000000000001930Dh) bytes
+  offset of local header from start of archive:   116915
+                                                  (000000000001C8B3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         293f18d1
-  compressed size:                                630 bytes
-  uncompressed size:                              2195 bytes
-  length of filename:                             51 characters
+  32-bit CRC value (hex):                         fbe0b866
+  compressed size:                                555 bytes
+  uncompressed size:                              1603 bytes
+  length of filename:                             74 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6960,33 +6951,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #190:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/ark_sm_get_session.py
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_authorization_rule.py
 
-  offset of local header from start of archive:   103920
-                                                  (00000000000195F0h) bytes
+  offset of local header from start of archive:   117602
+                                                  (000000000001CB62h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         d0e42846
-  compressed size:                                124 bytes
-  uncompressed size:                              167 bytes
-  length of filename:                             55 characters
+  32-bit CRC value (hex):                         8dcbb607
+  compressed size:                                537 bytes
+  uncompressed size:                              1662 bytes
+  length of filename:                             79 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -6997,33 +6988,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #191:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/ark_sm_session_activity_filter.py
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_providers.py
 
-  offset of local header from start of archive:   104157
-                                                  (00000000000196DDh) bytes
+  offset of local header from start of archive:   118276
+                                                  (000000000001CE04h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         2dcc0f3f
-  compressed size:                                169 bytes
-  uncompressed size:                              281 bytes
-  length of filename:                             67 characters
+  32-bit CRC value (hex):                         4a084550
+  compressed size:                                759 bytes
+  uncompressed size:                              2862 bytes
+  length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7034,33 +7025,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #192:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/ark_sm_workspace_type_serializer.py
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy_list_item.py
 
-  offset of local header from start of archive:   104451
-                                                  (0000000000019803h) bytes
+  offset of local header from start of archive:   119163
+                                                  (000000000001D17Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         2c0ab50d
-  compressed size:                                240 bytes
-  uncompressed size:                              627 bytes
-  length of filename:                             69 characters
+  32-bit CRC value (hex):                         79f5ddda
+  compressed size:                                395 bytes
+  uncompressed size:                              927 bytes
+  length of filename:                             77 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7071,33 +7062,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #193:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/__init__.py
+  ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_add_policy.py
 
-  offset of local header from start of archive:   104818
-                                                  (0000000000019972h) bytes
+  offset of local header from start of archive:   119693
+                                                  (000000000001D38Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7ed0f4c4
-  compressed size:                                259 bytes
-  uncompressed size:                              1255 bytes
-  length of filename:                             45 characters
+  32-bit CRC value (hex):                         d28713be
+  compressed size:                                645 bytes
+  uncompressed size:                              1826 bytes
+  length of filename:                             71 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7108,107 +7099,105 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #194:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/ark_sm_sessions_stats.py
+  ark_sdk_python/models/services/dpa/policies/__init__.py
 
-  offset of local header from start of archive:   105180
-                                                  (0000000000019ADCh) bytes
+  offset of local header from start of archive:   120467
+                                                  (000000000001D693h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         67738cb4
-  compressed size:                                563 bytes
-  uncompressed size:                              2089 bytes
-  length of filename:                             58 characters
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             55 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #195:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/ark_sm_session_activity.py
+  ark_sdk_python/models/services/dpa/policies/common/
 
-  offset of local header from start of archive:   105859
-                                                  (0000000000019D83h) bytes
+  offset of local header from start of archive:   120580
+                                                  (000000000001D704h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         86a4c495
-  compressed size:                                474 bytes
-  uncompressed size:                              1689 bytes
-  length of filename:                             60 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             51 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #196:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/ark_sm_sessions_filter.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_rule_status.py
 
-  offset of local header from start of archive:   106451
-                                                  (0000000000019FD3h) bytes
+  offset of local header from start of archive:   120689
+                                                  (000000000001D771h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         19840fab
-  compressed size:                                374 bytes
-  uncompressed size:                              952 bytes
-  length of filename:                             59 characters
+  32-bit CRC value (hex):                         4a6a3dd3
+  compressed size:                                103 bytes
+  uncompressed size:                              153 bytes
+  length of filename:                             73 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7219,33 +7208,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #197:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/ark_sm_get_session_activities.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_connection_information.py
 
-  offset of local header from start of archive:   106942
-                                                  (000000000001A1BEh) bytes
+  offset of local header from start of archive:   120923
+                                                  (000000000001D85Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         cd7938d6
-  compressed size:                                139 bytes
-  uncompressed size:                              196 bytes
-  length of filename:                             66 characters
+  32-bit CRC value (hex):                         36818b67
+  compressed size:                                557 bytes
+  uncompressed size:                              1272 bytes
+  length of filename:                             89 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7256,33 +7245,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #198:
 ---------------------------
 
-  ark_sdk_python/models/services/sm/ark_sm_protocol_type_serializer.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policy.py
 
-  offset of local header from start of archive:   107205
-                                                  (000000000001A2C5h) bytes
+  offset of local header from start of archive:   121627
+                                                  (000000000001DB1Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         316d348c
-  compressed size:                                253 bytes
-  uncompressed size:                              812 bytes
-  length of filename:                             68 characters
+  32-bit CRC value (hex):                         04cb14f9
+  compressed size:                                252 bytes
+  uncompressed size:                              691 bytes
+  length of filename:                             73 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7293,69 +7282,70 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #199:
 ---------------------------
 
-  ark_sdk_python/models/common/
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_update_policy_status.py
 
-  offset of local header from start of archive:   107584
-                                                  (000000000001A440h) bytes
+  offset of local header from start of archive:   122010
+                                                  (000000000001DC9Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             29 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         57334be9
+  compressed size:                                360 bytes
+  uncompressed size:                              798 bytes
+  length of filename:                             82 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #200:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_status.py
+  ark_sdk_python/models/services/dpa/policies/common/__init__.py
 
-  offset of local header from start of archive:   107671
-                                                  (000000000001A497h) bytes
+  offset of local header from start of archive:   122510
+                                                  (000000000001DE8Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         f9a9b887
-  compressed size:                                724 bytes
-  uncompressed size:                              2504 bytes
-  length of filename:                             42 characters
+  32-bit CRC value (hex):                         736492e1
+  compressed size:                                367 bytes
+  uncompressed size:                              1942 bytes
+  length of filename:                             62 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7366,33 +7356,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #201:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_validations.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policy_list_item.py
 
-  offset of local header from start of archive:   108495
-                                                  (000000000001A7CFh) bytes
+  offset of local header from start of archive:   122997
+                                                  (000000000001E075h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         e65b560d
-  compressed size:                                138 bytes
-  uncompressed size:                              184 bytes
-  length of filename:                             47 characters
+  32-bit CRC value (hex):                         b81435bb
+  compressed size:                                288 bytes
+  uncompressed size:                              723 bytes
+  length of filename:                             83 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7403,33 +7393,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #202:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_connector_type.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_delete_policy.py
 
-  offset of local header from start of archive:   108738
-                                                  (000000000001A8C2h) bytes
+  offset of local header from start of archive:   123426
+                                                  (000000000001E222h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         880a652a
-  compressed size:                                82 bytes
-  uncompressed size:                              94 bytes
-  length of filename:                             50 characters
+  32-bit CRC value (hex):                         76dd9763
+  compressed size:                                293 bytes
+  uncompressed size:                              589 bytes
+  length of filename:                             75 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7440,33 +7430,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #203:
 ---------------------------
 
-  ark_sdk_python/models/common/__init__.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_add_policy.py
 
-  offset of local header from start of archive:   108928
-                                                  (000000000001A980h) bytes
+  offset of local header from start of archive:   123852
+                                                  (000000000001E3CCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         d361b870
-  compressed size:                                459 bytes
-  uncompressed size:                              1877 bytes
-  length of filename:                             40 characters
+  32-bit CRC value (hex):                         8d7ce2ec
+  compressed size:                                328 bytes
+  uncompressed size:                              807 bytes
+  length of filename:                             77 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7477,33 +7467,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #204:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_network_entity_type.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policies_stats.py
 
-  offset of local header from start of archive:   109485
-                                                  (000000000001ABADh) bytes
+  offset of local header from start of archive:   124315
+                                                  (000000000001E59Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         89839e5a
-  compressed size:                                192 bytes
-  uncompressed size:                              391 bytes
-  length of filename:                             55 characters
+  32-bit CRC value (hex):                         3876d342
+  compressed size:                                220 bytes
+  uncompressed size:                              425 bytes
+  length of filename:                             81 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7514,69 +7504,70 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #205:
 ---------------------------
 
-  ark_sdk_python/models/common/aws/
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_update_policy.py
 
-  offset of local header from start of archive:   109790
-                                                  (000000000001ACDEh) bytes
+  offset of local header from start of archive:   124674
+                                                  (000000000001E702h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         8ddfdc21
+  compressed size:                                421 bytes
+  uncompressed size:                              1137 bytes
+  length of filename:                             80 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #206:
 ---------------------------
 
-  ark_sdk_python/models/common/aws/__init__.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_authorization_rule.py
 
-  offset of local header from start of archive:   109881
-                                                  (000000000001AD39h) bytes
+  offset of local header from start of archive:   125233
+                                                  (000000000001E931h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         0748bece
-  compressed size:                                92 bytes
-  uncompressed size:                              111 bytes
-  length of filename:                             44 characters
+  32-bit CRC value (hex):                         9f887eef
+  compressed size:                                211 bytes
+  uncompressed size:                              386 bytes
+  length of filename:                             85 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7587,33 +7578,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #207:
 ---------------------------
 
-  ark_sdk_python/models/common/aws/ark_cfn_async_task.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_get_policy.py
 
-  offset of local header from start of archive:   110075
-                                                  (000000000001ADFBh) bytes
+  offset of local header from start of archive:   125587
+                                                  (000000000001EA93h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         cf8384fc
-  compressed size:                                269 bytes
-  uncompressed size:                              566 bytes
-  length of filename:                             54 characters
+  32-bit CRC value (hex):                         d0fc88bb
+  compressed size:                                290 bytes
+  uncompressed size:                              580 bytes
+  length of filename:                             72 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7624,33 +7615,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #208:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_status_stats.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policies_filter.py
 
-  offset of local header from start of archive:   110456
-                                                  (000000000001AF78h) bytes
+  offset of local header from start of archive:   126007
+                                                  (000000000001EC37h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         6c5bf307
-  compressed size:                                170 bytes
-  uncompressed size:                              271 bytes
-  length of filename:                             48 characters
+  32-bit CRC value (hex):                         7d5dc2d4
+  compressed size:                                229 bytes
+  uncompressed size:                              437 bytes
+  length of filename:                             82 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7661,33 +7652,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #209:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_protocol_type.py
+  ark_sdk_python/models/services/dpa/policies/common/ark_dpa_user_data.py
 
-  offset of local header from start of archive:   110732
-                                                  (000000000001B08Ch) bytes
+  offset of local header from start of archive:   126376
+                                                  (000000000001EDA8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         fca4a933
-  compressed size:                                190 bytes
-  uncompressed size:                              328 bytes
-  length of filename:                             49 characters
+  32-bit CRC value (hex):                         c749a8eb
+  compressed size:                                273 bytes
+  uncompressed size:                              769 bytes
+  length of filename:                             71 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7698,70 +7689,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #210:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_workspace_type.py
+  ark_sdk_python/models/services/dpa/policies/db/
 
-  offset of local header from start of archive:   111029
-                                                  (000000000001B1B5h) bytes
+  offset of local header from start of archive:   126778
+                                                  (000000000001EF3Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         bc9ff7c2
-  compressed size:                                279 bytes
-  uncompressed size:                              495 bytes
-  length of filename:                             50 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             47 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #211:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_application_code.py
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_connection_data.py
 
-  offset of local header from start of archive:   111416
-                                                  (000000000001B338h) bytes
+  offset of local header from start of archive:   126883
+                                                  (000000000001EFA3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         45bccf01
-  compressed size:                                166 bytes
-  uncompressed size:                              319 bytes
-  length of filename:                             52 characters
+  32-bit CRC value (hex):                         52d03349
+  compressed size:                                709 bytes
+  uncompressed size:                              2810 bytes
+  length of filename:                             76 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7772,33 +7762,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #212:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_async_task.py
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy_list_item.py
 
-  offset of local header from start of archive:   111692
-                                                  (000000000001B44Ch) bytes
+  offset of local header from start of archive:   127726
+                                                  (000000000001F2EEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         d313e9dc
-  compressed size:                                271 bytes
-  uncompressed size:                              525 bytes
-  length of filename:                             46 characters
+  32-bit CRC value (hex):                         58ab2e5b
+  compressed size:                                458 bytes
+  uncompressed size:                              1157 bytes
+  length of filename:                             77 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7809,33 +7799,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #213:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_connection_method.py
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_workspace_type_serializer.py
 
-  offset of local header from start of archive:   112067
-                                                  (000000000001B5C3h) bytes
+  offset of local header from start of archive:   128319
+                                                  (000000000001F53Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         28d71508
-  compressed size:                                118 bytes
-  uncompressed size:                              143 bytes
-  length of filename:                             53 characters
+  32-bit CRC value (hex):                         b95552b2
+  compressed size:                                285 bytes
+  uncompressed size:                              800 bytes
+  length of filename:                             95 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7846,33 +7836,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #214:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_async_status.py
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_providers.py
 
-  offset of local header from start of archive:   112296
-                                                  (000000000001B6A8h) bytes
+  offset of local header from start of archive:   128757
+                                                  (000000000001F6F5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         5e6b5fab
-  compressed size:                                129 bytes
-  uncompressed size:                              178 bytes
-  length of filename:                             48 characters
+  32-bit CRC value (hex):                         c8766514
+  compressed size:                                594 bytes
+  uncompressed size:                              1958 bytes
+  length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7883,69 +7873,70 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #215:
 ---------------------------
 
-  ark_sdk_python/models/common/connections/
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_update_policy.py
 
-  offset of local header from start of archive:   112531
-                                                  (000000000001B793h) bytes
+  offset of local header from start of archive:   129479
+                                                  (000000000001F9C7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             41 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         883fc8b2
+  compressed size:                                359 bytes
+  uncompressed size:                              906 bytes
+  length of filename:                             74 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #216:
 ---------------------------
 
-  ark_sdk_python/models/common/connections/__init__.py
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_filter.py
 
-  offset of local header from start of archive:   112630
-                                                  (000000000001B7F6h) bytes
+  offset of local header from start of archive:   129970
+                                                  (000000000001FBB2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         80c93fa6
-  compressed size:                                158 bytes
-  uncompressed size:                              545 bytes
-  length of filename:                             52 characters
+  32-bit CRC value (hex):                         d62a9ef4
+  compressed size:                                418 bytes
+  uncompressed size:                              1065 bytes
+  length of filename:                             76 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7956,33 +7947,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #217:
 ---------------------------
 
-  ark_sdk_python/models/common/connections/ark_connection_command.py
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_add_policy.py
 
-  offset of local header from start of archive:   112898
-                                                  (000000000001B902h) bytes
+  offset of local header from start of archive:   130522
+                                                  (000000000001FDDAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         786ba61f
-  compressed size:                                205 bytes
-  uncompressed size:                              352 bytes
-  length of filename:                             66 characters
+  32-bit CRC value (hex):                         f55c07bd
+  compressed size:                                371 bytes
+  uncompressed size:                              906 bytes
+  length of filename:                             71 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -7993,33 +7984,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #218:
 ---------------------------
 
-  ark_sdk_python/models/common/connections/ark_connection_credentials.py
+  ark_sdk_python/models/services/dpa/policies/db/__init__.py
 
-  offset of local header from start of archive:   113227
-                                                  (000000000001BA4Bh) bytes
+  offset of local header from start of archive:   131022
+                                                  (000000000001FFCEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         905c9662
-  compressed size:                                233 bytes
-  uncompressed size:                              536 bytes
-  length of filename:                             70 characters
+  32-bit CRC value (hex):                         49c3bd81
+  compressed size:                                531 bytes
+  uncompressed size:                              2530 bytes
+  length of filename:                             58 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8030,69 +8021,70 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #219:
 ---------------------------
 
-  ark_sdk_python/models/common/connections/connection_data/
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy.py
 
-  offset of local header from start of archive:   113588
-                                                  (000000000001BBB4h) bytes
+  offset of local header from start of archive:   131669
+                                                  (0000000000020255h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             57 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         54792f18
+  compressed size:                                292 bytes
+  uncompressed size:                              718 bytes
+  length of filename:                             67 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #220:
 ---------------------------
 
-  ark_sdk_python/models/common/connections/connection_data/__init__.py
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_enums.py
 
-  offset of local header from start of archive:   113703
-                                                  (000000000001BC27h) bytes
+  offset of local header from start of archive:   132086
+                                                  (00000000000203F6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         b4dd4d81
-  compressed size:                                124 bytes
-  uncompressed size:                              294 bytes
-  length of filename:                             68 characters
+  32-bit CRC value (hex):                         2a2b3ea9
+  compressed size:                                257 bytes
+  uncompressed size:                              671 bytes
+  length of filename:                             66 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8103,33 +8095,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #221:
 ---------------------------
 
-  ark_sdk_python/models/common/connections/connection_data/ark_winrm_connection_data.py
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_stats.py
 
-  offset of local header from start of archive:   113953
-                                                  (000000000001BD21h) bytes
+  offset of local header from start of archive:   132467
+                                                  (0000000000020573h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         5e80c9fa
-  compressed size:                                160 bytes
-  uncompressed size:                              240 bytes
-  length of filename:                             85 characters
+  32-bit CRC value (hex):                         21010cf6
+  compressed size:                                405 bytes
+  uncompressed size:                              1011 bytes
+  length of filename:                             75 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8140,33 +8132,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #222:
 ---------------------------
 
-  ark_sdk_python/models/common/connections/connection_data/ark_ssh_connection_data.py
+  ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_authorization_rule.py
 
-  offset of local header from start of archive:   114256
-                                                  (000000000001BE50h) bytes
+  offset of local header from start of archive:   133005
+                                                  (000000000002078Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         b674b469
-  compressed size:                                81 bytes
-  uncompressed size:                              92 bytes
-  length of filename:                             83 characters
+  32-bit CRC value (hex):                         d7b8567b
+  compressed size:                                262 bytes
+  uncompressed size:                              739 bytes
+  length of filename:                             79 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8177,70 +8169,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #223:
 ---------------------------
 
-  ark_sdk_python/models/common/connections/ark_connection_result.py
+  ark_sdk_python/models/services/dpa/certificates/
 
-  offset of local header from start of archive:   114478
-                                                  (000000000001BF2Eh) bytes
+  offset of local header from start of archive:   133404
+                                                  (000000000002091Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         1bc99a8d
-  compressed size:                                172 bytes
-  uncompressed size:                              344 bytes
-  length of filename:                             65 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             48 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #224:
 ---------------------------
 
-  ark_sdk_python/models/common/connections/ark_connection_details.py
+  ark_sdk_python/models/services/dpa/certificates/__init__.py
 
-  offset of local header from start of archive:   114773
-                                                  (000000000001C055h) bytes
+  offset of local header from start of archive:   133510
+                                                  (0000000000020986h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         f4e88e30
-  compressed size:                                541 bytes
-  uncompressed size:                              1508 bytes
-  length of filename:                             66 characters
+  32-bit CRC value (hex):                         a0ccd7f1
+  compressed size:                                227 bytes
+  uncompressed size:                              1036 bytes
+  length of filename:                             59 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8251,33 +8242,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #225:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_region.py
+  ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_update_certificate.py
 
-  offset of local header from start of archive:   115438
-                                                  (000000000001C2EEh) bytes
+  offset of local header from start of archive:   133854
+                                                  (0000000000020ADEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         99dc6b84
-  compressed size:                                1029 bytes
-  uncompressed size:                              3495 bytes
-  length of filename:                             42 characters
+  32-bit CRC value (hex):                         17537990
+  compressed size:                                238 bytes
+  uncompressed size:                              547 bytes
+  length of filename:                             90 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8288,33 +8279,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #226:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_access_method.py
+  ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_certificate.py
 
-  offset of local header from start of archive:   116567
-                                                  (000000000001C757h) bytes
+  offset of local header from start of archive:   134240
+                                                  (0000000000020C60h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7a1acb83
-  compressed size:                                87 bytes
-  uncompressed size:                              98 bytes
-  length of filename:                             49 characters
+  32-bit CRC value (hex):                         cf550e80
+  compressed size:                                754 bytes
+  uncompressed size:                              3706 bytes
+  length of filename:                             83 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8325,33 +8316,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #227:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_counted_values.py
+  ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_get_certificate.py
 
-  offset of local header from start of archive:   116761
-                                                  (000000000001C819h) bytes
+  offset of local header from start of archive:   135135
+                                                  (0000000000020FDFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         eb570195
-  compressed size:                                170 bytes
-  uncompressed size:                              272 bytes
-  length of filename:                             50 characters
+  32-bit CRC value (hex):                         73d15338
+  compressed size:                                144 bytes
+  uncompressed size:                              204 bytes
+  length of filename:                             87 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8362,33 +8353,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #228:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_os_type.py
+  ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_filter.py
 
-  offset of local header from start of archive:   117039
-                                                  (000000000001C92Fh) bytes
+  offset of local header from start of archive:   135424
+                                                  (0000000000021100h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         4be765ae
-  compressed size:                                202 bytes
-  uncompressed size:                              452 bytes
-  length of filename:                             43 characters
+  32-bit CRC value (hex):                         1b244466
+  compressed size:                                179 bytes
+  uncompressed size:                              337 bytes
+  length of filename:                             78 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8399,142 +8390,141 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #229:
 ---------------------------
 
-  ark_sdk_python/models/common/isp/
+  ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_delete_certificate.py
 
-  offset of local header from start of archive:   117342
-                                                  (000000000001CA5Eh) bytes
+  offset of local header from start of archive:   135739
+                                                  (000000000002123Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         ebda57cb
+  compressed size:                                148 bytes
+  uncompressed size:                              207 bytes
+  length of filename:                             90 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #230:
 ---------------------------
 
-  ark_sdk_python/models/common/isp/__init__.py
+  ark_sdk_python/models/services/dpa/workspaces/
 
-  offset of local header from start of archive:   117433
-                                                  (000000000001CAB9h) bytes
+  offset of local header from start of archive:   136035
+                                                  (0000000000021363h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         199b0474
-  compressed size:                                106 bytes
-  uncompressed size:                              141 bytes
-  length of filename:                             44 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             46 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #231:
 ---------------------------
 
-  ark_sdk_python/models/common/isp/ark_platform_discovery_schemas.py
+  ark_sdk_python/models/services/dpa/workspaces/__init__.py
 
-  offset of local header from start of archive:   117641
-                                                  (000000000001CB89h) bytes
+  offset of local header from start of archive:   136139
+                                                  (00000000000213CBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         87d5f682
-  compressed size:                                109 bytes
-  uncompressed size:                              139 bytes
-  length of filename:                             66 characters
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             57 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #232:
 ---------------------------
 
-  ark_sdk_python/models/common/identity/
+  ark_sdk_python/models/services/dpa/workspaces/db/
 
-  offset of local header from start of archive:   117874
-                                                  (000000000001CC72h) bytes
+  offset of local header from start of archive:   136254
+                                                  (000000000002143Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             38 characters
+  length of filename:                             49 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -8545,33 +8535,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #233:
 ---------------------------
 
-  ark_sdk_python/models/common/identity/ark_identity_directory_schemas.py
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_databases_filter.py
 
-  offset of local header from start of archive:   117970
-                                                  (000000000001CCD2h) bytes
+  offset of local header from start of archive:   136361
+                                                  (00000000000214A9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         913b540a
-  compressed size:                                1176 bytes
-  uncompressed size:                              4706 bytes
-  length of filename:                             71 characters
+  32-bit CRC value (hex):                         ca199899
+  compressed size:                                361 bytes
+  uncompressed size:                              1135 bytes
+  length of filename:                             79 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8582,33 +8572,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #234:
 ---------------------------
 
-  ark_sdk_python/models/common/identity/__init__.py
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_databases_stats.py
 
-  offset of local header from start of archive:   119275
-                                                  (000000000001D1EBh) bytes
+  offset of local header from start of archive:   136859
+                                                  (000000000002169Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         233cb730
-  compressed size:                                455 bytes
-  uncompressed size:                              1945 bytes
-  length of filename:                             49 characters
+  32-bit CRC value (hex):                         b48a7e63
+  compressed size:                                361 bytes
+  uncompressed size:                              1246 bytes
+  length of filename:                             78 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8619,33 +8609,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #235:
 ---------------------------
 
-  ark_sdk_python/models/common/identity/ark_identity_common_schemas.py
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_add_database.py
 
-  offset of local header from start of archive:   119837
-                                                  (000000000001D41Dh) bytes
+  offset of local header from start of archive:   137356
+                                                  (000000000002188Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         2b244a35
-  compressed size:                                212 bytes
-  uncompressed size:                              442 bytes
-  length of filename:                             68 characters
+  32-bit CRC value (hex):                         d30f7601
+  compressed size:                                962 bytes
+  uncompressed size:                              3082 bytes
+  length of filename:                             75 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8656,33 +8646,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #236:
 ---------------------------
 
-  ark_sdk_python/models/common/identity/ark_identity_auth_schemas.py
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_warning.py
 
-  offset of local header from start of archive:   120175
-                                                  (000000000001D56Fh) bytes
+  offset of local header from start of archive:   138451
+                                                  (0000000000021CD3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c5dc718c
-  compressed size:                                748 bytes
-  uncompressed size:                              3077 bytes
-  length of filename:                             66 characters
+  32-bit CRC value (hex):                         edf3a6c9
+  compressed size:                                116 bytes
+  uncompressed size:                              153 bytes
+  length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8693,33 +8683,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #237:
 ---------------------------
 
-  ark_sdk_python/models/common/ark_async_request_settings.py
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_get_database.py
 
-  offset of local header from start of archive:   121047
-                                                  (000000000001D8D7h) bytes
+  offset of local header from start of archive:   138695
+                                                  (0000000000021DC7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         e4d10a5d
-  compressed size:                                406 bytes
-  uncompressed size:                              924 bytes
-  length of filename:                             58 characters
+  32-bit CRC value (hex):                         8f59dea0
+  compressed size:                                302 bytes
+  uncompressed size:                              574 bytes
+  length of filename:                             75 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8730,33 +8720,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #238:
 ---------------------------
 
-  ark_sdk_python/models/ark_profile.py
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_database.py
 
-  offset of local header from start of archive:   121569
-                                                  (000000000001DAE1h) bytes
+  offset of local header from start of archive:   139130
+                                                  (0000000000021F7Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c80c5ecd
-  compressed size:                                1492 bytes
-  uncompressed size:                              6300 bytes
-  length of filename:                             36 characters
+  32-bit CRC value (hex):                         3732c6c4
+  compressed size:                                862 bytes
+  uncompressed size:                              2644 bytes
+  length of filename:                             71 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -8767,249 +8757,218 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #239:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/
+  ark_sdk_python/models/services/dpa/workspaces/db/__init__.py
 
-  offset of local header from start of archive:   123155
-                                                  (000000000001E113h) bytes
+  offset of local header from start of archive:   140121
+                                                  (0000000000022359h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         64dd8afe
+  compressed size:                                406 bytes
+  uncompressed size:                              2080 bytes
+  length of filename:                             60 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #240:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/__init__.py
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_database_info.py
 
-  offset of local header from start of archive:   123248
-                                                  (000000000001E170h) bytes
+  offset of local header from start of archive:   140645
+                                                  (0000000000022565h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             46 characters
+  32-bit CRC value (hex):                         c86caf7a
+  compressed size:                                687 bytes
+  uncompressed size:                              1835 bytes
+  length of filename:                             76 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #241:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_delete_database.py
 
-  offset of local header from start of archive:   123352
-                                                  (000000000001E1D8h) bytes
+  offset of local header from start of archive:   141466
+                                                  (000000000002289Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             39 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         b99a8d79
+  compressed size:                                304 bytes
+  uncompressed size:                              583 bytes
+  length of filename:                             78 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #242:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/__init__.py
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_platform_type_serializer.py
 
-  offset of local header from start of archive:   123449
-                                                  (000000000001E239h) bytes
+  offset of local header from start of archive:   141906
+                                                  (0000000000022A52h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             50 characters
+  32-bit CRC value (hex):                         e78da1af
+  compressed size:                                232 bytes
+  uncompressed size:                              558 bytes
+  length of filename:                             87 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #243:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_provider.py
 
-  offset of local header from start of archive:   123557
-                                                  (000000000001E2A5h) bytes
+  offset of local header from start of archive:   142283
+                                                  (0000000000022BCBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             55 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         b3817a77
+  compressed size:                                829 bytes
+  uncompressed size:                              4041 bytes
+  length of filename:                             71 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #244:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/vm/
-
-  offset of local header from start of archive:   123670
-                                                  (000000000001E316h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             58 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e9 03 00 00 04 7f 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #245:
----------------------------
-
-  ark_sdk_python/models/cli_services/dpa/policies_editor/vm/__init__.py
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_tag.py
 
-  offset of local header from start of archive:   123786
-                                                  (000000000001E38Ah) bytes
+  offset of local header from start of archive:   143241
+                                                  (0000000000022F89h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         2b290ee1
-  compressed size:                                118 bytes
-  uncompressed size:                              158 bytes
-  length of filename:                             69 characters
+  32-bit CRC value (hex):                         2e0eb04c
+  compressed size:                                241 bytes
+  uncompressed size:                              490 bytes
+  length of filename:                             66 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9017,36 +8976,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #246:
+Central directory entry #245:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/vm/ark_dpa_vm_generate_policy.py
+  ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_update_database.py
 
-  offset of local header from start of archive:   124031
-                                                  (000000000001E47Fh) bytes
+  offset of local header from start of archive:   143606
+                                                  (00000000000230F6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7ac6e730
-  compressed size:                                266 bytes
-  uncompressed size:                              522 bytes
-  length of filename:                             87 characters
+  32-bit CRC value (hex):                         afe921f2
+  compressed size:                                992 bytes
+  uncompressed size:                              3413 bytes
+  length of filename:                             78 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9054,35 +9013,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #247:
+Central directory entry #246:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/__init__.py
+  ark_sdk_python/models/services/dpa/__init__.py
 
-  offset of local header from start of archive:   124442
-                                                  (000000000001E61Ah) bytes
+  offset of local header from start of archive:   144734
+                                                  (000000000002355Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             66 characters
+  length of filename:                             46 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9090,35 +9049,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #248:
+Central directory entry #247:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/
+  ark_sdk_python/models/services/dpa/k8s/
 
-  offset of local header from start of archive:   124566
-                                                  (000000000001E696h) bytes
+  offset of local header from start of archive:   144838
+                                                  (00000000000235C6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             62 characters
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -9126,36 +9085,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #249:
+Central directory entry #248:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_policies_diff.py
+  ark_sdk_python/models/services/dpa/k8s/ark_dpa_k8s_generate_kubeconfig.py
 
-  offset of local header from start of archive:   124686
-                                                  (000000000001E70Eh) bytes
+  offset of local header from start of archive:   144935
+                                                  (0000000000023627h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         1be3547a
-  compressed size:                                218 bytes
-  uncompressed size:                              349 bytes
-  length of filename:                             86 characters
+  32-bit CRC value (hex):                         df72a0f4
+  compressed size:                                165 bytes
+  uncompressed size:                              218 bytes
+  length of filename:                             73 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9163,36 +9122,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #250:
+Central directory entry #249:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/__init__.py
+  ark_sdk_python/models/services/dpa/k8s/__init__.py
 
-  offset of local header from start of archive:   125048
-                                                  (000000000001E878h) bytes
+  offset of local header from start of archive:   145231
+                                                  (000000000002374Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         54b23c2a
-  compressed size:                                283 bytes
-  uncompressed size:                              1628 bytes
-  length of filename:                             73 characters
+  32-bit CRC value (hex):                         55723d6e
+  compressed size:                                114 bytes
+  uncompressed size:                              154 bytes
+  length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9200,36 +9159,72 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
+Central directory entry #250:
+---------------------------
+
+  ark_sdk_python/models/services/dpa/db/
+
+  offset of local header from start of archive:   145453
+                                                  (000000000002382Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             38 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 7f 00 00 00.
+
+  There is no file comment.
+
 Central directory entry #251:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_base_generate_policy.py
+  ark_sdk_python/models/services/dpa/db/ark_dpa_db_proxy_fullchain_generate_assets.py
 
-  offset of local header from start of archive:   125462
-                                                  (000000000001EA16h) bytes
+  offset of local header from start of archive:   145549
+                                                  (000000000002388Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         1930969b
-  compressed size:                                219 bytes
-  uncompressed size:                              342 bytes
-  length of filename:                             93 characters
+  32-bit CRC value (hex):                         ed65cc76
+  compressed size:                                128 bytes
+  uncompressed size:                              192 bytes
+  length of filename:                             83 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9240,33 +9235,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #252:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_remove_policies.py
+  ark_sdk_python/models/services/dpa/db/ark_dpa_db_generated_assets.py
 
-  offset of local header from start of archive:   125832
-                                                  (000000000001EB88h) bytes
+  offset of local header from start of archive:   145818
+                                                  (000000000002399Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7566ada9
-  compressed size:                                187 bytes
-  uncompressed size:                              278 bytes
-  length of filename:                             88 characters
+  32-bit CRC value (hex):                         3146e552
+  compressed size:                                159 bytes
+  uncompressed size:                              227 bytes
+  length of filename:                             68 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9277,33 +9272,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #253:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_loaded_policies.py
+  ark_sdk_python/models/services/dpa/db/ark_dpa_db_assets_type.py
 
-  offset of local header from start of archive:   126165
-                                                  (000000000001ECD5h) bytes
+  offset of local header from start of archive:   146103
+                                                  (0000000000023AB7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         5cea6949
-  compressed size:                                229 bytes
-  uncompressed size:                              559 bytes
-  length of filename:                             88 characters
+  32-bit CRC value (hex):                         a36756f4
+  compressed size:                                139 bytes
+  uncompressed size:                              174 bytes
+  length of filename:                             63 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9314,33 +9309,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #254:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_view_policies.py
+  ark_sdk_python/models/services/dpa/db/__init__.py
 
-  offset of local header from start of archive:   126540
-                                                  (000000000001EE4Ch) bytes
+  offset of local header from start of archive:   146363
+                                                  (0000000000023BBBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         0382245b
-  compressed size:                                239 bytes
-  uncompressed size:                              371 bytes
-  length of filename:                             86 characters
+  32-bit CRC value (hex):                         b078e741
+  compressed size:                                265 bytes
+  uncompressed size:                              1182 bytes
+  length of filename:                             49 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9351,33 +9346,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #255:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_get_policies_status.py
+  ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_execution.py
 
-  offset of local header from start of archive:   126923
-                                                  (000000000001EFCBh) bytes
+  offset of local header from start of archive:   146735
+                                                  (0000000000023D2Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         e5bff3c0
+  32-bit CRC value (hex):                         7e2779cb
   compressed size:                                183 bytes
-  uncompressed size:                              278 bytes
-  length of filename:                             92 characters
+  uncompressed size:                              306 bytes
+  length of filename:                             66 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9388,33 +9383,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #256:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_edit_policies.py
+  ark_sdk_python/models/services/dpa/db/ark_dpa_db_oracle_generate_assets.py
 
-  offset of local header from start of archive:   127256
-                                                  (000000000001F118h) bytes
+  offset of local header from start of archive:   147042
+                                                  (0000000000023E62h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         5018b9a2
-  compressed size:                                185 bytes
-  uncompressed size:                              274 bytes
-  length of filename:                             86 characters
+  32-bit CRC value (hex):                         12c176af
+  compressed size:                                222 bytes
+  uncompressed size:                              392 bytes
+  length of filename:                             74 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9425,33 +9420,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #257:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_policies_status.py
+  ark_sdk_python/models/services/dpa/db/ark_dpa_db_psql_execution.py
 
-  offset of local header from start of archive:   127585
-                                                  (000000000001F261h) bytes
+  offset of local header from start of archive:   147396
+                                                  (0000000000023FC4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         c2f1dd97
-  compressed size:                                175 bytes
-  uncompressed size:                              398 bytes
-  length of filename:                             88 characters
+  32-bit CRC value (hex):                         4b5337c4
+  compressed size:                                174 bytes
+  uncompressed size:                              266 bytes
+  length of filename:                             66 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9462,33 +9457,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #258:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_commit_policies.py
+  ark_sdk_python/models/services/dpa/db/ark_dpa_db_mysql_execution.py
 
-  offset of local header from start of archive:   127906
-                                                  (000000000001F3A2h) bytes
+  offset of local header from start of archive:   147694
+                                                  (00000000000240EEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         ce252390
-  compressed size:                                249 bytes
-  uncompressed size:                              408 bytes
-  length of filename:                             88 characters
+  32-bit CRC value (hex):                         910ccef9
+  compressed size:                                177 bytes
+  uncompressed size:                              269 bytes
+  length of filename:                             67 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9499,33 +9494,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #259:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_reset_policies.py
+  ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_generate_assets.py
 
-  offset of local header from start of archive:   128301
-                                                  (000000000001F52Dh) bytes
+  offset of local header from start of archive:   147996
+                                                  (000000000002421Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         bbacfaaf
-  compressed size:                                232 bytes
-  uncompressed size:                              376 bytes
-  length of filename:                             87 characters
+  32-bit CRC value (hex):                         8ececf34
+  compressed size:                                324 bytes
+  uncompressed size:                              724 bytes
+  length of filename:                             72 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9536,69 +9531,104 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #260:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_load_policies.py
+  ark_sdk_python/models/services/dpa/secrets/
 
-  offset of local header from start of archive:   128678
-                                                  (000000000001F6A6h) bytes
+  offset of local header from start of archive:   148450
+                                                  (00000000000243E2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             43 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 7f 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #261:
+---------------------------
+
+  ark_sdk_python/models/services/dpa/secrets/__init__.py
+
+  offset of local header from start of archive:   148551
+                                                  (0000000000024447h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         840981f9
-  compressed size:                                151 bytes
-  uncompressed size:                              204 bytes
-  length of filename:                             86 characters
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             54 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #261:
+Central directory entry #262:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/db/
+  ark_sdk_python/models/services/dpa/secrets/db/
 
-  offset of local header from start of archive:   128973
-                                                  (000000000001F7CDh) bytes
+  offset of local header from start of archive:   148663
+                                                  (00000000000244B7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             58 characters
+  length of filename:                             46 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -9606,36 +9636,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #262:
+Central directory entry #263:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/db/__init__.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secret_metadata.py
 
-  offset of local header from start of archive:   129089
-                                                  (000000000001F841h) bytes
+  offset of local header from start of archive:   148767
+                                                  (000000000002451Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         df9469a1
-  compressed size:                                116 bytes
-  uncompressed size:                              158 bytes
-  length of filename:                             69 characters
+  32-bit CRC value (hex):                         5bc8dca5
+  compressed size:                                586 bytes
+  uncompressed size:                              2091 bytes
+  length of filename:                             75 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9643,36 +9673,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #263:
+Central directory entry #264:
 ---------------------------
 
-  ark_sdk_python/models/cli_services/dpa/policies_editor/db/ark_dpa_db_generate_policy.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secret_type.py
 
-  offset of local header from start of archive:   129332
-                                                  (000000000001F934h) bytes
+  offset of local header from start of archive:   149486
+                                                  (00000000000247EEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         2b26d447
-  compressed size:                                261 bytes
-  uncompressed size:                              449 bytes
-  length of filename:                             87 characters
+  32-bit CRC value (hex):                         af15e4ea
+  compressed size:                                135 bytes
+  uncompressed size:                              168 bytes
+  length of filename:                             71 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9680,36 +9710,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #264:
+Central directory entry #265:
 ---------------------------
 
-  ark_sdk_python/models/ark_model.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_add_secret.py
 
-  offset of local header from start of archive:   129738
-                                                  (000000000001FACAh) bytes
+  offset of local header from start of archive:   149750
+                                                  (00000000000248F6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         029b0fd6
-  compressed size:                                739 bytes
-  uncompressed size:                              1798 bytes
-  length of filename:                             34 characters
+  32-bit CRC value (hex):                         20ad8b65
+  compressed size:                                528 bytes
+  uncompressed size:                              1572 bytes
+  length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9717,35 +9747,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #265:
+Central directory entry #266:
 ---------------------------
 
-  ark_sdk_python/models/actions/
+  ark_sdk_python/models/services/dpa/secrets/db/secret_links/
 
-  offset of local header from start of archive:   130569
-                                                  (000000000001FE09h) bytes
+  offset of local header from start of archive:   150406
+                                                  (0000000000024B86h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             30 characters
+  length of filename:                             59 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -9753,36 +9783,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #266:
+Central directory entry #267:
 ---------------------------
 
-  ark_sdk_python/models/actions/__init__.py
+  ark_sdk_python/models/services/dpa/secrets/db/secret_links/__init__.py
 
-  offset of local header from start of archive:   130657
-                                                  (000000000001FE61h) bytes
+  offset of local header from start of archive:   150523
+                                                  (0000000000024BFBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         46ad05f9
-  compressed size:                                228 bytes
-  uncompressed size:                              743 bytes
-  length of filename:                             41 characters
+  32-bit CRC value (hex):                         9efed661
+  compressed size:                                138 bytes
+  uncompressed size:                              220 bytes
+  length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9790,36 +9820,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #267:
+Central directory entry #268:
 ---------------------------
 
-  ark_sdk_python/models/actions/ark_service_action_definition.py
+  ark_sdk_python/models/services/dpa/secrets/db/secret_links/ark_dpa_db_pam_account_secret_link.py
 
-  offset of local header from start of archive:   130984
-                                                  (000000000001FFA8h) bytes
+  offset of local header from start of archive:   150789
+                                                  (0000000000024D05h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         52c2076c
-  compressed size:                                336 bytes
-  uncompressed size:                              785 bytes
-  length of filename:                             62 characters
+  32-bit CRC value (hex):                         25434eb9
+  compressed size:                                171 bytes
+  uncompressed size:                              293 bytes
+  length of filename:                             96 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9827,72 +9857,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #268:
----------------------------
-
-  ark_sdk_python/models/actions/services/
-
-  offset of local header from start of archive:   131440
-                                                  (0000000000020170h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             39 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e9 03 00 00 04 7f 00 00 00.
-
-  There is no file comment.
-
 Central directory entry #269:
 ---------------------------
 
-  ark_sdk_python/models/actions/services/__init__.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_delete_secret.py
 
-  offset of local header from start of archive:   131537
-                                                  (00000000000201D1h) bytes
+  offset of local header from start of archive:   151114
+                                                  (0000000000024E4Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         fc8496dd
-  compressed size:                                182 bytes
-  uncompressed size:                              370 bytes
-  length of filename:                             50 characters
+  32-bit CRC value (hex):                         cd19d8e4
+  compressed size:                                307 bytes
+  uncompressed size:                              615 bytes
+  length of filename:                             73 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9903,33 +9897,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #270:
 ---------------------------
 
-  ark_sdk_python/models/actions/services/ark_sm_exec_action_consts.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_update_secret.py
 
-  offset of local header from start of archive:   131827
-                                                  (00000000000202F3h) bytes
+  offset of local header from start of archive:   151552
+                                                  (0000000000025000h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         28612258
-  compressed size:                                379 bytes
-  uncompressed size:                              1161 bytes
-  length of filename:                             67 characters
+  32-bit CRC value (hex):                         29b72961
+  compressed size:                                581 bytes
+  uncompressed size:                              1629 bytes
+  length of filename:                             73 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9940,33 +9934,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #271:
 ---------------------------
 
-  ark_sdk_python/models/actions/services/ark_dpa_exec_action_consts.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secrets_stats.py
 
-  offset of local header from start of archive:   132331
-                                                  (00000000000204EBh) bytes
+  offset of local header from start of archive:   152264
+                                                  (00000000000252C8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         77924c18
-  compressed size:                                1329 bytes
-  uncompressed size:                              7763 bytes
-  length of filename:                             68 characters
+  32-bit CRC value (hex):                         fc4f0e5f
+  compressed size:                                259 bytes
+  uncompressed size:                              799 bytes
+  length of filename:                             73 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -9977,33 +9971,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #272:
 ---------------------------
 
-  ark_sdk_python/models/actions/ark_configure_action_consts.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_get_secret.py
 
-  offset of local header from start of archive:   133786
-                                                  (0000000000020A9Ah) bytes
+  offset of local header from start of archive:   152654
+                                                  (000000000002544Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         6cbaf971
-  compressed size:                                414 bytes
-  uncompressed size:                              1143 bytes
-  length of filename:                             60 characters
+  32-bit CRC value (hex):                         938f2846
+  compressed size:                                304 bytes
+  uncompressed size:                              606 bytes
+  length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10014,69 +10008,70 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #273:
 ---------------------------
 
-  ark_sdk_python/examples/
+  ark_sdk_python/models/services/dpa/secrets/db/__init__.py
 
-  offset of local header from start of archive:   134318
-                                                  (0000000000020CAEh) bytes
+  offset of local header from start of archive:   153086
+                                                  (00000000000255FEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             24 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         27fcacbc
+  compressed size:                                320 bytes
+  uncompressed size:                              1709 bytes
+  length of filename:                             57 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #274:
 ---------------------------
 
-  ark_sdk_python/examples/session_monitoring_activites.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_enable_secret.py
 
-  offset of local header from start of archive:   134400
-                                                  (0000000000020D00h) bytes
+  offset of local header from start of archive:   153521
+                                                  (00000000000257B1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         9a41daa0
-  compressed size:                                578 bytes
-  uncompressed size:                              1632 bytes
-  length of filename:                             55 characters
+  32-bit CRC value (hex):                         25cb0188
+  compressed size:                                306 bytes
+  uncompressed size:                              615 bytes
+  length of filename:                             73 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10087,33 +10082,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #275:
 ---------------------------
 
-  ark_sdk_python/examples/create_dpa_db_environment.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_store_descriptor.py
 
-  offset of local header from start of archive:   135091
-                                                  (0000000000020FB3h) bytes
+  offset of local header from start of archive:   153958
+                                                  (0000000000025966h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         42e1fc46
-  compressed size:                                1110 bytes
-  uncompressed size:                              3744 bytes
-  length of filename:                             52 characters
+  32-bit CRC value (hex):                         591c5d18
+  compressed size:                                200 bytes
+  uncompressed size:                              403 bytes
+  length of filename:                             76 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10124,69 +10119,70 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #276:
 ---------------------------
 
-  ark_sdk_python/args/
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_store_type.py
 
-  offset of local header from start of archive:   136311
-                                                  (0000000000021477h) bytes
+  offset of local header from start of archive:   154292
+                                                  (0000000000025AB4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             20 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         b2585378
+  compressed size:                                267 bytes
+  uncompressed size:                              476 bytes
+  length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #277:
 ---------------------------
 
-  ark_sdk_python/args/__init__.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secrets_filter.py
 
-  offset of local header from start of archive:   136389
-                                                  (00000000000214C5h) bytes
+  offset of local header from start of archive:   154687
+                                                  (0000000000025C3Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         3218a1fc
-  compressed size:                                154 bytes
-  uncompressed size:                              279 bytes
-  length of filename:                             31 characters
+  32-bit CRC value (hex):                         03ba2ead
+  compressed size:                                287 bytes
+  uncompressed size:                              850 bytes
+  length of filename:                             74 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10197,33 +10193,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #278:
 ---------------------------
 
-  ark_sdk_python/args/ark_pydantic_argparse.py
+  ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_disable_secret.py
 
-  offset of local header from start of archive:   136632
-                                                  (00000000000215B8h) bytes
+  offset of local header from start of archive:   155106
+                                                  (0000000000025DE2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         982eeefd
-  compressed size:                                5065 bytes
-  uncompressed size:                              33777 bytes
-  length of filename:                             44 characters
+  32-bit CRC value (hex):                         6e69a5c9
+  compressed size:                                305 bytes
+  uncompressed size:                              618 bytes
+  length of filename:                             74 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10234,106 +10230,106 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #279:
 ---------------------------
 
-  ark_sdk_python/args/ark_args_formatter.py
+  ark_sdk_python/models/services/dpa/secrets/db/secrets_data/
 
-  offset of local header from start of archive:   141799
-                                                  (00000000000229E7h) bytes
+  offset of local header from start of archive:   155543
+                                                  (0000000000025F97h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         d01e8893
-  compressed size:                                2189 bytes
-  uncompressed size:                              9204 bytes
-  length of filename:                             41 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             59 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #280:
 ---------------------------
 
-  ark_sdk_python/cli_services/
+  ark_sdk_python/models/services/dpa/secrets/db/secrets_data/__init__.py
 
-  offset of local header from start of archive:   144087
-                                                  (00000000000232D7h) bytes
+  offset of local header from start of archive:   155660
+                                                  (000000000002600Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         407a0f5d
+  compressed size:                                168 bytes
+  uncompressed size:                              360 bytes
+  length of filename:                             70 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #281:
 ---------------------------
 
-  ark_sdk_python/cli_services/__init__.py
+  ark_sdk_python/models/services/dpa/secrets/db/secrets_data/ark_dpa_db_user_password_secret_data.py
 
-  offset of local header from start of archive:   144173
-                                                  (000000000002332Dh) bytes
+  offset of local header from start of archive:   155956
+                                                  (0000000000026134h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         9c432aca
-  compressed size:                                77 bytes
-  uncompressed size:                              87 bytes
-  length of filename:                             39 characters
+  32-bit CRC value (hex):                         8bc6c55a
+  compressed size:                                297 bytes
+  uncompressed size:                              650 bytes
+  length of filename:                             98 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10344,32 +10340,32 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #282:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/
+  ark_sdk_python/models/services/dpa/sso/
 
-  offset of local header from start of archive:   144347
-                                                  (00000000000233DBh) bytes
+  offset of local header from start of archive:   156409
+                                                  (00000000000262F9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             32 characters
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -10380,69 +10376,70 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #283:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/vm/
+  ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_client_certificate.py
 
-  offset of local header from start of archive:   144437
-                                                  (0000000000023435h) bytes
+  offset of local header from start of archive:   156506
+                                                  (000000000002635Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         c03bb310
+  compressed size:                                454 bytes
+  uncompressed size:                              942 bytes
+  length of filename:                             88 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #284:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/vm/__init__.py
+  ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_password.py
 
-  offset of local header from start of archive:   144530
-                                                  (0000000000023492h) bytes
+  offset of local header from start of archive:   157106
+                                                  (00000000000265B2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         1a2ea348
-  compressed size:                                109 bytes
-  uncompressed size:                              157 bytes
-  length of filename:                             46 characters
+  32-bit CRC value (hex):                         18247993
+  compressed size:                                161 bytes
+  uncompressed size:                              215 bytes
+  length of filename:                             78 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10453,33 +10450,33 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #285:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/vm/ark_dpa_vm_policies_editor_service.py
+  ark_sdk_python/models/services/dpa/sso/__init__.py
 
-  offset of local header from start of archive:   144743
-                                                  (0000000000023567h) bytes
+  offset of local header from start of archive:   157403
+                                                  (00000000000266DBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         f95507f4
-  compressed size:                                2202 bytes
-  uncompressed size:                              8807 bytes
-  length of filename:                             72 characters
+  32-bit CRC value (hex):                         e8434ec1
+  compressed size:                                276 bytes
+  uncompressed size:                              1033 bytes
+  length of filename:                             50 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10490,141 +10487,144 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #286:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/__init__.py
+  ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_oracle_wallet.py
 
-  offset of local header from start of archive:   147075
-                                                  (0000000000023E83h) bytes
+  offset of local header from start of archive:   157787
+                                                  (000000000002685Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             43 characters
+  32-bit CRC value (hex):                         4868e5cb
+  compressed size:                                345 bytes
+  uncompressed size:                              731 bytes
+  length of filename:                             83 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #287:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/common/
+  ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_acquire_token_response.py
 
-  offset of local header from start of archive:   147176
-                                                  (0000000000023EE8h) bytes
+  offset of local header from start of archive:   158273
+                                                  (0000000000026A41h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             39 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         833f0d09
+  compressed size:                                167 bytes
+  uncompressed size:                              277 bytes
+  length of filename:                             76 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #288:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/common/__init__.py
+  ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_rdp_file.py
 
-  offset of local header from start of archive:   147273
-                                                  (0000000000023F49h) bytes
+  offset of local header from start of archive:   158574
+                                                  (0000000000026B6Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             50 characters
+  32-bit CRC value (hex):                         fe31df39
+  compressed size:                                326 bytes
+  uncompressed size:                              703 bytes
+  length of filename:                             78 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #289:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/common/ark_dpa_base_policies_editor_service.py
+  ark_sdk_python/models/services/__init__.py
 
-  offset of local header from start of archive:   147381
-                                                  (0000000000023FB5h) bytes
+  offset of local header from start of archive:   159036
+                                                  (0000000000026D3Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         ce4aecda
-  compressed size:                                4913 bytes
-  uncompressed size:                              27869 bytes
-  length of filename:                             78 characters
+  32-bit CRC value (hex):                         9bf17704
+  compressed size:                                84 bytes
+  uncompressed size:                              111 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10635,32 +10635,69 @@
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
 Central directory entry #290:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/db/
+  ark_sdk_python/models/services/ark_service_config.py
 
-  offset of local header from start of archive:   152430
-                                                  (000000000002536Eh) bytes
+  offset of local header from start of archive:   159220
+                                                  (0000000000026DF4h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         1bbe4d36
+  compressed size:                                245 bytes
+  uncompressed size:                              487 bytes
+  length of filename:                             52 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 7f 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #291:
+---------------------------
+
+  ark_sdk_python/models/services/sm/
+
+  offset of local header from start of archive:   159575
+                                                  (0000000000026F57h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             35 characters
+  length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
@@ -10668,36 +10705,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #291:
+Central directory entry #292:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/db/__init__.py
+  ark_sdk_python/models/services/sm/ark_sm_get_session.py
 
-  offset of local header from start of archive:   152523
-                                                  (00000000000253CBh) bytes
+  offset of local header from start of archive:   159667
+                                                  (0000000000026FB3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         0df547f0
-  compressed size:                                108 bytes
-  uncompressed size:                              157 bytes
-  length of filename:                             46 characters
+  32-bit CRC value (hex):                         d0e42846
+  compressed size:                                124 bytes
+  uncompressed size:                              167 bytes
+  length of filename:                             55 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10705,36 +10742,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #292:
+Central directory entry #293:
 ---------------------------
 
-  ark_sdk_python/cli_services/dpa/db/ark_dpa_db_policies_editor_service.py
+  ark_sdk_python/models/services/sm/ark_sm_workspace_type_serializer.py
 
-  offset of local header from start of archive:   152735
-                                                  (000000000002549Fh) bytes
+  offset of local header from start of archive:   159904
+                                                  (00000000000270A0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         18357480
-  compressed size:                                2356 bytes
-  uncompressed size:                              10620 bytes
-  length of filename:                             72 characters
+  32-bit CRC value (hex):                         2c0ab50d
+  compressed size:                                240 bytes
+  uncompressed size:                              627 bytes
+  length of filename:                             69 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10742,36 +10779,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #293:
+Central directory entry #294:
 ---------------------------
 
-  ark_sdk_python/cli_services/ark_cli_api.py
+  ark_sdk_python/models/services/sm/ark_sm_protocol_type_serializer.py
 
-  offset of local header from start of archive:   155221
-                                                  (0000000000025E55h) bytes
+  offset of local header from start of archive:   160271
+                                                  (000000000002720Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         9e30d8a1
-  compressed size:                                288 bytes
-  uncompressed size:                              912 bytes
-  length of filename:                             42 characters
+  32-bit CRC value (hex):                         316d348c
+  compressed size:                                253 bytes
+  uncompressed size:                              812 bytes
+  length of filename:                             68 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10779,109 +10816,110 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #294:
+Central directory entry #295:
 ---------------------------
 
-  ark_sdk_python/ark.py
+  ark_sdk_python/models/services/sm/__init__.py
 
-  offset of local header from start of archive:   155609
-                                                  (0000000000025FD9h) bytes
+  offset of local header from start of archive:   160650
+                                                  (000000000002738Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         f87196aa
-  compressed size:                                542 bytes
-  uncompressed size:                              1280 bytes
-  length of filename:                             21 characters
+  32-bit CRC value (hex):                         7ed0f4c4
+  compressed size:                                259 bytes
+  uncompressed size:                              1255 bytes
+  length of filename:                             45 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100755 octal):            -rwxr-xr-x
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #295:
+Central directory entry #296:
 ---------------------------
 
-  ark_sdk_python/actions/
+  ark_sdk_python/models/services/sm/ark_sm_session.py
 
-  offset of local header from start of archive:   156230
-                                                  (0000000000026246h) bytes
+  offset of local header from start of archive:   161012
+                                                  (00000000000274F4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             23 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         293f18d1
+  compressed size:                                630 bytes
+  uncompressed size:                              2195 bytes
+  length of filename:                             51 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #296:
+Central directory entry #297:
 ---------------------------
 
-  ark_sdk_python/actions/ark_login_action.py
+  ark_sdk_python/models/services/sm/ark_sm_get_session_activities.py
 
-  offset of local header from start of archive:   156311
-                                                  (0000000000026297h) bytes
+  offset of local header from start of archive:   161751
+                                                  (00000000000277D7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         755a6417
-  compressed size:                                2399 bytes
-  uncompressed size:                              10357 bytes
-  length of filename:                             42 characters
+  32-bit CRC value (hex):                         cd7938d6
+  compressed size:                                139 bytes
+  uncompressed size:                              196 bytes
+  length of filename:                             66 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10889,36 +10927,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #297:
+Central directory entry #298:
 ---------------------------
 
-  ark_sdk_python/actions/ark_profiles_action.py
+  ark_sdk_python/models/services/sm/ark_sm_sessions_stats.py
 
-  offset of local header from start of archive:   158810
-                                                  (0000000000026C5Ah) bytes
+  offset of local header from start of archive:   162014
+                                                  (00000000000278DEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         79e016a0
-  compressed size:                                1995 bytes
-  uncompressed size:                              9638 bytes
-  length of filename:                             45 characters
+  32-bit CRC value (hex):                         67738cb4
+  compressed size:                                563 bytes
+  uncompressed size:                              2089 bytes
+  length of filename:                             58 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10926,36 +10964,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #298:
+Central directory entry #299:
 ---------------------------
 
-  ark_sdk_python/actions/__init__.py
+  ark_sdk_python/models/services/sm/ark_sm_sessions_filter.py
 
-  offset of local header from start of archive:   160908
-                                                  (000000000002748Ch) bytes
+  offset of local header from start of archive:   162693
+                                                  (0000000000027B85h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         98b326d0
-  compressed size:                                175 bytes
-  uncompressed size:                              659 bytes
-  length of filename:                             34 characters
+  32-bit CRC value (hex):                         19840fab
+  compressed size:                                374 bytes
+  uncompressed size:                              952 bytes
+  length of filename:                             59 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -10963,36 +11001,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #299:
+Central directory entry #300:
 ---------------------------
 
-  ark_sdk_python/actions/ark_exec_action.py
+  ark_sdk_python/models/services/sm/ark_sm_session_activity.py
 
-  offset of local header from start of archive:   161175
-                                                  (0000000000027597h) bytes
+  offset of local header from start of archive:   163184
+                                                  (0000000000027D70h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         dc6fe184
-  compressed size:                                3117 bytes
-  uncompressed size:                              14323 bytes
-  length of filename:                             41 characters
+  32-bit CRC value (hex):                         86a4c495
+  compressed size:                                474 bytes
+  uncompressed size:                              1689 bytes
+  length of filename:                             60 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -11000,36 +11038,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #300:
+Central directory entry #301:
 ---------------------------
 
-  ark_sdk_python/actions/ark_configure_action.py
+  ark_sdk_python/models/services/sm/ark_sm_session_activity_filter.py
 
-  offset of local header from start of archive:   164391
-                                                  (0000000000028227h) bytes
+  offset of local header from start of archive:   163776
+                                                  (0000000000027FC0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         fbbc9923
-  compressed size:                                2981 bytes
-  uncompressed size:                              15926 bytes
-  length of filename:                             46 characters
+  32-bit CRC value (hex):                         2dcc0f3f
+  compressed size:                                169 bytes
+  uncompressed size:                              281 bytes
+  length of filename:                             67 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -11037,36 +11075,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #301:
+Central directory entry #302:
 ---------------------------
 
-  ark_sdk_python/actions/ark_action.py
+  ark_sdk_python/models/ark_model.py
 
-  offset of local header from start of archive:   167476
-                                                  (0000000000028E34h) bytes
+  offset of local header from start of archive:   164070
+                                                  (00000000000280E6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         50be69ae
-  compressed size:                                1049 bytes
-  uncompressed size:                              3546 bytes
-  length of filename:                             36 characters
+  32-bit CRC value (hex):                         564a1eab
+  compressed size:                                735 bytes
+  uncompressed size:                              1799 bytes
+  length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -11074,36 +11112,72 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #302:
+Central directory entry #303:
 ---------------------------
 
-  ark_sdk_python/actions/ark_service_exec_action.py
+  ark_sdk_python/args/
+
+  offset of local header from start of archive:   164897
+                                                  (0000000000028421h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             20 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 7f 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #304:
+---------------------------
+
+  ark_sdk_python/args/ark_args_formatter.py
 
-  offset of local header from start of archive:   168619
-                                                  (00000000000292ABh) bytes
+  offset of local header from start of archive:   164975
+                                                  (000000000002846Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         bae7a058
-  compressed size:                                1152 bytes
-  uncompressed size:                              5109 bytes
-  length of filename:                             49 characters
+  32-bit CRC value (hex):                         d01e8893
+  compressed size:                                2189 bytes
+  uncompressed size:                              9204 bytes
+  length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -11111,36 +11185,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #303:
+Central directory entry #305:
 ---------------------------
 
-  ark_sdk_python/actions/ark_cache_action.py
+  ark_sdk_python/args/__init__.py
 
-  offset of local header from start of archive:   169878
-                                                  (0000000000029796h) bytes
+  offset of local header from start of archive:   167263
+                                                  (0000000000028D5Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         f5d8dbab
-  compressed size:                                790 bytes
-  uncompressed size:                              2392 bytes
-  length of filename:                             42 characters
+  32-bit CRC value (hex):                         3218a1fc
+  compressed size:                                154 bytes
+  uncompressed size:                              279 bytes
+  length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -11148,31 +11222,68 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #304:
+Central directory entry #306:
+---------------------------
+
+  ark_sdk_python/args/ark_pydantic_argparse.py
+
+  offset of local header from start of archive:   167506
+                                                  (0000000000028E52h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         982eeefd
+  compressed size:                                5065 bytes
+  uncompressed size:                              33777 bytes
+  length of filename:                             44 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 7f 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #307:
 ---------------------------
 
-  ark_sdk_python-1.0.6.dist-info/
+  ark_sdk_python-1.0.7.dist-info/
 
-  offset of local header from start of archive:   170768
-                                                  (0000000000029B10h) bytes
+  offset of local header from start of archive:   172673
+                                                  (000000000002A281h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -11184,36 +11295,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #305:
+Central directory entry #308:
 ---------------------------
 
-  ark_sdk_python-1.0.6.dist-info/RECORD
+  ark_sdk_python-1.0.7.dist-info/NOTICES.md
 
-  offset of local header from start of archive:   170857
-                                                  (0000000000029B69h) bytes
+  offset of local header from start of archive:   172762
+                                                  (000000000002A2DAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2016 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 2016 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 2016 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         8ec23bf3
-  compressed size:                                11073 bytes
-  uncompressed size:                              28913 bytes
-  length of filename:                             37 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         70a01143
+  compressed size:                                17235 bytes
+  uncompressed size:                              95918 bytes
+  length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -11221,36 +11332,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #306:
+Central directory entry #309:
 ---------------------------
 
-  ark_sdk_python-1.0.6.dist-info/entry_points.txt
+  ark_sdk_python-1.0.7.dist-info/METADATA
 
-  offset of local header from start of archive:   182025
-                                                  (000000000002C709h) bytes
+  offset of local header from start of archive:   190096
+                                                  (000000000002E690h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         7bcece10
-  compressed size:                                46 bytes
-  uncompressed size:                              47 bytes
-  length of filename:                             47 characters
+  32-bit CRC value (hex):                         e054d4d9
+  compressed size:                                5172 bytes
+  uncompressed size:                              17728 bytes
+  length of filename:                             39 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -11258,36 +11369,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #307:
+Central directory entry #310:
 ---------------------------
 
-  ark_sdk_python-1.0.6.dist-info/METADATA
+  ark_sdk_python-1.0.7.dist-info/WHEEL
 
-  offset of local header from start of archive:   182176
-                                                  (000000000002C7A0h) bytes
+  offset of local header from start of archive:   195365
+                                                  (000000000002FB25h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         85e8a91b
-  compressed size:                                5172 bytes
-  uncompressed size:                              17726 bytes
-  length of filename:                             39 characters
+  file last modified on (DOS date/time):          2024 Apr 3 13:44:54
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 local
+  file last modified on (UT extra field modtime): 2024 Apr 3 13:44:54 UTC
+  32-bit CRC value (hex):                         e495fd74
+  compressed size:                                84 bytes
+  uncompressed size:                              88 bytes
+  length of filename:                             36 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -11295,36 +11406,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #308:
+Central directory entry #311:
 ---------------------------
 
-  ark_sdk_python-1.0.6.dist-info/NOTICES.md
+  ark_sdk_python-1.0.7.dist-info/entry_points.txt
 
-  offset of local header from start of archive:   187445
-                                                  (000000000002DC35h) bytes
+  offset of local header from start of archive:   195543
+                                                  (000000000002FBD7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
   file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         70a01143
-  compressed size:                                17235 bytes
-  uncompressed size:                              95918 bytes
-  length of filename:                             41 characters
+  32-bit CRC value (hex):                         7bcece10
+  compressed size:                                46 bytes
+  uncompressed size:                              47 bytes
+  length of filename:                             47 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -11332,36 +11443,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #309:
+Central directory entry #312:
 ---------------------------
 
-  ark_sdk_python-1.0.6.dist-info/WHEEL
+  ark_sdk_python-1.0.7.dist-info/LICENSE.txt
 
-  offset of local header from start of archive:   204779
-                                                  (0000000000031FEBh) bytes
+  offset of local header from start of archive:   195694
+                                                  (000000000002FC6Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Mar 21 20:37:10
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 local
-  file last modified on (UT extra field modtime): 2024 Mar 21 20:37:09 UTC
-  32-bit CRC value (hex):                         e495fd74
-  compressed size:                                84 bytes
-  uncompressed size:                              88 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         02d5f591
+  compressed size:                                3958 bytes
+  uncompressed size:                              11358 bytes
+  length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -11369,36 +11480,36 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 7f 00 00 00.
 
   There is no file comment.
 
-Central directory entry #310:
+Central directory entry #313:
 ---------------------------
 
-  ark_sdk_python-1.0.6.dist-info/LICENSE.txt
+  ark_sdk_python-1.0.7.dist-info/RECORD
 
-  offset of local header from start of archive:   204957
-                                                  (000000000003209Dh) bytes
+  offset of local header from start of archive:   199752
+                                                  (0000000000030C48h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 local
-  file last modified on (UT extra field modtime): 1980 Jan 1 00:00:00 UTC
-  32-bit CRC value (hex):                         02d5f591
-  compressed size:                                3958 bytes
-  uncompressed size:                              11358 bytes
-  length of filename:                             42 characters
+  file last modified on (DOS date/time):          2016 Jan 1 00:00:00
+  file last modified on (UT extra field modtime): 2016 Jan 1 00:00:00 local
+  file last modified on (UT extra field modtime): 2016 Jan 1 00:00:00 UTC
+  32-bit CRC value (hex):                         edcec006
+  compressed size:                                11225 bytes
+  uncompressed size:                              29298 bytes
+  length of filename:                             37 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
```

## zipnote {}

```diff
@@ -1,931 +1,940 @@
 Filename: ark_sdk_python/
 Comment: 
 
+Filename: ark_sdk_python/examples/
+Comment: 
+
+Filename: ark_sdk_python/examples/session_monitoring_activites.py
+Comment: 
+
+Filename: ark_sdk_python/examples/create_dpa_db_environment.py
+Comment: 
+
 Filename: ark_sdk_python/ark_api.py
 Comment: 
 
 Filename: ark_sdk_python/auth/
 Comment: 
 
 Filename: ark_sdk_python/auth/__init__.py
 Comment: 
 
 Filename: ark_sdk_python/auth/ark_isp_auth.py
 Comment: 
 
-Filename: ark_sdk_python/auth/ark_auth.py
+Filename: ark_sdk_python/auth/identity/
 Comment: 
 
-Filename: ark_sdk_python/auth/identity/
+Filename: ark_sdk_python/auth/identity/ark_identity_fqdn_resolver.py
 Comment: 
 
 Filename: ark_sdk_python/auth/identity/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/auth/identity/ark_identity.py
+Filename: ark_sdk_python/auth/identity/ark_identity_service_user.py
 Comment: 
 
-Filename: ark_sdk_python/auth/identity/ark_identity_fqdn_resolver.py
+Filename: ark_sdk_python/auth/identity/ark_identity.py
 Comment: 
 
-Filename: ark_sdk_python/auth/identity/ark_identity_service_user.py
+Filename: ark_sdk_python/auth/ark_auth.py
 Comment: 
 
-Filename: ark_sdk_python/__init__.py
+Filename: ark_sdk_python/cli_services/
 Comment: 
 
-Filename: ark_sdk_python/services/
+Filename: ark_sdk_python/cli_services/dpa/
 Comment: 
 
-Filename: ark_sdk_python/services/__init__.py
+Filename: ark_sdk_python/cli_services/dpa/vm/
 Comment: 
 
-Filename: ark_sdk_python/services/ark_service.py
+Filename: ark_sdk_python/cli_services/dpa/vm/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/
+Filename: ark_sdk_python/cli_services/dpa/vm/ark_dpa_vm_policies_editor_service.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/sso/
+Filename: ark_sdk_python/cli_services/dpa/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/sso/__init__.py
+Filename: ark_sdk_python/cli_services/dpa/common/
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/sso/ark_dpa_sso_service.py
+Filename: ark_sdk_python/cli_services/dpa/common/ark_dpa_base_policies_editor_service.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/__init__.py
+Filename: ark_sdk_python/cli_services/dpa/common/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/ark_dpa_api.py
+Filename: ark_sdk_python/cli_services/dpa/db/
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/db/
+Filename: ark_sdk_python/cli_services/dpa/db/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/db/__init__.py
+Filename: ark_sdk_python/cli_services/dpa/db/ark_dpa_db_policies_editor_service.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/db/ark_dpa_db_service.py
+Filename: ark_sdk_python/cli_services/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/policies/
+Filename: ark_sdk_python/cli_services/ark_cli_api.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/policies/vm/
+Filename: ark_sdk_python/actions/
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/policies/vm/ark_dpa_vm_policies_service.py
+Filename: ark_sdk_python/actions/ark_action.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/policies/vm/__init__.py
+Filename: ark_sdk_python/actions/ark_service_exec_action.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/policies/__init__.py
+Filename: ark_sdk_python/actions/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/policies/db/
+Filename: ark_sdk_python/actions/ark_configure_action.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/policies/db/__init__.py
+Filename: ark_sdk_python/actions/ark_profiles_action.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/policies/db/ark_dpa_db_policies_service.py
+Filename: ark_sdk_python/actions/ark_cache_action.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/secrets/
+Filename: ark_sdk_python/actions/ark_exec_action.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/secrets/__init__.py
+Filename: ark_sdk_python/actions/ark_login_action.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/secrets/db/
+Filename: ark_sdk_python/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/secrets/db/__init__.py
+Filename: ark_sdk_python/common/
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/secrets/db/ark_dpa_db_secrets_service.py
+Filename: ark_sdk_python/common/ark_system_config.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/certificates/
+Filename: ark_sdk_python/common/ark_random_utils.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/certificates/__init__.py
+Filename: ark_sdk_python/common/env/
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/certificates/ark_dpa_certificates_service.py
+Filename: ark_sdk_python/common/env/ark_env_mapping.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/k8s/
+Filename: ark_sdk_python/common/env/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/k8s/__init__.py
+Filename: ark_sdk_python/common/ark_keyring.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/k8s/ark_dpa_k8s_service.py
+Filename: ark_sdk_python/common/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/workspaces/
+Filename: ark_sdk_python/common/ark_logger.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/workspaces/__init__.py
+Filename: ark_sdk_python/common/ark_client.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/workspaces/db/
+Filename: ark_sdk_python/common/isp/
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/workspaces/db/__init__.py
+Filename: ark_sdk_python/common/isp/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/services/dpa/workspaces/db/ark_dpa_db_workspace_service.py
+Filename: ark_sdk_python/common/isp/ark_isp_service_client.py
 Comment: 
 
-Filename: ark_sdk_python/services/sm/
+Filename: ark_sdk_python/common/ark_pollers.py
 Comment: 
 
-Filename: ark_sdk_python/services/sm/__init__.py
+Filename: ark_sdk_python/common/ark_async_client.py
 Comment: 
 
-Filename: ark_sdk_python/services/sm/ark_sm_service.py
+Filename: ark_sdk_python/common/ark_page.py
 Comment: 
 
-Filename: ark_sdk_python/common/
+Filename: ark_sdk_python/common/ark_async_request.py
 Comment: 
 
-Filename: ark_sdk_python/common/ark_async_client.py
+Filename: ark_sdk_python/services/
 Comment: 
 
-Filename: ark_sdk_python/common/__init__.py
+Filename: ark_sdk_python/services/dpa/
 Comment: 
 
-Filename: ark_sdk_python/common/ark_async_request.py
+Filename: ark_sdk_python/services/dpa/policies/
 Comment: 
 
-Filename: ark_sdk_python/common/ark_page.py
+Filename: ark_sdk_python/services/dpa/policies/vm/
 Comment: 
 
-Filename: ark_sdk_python/common/ark_logger.py
+Filename: ark_sdk_python/services/dpa/policies/vm/ark_dpa_vm_policies_service.py
 Comment: 
 
-Filename: ark_sdk_python/common/env/
+Filename: ark_sdk_python/services/dpa/policies/vm/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/common/env/__init__.py
+Filename: ark_sdk_python/services/dpa/policies/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/common/env/ark_env_mapping.py
+Filename: ark_sdk_python/services/dpa/policies/db/
 Comment: 
 
-Filename: ark_sdk_python/common/ark_client.py
+Filename: ark_sdk_python/services/dpa/policies/db/ark_dpa_db_policies_service.py
 Comment: 
 
-Filename: ark_sdk_python/common/ark_random_utils.py
+Filename: ark_sdk_python/services/dpa/policies/db/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/common/ark_keyring.py
+Filename: ark_sdk_python/services/dpa/certificates/
 Comment: 
 
-Filename: ark_sdk_python/common/ark_pollers.py
+Filename: ark_sdk_python/services/dpa/certificates/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/common/ark_system_config.py
+Filename: ark_sdk_python/services/dpa/certificates/ark_dpa_certificates_service.py
 Comment: 
 
-Filename: ark_sdk_python/common/isp/
+Filename: ark_sdk_python/services/dpa/workspaces/
 Comment: 
 
-Filename: ark_sdk_python/common/isp/__init__.py
+Filename: ark_sdk_python/services/dpa/workspaces/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/common/isp/ark_isp_service_client.py
+Filename: ark_sdk_python/services/dpa/workspaces/db/
 Comment: 
 
-Filename: ark_sdk_python/models/
+Filename: ark_sdk_python/services/dpa/workspaces/db/ark_dpa_db_workspace_service.py
 Comment: 
 
-Filename: ark_sdk_python/models/auth/
+Filename: ark_sdk_python/services/dpa/workspaces/db/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/auth/__init__.py
+Filename: ark_sdk_python/services/dpa/ark_dpa_api.py
 Comment: 
 
-Filename: ark_sdk_python/models/auth/ark_secret.py
+Filename: ark_sdk_python/services/dpa/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/auth/ark_auth_profile.py
+Filename: ark_sdk_python/services/dpa/k8s/
 Comment: 
 
-Filename: ark_sdk_python/models/auth/ark_token.py
+Filename: ark_sdk_python/services/dpa/k8s/ark_dpa_k8s_service.py
 Comment: 
 
-Filename: ark_sdk_python/models/auth/ark_auth_method.py
+Filename: ark_sdk_python/services/dpa/k8s/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/__init__.py
+Filename: ark_sdk_python/services/dpa/db/
 Comment: 
 
-Filename: ark_sdk_python/models/ark_exceptions.py
+Filename: ark_sdk_python/services/dpa/db/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/
+Filename: ark_sdk_python/services/dpa/db/ark_dpa_db_service.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/__init__.py
+Filename: ark_sdk_python/services/dpa/secrets/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/
+Filename: ark_sdk_python/services/dpa/secrets/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/sso/
+Filename: ark_sdk_python/services/dpa/secrets/db/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_oracle_wallet.py
+Filename: ark_sdk_python/services/dpa/secrets/db/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_rdp_file.py
+Filename: ark_sdk_python/services/dpa/secrets/db/ark_dpa_db_secrets_service.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/sso/__init__.py
+Filename: ark_sdk_python/services/dpa/sso/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_acquire_token_response.py
+Filename: ark_sdk_python/services/dpa/sso/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_client_certificate.py
+Filename: ark_sdk_python/services/dpa/sso/ark_dpa_sso_service.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_password.py
+Filename: ark_sdk_python/services/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/__init__.py
+Filename: ark_sdk_python/services/sm/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/db/
+Filename: ark_sdk_python/services/sm/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/db/__init__.py
+Filename: ark_sdk_python/services/sm/ark_sm_service.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_generated_assets.py
+Filename: ark_sdk_python/services/ark_service.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_generate_assets.py
+Filename: ark_sdk_python/ark.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_psql_execution.py
+Filename: ark_sdk_python/models/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_mysql_execution.py
+Filename: ark_sdk_python/models/auth/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_oracle_generate_assets.py
+Filename: ark_sdk_python/models/auth/ark_auth_profile.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_execution.py
+Filename: ark_sdk_python/models/auth/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/
+Filename: ark_sdk_python/models/auth/ark_token.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/
+Filename: ark_sdk_python/models/auth/ark_auth_method.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_providers.py
+Filename: ark_sdk_python/models/auth/ark_secret.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_add_policy.py
+Filename: ark_sdk_python/models/cli_services/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/__init__.py
+Filename: ark_sdk_python/models/cli_services/dpa/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy_list_item.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_authorization_rule.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/vm/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_protocol_type_serializer.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/vm/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_stats.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/vm/ark_dpa_vm_generate_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_update_policy.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_filter.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_workspace_type_serializer.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_base_generate_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_edit_policies.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_connection_data.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/__init__.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_policies_status.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_load_policies.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policies_stats.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_get_policies_status.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/__init__.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_commit_policies.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_user_data.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_view_policies.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policy.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_policies_diff.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policy_list_item.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_loaded_policies.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_connection_information.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_reset_policies.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_get_policy.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_remove_policies.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_delete_policy.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/db/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_update_policy.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/db/ark_dpa_db_generate_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_update_policy_status.py
+Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/db/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_rule_status.py
+Filename: ark_sdk_python/models/cli_services/dpa/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policies_filter.py
+Filename: ark_sdk_python/models/cli_services/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_add_policy.py
+Filename: ark_sdk_python/models/actions/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_authorization_rule.py
+Filename: ark_sdk_python/models/actions/ark_service_action_definition.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/
+Filename: ark_sdk_python/models/actions/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_stats.py
+Filename: ark_sdk_python/models/actions/services/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy_list_item.py
+Filename: ark_sdk_python/models/actions/services/ark_sm_exec_action_consts.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/__init__.py
+Filename: ark_sdk_python/models/actions/services/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_add_policy.py
+Filename: ark_sdk_python/models/actions/services/ark_dpa_exec_action_consts.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_authorization_rule.py
+Filename: ark_sdk_python/models/actions/ark_configure_action_consts.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy.py
+Filename: ark_sdk_python/models/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_workspace_type_serializer.py
+Filename: ark_sdk_python/models/common/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_providers.py
+Filename: ark_sdk_python/models/common/ark_application_code.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_connection_data.py
+Filename: ark_sdk_python/models/common/connections/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_filter.py
+Filename: ark_sdk_python/models/common/connections/ark_connection_command.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_update_policy.py
+Filename: ark_sdk_python/models/common/connections/connection_data/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/
+Filename: ark_sdk_python/models/common/connections/connection_data/ark_winrm_connection_data.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/__init__.py
+Filename: ark_sdk_python/models/common/connections/connection_data/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/
+Filename: ark_sdk_python/models/common/connections/connection_data/ark_ssh_connection_data.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secrets_stats.py
+Filename: ark_sdk_python/models/common/connections/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/__init__.py
+Filename: ark_sdk_python/models/common/connections/ark_connection_result.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_update_secret.py
+Filename: ark_sdk_python/models/common/connections/ark_connection_credentials.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secret_type.py
+Filename: ark_sdk_python/models/common/connections/ark_connection_details.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/secret_links/
+Filename: ark_sdk_python/models/common/ark_validations.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/secret_links/__init__.py
+Filename: ark_sdk_python/models/common/ark_os_type.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/secret_links/ark_dpa_db_pam_account_secret_link.py
+Filename: ark_sdk_python/models/common/ark_region.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_disable_secret.py
+Filename: ark_sdk_python/models/common/ark_async_status.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secret_metadata.py
+Filename: ark_sdk_python/models/common/ark_access_method.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_delete_secret.py
+Filename: ark_sdk_python/models/common/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_store_descriptor.py
+Filename: ark_sdk_python/models/common/ark_connection_method.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_store_type.py
+Filename: ark_sdk_python/models/common/ark_status_stats.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secrets_filter.py
+Filename: ark_sdk_python/models/common/ark_network_entity_type.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_enable_secret.py
+Filename: ark_sdk_python/models/common/isp/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_get_secret.py
+Filename: ark_sdk_python/models/common/isp/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_add_secret.py
+Filename: ark_sdk_python/models/common/isp/ark_platform_discovery_schemas.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/secrets_data/
+Filename: ark_sdk_python/models/common/identity/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/secrets_data/__init__.py
+Filename: ark_sdk_python/models/common/identity/ark_identity_common_schemas.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/secrets/db/secrets_data/ark_dpa_db_user_password_secret_data.py
+Filename: ark_sdk_python/models/common/identity/ark_identity_auth_schemas.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/certificates/
+Filename: ark_sdk_python/models/common/identity/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_update_certificate.py
+Filename: ark_sdk_python/models/common/identity/ark_identity_directory_schemas.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/certificates/__init__.py
+Filename: ark_sdk_python/models/common/aws/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_certificate.py
+Filename: ark_sdk_python/models/common/aws/ark_cfn_async_task.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_delete_certificate.py
+Filename: ark_sdk_python/models/common/aws/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_filter.py
+Filename: ark_sdk_python/models/common/ark_status.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_get_certificate.py
+Filename: ark_sdk_python/models/common/ark_protocol_type.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/k8s/
+Filename: ark_sdk_python/models/common/ark_connector_type.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/k8s/__init__.py
+Filename: ark_sdk_python/models/common/ark_async_task.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/k8s/ark_dpa_k8s_generate_kubeconfig.py
+Filename: ark_sdk_python/models/common/ark_workspace_type.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/
+Filename: ark_sdk_python/models/common/ark_async_request_settings.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/__init__.py
+Filename: ark_sdk_python/models/common/ark_counted_values.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/
+Filename: ark_sdk_python/models/ark_exceptions.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_tag.py
+Filename: ark_sdk_python/models/ark_profile.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_databases_filter.py
+Filename: ark_sdk_python/models/services/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/__init__.py
+Filename: ark_sdk_python/models/services/dpa/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_delete_database.py
+Filename: ark_sdk_python/models/services/dpa/policies/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_provider.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_get_database.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_warning.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_connection_data.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_databases_stats.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_workspace_type_serializer.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_update_database.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_filter.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_add_database.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_stats.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_platform_type_serializer.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_database_info.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_protocol_type_serializer.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_database.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_update_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/ark_service_config.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_authorization_rule.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_providers.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/ark_sm_session.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy_list_item.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/ark_sm_get_session.py
+Filename: ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_add_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/ark_sm_session_activity_filter.py
+Filename: ark_sdk_python/models/services/dpa/policies/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/ark_sm_workspace_type_serializer.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/__init__.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_rule_status.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/ark_sm_sessions_stats.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_connection_information.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/ark_sm_session_activity.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/ark_sm_sessions_filter.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_update_policy_status.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/ark_sm_get_session_activities.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/services/sm/ark_sm_protocol_type_serializer.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policy_list_item.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_delete_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_status.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_add_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_validations.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policies_stats.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_connector_type.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_update_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/__init__.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_authorization_rule.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_network_entity_type.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_get_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/aws/
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policies_filter.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/aws/__init__.py
+Filename: ark_sdk_python/models/services/dpa/policies/common/ark_dpa_user_data.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/aws/ark_cfn_async_task.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_status_stats.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_connection_data.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_protocol_type.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy_list_item.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_workspace_type.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_workspace_type_serializer.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_application_code.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_providers.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_async_task.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_update_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_connection_method.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_filter.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_async_status.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_add_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/connections/
+Filename: ark_sdk_python/models/services/dpa/policies/db/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/connections/__init__.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/connections/ark_connection_command.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_enums.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/connections/ark_connection_credentials.py
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_stats.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/connections/connection_data/
+Filename: ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_authorization_rule.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/connections/connection_data/__init__.py
+Filename: ark_sdk_python/models/services/dpa/certificates/
 Comment: 
 
-Filename: ark_sdk_python/models/common/connections/connection_data/ark_winrm_connection_data.py
+Filename: ark_sdk_python/models/services/dpa/certificates/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/connections/connection_data/ark_ssh_connection_data.py
+Filename: ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_update_certificate.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/connections/ark_connection_result.py
+Filename: ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_certificate.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/connections/ark_connection_details.py
+Filename: ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_get_certificate.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_region.py
+Filename: ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_filter.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_access_method.py
+Filename: ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_delete_certificate.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_counted_values.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_os_type.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/isp/
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/
 Comment: 
 
-Filename: ark_sdk_python/models/common/isp/__init__.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_databases_filter.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/isp/ark_platform_discovery_schemas.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_databases_stats.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/identity/
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_add_database.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/identity/ark_identity_directory_schemas.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_warning.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/identity/__init__.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_get_database.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/identity/ark_identity_common_schemas.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_database.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/identity/ark_identity_auth_schemas.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/common/ark_async_request_settings.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_database_info.py
 Comment: 
 
-Filename: ark_sdk_python/models/ark_profile.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_delete_database.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_platform_type_serializer.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/__init__.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_provider.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_tag.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/__init__.py
+Filename: ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_update_database.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/
+Filename: ark_sdk_python/models/services/dpa/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/vm/
+Filename: ark_sdk_python/models/services/dpa/k8s/
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/vm/__init__.py
+Filename: ark_sdk_python/models/services/dpa/k8s/ark_dpa_k8s_generate_kubeconfig.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/vm/ark_dpa_vm_generate_policy.py
+Filename: ark_sdk_python/models/services/dpa/k8s/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/__init__.py
+Filename: ark_sdk_python/models/services/dpa/db/
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/
+Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_proxy_fullchain_generate_assets.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_policies_diff.py
+Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_generated_assets.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/__init__.py
+Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_assets_type.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_base_generate_policy.py
+Filename: ark_sdk_python/models/services/dpa/db/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_remove_policies.py
+Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_execution.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_loaded_policies.py
+Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_oracle_generate_assets.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_view_policies.py
+Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_psql_execution.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_get_policies_status.py
+Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_mysql_execution.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_edit_policies.py
+Filename: ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_generate_assets.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_policies_status.py
+Filename: ark_sdk_python/models/services/dpa/secrets/
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_commit_policies.py
+Filename: ark_sdk_python/models/services/dpa/secrets/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_reset_policies.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/common/ark_dpa_load_policies.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secret_metadata.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/db/
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secret_type.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/db/__init__.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_add_secret.py
 Comment: 
 
-Filename: ark_sdk_python/models/cli_services/dpa/policies_editor/db/ark_dpa_db_generate_policy.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/secret_links/
 Comment: 
 
-Filename: ark_sdk_python/models/ark_model.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/secret_links/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/actions/
+Filename: ark_sdk_python/models/services/dpa/secrets/db/secret_links/ark_dpa_db_pam_account_secret_link.py
 Comment: 
 
-Filename: ark_sdk_python/models/actions/__init__.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_delete_secret.py
 Comment: 
 
-Filename: ark_sdk_python/models/actions/ark_service_action_definition.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_update_secret.py
 Comment: 
 
-Filename: ark_sdk_python/models/actions/services/
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secrets_stats.py
 Comment: 
 
-Filename: ark_sdk_python/models/actions/services/__init__.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_get_secret.py
 Comment: 
 
-Filename: ark_sdk_python/models/actions/services/ark_sm_exec_action_consts.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/models/actions/services/ark_dpa_exec_action_consts.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_enable_secret.py
 Comment: 
 
-Filename: ark_sdk_python/models/actions/ark_configure_action_consts.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_store_descriptor.py
 Comment: 
 
-Filename: ark_sdk_python/examples/
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_store_type.py
 Comment: 
 
-Filename: ark_sdk_python/examples/session_monitoring_activites.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_secrets_filter.py
 Comment: 
 
-Filename: ark_sdk_python/examples/create_dpa_db_environment.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_disable_secret.py
 Comment: 
 
-Filename: ark_sdk_python/args/
+Filename: ark_sdk_python/models/services/dpa/secrets/db/secrets_data/
 Comment: 
 
-Filename: ark_sdk_python/args/__init__.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/secrets_data/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/args/ark_pydantic_argparse.py
+Filename: ark_sdk_python/models/services/dpa/secrets/db/secrets_data/ark_dpa_db_user_password_secret_data.py
 Comment: 
 
-Filename: ark_sdk_python/args/ark_args_formatter.py
+Filename: ark_sdk_python/models/services/dpa/sso/
 Comment: 
 
-Filename: ark_sdk_python/cli_services/
+Filename: ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_client_certificate.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/__init__.py
+Filename: ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_password.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/
+Filename: ark_sdk_python/models/services/dpa/sso/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/vm/
+Filename: ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_oracle_wallet.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/vm/__init__.py
+Filename: ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_acquire_token_response.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/vm/ark_dpa_vm_policies_editor_service.py
+Filename: ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_rdp_file.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/__init__.py
+Filename: ark_sdk_python/models/services/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/common/
+Filename: ark_sdk_python/models/services/ark_service_config.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/common/__init__.py
+Filename: ark_sdk_python/models/services/sm/
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/common/ark_dpa_base_policies_editor_service.py
+Filename: ark_sdk_python/models/services/sm/ark_sm_get_session.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/db/
+Filename: ark_sdk_python/models/services/sm/ark_sm_workspace_type_serializer.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/db/__init__.py
+Filename: ark_sdk_python/models/services/sm/ark_sm_protocol_type_serializer.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/dpa/db/ark_dpa_db_policies_editor_service.py
+Filename: ark_sdk_python/models/services/sm/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/cli_services/ark_cli_api.py
+Filename: ark_sdk_python/models/services/sm/ark_sm_session.py
 Comment: 
 
-Filename: ark_sdk_python/ark.py
+Filename: ark_sdk_python/models/services/sm/ark_sm_get_session_activities.py
 Comment: 
 
-Filename: ark_sdk_python/actions/
+Filename: ark_sdk_python/models/services/sm/ark_sm_sessions_stats.py
 Comment: 
 
-Filename: ark_sdk_python/actions/ark_login_action.py
+Filename: ark_sdk_python/models/services/sm/ark_sm_sessions_filter.py
 Comment: 
 
-Filename: ark_sdk_python/actions/ark_profiles_action.py
+Filename: ark_sdk_python/models/services/sm/ark_sm_session_activity.py
 Comment: 
 
-Filename: ark_sdk_python/actions/__init__.py
+Filename: ark_sdk_python/models/services/sm/ark_sm_session_activity_filter.py
 Comment: 
 
-Filename: ark_sdk_python/actions/ark_exec_action.py
+Filename: ark_sdk_python/models/ark_model.py
 Comment: 
 
-Filename: ark_sdk_python/actions/ark_configure_action.py
+Filename: ark_sdk_python/args/
 Comment: 
 
-Filename: ark_sdk_python/actions/ark_action.py
+Filename: ark_sdk_python/args/ark_args_formatter.py
 Comment: 
 
-Filename: ark_sdk_python/actions/ark_service_exec_action.py
+Filename: ark_sdk_python/args/__init__.py
 Comment: 
 
-Filename: ark_sdk_python/actions/ark_cache_action.py
+Filename: ark_sdk_python/args/ark_pydantic_argparse.py
 Comment: 
 
-Filename: ark_sdk_python-1.0.6.dist-info/
+Filename: ark_sdk_python-1.0.7.dist-info/
 Comment: 
 
-Filename: ark_sdk_python-1.0.6.dist-info/RECORD
+Filename: ark_sdk_python-1.0.7.dist-info/NOTICES.md
 Comment: 
 
-Filename: ark_sdk_python-1.0.6.dist-info/entry_points.txt
+Filename: ark_sdk_python-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: ark_sdk_python-1.0.6.dist-info/METADATA
+Filename: ark_sdk_python-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: ark_sdk_python-1.0.6.dist-info/NOTICES.md
+Filename: ark_sdk_python-1.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ark_sdk_python-1.0.6.dist-info/WHEEL
+Filename: ark_sdk_python-1.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: ark_sdk_python-1.0.6.dist-info/LICENSE.txt
+Filename: ark_sdk_python-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ark_sdk_python/auth/ark_auth.py

```diff
@@ -176,22 +176,25 @@
             if self.__token and self.__token.expires_in.replace(tzinfo=None) <= datetime.now():
                 self.__token = None
             else:
                 self._logger.info('Loaded token from cache successfully')
             return self.__token != None
         return False
 
-    def load_authentication(self, profile: Optional[ArkProfile] = None, refresh_auth: bool = False) -> Optional[ArkToken]:
+    def load_authentication(
+        self, profile: Optional[ArkProfile] = None, refresh_auth: bool = False, grace_seconds: Optional[int] = None
+    ) -> Optional[ArkToken]:
         """
         Loads and returns the authentication token from the cache, if it exists.
         If specified, the method also attempts to refresh the token as needed.
 
         Args:
             profile (Optional[ArkProfile], optional): _description_. Defaults to None.
             refresh_auth (bool, optional): _description_. Defaults to False.
+            grace_seconds (Optional[int], optional): try to refresh in case there is less than grace_seconds until expired. Defaults to None.
 
         Returns:
             Optional[ArkToken]: _description_
         """
         self._logger.info(f'Trying to load [{self.authenticator_name()}] authentication')
         if not profile:
             if self._active_profile:
@@ -204,19 +207,16 @@
         if auth_profile:
             self._logger.info(
                 f'Loading authentication for profile [{profile.profile_name}] and auth profile [{self.authenticator_name()}] of type [{auth_profile.auth_method.value}]'
             )
             if self._cache_keyring:
                 self.__token = self._cache_keyring.load_token(profile, self._resolve_cache_postfix(auth_profile))
             if refresh_auth:
-                if (
-                    self.__token
-                    and self.__token.expires_in.replace(tzinfo=None) - timedelta(seconds=DEFAULT_EXPIRATION_GRACE_DELTA_SECONDS)
-                    > datetime.now()
-                ):
+                grace_seconds = grace_seconds if grace_seconds is not None else DEFAULT_EXPIRATION_GRACE_DELTA_SECONDS
+                if self.__token and self.__token.expires_in.replace(tzinfo=None) - timedelta(seconds=grace_seconds) > datetime.now():
                     self._logger.info('Token did not pass grace expiration, no need to refresh')
                 else:
                     self._logger.info('Trying to refresh token authentication')
                     self.__token = self._perform_refresh_authentication(profile, auth_profile, self.__token)
                     if self.__token and self.__token.expires_in.replace(tzinfo=None) > datetime.now():
                         self._logger.info('Token refreshed')
                     if self.__token and self._cache_authentication and self._cache_keyring:
```

## ark_sdk_python/services/dpa/db/ark_dpa_db_service.py

```diff
@@ -17,17 +17,19 @@
 from ark_sdk_python.common.isp import ArkISPServiceClient
 from ark_sdk_python.models import ArkServiceException
 from ark_sdk_python.models.common import running_os
 from ark_sdk_python.models.common.ark_connection_method import ArkConnectionMethod
 from ark_sdk_python.models.services import ArkServiceConfig
 from ark_sdk_python.models.services.dpa.db import (
     ArkDPADBAssetsResponseFormat,
+    ArkDPADBAssetsType,
     ArkDPADBGeneratedAssets,
     ArkDPADBMysqlExecution,
     ArkDPADBOracleGenerateAssets,
+    ArkDPADBProxyFullchainGenerateAssets,
     ArkDPADBPsqlExecution,
 )
 from ark_sdk_python.models.services.dpa.sso import ArkDPASSOGetShortLivedPassword
 from ark_sdk_python.models.services.dpa.workspaces.db.ark_dpa_db_provider import ArkDPADBDatabaseFamilyType
 from ark_sdk_python.services.ark_service import ArkService
 from ark_sdk_python.services.dpa.sso.ark_dpa_sso_service import ArkDPASSOService
 
@@ -140,30 +142,36 @@
         try:
             self.__execute(execution_action)
         finally:
             os.unlink(temp_cnf_login)
 
     def __generate_assets(
         self,
-        resource_type: ArkDPADBDatabaseFamilyType,
+        asset_type: ArkDPADBAssetsType,
         connection_method: ArkConnectionMethod,
         response_format: ArkDPADBAssetsResponseFormat,
-        include_sso: bool,
-        generation_hints: Dict[str, Any],
+        generation_hints: Optional[Dict[str, Any]] = None,
+        include_sso: Optional[bool] = None,
+        resource_type: Optional[ArkDPADBDatabaseFamilyType] = None,
     ) -> ArkDPADBGeneratedAssets:
+        body = {
+            'asset_type': asset_type,
+            'os_type': running_os().value,
+            'connection_method': connection_method.value,
+            'response_format': response_format.value,
+        }
+        if generation_hints:
+            body['generation_hints'] = generation_hints
+        if include_sso is not None:
+            body['include_sso'] = include_sso
+        if resource_type:
+            body['resource_type'] = resource_type.value
         resp: Response = self.__client.post(
             ASSETS_API,
-            json={
-                'resource_type': resource_type.value,
-                'os_type': running_os().value,
-                'connection_method': connection_method.value,
-                'response_format': response_format.value,
-                'include_sso': include_sso,
-                'generation_hints': generation_hints,
-            },
+            json=body,
         )
         if resp.status_code == HTTPStatus.OK:
             try:
                 if response_format == ArkDPADBAssetsResponseFormat.RAW:
                     return resp.text
                 return ArkDPADBGeneratedAssets.parse_obj(resp.json())
             except (ValidationError, JSONDecodeError) as ex:
@@ -179,30 +187,54 @@
             generate_oracle_assets (ArkDPADBOracleGenerateAssets): _description_
 
         Raises:
             ArkServiceException: _description_
         """
         self._logger.info('Generating oracle tns names')
         assets_data = self.__generate_assets(
-            ArkDPADBDatabaseFamilyType.Oracle,
-            generate_oracle_assets.connection_method,
-            generate_oracle_assets.response_format,
-            generate_oracle_assets.include_sso,
-            {'folder': generate_oracle_assets.folder},
+            asset_type=ArkDPADBAssetsType.OracleTNSAssets,
+            connection_method=generate_oracle_assets.connection_method,
+            response_format=generate_oracle_assets.response_format,
+            generation_hints={'folder': generate_oracle_assets.folder},
+            include_sso=generate_oracle_assets.include_sso,
+            resource_type=ArkDPADBDatabaseFamilyType.Oracle,
         )
         if isinstance(assets_data, ArkDPADBGeneratedAssets):
             assets_data = assets_data.assets['generated_assets']
         assets_data = base64.b64decode(assets_data)
         if not os.path.exists(generate_oracle_assets.folder):
             os.makedirs(generate_oracle_assets.folder)
         if not generate_oracle_assets.unzip:
             with open(f'{generate_oracle_assets.folder}{os.path.sep}oracle_assets.zip', 'wb') as file_handle:
                 file_handle.write(assets_data)
         else:
             assets_bytes = BytesIO(assets_data)
             with zipfile.ZipFile(assets_bytes, 'r') as zipf:
                 zipf.extractall(generate_oracle_assets.folder)
 
+    def generate_proxy_fullchain(self, generate_proxy_fullchain: ArkDPADBProxyFullchainGenerateAssets) -> None:
+        """
+        Generates the proxy fullchain certificates for full certificate validation.
+
+        Args:
+            generate_proxy_fullchain (ArkDPADBProxyFullchainGenerateAssets): _description_
+
+        Raises:
+            ArkServiceException: _description_
+        """
+        self._logger.info('Generating proxy fullchain')
+        assets_data = self.__generate_assets(
+            asset_type=ArkDPADBAssetsType.ProxyFullChain,
+            connection_method=generate_proxy_fullchain.connection_method,
+            response_format=generate_proxy_fullchain.response_format,
+        )
+        if isinstance(assets_data, ArkDPADBGeneratedAssets):
+            assets_data = assets_data.assets['generated_assets']
+        if not os.path.exists(generate_proxy_fullchain.folder):
+            os.makedirs(generate_proxy_fullchain.folder)
+        with open(f'{generate_proxy_fullchain.folder}{os.path.sep}proxy_fullchain.pem', 'w', encoding='utf-8') as file_handle:
+            file_handle.write(assets_data)
+
     @staticmethod
     @overrides
     def service_config() -> ArkServiceConfig:
         return SERVICE_CONFIG
```

## ark_sdk_python/models/services/dpa/sso/__init__.py

```diff
@@ -1,17 +1,21 @@
 from ark_sdk_python.models.services.dpa.sso.ark_dpa_sso_acquire_token_response import ArkDPASSOAcquireTokenResponse
-from ark_sdk_python.models.services.dpa.sso.ark_dpa_sso_get_short_lived_client_certificate import ArkDPASSOGetShortLivedClientCertificate
+from ark_sdk_python.models.services.dpa.sso.ark_dpa_sso_get_short_lived_client_certificate import (
+    ArkDPASSOGetShortLivedClientCertificate,
+    ArkDPASSOShortLiveClientCertificateFormat,
+)
 from ark_sdk_python.models.services.dpa.sso.ark_dpa_sso_get_short_lived_oracle_wallet import (
     ArkDPASSOGetShortLivedOracleWallet,
     ArkDPASSOShortLivedOracleWalletType,
 )
 from ark_sdk_python.models.services.dpa.sso.ark_dpa_sso_get_short_lived_password import ArkDPASSOGetShortLivedPassword
 from ark_sdk_python.models.services.dpa.sso.ark_dpa_sso_get_short_lived_rdp_file import ArkDPASSOGetShortLivedRDPFile
 
 __all__ = [
     'ArkDPASSOGetShortLivedClientCertificate',
+    'ArkDPASSOShortLiveClientCertificateFormat',
     'ArkDPASSOGetShortLivedPassword',
     'ArkDPASSOGetShortLivedOracleWallet',
     'ArkDPASSOShortLivedOracleWalletType',
     'ArkDPASSOAcquireTokenResponse',
     'ArkDPASSOGetShortLivedRDPFile',
 ]
```

## ark_sdk_python/models/services/dpa/db/__init__.py

```diff
@@ -1,16 +1,20 @@
+from ark_sdk_python.models.services.dpa.db.ark_dpa_db_assets_type import ArkDPADBAssetsType
 from ark_sdk_python.models.services.dpa.db.ark_dpa_db_base_execution import ArkDPADBBaseExecution
 from ark_sdk_python.models.services.dpa.db.ark_dpa_db_base_generate_assets import ArkDPADBAssetsResponseFormat, ArkDPADBBaseGenerateAssets
 from ark_sdk_python.models.services.dpa.db.ark_dpa_db_generated_assets import ArkDPADBGeneratedAssets
 from ark_sdk_python.models.services.dpa.db.ark_dpa_db_mysql_execution import ArkDPADBMysqlExecution
 from ark_sdk_python.models.services.dpa.db.ark_dpa_db_oracle_generate_assets import ArkDPADBOracleGenerateAssets
+from ark_sdk_python.models.services.dpa.db.ark_dpa_db_proxy_fullchain_generate_assets import ArkDPADBProxyFullchainGenerateAssets
 from ark_sdk_python.models.services.dpa.db.ark_dpa_db_psql_execution import ArkDPADBPsqlExecution
 
 __all__ = [
     'ArkDPADBBaseExecution',
     'ArkDPADBPsqlExecution',
     'ArkDPADBMysqlExecution',
     'ArkDPADBBaseGenerateAssets',
     'ArkDPADBAssetsResponseFormat',
     'ArkDPADBOracleGenerateAssets',
     'ArkDPADBGeneratedAssets',
+    'ArkDPADBProxyFullchainGenerateAssets',
+    'ArkDPADBAssetsType',
 ]
```

## ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_generate_assets.py

```diff
@@ -14,8 +14,8 @@
 class ArkDPADBBaseGenerateAssets(ArkModel):
     connection_method: ArkConnectionMethod = Field(
         description='Whether to generate assets for standing or dynamic access', default=ArkConnectionMethod.Standing
     )
     response_format: ArkDPADBAssetsResponseFormat = Field(
         description='In which format to return the assets', default=ArkDPADBAssetsResponseFormat.RAW
     )
-    include_sso: bool = Field(description='Whether to generate the asset with SSO details', default=True)
+    folder: str = Field(description='Where to output the assets')
```

## ark_sdk_python/models/services/dpa/db/ark_dpa_db_oracle_generate_assets.py

```diff
@@ -1,8 +1,8 @@
 from pydantic import Field
 
 from ark_sdk_python.models.services.dpa.db.ark_dpa_db_base_generate_assets import ArkDPADBBaseGenerateAssets
 
 
 class ArkDPADBOracleGenerateAssets(ArkDPADBBaseGenerateAssets):
-    folder: str = Field(description='Where to output the assets')
     unzip: bool = Field(description='Whether to save zipped or not', default=True)
+    include_sso: bool = Field(description='Whether to generate the asset with SSO details', default=True)
```

## ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_providers.py

```diff
@@ -26,24 +26,19 @@
     vnet_ids: Optional[List[str]] = Field(description='Vnets Azure Filter')
     subscriptions: Optional[List[str]] = Field(description='Subscriptions Azure Filter')
 
 
 class ArkDPAVMGCPProviderData(ArkCamelizedModel):
     provider_name: Literal['GCP'] = Field(alias='providerName', default='GCP', exclude=True)
     regions: Optional[List[str]] = Field(description='Regions GCP Filter')
-    tags: Optional[List[Dict]] = Field(description='Tags GCP Filter')
-    network_ids: Optional[List[str]] = Field(description='Networks GCP Filter')
+    labels: Optional[List[Dict]] = Field(description='Labels GCP Filter')
+    vpc_Ids: Optional[List[str]] = Field(description='Vpc GCP Filter')
     projects: Optional[List[str]] = Field(description='Projects GCP Filter')
 
 
-class ArkDPAVMFQDNRulesConjunction(str, Enum):
-    AND = 'AND'
-    OR = 'OR'
-
-
 class ArkDPAVMFQDNOperator(str, Enum):
     EXACTLY = 'EXACTLY'
     WILDCARD = 'WILDCARD'
     PREFIX = 'PREFIX'
     SUFFIX = 'SUFFIX'
     CONTAINS = 'CONTAINS'
 
@@ -52,15 +47,14 @@
     operator: Optional[ArkDPAVMFQDNOperator] = Field(description='Operator to perform on the FQDN')
     computername_pattern: Optional[str] = Field(description='The pattern in relations to the operator')
     domain: Optional[str] = Field(description='The domain in which to execute the operator on the pattern')
 
 
 class ArkDPAVMOnPremProviderData(ArkCamelizedModel):
     provider_name: Literal['OnPrem'] = Field(alias='providerName', default='OnPrem', exclude=True)
-    fqdn_rules_conjunction: Optional[ArkDPAVMFQDNRulesConjunction] = Field(description='Rules relationships')
     fqdn_rules: Optional[List[ArkDPAVMFQDNRule]] = Field(description='List of FQDN rules applied to the connection')
 
 
 ArkDPAVMProvider = Annotated[
     Union[ArkDPAVMAWSProviderData, ArkDPAVMAzureProviderData, ArkDPAVMGCPProviderData, ArkDPAVMOnPremProviderData],
     Field(discriminator='provider_name'),
 ]
```

## ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_add_policy.py

```diff
@@ -21,11 +21,14 @@
     )
 
     # pylint: disable=no-self-use,no-self-argument
     @validator('providers_data', pre=True)
     def validate_providers_data(cls, val):
         if val is not None:
             for k in val.keys():
-                val[k]['providerName'] = serialize_dpa_vm_policies_workspace_type(ArkWorkspaceType(k))
+                if isinstance(val[k], dict):
+                    val[k]['providerName'] = serialize_dpa_vm_policies_workspace_type(ArkWorkspaceType(k))
+                else:
+                    val[k].provider_name = serialize_dpa_vm_policies_workspace_type(ArkWorkspaceType(k))
                 if ArkWorkspaceType(k) not in [ArkWorkspaceType.AWS, ArkWorkspaceType.AZURE, ArkWorkspaceType.GCP, ArkWorkspaceType.ONPREM]:
                     raise ValueError('Invalid Platform / Workspace Type')
         return val
```

## ark_sdk_python/models/services/dpa/policies/vm/__init__.py

```diff
@@ -22,15 +22,14 @@
 from ark_sdk_python.models.services.dpa.policies.vm.ark_dpa_vm_policy import ArkDPAVMPolicy
 from ark_sdk_python.models.services.dpa.policies.vm.ark_dpa_vm_policy_list_item import ArkDPAVMPolicyListItem
 from ark_sdk_python.models.services.dpa.policies.vm.ark_dpa_vm_providers import (
     ArkDPAVMAWSProviderData,
     ArkDPAVMAzureProviderData,
     ArkDPAVMFQDNOperator,
     ArkDPAVMFQDNRule,
-    ArkDPAVMFQDNRulesConjunction,
     ArkDPAVMGCPProviderData,
     ArkDPAVMKeyValTag,
     ArkDPAVMOnPremProviderData,
     ArkDPAVMProvider,
     ArkDPAVMProvidersDict,
 )
 from ark_sdk_python.models.services.dpa.policies.vm.ark_dpa_vm_update_policy import ArkDPAVMUpdatePolicy
@@ -52,14 +51,13 @@
     'ArkDPAVMRDPLocalEphemeralUserConnectionData',
     'ArkDPAVMAWSProviderData',
     'ArkDPAVMAzureProviderData',
     'ArkDPAVMProvider',
     'ArkDPAVMProvidersDict',
     'ArkDPAVMFQDNOperator',
     'ArkDPAVMFQDNRule',
-    'ArkDPAVMFQDNRulesConjunction',
     'ArkDPAVMGCPProviderData',
     'ArkDPAVMKeyValTag',
     'ArkDPAVMOnPremProviderData',
     'serialize_dpa_vm_policies_protocol_type',
     'serialize_dpa_vm_policies_workspace_type',
 ]
```

## ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_update_policy.py

```diff
@@ -16,11 +16,14 @@
     user_access_rules: Optional[List[ArkDPAVMAuthorizationRule]] = Field(description='New access rules to update')
 
     # pylint: disable=no-self-use,no-self-argument
     @validator('providers_data', pre=True)
     def validate_providers_data(cls, val):
         if val is not None:
             for k in val.keys():
-                val[k]['providerName'] = serialize_dpa_vm_policies_workspace_type(ArkWorkspaceType(k))
+                if isinstance(val[k], dict):
+                    val[k]['providerName'] = serialize_dpa_vm_policies_workspace_type(ArkWorkspaceType(k))
+                else:
+                    val[k].provider_name = serialize_dpa_vm_policies_workspace_type(ArkWorkspaceType(k))
                 if ArkWorkspaceType(k) not in [ArkWorkspaceType.AWS, ArkWorkspaceType.AZURE, ArkWorkspaceType.GCP, ArkWorkspaceType.ONPREM]:
                     raise ValueError('Invalid Platform / Workspace Type')
         return val
```

## ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_workspace_type_serializer.py

```diff
@@ -5,10 +5,12 @@
 def serialize_dpa_vm_policies_workspace_type(ws_type: ArkWorkspaceType) -> str:
     if isinstance(ws_type, str):
         ws_type = ArkWorkspaceType(ws_type)
     if ws_type == ArkWorkspaceType.AWS:
         return 'AWS'
     elif ws_type == ArkWorkspaceType.AZURE:
         return 'Azure'
+    elif ws_type == ArkWorkspaceType.GCP:
+        return 'GCP'
     elif ws_type == ArkWorkspaceType.ONPREM:
         return 'OnPrem'
     raise ArkException('Invalid VM Policies Workspace Type')
```

## ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy.py

```diff
@@ -16,11 +16,14 @@
     user_access_rules: Optional[List[ArkDPAVMAuthorizationRule]] = Field(description='Authorization rules of the policy')
 
     # pylint: disable=no-self-use,no-self-argument
     @validator('providers_data', pre=True)
     def validate_providers_data(cls, val):
         if val is not None:
             for k in val.keys():
-                val[k]['providerName'] = serialize_dpa_vm_policies_workspace_type(ArkWorkspaceType(k))
+                if isinstance(val[k], dict):
+                    val[k]['providerName'] = serialize_dpa_vm_policies_workspace_type(ArkWorkspaceType(k))
+                else:
+                    val[k].provider_name = serialize_dpa_vm_policies_workspace_type(ArkWorkspaceType(k))
                 if ArkWorkspaceType(k) not in [ArkWorkspaceType.AWS, ArkWorkspaceType.AZURE, ArkWorkspaceType.GCP, ArkWorkspaceType.ONPREM]:
                     raise ValueError('Invalid Platform / Workspace Type')
         return val
```

## ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_stats.py

```diff
@@ -15,10 +15,12 @@
         for k in val.keys():
             if ArkWorkspaceType(k) not in [
                 ArkWorkspaceType.MYSQL,
                 ArkWorkspaceType.MARIADB,
                 ArkWorkspaceType.POSTGRES,
                 ArkWorkspaceType.MSSQL,
                 ArkWorkspaceType.ORACLE,
+                ArkWorkspaceType.MONGO,
+                ArkWorkspaceType.DB2,
             ]:
                 raise ValueError('Invalid Database Type')
         return val
```

## ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy_list_item.py

```diff
@@ -17,10 +17,12 @@
             for plat in val:
                 if ArkWorkspaceType(plat) not in [
                     ArkWorkspaceType.MYSQL,
                     ArkWorkspaceType.MARIADB,
                     ArkWorkspaceType.POSTGRES,
                     ArkWorkspaceType.MSSQL,
                     ArkWorkspaceType.ORACLE,
+                    ArkWorkspaceType.MONGO,
+                    ArkWorkspaceType.DB2,
                 ]:
                     raise ValueError('Invalid Database Type')
         return val
```

## ark_sdk_python/models/services/dpa/policies/db/__init__.py

```diff
@@ -5,28 +5,32 @@
 )
 from ark_sdk_python.models.services.dpa.policies.db.ark_dpa_db_connection_data import (
     ArkDPADBAppliedTo,
     ArkDPADBBaseAuth,
     ArkDPADBConnectAs,
     ArkDPADBLDAPAuth,
     ArkDPADBLocalDBAuth,
+    ArkDPADBMongoDBAuth,
     ArkDPADBOracleDBAuth,
     ArkDPADBResourceIdentifierType,
 )
+from ark_sdk_python.models.services.dpa.policies.db.ark_dpa_db_enums import ArkDPADBMongoDatabaseBuiltinRole, ArkDPADBMongoGlobalBuiltinRole
 from ark_sdk_python.models.services.dpa.policies.db.ark_dpa_db_policies_filter import ArkDPADBPoliciesFilter
 from ark_sdk_python.models.services.dpa.policies.db.ark_dpa_db_policies_stats import ArkDPADBPoliciesStats
 from ark_sdk_python.models.services.dpa.policies.db.ark_dpa_db_policies_workspace_type_serializer import (
     serialize_dpa_db_policies_workspace_type,
 )
 from ark_sdk_python.models.services.dpa.policies.db.ark_dpa_db_policy import ArkDPADBPolicy
 from ark_sdk_python.models.services.dpa.policies.db.ark_dpa_db_policy_list_item import ArkDPADBPolicyListItem
 from ark_sdk_python.models.services.dpa.policies.db.ark_dpa_db_providers import (
     ArkDPADB,
+    ArkDPADBDb2,
     ArkDPADBIdentifiers,
     ArkDPADBMariaDB,
+    ArkDPADBMongo,
     ArkDPADBMSSQL,
     ArkDPADBMySQL,
     ArkDPADBOracle,
     ArkDPADBOracleResource,
     ArkDPADBPostgres,
     ArkDPADBProvidersData,
 )
@@ -38,24 +42,29 @@
     'ArkDPADBConnectionInformation',
     'ArkDPADBBaseAuth',
     'ArkDPADBAppliedTo',
     'ArkDPADBConnectAs',
     'ArkDPADBLDAPAuth',
     'ArkDPADBLocalDBAuth',
     'ArkDPADBOracleDBAuth',
+    'ArkDPADBMongoDBAuth',
     'ArkDPADBResourceIdentifierType',
     'ArkDPADBPoliciesFilter',
     'ArkDPADBPoliciesStats',
     'serialize_dpa_db_policies_workspace_type',
     'ArkDPADBPolicyListItem',
     'ArkDPADBPolicy',
     'ArkDPADB',
     'ArkDPADBIdentifiers',
     'ArkDPADBMariaDB',
     'ArkDPADBMySQL',
     'ArkDPADBMSSQL',
     'ArkDPADBOracleResource',
     'ArkDPADBPostgres',
     'ArkDPADBOracle',
+    'ArkDPADBMongo',
     'ArkDPADBProvidersData',
     'ArkDPADBUpdatePolicy',
+    'ArkDPADBMongoDatabaseBuiltinRole',
+    'ArkDPADBMongoGlobalBuiltinRole',
+    'ArkDPADBDb2',
 ]
```

## ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_workspace_type_serializer.py

```diff
@@ -11,8 +11,12 @@
         return 'MySQL'
     elif ws_type == ArkWorkspaceType.MARIADB:
         return 'MariaDB'
     elif ws_type == ArkWorkspaceType.POSTGRES:
         return 'Postgres'
     elif ws_type == ArkWorkspaceType.ORACLE:
         return 'Oracle'
+    elif ws_type == ArkWorkspaceType.MONGO:
+        return 'Mongo'
+    elif ws_type == ArkWorkspaceType.DB2:
+        return 'Db2'
     raise ArkException('Invalid DB Policies Workspace Type')
```

## ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_providers.py

```diff
@@ -25,14 +25,22 @@
     pass
 
 
 class ArkDPADBPostgres(ArkDPADBIdentifiers):
     pass
 
 
+class ArkDPADBMongo(ArkDPADBIdentifiers):
+    pass
+
+
+class ArkDPADBDb2(ArkDPADBIdentifiers):
+    pass
+
+
 class ArkDPADBOracleResource(ArkCamelizedModel):
     name: str = Field(description='Name of the oracle db resource / asset')
     services: Optional[List[str]] = Field(description='Oracle services in the database')
 
 
 class ArkDPADBOracle(ArkDPADB):
     resources: List[Union[str, ArkDPADBOracleResource]] = Field(description='List of oracle resources / assets for the policy')
@@ -40,14 +48,16 @@
 
 class ArkDPADBProvidersData(ArkCamelizedModel):
     mssql: Optional[ArkDPADBMSSQL] = Field(description='MSSQL related resources')
     mysql: Optional[ArkDPADBMySQL] = Field(description='MySQL related resources')
     mariadb: Optional[ArkDPADBMariaDB] = Field(description='MariaDB related resources')
     postgres: Optional[ArkDPADBPostgres] = Field(description='PostgreSQL related resources')
     oracle: Optional[ArkDPADBOracle] = Field(description='Oracle related resources')
+    mongo: Optional[ArkDPADBMongo] = Field(description='Mongo related resources')
+    db2: Optional[ArkDPADBDb2] = Field(description='Db2 related resources')
 
     @root_validator
     @classmethod
     def validate_min_providers(cls, data: Dict) -> Dict[str, Any]:
         if isinstance(data, dict):
             if all(value is None for value in data.values()):
                 raise ValueError('policy should contain at least one provider')
```

## ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_connection_data.py

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
-from typing import List, Optional
+from typing import Dict, List, Optional
 
 from pydantic import Field
 
 from ark_sdk_python.models.ark_model import ArkCamelizedModel
+from ark_sdk_python.models.services.dpa.policies.db.ark_dpa_db_enums import ArkDPADBMongoDatabaseBuiltinRole, ArkDPADBMongoGlobalBuiltinRole
 
 
 class ArkDPADBBaseAuth(ArkCamelizedModel):
     pass
 
 
 class ArkDPADBResourceIdentifierType(str, Enum):
@@ -34,13 +35,21 @@
     roles: List[str] = Field(description='Local DB roles to assign the ephemeral user to')
     applied_to: Optional[List[ArkDPADBAppliedTo]] = Field(description='Which resources to apply to')
     dba_role: bool = Field(description='Whether to apply to the ephemeral user the DBA role', default=False)
     sysdba_role: bool = Field(description='Whether to apply to the ephemeral user the SYSDBA role', default=False)
     sysoper_role: bool = Field(description='Whether to apply to the ephemeral user the SYSOPER role', default=False)
 
 
+class ArkDPADBMongoDBAuth(ArkDPADBBaseAuth):
+    global_builtin_roles: List[ArkDPADBMongoGlobalBuiltinRole] = Field(description='Global builtin roles across all databases')
+    database_builtin_roles: Dict[str, List[ArkDPADBMongoDatabaseBuiltinRole]] = Field(description='Per database builtin roles')
+    database_custom_roles: Dict[str, List[str]] = Field(description='Custom per database roles')
+    applied_to: Optional[List[ArkDPADBAppliedTo]] = Field(description='Which resources to apply to')
+
+
 class ArkDPADBConnectAs(ArkCamelizedModel):
     ldap_auth: Optional[List[ArkDPADBLDAPAuth]] = Field(description='LDAP related authentication, only applies to MSSQL DB')
     db_auth: Optional[List[ArkDPADBLocalDBAuth]] = Field(
         description='Local DB related authentication, only applies to MySQL / MariaDB / Postgres'
     )
     oracle_auth: Optional[List[ArkDPADBOracleDBAuth]] = Field(description='Oracle DB related authentication, only applies to Oracle')
+    mongo_auth: Optional[List[ArkDPADBMongoDBAuth]] = Field(description='Mongo DB related authentication, only applies to Mongo')
```

## ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_filter.py

```diff
@@ -16,10 +16,12 @@
             for plat in val:
                 if ArkWorkspaceType(plat) not in [
                     ArkWorkspaceType.MYSQL,
                     ArkWorkspaceType.MARIADB,
                     ArkWorkspaceType.POSTGRES,
                     ArkWorkspaceType.MSSQL,
                     ArkWorkspaceType.ORACLE,
+                    ArkWorkspaceType.MONGO,
+                    ArkWorkspaceType.DB2,
                 ]:
                     raise ValueError('Invalid Database Type')
         return val
```

## ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_provider.py

```diff
@@ -25,23 +25,26 @@
     MSSQLSH = 'mssql-sh'
     MySQLSH = 'mysql-sh'
     MariaDBSH = 'mariadb-sh'
     PostgresSH = 'postgres-sh'
     OracleSH = 'oracle-sh'
     DB2 = 'db2'
     DB2SH = 'db2-sh'
+    Mongo = 'mongo'
+    MongoSH = 'mongo-sh'
 
 
 class ArkDPADBDatabaseFamilyType(str, Enum):
     Postgres = 'Postgres'
     Oracle = 'Oracle'
     MSSQL = 'MSSQL'
     MySQL = 'MySQL'
     MariaDB = 'MariaDB'
     DB2 = 'DB2'
+    Mongo = 'Mongo'
     Unknown = 'Unknown'
 
 
 class ArkDPADBDatabaseWorkspaceType(str, Enum):
     Cloud = 'cloud'
     SelfHosted = 'self-hosted'
 
@@ -73,18 +76,21 @@
     ArkDPADBDatabaseEngineType.OracleSE2: ArkDPADBDatabaseFamilyType.Oracle,
     ArkDPADBDatabaseEngineType.Postgres: ArkDPADBDatabaseFamilyType.Postgres,
     ArkDPADBDatabaseEngineType.PostgresSH: ArkDPADBDatabaseFamilyType.Postgres,
     ArkDPADBDatabaseEngineType.SqlServer: ArkDPADBDatabaseFamilyType.MSSQL,
     ArkDPADBDatabaseEngineType.SqlServerSH: ArkDPADBDatabaseFamilyType.MSSQL,
     ArkDPADBDatabaseEngineType.DB2: ArkDPADBDatabaseFamilyType.DB2,
     ArkDPADBDatabaseEngineType.DB2SH: ArkDPADBDatabaseFamilyType.DB2,
+    ArkDPADBDatabaseEngineType.Mongo: ArkDPADBDatabaseFamilyType.Mongo,
+    ArkDPADBDatabaseEngineType.MongoSH: ArkDPADBDatabaseFamilyType.Mongo,
 }
 
 
 DATABASE_FAMILIES_DEFAULT_PORTS: Final[Dict[ArkDPADBDatabaseFamilyType, int]] = {
     ArkDPADBDatabaseFamilyType.Postgres: 5432,
     ArkDPADBDatabaseFamilyType.Oracle: 2484,
     ArkDPADBDatabaseFamilyType.MSSQL: 1433,
     ArkDPADBDatabaseFamilyType.MySQL: 3306,
     ArkDPADBDatabaseFamilyType.MariaDB: 3306,
     ArkDPADBDatabaseFamilyType.DB2: 50002,
+    ArkDPADBDatabaseFamilyType.Mongo: 27017,
 }
```

## ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_update_database.py

```diff
@@ -14,14 +14,19 @@
     new_name: Optional[str] = Field(description='New name for the database')
     network_name: Optional[str] = Field(description='Name of the network the database resides in', default='ON-PREMISE')
     platform: Optional[ArkWorkspaceType] = Field(description='Platform of the database, as in, where it resides')
     services: Optional[List[str]] = Field(description='Services related to the database, most commonly used with oracle')
     domain: Optional[str] = Field(description='The domain the DB resides in')
     domain_controller_name: Optional[str] = Field(description='Domain controller name associated to this database')
     domain_controller_netbios: Optional[str] = Field(description='Domain controller netbios associated to this database')
+    domain_controller_use_ldaps: bool = Field(description='Whether to work with LDAP secure or not', default=False)
+    domain_controller_enable_certificate_validation: bool = Field(
+        description='Whether to enforce certificate validation on TLS comm to the DC', default=True
+    )
+    domain_controller_ldaps_certificate: Optional[str] = Field(description='Certificate id to use for the domain controller TLS comm')
     provider_engine: Optional[ArkDPADBDatabaseEngineType] = Field(
         description='Provider engine, will be later deduced to the identifer of the provider'
     )
     enable_certificate_validation: bool = Field(description='Whether to enable and enforce certificate validation', default=True)
     certificate: Optional[str] = Field(description='Certificate id used for this database that resides in the certificates service')
     read_write_endpoint: Optional[str] = Field(description='Read write endpoint of the database')
     read_only_endpoint: Optional[str] = Field(description='Optionally, a read only endpoint of the database')
```

## ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_add_database.py

```diff
@@ -14,14 +14,19 @@
     platform: ArkWorkspaceType = Field(
         description='Platform of the database, as in, where it resides, defaulted to on premises', default=ArkWorkspaceType.ONPREM
     )
     services: Optional[List[str]] = Field(description='Services related to the database, most commonly used with oracle')
     domain: Optional[str] = Field(description='The domain the DB resides in')
     domain_controller_name: Optional[str] = Field(description='Domain controller name associated to this database')
     domain_controller_netbios: Optional[str] = Field(description='Domain controller netbios associated to this database')
+    domain_controller_use_ldaps: bool = Field(description='Whether to work with LDAP secure or not', default=False)
+    domain_controller_enable_certificate_validation: bool = Field(
+        description='Whether to enforce certificate validation on TLS comm to the DC', default=True
+    )
+    domain_controller_ldaps_certificate: Optional[str] = Field(description='Certificate id to use for the domain controller TLS comm')
     provider_engine: ArkDPADBDatabaseEngineType = Field(
         description='Provider engine, will be later deduced to the identifer of the provider'
     )
     enable_certificate_validation: bool = Field(description='Whether to enable and enforce certificate validation', default=True)
     certificate: Optional[str] = Field(description='Certificate id used for this database that resides in the certificates service')
     read_write_endpoint: str = Field(description='Read write endpoint of the database')
     read_only_endpoint: Optional[str] = Field(description='Optionally, a read only endpoint of the database')
```

## ark_sdk_python/models/common/ark_workspace_type.py

```diff
@@ -8,9 +8,11 @@
     DB = 'db', 'DATABASES', 'Databases'
     GCP = 'gcp', 'GCP'
     MYSQL = 'mysql', 'MySQL'
     MARIADB = 'mariadb', 'MariaDB'
     MSSQL = 'mssql', 'MSSQL'
     ORACLE = 'oracle', 'Oracle'
     POSTGRES = 'postgres', 'Postgres'
+    MONGO = 'mongo', 'Mongo'
+    DB2 = 'db2', 'Db2'
     FAULT = 'fault', 'FAULT'
     UNKNOWN = 'unknown', 'UNKNOWN', 'Unknown'
```

## ark_sdk_python/models/common/ark_region.py

```diff
@@ -26,15 +26,17 @@
     Bahrain = 'me-south-1'
     SaoPaulo = 'sa-east-1'
     USEast = 'us-gov-east-1'
     USWest = 'us-gov-west-1'
     USEastPerf = 'us-east-perf'
     USEastPod = 'us-east-pod'
     Jakarta = 'ap-southeast-3'
+    Indonesia = 'ap-southeast-3'
     Melbourne = 'ap-southeast-4'
+    UAE = 'me-central-1'
 
 
 regions_full_names = {
     ArkRegion.Ohio: 'us-east-2 (Ohio)',
     ArkRegion.NorthVirginia: 'us-east-1 (N. Virginia)',
     ArkRegion.NorthCalifornia: 'us-west-1 (N. California)',
     ArkRegion.Oregon: 'us-west-2 (Oregon)',
@@ -58,15 +60,17 @@
     ArkRegion.Bahrain: 'me-south-1 (Bahrain)',
     ArkRegion.SaoPaulo: 'sa-east-1 (São Paulo)',
     ArkRegion.USEast: 'us-gov-east-1 (US-East)',
     ArkRegion.USWest: 'us-gov-west-1 (US-West)',
     ArkRegion.USEastPerf: 'us-east-perf (US-East-Perf)',
     ArkRegion.USEastPod: 'us-east-pod (US-East-Pod)',
     ArkRegion.Jakarta: 'ap-southeast-3 (Jakarta)',
+    ArkRegion.Indonesia: 'ap-southeast-3 (Indonesia)',
     ArkRegion.Melbourne: 'ap-southeast-4 (Melbourne)',
+    ArkRegion.UAE: 'me-central-1 (UAE)',
 }
 
 platform_region_dict = {
     'America East': 'us-east-1',
     'America West': 'us-west-1',
     'Oregon': 'us-west-2',
     'Canada': 'ca-central-1',
@@ -90,13 +94,15 @@
     'GovCloud (US West)': 'us-gov-east-1',
     'US-East-Perf': 'us-east-perf',
     'us-east-perf': 'US-East-Perf',
     'US-East-Pod': 'us-east-pod',
     'us-east-pod': 'US-East-Pod',
     'ISP-PcloudPerf-US East': 'isp-pcloudperf-us east',
     'Jakarta': 'ap-southeast-3',
+    'Indonesia': 'ap-southeast-3',
     'Melbourne': 'ap-southeast-4',
+    'UAE': 'me-central-1',
 }
 
 
 def region_to_platform_region(region: str) -> str:
     return list(platform_region_dict.keys())[list(platform_region_dict.values()).index(region)]
```

## ark_sdk_python/models/ark_model.py

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Callable, Optional
 
-from humps import camel
+from humps import camelize
 from pydantic import BaseModel, Field, validator
 from pydantic.generics import GenericModel
 
 
 class ArkModel(BaseModel):
     class Config:
         allow_population_by_field_name = True
@@ -17,15 +17,15 @@
 class ArkPresentableModel(ArkModel):
     class Config:
         use_enum_values = True
 
 
 class ArkCamelizedModel(ArkPresentableModel):
     class Config:
-        alias_generator = camel.case
+        alias_generator = camelize
 
 
 class ArkTitleizedModel(ArkPresentableModel):
     class Config:
         alias_generator = lambda s: s.replace("_", " ").title().replace(" ", "")
```

## ark_sdk_python/models/actions/services/ark_dpa_exec_action_consts.py

```diff
@@ -17,15 +17,20 @@
 from ark_sdk_python.models.services.dpa.certificates import (
     ArkDPACertificatesFilter,
     ArkDPACreateCertificate,
     ArkDPADeleteCertificate,
     ArkDPAGetCertificate,
     ArkDPAUpdateCertificate,
 )
-from ark_sdk_python.models.services.dpa.db import ArkDPADBMysqlExecution, ArkDPADBOracleGenerateAssets, ArkDPADBPsqlExecution
+from ark_sdk_python.models.services.dpa.db import (
+    ArkDPADBMysqlExecution,
+    ArkDPADBOracleGenerateAssets,
+    ArkDPADBProxyFullchainGenerateAssets,
+    ArkDPADBPsqlExecution,
+)
 from ark_sdk_python.models.services.dpa.k8s.ark_dpa_k8s_generate_kubeconfig import ArkDPAK8SGenerateKubeConfig
 from ark_sdk_python.models.services.dpa.policies.common import ArkDPADeletePolicy, ArkDPAGetPolicy, ArkDPAUpdatePolicyStatus
 from ark_sdk_python.models.services.dpa.policies.db import ArkDPADBAddPolicy, ArkDPADBPoliciesFilter, ArkDPADBUpdatePolicy
 from ark_sdk_python.models.services.dpa.policies.vm import ArkDPAVMAddPolicy, ArkDPAVMPoliciesFilter, ArkDPAVMUpdatePolicy
 from ark_sdk_python.models.services.dpa.secrets.db import (
     ArkDPADBAddSecret,
     ArkDPADBDeleteSecret,
@@ -150,14 +155,15 @@
     'short-lived-rdp-file': ArkDPASSOGetShortLivedRDPFile,
 }
 SSO_ACTION: Final[ArkServiceActionDefinition] = ArkServiceActionDefinition(action_name='sso', schemas=SSO_ACTION_TO_SCHEMA_MAP)
 DB_ACTION_TO_SCHEMA_MAP: Final[Dict[(str, Optional[Type[ArkModel]])]] = {
     'psql': ArkDPADBPsqlExecution,
     'mysql': ArkDPADBMysqlExecution,
     'generate-oracle-tnsnames': ArkDPADBOracleGenerateAssets,
+    'generate-proxy-fullchain': ArkDPADBProxyFullchainGenerateAssets,
 }
 DB_ACTION: Final[ArkServiceActionDefinition] = ArkServiceActionDefinition(action_name='db', schemas=DB_ACTION_TO_SCHEMA_MAP)
 K8S_ACTION_TO_SCHEMA_MAP: Final[Dict[(str, Optional[Type[ArkModel]])]] = {'generate-kubeconfig': ArkDPAK8SGenerateKubeConfig}
 K8S_ACTION: Final[ArkServiceActionDefinition] = ArkServiceActionDefinition(action_name='k8s', schemas=K8S_ACTION_TO_SCHEMA_MAP)
 DPA_ACTIONS: Final[ArkServiceActionDefinition] = ArkServiceActionDefinition(
     action_name='dpa',
     subactions=[POLICIES_ACTION, WORKSPACES_ACTION, SECRETS_ACTION, SSO_ACTION, DB_ACTION, CERTIFICATES_ACTION, K8S_ACTION],
```

## ark_sdk_python/cli_services/dpa/vm/ark_dpa_vm_policies_editor_service.py

```diff
@@ -17,15 +17,14 @@
     ArkDPAVMAuthorizationRule,
     ArkDPAVMAWSProviderData,
     ArkDPAVMAzureProviderData,
     ArkDPAVMConnectionDataType,
     ArkDPAVMConnectionInformation,
     ArkDPAVMFQDNOperator,
     ArkDPAVMFQDNRule,
-    ArkDPAVMFQDNRulesConjunction,
     ArkDPAVMGCPProviderData,
     ArkDPAVMLocalEphemeralUserConnectionMethodData,
     ArkDPAVMOnPremProviderData,
     ArkDPAVMPolicy,
     ArkDPAVMPolicyListItem,
     ArkDPAVMProvider,
     ArkDPAVMRDPLocalEphemeralUserConnectionData,
@@ -62,15 +61,14 @@
 DEFAULT_GENERATED_PROVIDERS: Final[Dict[ArkWorkspaceType, ArkDPAVMProvider]] = {
     ArkWorkspaceType.AWS: ArkDPAVMAWSProviderData(regions=[], tags=[{'key': 'value'}], vpc_ids=[], account_ids=[]),
     ArkWorkspaceType.AZURE: ArkDPAVMAzureProviderData(
         regions=[], tags=[{'key': 'value'}], resource_groups=[], vnet_ids=[], subscriptions=[]
     ),
     ArkWorkspaceType.GCP: ArkDPAVMGCPProviderData(regions=[], tags=[{'key': 'value'}], network_ids=[], projects=[]),
     ArkWorkspaceType.ONPREM: ArkDPAVMOnPremProviderData(
-        fqdn_rules_conjunction=ArkDPAVMFQDNRulesConjunction.OR,
         fqdn_rules=[ArkDPAVMFQDNRule(operator=ArkDPAVMFQDNOperator.WILDCARD, computername_pattern='*', domain='default.com')],
     ),
 }
 DEFAULT_GENERATED_PROTOCOLS: Final[Dict[ArkProtocolType, ArkDPAVMConnectionDataType]] = {
     ArkProtocolType.SSH: 'root',
     ArkProtocolType.RDP: ArkDPAVMRDPLocalEphemeralUserConnectionData(
         local_ephemeral_user=ArkDPAVMLocalEphemeralUserConnectionMethodData(assign_groups={'Administrators'})
```

## ark_sdk_python/ark.py

```diff
@@ -13,15 +13,15 @@
 import argcomplete
 import urllib3
 
 from ark_sdk_python.actions import ArkAction, ArkCacheAction, ArkConfigureAction, ArkLoginAction, ArkProfilesAction, ArkServiceExecAction
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-__version__ = '1.0.6'
+__version__ = '1.0.7'
 
 
 def main():
     parser: argparse.ArgumentParser = argparse.ArgumentParser()
     parser.add_argument('-v', '--version', action='version', version=__version__)
     subparsers = parser.add_subparsers(dest="action")
     subparsers.required = True
```

## Comparing `ark_sdk_python-1.0.6.dist-info/RECORD` & `ark_sdk_python-1.0.7.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 ark_sdk_python/actions/ark_exec_action.py,sha256=eNWbCkb6ntuvQRa1kpSzKXeNBTTczwqgghVry-eZzSg,14323
 ark_sdk_python/actions/ark_login_action.py,sha256=tqYfml92rAsaEWYDfMwi9a5bsMFHWdryGS-dypeRZE4,10357
 ark_sdk_python/actions/ark_profiles_action.py,sha256=sOO6xEYMjrs6-K5wY0epi4wVo6XXUE-ozytAmhoBDNM,9638
 ark_sdk_python/actions/ark_service_exec_action.py,sha256=O9rU9KuRYHaxrk4Diollot4o4NWQ0duy-Af91N9GBlA,5109
 ark_sdk_python/args/__init__.py,sha256=mCb4UrIRL4u58QyUbqqH2xAU0VN91pxjK5sa_UwCM_k,279
 ark_sdk_python/args/ark_args_formatter.py,sha256=-Rs_rGMIr1bprD1SfYlMsLoSOFgr_RFrRdREvbmPU6k,9204
 ark_sdk_python/args/ark_pydantic_argparse.py,sha256=AzwkdhUoxHd9Hreki_iWCdT8lY-1um8OOfbvOedduBE,33777
-ark_sdk_python/ark.py,sha256=NH1LR_F58Q5nRRnCUPvfwsM5dubD7J9rbo_e9H3TyOM,1280
+ark_sdk_python/ark.py,sha256=F-H-o1h-yQGGGQNDc9_N5PHRbQNChswiQJhMDJJY5yQ,1280
 ark_sdk_python/ark_api.py,sha256=VW3kUoGDcmd7lQMWRaWejfaqQvHMZwf7Si-YAkEA1LQ,6836
 ark_sdk_python/auth/__init__.py,sha256=1l29Rf3VhwmV8z3YROiQVcgrZYSeeCqVN4zna77tnlk,620
-ark_sdk_python/auth/ark_auth.py,sha256=AfjlA2ETpuPxkLgeTnekkXm5u-yuXRCisfop6LedoqI,12740
+ark_sdk_python/auth/ark_auth.py,sha256=eycipVTr2uNHZ4XdqCyXN7Cwx4g_wmoj71OkIVzjSTQ,12947
 ark_sdk_python/auth/ark_isp_auth.py,sha256=Xuf8J7-VgN6a6oJOem5Rf8LzOI5NCNqUeT5Snb4VNK4,9572
 ark_sdk_python/auth/identity/__init__.py,sha256=2Yyc_Rrx-D4PsSdg-ESl5pFFTpqu6LUPSc4ZW59oOP8,328
 ark_sdk_python/auth/identity/ark_identity.py,sha256=mFK4DoWd1E9PMHaV3DV-2mIO3B8V_8MZ0xBK1M9F1RU,28247
 ark_sdk_python/auth/identity/ark_identity_fqdn_resolver.py,sha256=_WKm31eVlT-vLRTmp-tTswpXgdl9_Iqqvp5ZPKRvDwg,4777
 ark_sdk_python/auth/identity/ark_identity_service_user.py,sha256=QlqUHGUh4iqmfqmV_YlXs6xNM_U-xz6VqW5hHZoxwSQ,7495
 ark_sdk_python/cli_services/__init__.py,sha256=e9vdwqNiYqhZmK05Wgpz-Hf9SycK_3X-RS3CK9n2lIs,87
 ark_sdk_python/cli_services/ark_cli_api.py,sha256=caHrIEkTtcCZ0OK5zkgnVpqzhRfgOQ7SvBOtAHu20mI,912
 ark_sdk_python/cli_services/dpa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ark_sdk_python/cli_services/dpa/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ark_sdk_python/cli_services/dpa/common/ark_dpa_base_policies_editor_service.py,sha256=Sig78RDD8zgKHtsp5PO9JDPc71xboPH4TxWLJbXY6fY,27869
 ark_sdk_python/cli_services/dpa/db/__init__.py,sha256=fPXWHDxIUlriFM-9I2YFNwGTnIvfHc1PdHaCQLVL_vo,157
 ark_sdk_python/cli_services/dpa/db/ark_dpa_db_policies_editor_service.py,sha256=NnMvNLxJqBKhmMC8yfvrWcPkO-Gwld6DbQEw1eUkv7c,10620
 ark_sdk_python/cli_services/dpa/vm/__init__.py,sha256=34qKE_DVp5PJ-9W3osyTbnJpOsXrNlhEDqJ6xHz-7y8,157
-ark_sdk_python/cli_services/dpa/vm/ark_dpa_vm_policies_editor_service.py,sha256=T_7-QeP7hTR4ziAlC-MYF2_6CRCqPAXcbnRpmUne248,8807
+ark_sdk_python/cli_services/dpa/vm/ark_dpa_vm_policies_editor_service.py,sha256=zPIdlCx2gQshnfCh3W1s21wYWBlzPN4Cuiqw9zgUO-A,8709
 ark_sdk_python/common/__init__.py,sha256=QpzMfvy7yl_kw5B5uYuQkVhIw_p1QH5Vvm4lHpK4FzY,763
 ark_sdk_python/common/ark_async_client.py,sha256=Dk4hKceA3qwYRYz97NNcAUU7YsVDTGQdoKUXyQJMpy4,2234
 ark_sdk_python/common/ark_async_request.py,sha256=03q-U4K6oHJ18UNjQcJWT01plfZDNe74RI7iQqJmQmY,1885
 ark_sdk_python/common/ark_client.py,sha256=k0_fIDPkx7hxlVGT961Fn-paAWPhSY3CJnrTpCP-Lo4,6606
 ark_sdk_python/common/ark_keyring.py,sha256=Go0dp7Dx2RJPSsFxMi3iutGLicEM7oldurZw1zBO_bA,11252
 ark_sdk_python/common/ark_logger.py,sha256=l06FH2dg6AkpR8M6zVoZVgaiyOZ2G9ANxHNahPDHVEE,2445
 ark_sdk_python/common/ark_page.py,sha256=4_kycDX8vLloyZOlbM8N9XYXiF2cb5O-l4FbZ5hA7CY,358
@@ -45,18 +45,18 @@
 ark_sdk_python/examples/create_dpa_db_environment.py,sha256=E_gI-Ct7P1xQtMQGBeiN9FG_kuCg5X-Q8tfRSJx0wI4,3744
 ark_sdk_python/examples/session_monitoring_activites.py,sha256=WSGISA4Qye8q22WpiHq0HKYTfbwLK7038mRHp2Kr9IQ,1632
 ark_sdk_python/models/__init__.py,sha256=Lh_ZYHzx7xPIjbHr5mbQjZ0YyQEjFVlX0uxC-D8sdxQ,956
 ark_sdk_python/models/actions/__init__.py,sha256=2xPZhoHco50bmPX7rm6uPOAcYURoTP9J5KF4E3XNaFA,743
 ark_sdk_python/models/actions/ark_configure_action_consts.py,sha256=-YNgiGv1GsQx-JvO0eXXrrOlDcH6sRDLdO7kvTHto-M,1143
 ark_sdk_python/models/actions/ark_service_action_definition.py,sha256=cNQ28O1Xz3vIuJm7eQU--tFE7c4tE48VGf86qdx9QX4,785
 ark_sdk_python/models/actions/services/__init__.py,sha256=J9oit0bUS2SeUDtSbg1qYeJvtBPViH1_AR7RPB2gz1Y,370
-ark_sdk_python/models/actions/services/ark_dpa_exec_action_consts.py,sha256=3U0_1TrEX00r54eukrp1RmcsD0_80GfxJMlM6eTRpTs,7763
+ark_sdk_python/models/actions/services/ark_dpa_exec_action_consts.py,sha256=bjStqTzJXlW-3DVcSlcq_KiXBAkFIUo-I4fOt3n9J9A,7892
 ark_sdk_python/models/actions/services/ark_sm_exec_action_consts.py,sha256=xMfQ79d7XKG5iZ5ItqNRN5lre5FWWN3VWXDGwVegfY4,1161
 ark_sdk_python/models/ark_exceptions.py,sha256=lW4-kyHvHiKJEThl1j50mffmNGbv-anUixXNLUpjJe4,562
-ark_sdk_python/models/ark_model.py,sha256=fILD9I0PKnC2a-rs7a5OIb9lV0qFlVBRvwJW84zFQsQ,1798
+ark_sdk_python/models/ark_model.py,sha256=gEWiyMeyu5MvZVCHnv2d6Vmh8Bmz55cEFhzNqA7UxrU,1799
 ark_sdk_python/models/ark_profile.py,sha256=6A1oVIxxVokwUV7WFVglEPDmSpjqyUSmxNT5EVGK8N4,6300
 ark_sdk_python/models/auth/__init__.py,sha256=zIRXj7AlSvPI2nanPM1tpc_lx8cwaYJUgI_FU4YjGzw,1065
 ark_sdk_python/models/auth/ark_auth_method.py,sha256=ROFPC3ijlAwOdOnpkWF_8SzAxA7tbhFFnmyWLIpo1rk,3150
 ark_sdk_python/models/auth/ark_auth_profile.py,sha256=fEbxob2wKGArhrO5cbGc93tjqpbVDy7Lw05xmNSKpsw,1289
 ark_sdk_python/models/auth/ark_secret.py,sha256=RNNcAcBYJvl8DV9VvGJ6sbGaejgwc8oherQ5KjHAO9M,326
 ark_sdk_python/models/auth/ark_token.py,sha256=q1eAz5UNBfSABm5VHANtGZ_TsRFhrFVbEVPX0vixYaQ,1438
 ark_sdk_python/models/cli_services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -86,19 +86,19 @@
 ark_sdk_python/models/common/ark_async_task.py,sha256=LUWRB7K6Rnm5uYnQAGMs75etQGTGLxo6u1mPAyMs_lY,525
 ark_sdk_python/models/common/ark_connection_method.py,sha256=-zrqoCuLaRYuWH8xhjAwwGIHJ9cBERKp5UMH9uErk5U,143
 ark_sdk_python/models/common/ark_connector_type.py,sha256=dxyUtBEKVOvQa7sneu4i4fjCgw_cew2SyAxix6wCZWc,94
 ark_sdk_python/models/common/ark_counted_values.py,sha256=kZp01_7yyaR_8eVbWZsFib5kgs3RtRJGc93YFu-UF9Q,272
 ark_sdk_python/models/common/ark_network_entity_type.py,sha256=J9rXuxdw27odsndtz3K21UWyLBSgjX3kDmm4fHzyCak,391
 ark_sdk_python/models/common/ark_os_type.py,sha256=lcEPfGQzrLkfOaJcvkS0v10okW-5Dsb7zgPNqeCmXBE,452
 ark_sdk_python/models/common/ark_protocol_type.py,sha256=gF0h6n3iQnZYe9dc_a0P4k-7j9HEJbfR2Oe7288hdOA,328
-ark_sdk_python/models/common/ark_region.py,sha256=t-_Lb7vYxxSCXoWdxAzG5EKasn7LD1dpw5JmI66iNKI,3495
+ark_sdk_python/models/common/ark_region.py,sha256=FFqBfZF0P0IZf1QImYZbLzkMjTUOhXTQYz2RtFm-5fs,3711
 ark_sdk_python/models/common/ark_status.py,sha256=6TE8nUu0Vg4KZzr-8x4hkPPvUK_dOJEkYRQ_ShWg8-s,2504
 ark_sdk_python/models/common/ark_status_stats.py,sha256=4TCJp9g6V5eK_V7P_Z4gygfJe77ucR3g3IhtsliaLiA,271
 ark_sdk_python/models/common/ark_validations.py,sha256=uIOv7s-UMvphTp3VEyqgmreZT8s2zERrdkzv7tYovNc,184
-ark_sdk_python/models/common/ark_workspace_type.py,sha256=qaA565dt3R20ElEEXz2-APvbCIxtJeKhNS3_SSM5fWw,495
+ark_sdk_python/models/common/ark_workspace_type.py,sha256=ZAYTHQLFr5ooof55Eth--0afc22rD2wImN-e8NFu7XM,547
 ark_sdk_python/models/common/aws/__init__.py,sha256=9XbxkEExv4H8r-hPG3AZLn-zlC1-rtP_eycpoI4avNM,111
 ark_sdk_python/models/common/aws/ark_cfn_async_task.py,sha256=IfaUoFpAEbykDcOMGQ_oYAr8hIvK8qsolWZd0uKsxPM,566
 ark_sdk_python/models/common/connections/__init__.py,sha256=GkDAw47UpWfidJU5sycgNvSdWUoCA8MX9k2v9pRhiKE,545
 ark_sdk_python/models/common/connections/ark_connection_command.py,sha256=-T9XcZdONFEdq1GRzTOWozq76g4_lD-1NjsiSjPA0Sw,352
 ark_sdk_python/models/common/connections/ark_connection_credentials.py,sha256=RfXKvQKX0YfNSW8xtMHQ71qiOSKCT6ozUo6QFP6kHKg,536
 ark_sdk_python/models/common/connections/ark_connection_details.py,sha256=HQdu7SbxBc5U9-BJBj8Qv3KT9NuuYfvImiUy3je-njQ,1508
 ark_sdk_python/models/common/connections/ark_connection_result.py,sha256=0XpLZmf0p4vPRFGxRHJ1v9erDOoGZYQnM_mq99wAYyA,344
@@ -116,20 +116,22 @@
 ark_sdk_python/models/services/dpa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ark_sdk_python/models/services/dpa/certificates/__init__.py,sha256=Fop7HbDHwt-4leApWUIl42CCIMgD9frRWg093UXy4Vw,1036
 ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_certificate.py,sha256=svdf5Sq3LkmG0EyoxXzclDNIvpCy0MjDEvFDMQguexo,3706
 ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_delete_certificate.py,sha256=j_Gn4D9q3lNiNCawKA4AcnMS5BjWnhyz1VpaxDVF9h8,207
 ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_filter.py,sha256=n1_Sf2Un1cI6xRrUKZrg0QK34ZMZQvM0paWxCXcq5A4,337
 ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_get_certificate.py,sha256=cD_9xmqsP9c6XzgQu-ydtwb07-NDoV1SmQHLsEvqBa8,204
 ark_sdk_python/models/services/dpa/certificates/ark_dpa_certificates_update_certificate.py,sha256=rKUZLbQvBCP3RpLFWTxwGhhRsYYmfDdE8Jyq9C68SR8,547
-ark_sdk_python/models/services/dpa/db/__init__.py,sha256=ALbQh8wYmO-3ITqMpxHVfBwfcAwLbxAMI8SXxOcCD-A,890
+ark_sdk_python/models/services/dpa/db/__init__.py,sha256=LI1KrU3yDdZCGs9nVW6p3Ttz_F1_Jgo1_zG3Xjuqqrg,1182
+ark_sdk_python/models/services/dpa/db/ark_dpa_db_assets_type.py,sha256=YQjKsWzA6nHOrf4GgwbbV3_10QSVSL1lv7RVWjUV7Dk,174
 ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_execution.py,sha256=xpZVg7bQV7xRgpM6eWTFrj-duVFJe1QhU1jP4PoiogI,306
-ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_generate_assets.py,sha256=Hb-IglMXZUdamr43dk1NmwOx0hhEoeq4jVLcX7N4YVA,764
+ark_sdk_python/models/services/dpa/db/ark_dpa_db_base_generate_assets.py,sha256=YjwiwJBoUw17Sj73SuKabcIAoQlhj6dI2P6scQPaZUI,724
 ark_sdk_python/models/services/dpa/db/ark_dpa_db_generated_assets.py,sha256=opNCIvxiLyd1CKwlR-ev58g2X9vqvjzszhl6d_Rb_YQ,227
 ark_sdk_python/models/services/dpa/db/ark_dpa_db_mysql_execution.py,sha256=jYTcqA8H2PPEk5_ubIzf_OciNGypTq9yIFw50_vJCdg,269
-ark_sdk_python/models/services/dpa/db/ark_dpa_db_oracle_generate_assets.py,sha256=ghGGbVNX5OQZ4OugIw49DMYA7Xn8t3FT7rliMTf15fo,352
+ark_sdk_python/models/services/dpa/db/ark_dpa_db_oracle_generate_assets.py,sha256=5uZ54UbVbbTdyn7rlRFo7Nc3CYfe8NgCNzzVCpysegs,392
+ark_sdk_python/models/services/dpa/db/ark_dpa_db_proxy_fullchain_generate_assets.py,sha256=9swJf80FfKi1HIe3nn8lIzEV3EqoTvZ9od9bVe9HYbQ,192
 ark_sdk_python/models/services/dpa/db/ark_dpa_db_psql_execution.py,sha256=4NaxA9HjFP79GjJfZcM-VvWEJtpFa62gpDzoIXnLov0,266
 ark_sdk_python/models/services/dpa/k8s/__init__.py,sha256=kmqtxo2hBtFcs5DUNWVQsgqnCPNxzefQta2dAI2KhQY,154
 ark_sdk_python/models/services/dpa/k8s/ark_dpa_k8s_generate_kubeconfig.py,sha256=NraR7UT8INimkjI-y3C-w9DStwAGUmnU-eV8cN0CU-w,218
 ark_sdk_python/models/services/dpa/policies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ark_sdk_python/models/services/dpa/policies/common/__init__.py,sha256=96qMHXNEOrQwbXaToLmwOXQpFpeiG7XbLFXCuv-6BkU,1942
 ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_add_policy.py,sha256=4-o5l6TKb4eHm-sq_vzG7e0RdRd-rT6GEpdQyl-xY50,807
 ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_authorization_rule.py,sha256=Y8r09R7ENwgRaUyCrz1us5nNR673amaOViHw4854guk,386
@@ -140,37 +142,38 @@
 ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_policy_list_item.py,sha256=LG4E-QrASuUEsNmq7f3tLjoqNcOwAhbuI1GIzbX_IU0,723
 ark_sdk_python/models/services/dpa/policies/common/ark_dpa_base_update_policy.py,sha256=8CHD0U9M3HHmnBdYYbJM1Zxbx5LwS2D5XPaXk5shYsg,1137
 ark_sdk_python/models/services/dpa/policies/common/ark_dpa_delete_policy.py,sha256=8oFuwLvgAqPZJOw6CEpFi-pJDR7lTPBgUpwipXgiZCI,589
 ark_sdk_python/models/services/dpa/policies/common/ark_dpa_get_policy.py,sha256=NgzIcUcby2bY5FFzgghMesMmPVSKsXis3Z3VEBwAemY,580
 ark_sdk_python/models/services/dpa/policies/common/ark_dpa_rule_status.py,sha256=2xQpWSQfDQvZxPF1hDhm9pUt6Q0-SZa4Q8BIeXVQViY,153
 ark_sdk_python/models/services/dpa/policies/common/ark_dpa_update_policy_status.py,sha256=1iWoV5qT592KLwaT32GVcngSrNvfXZSpW9SevwdVRvQ,798
 ark_sdk_python/models/services/dpa/policies/common/ark_dpa_user_data.py,sha256=5YK9Fnt3JAL4iYsQ_4kBrlxQ5e8HwucQzv91eSJZvt0,769
-ark_sdk_python/models/services/dpa/policies/db/__init__.py,sha256=kd15H-092e5q7rKOmFvnANggF4f-ARYIp5Nn1sLRZeQ,2183
+ark_sdk_python/models/services/dpa/policies/db/__init__.py,sha256=JAKcqM6Ri1XGPsTewBAicuY7JkuYmopUd6Vmejw-ZMo,2530
 ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_add_policy.py,sha256=r8s3XBlMOr_RNX9UFFpjlykZZg1MMF7nOivbb8mt3b4,906
 ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_authorization_rule.py,sha256=WiJ3cPrVWwpvdyyz4wYIcjhcdY21FNYQ57SPe7Hpkf0,739
-ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_connection_data.py,sha256=tNWFr--m2FgomXxaCrWcZUkYYbbm9qr1KU5sZOFg5KI,2032
-ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_filter.py,sha256=wg2PWArnBrpaYDZtijdrC4k5-B0EzPhbMn4rKLaUvUA,979
-ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_stats.py,sha256=Fyha4mNBu_ZfXTbGEfoFcGvGSUbprA3RFyPyC2l8yxE,933
-ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_workspace_type_serializer.py,sha256=vBODvfREJ_p31Cj03D0IoL9i-bwWG4pkmGD7tjiQs0A,670
+ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_connection_data.py,sha256=NvKmbCIawVBS240dd8EXngANk32m3h0_XXVyy2YeXe8,2810
+ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_enums.py,sha256=qnMo6-07aVETlf1ep-b5TFIMa8qagG6e9fQ-ukbDr2I,671
+ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_filter.py,sha256=MxFRfTQaWpPufEpnwuLyYhnnFWQJ_xpfKxaUt1oKjCk,1065
+ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_stats.py,sha256=hLhLRBzLgmMx_hY08qsC4tVlNMt_t9J_6kKErbaOmRk,1011
+ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policies_workspace_type_serializer.py,sha256=y_4TvYSFwTZpwLkcQvoxTLMJvI1mOFIdvG5bXrvoE1w,800
 ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy.py,sha256=-AEIVKsBtD4Qj2IcOW_GGO-2-WoxsXdmfXoP41OgBLc,718
-ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy_list_item.py,sha256=rxD1Kzbnit3I6jFWms7iCfSbbNb012eEgtAqu35nFck,1071
-ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_providers.py,sha256=NBDdQVB7vY7ywmU88EKVZrRQQnW22R3dTg3By-UOQB8,1696
+ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_policy_list_item.py,sha256=uclIlS6tuecUhya-YzAtiVG7BCaRwIutHZ2ru7Kn9ks,1157
+ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_providers.py,sha256=LQ9eYcHhtGjPGEvriYR7XEFOAJphYPUgmMoT4qLhjwU,1958
 ark_sdk_python/models/services/dpa/policies/db/ark_dpa_db_update_policy.py,sha256=lN22q1lYysOpBbMDQv9tzQ2kfd_5rHKuKKcXwgQ8clk,906
-ark_sdk_python/models/services/dpa/policies/vm/__init__.py,sha256=iB5y595lPiX6ODBL2WiX3AiVj2XJgTxvPzk0rQuuot0,2669
-ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_add_policy.py,sha256=QUKE67-7QMhWi514khCzrmXfJ8AT-ZWChM4oRgMTMZ8,1650
+ark_sdk_python/models/services/dpa/policies/vm/__init__.py,sha256=DiiVkPng9JkCaCwdRB-Vo2loyU8ldlATu3nScDvs8vM,2599
+ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_add_policy.py,sha256=a-VsJezFKKWDhS3Rr-x7lT0x_VkC9u6p_ICj6-GChIA,1826
 ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_authorization_rule.py,sha256=42464JRP8s1dl2U1korRTkdbCgqsxBVOpQSiSAxL_1o,1662
 ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_connection_data.py,sha256=Bg9RDjb8Xgs6zY8F5ge6KbJAvfDuN9c-q2ogRNiZSw8,926
 ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_filter.py,sha256=RzMBqs_79cydKcBBPvEevQ5xKsrfcqZk2sFkXMPVks8,935
 ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_protocol_type_serializer.py,sha256=JpCVm2zNlFWhYmCfjIokjYFE6sQR25L6TxxodlcJEEI,679
 ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_stats.py,sha256=clvG4sEy8oGUdGToNDvgw09-bFx6E3uRYvcqQUnYcYg,896
-ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_workspace_type_serializer.py,sha256=FtS-fO9hKvylFaZ64--YGUD5DXILWnlbws4DKQnWpkM,522
-ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy.py,sha256=bXsmRoy7yZ_jIBFQ6BMkfoT1KwvHEo39uBNo2h7q45Q,1414
+ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policies_workspace_type_serializer.py,sha256=Be1NcJHzdX5cKN0BybibV-u6lTO5B-TuNTGwdJ9afe8,585
+ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy.py,sha256=9lALdaD5IORxZghHTzbFKAeaNBx1qqClUkXjErMeC5w,1590
 ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_policy_list_item.py,sha256=19yaG1CFkQpyBkv91bhvG0wj5hzEir1q9C7sMW2LzaY,927
-ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_providers.py,sha256=7Mj0Yu5mzyhlperjgY0C9OO5U0SGLcY_g0FsJJV9TdM,3056
-ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_update_policy.py,sha256=QmIHH8wYtrRhp6Rz8Kl1YN94y-il63AnwER8GlUfiPA,1427
+ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_providers.py,sha256=EVO6zrCp7m_mWpsF563CTSGcZIbZ39hC8cqv_WJ5-6I,2862
+ark_sdk_python/models/services/dpa/policies/vm/ark_dpa_vm_update_policy.py,sha256=EbLzk6eCnyOOdyvC_eGPZ6bUBQyi0pdr_if2E1L9mA0,1603
 ark_sdk_python/models/services/dpa/secrets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ark_sdk_python/models/services/dpa/secrets/db/__init__.py,sha256=MQolHX2anpBEIE-UETBiY88DsaYZdXbhNtXclaPONDg,1709
 ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_add_secret.py,sha256=GvXZ67VZHnw8_51gAsPfDhI4HewuZ-eQW9fCDg-2dWA,1572
 ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_delete_secret.py,sha256=XPez7ztN1mAk3iI6V-L12joY6h6PE1bHWEnD_HTKMvs,615
 ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_disable_secret.py,sha256=uAHWE-4Chh2h-8ocg5KWiusOAEPRWDcngj2-7K11RME,618
 ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_enable_secret.py,sha256=c8-DZhDcuA5IdtvINgxvi3VcO9dkOaxWK7AMqGErsVQ,615
 ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_get_secret.py,sha256=O53oRodRr4D-nmhE25J-JDAj_ZSoYgUJFphVLqSewXo,606
@@ -181,33 +184,33 @@
 ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_store_descriptor.py,sha256=Fr_P8pMnGpFFAdXToZidmmw9Hgt5maKSQkuUK7ycWKY,403
 ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_store_type.py,sha256=RJATAc1KQL1Cp4TUV2rKmvKYPrswJ9K2VemaYNkODlU,476
 ark_sdk_python/models/services/dpa/secrets/db/ark_dpa_db_update_secret.py,sha256=-gr9qCSNS0bBctbwrs8VW8Ba-Te9k0d3oJUu93VKNxQ,1629
 ark_sdk_python/models/services/dpa/secrets/db/secret_links/__init__.py,sha256=DtuPJbMMqSDIHzanJ9-LqnK2Yn2BYyHBAZkrFSzIYsA,220
 ark_sdk_python/models/services/dpa/secrets/db/secret_links/ark_dpa_db_pam_account_secret_link.py,sha256=ctGsvrfO-uEueGY4OuIobP_aVH03nKKhihhqcuKfsGU,293
 ark_sdk_python/models/services/dpa/secrets/db/secrets_data/__init__.py,sha256=Eg1RLncl2MDORsBgRruur3n1JAWyjyzX1FMTuF2uCx0,360
 ark_sdk_python/models/services/dpa/secrets/db/secrets_data/ark_dpa_db_user_password_secret_data.py,sha256=d-BYEzQsqd8XNi7GrkxYyZ2jNQJZVnhMKU7NLFoNBtw,650
-ark_sdk_python/models/services/dpa/sso/__init__.py,sha256=1kjq9ajLQ3y4W2T0wirazKfN7F-zNhEIqJqS-RH-OaE,928
+ark_sdk_python/models/services/dpa/sso/__init__.py,sha256=idXyQsCwN1tqNZDEbWBJTWF7SmmmScBtweVEqgOrVdU,1033
 ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_acquire_token_response.py,sha256=pGlxZw-SXqpMHdPQx06HCP6ueVdx3H2dMArWIxEpZ5E,277
 ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_client_certificate.py,sha256=sk6QNlrPWNNnSIU457GJuvGGbPLsTMjfkzqDer20NHw,942
 ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_oracle_wallet.py,sha256=CjZlRvlKkuGLMoUVVjlrXnt8vnthN8Bc_hEbvI__Hy0,731
 ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_password.py,sha256=t3o0ZTJUyRf66IgZB5ZJncOnVgcEqIgYczeWqM7Vh3U,215
 ark_sdk_python/models/services/dpa/sso/ark_dpa_sso_get_short_lived_rdp_file.py,sha256=nmWVpq5WfHUPDZmUTxgcN7QLiLqIC81fbeQI0fGT0-E,703
 ark_sdk_python/models/services/dpa/workspaces/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ark_sdk_python/models/services/dpa/workspaces/db/__init__.py,sha256=KFcZgfNDY5lwlALSj6j98j9lNFwP2HLuECbfohyuZPw,2080
-ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_add_database.py,sha256=QVrqW58j568J7Gxsa_aWAJIpFZJnTmWCimiPrfTPFQ4,2658
+ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_add_database.py,sha256=RlAy_sgSm2pYQnpcaF5n7SVv5vZvwgmxJGhPXS_pSps,3082
 ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_database.py,sha256=Dhjgaeh64272rSFDaKDPkCKC5msBbtCcoRPW7awqOdk,2644
 ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_database_info.py,sha256=qH8wnX7_jg1IY1mJG6kzO4hbnow-AEOE3HUqDywNUV0,1835
 ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_databases_filter.py,sha256=fxIpN9WAvQwD6CC-BZ0e7IudD9HuvWW_kJAORQfDZ-w,1135
 ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_databases_stats.py,sha256=uFeh3-TsBDAso6wgFl-EW0P7RWxoXtQFLqNZlp_fRnM,1246
 ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_delete_database.py,sha256=1mnT_4YlPKNnyZ3gd4abU8gqX_ZflpjOaktpLBDP4TU,583
 ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_get_database.py,sha256=7weIU4a83-GcVExzBu_hxFZ3-4fj3joEW-HSjMNI-xY,574
 ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_platform_type_serializer.py,sha256=7Lzyqu89mzIVgakpzP3-kGvunAojoaEP8I7vzhc3Ryk,558
-ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_provider.py,sha256=W67y2RqLGJkqcmaS_41yE_6AU3lVlM8MqOpVonkjJPU,3785
+ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_provider.py,sha256=JnsJvXO9p24BMKZld_tP2D5t9Uonu9jkYo6QN6UcvKY,4041
 ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_tag.py,sha256=qgpffuMUvC6qCZoT3Xo3-LLPbbBRwPPd4GpLYzM4OqY,490
-ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_update_database.py,sha256=yOK3HKlQjRNAD25alfAAfd2A1dg9q3Obg3FFe72r6jc,2989
+ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_update_database.py,sha256=WxVdMabhZjee8WMNfFYlcwe3iGJmo45J4YBthHdkkTY,3413
 ark_sdk_python/models/services/dpa/workspaces/db/ark_dpa_db_warning.py,sha256=bJ3-WkMTqNBIP92t8nA28oLUZkq70Lmit4gaoYSg8yg,153
 ark_sdk_python/models/services/sm/__init__.py,sha256=dJ8-e7AwH08LqIgnAW1l00QcAGVEJ5nM6Ra1p5ua1ZQ,1255
 ark_sdk_python/models/services/sm/ark_sm_get_session.py,sha256=Xn5uTDFa6ldmdMbxEN1SdPnLFVz0lAy69ulMATjIXOM,167
 ark_sdk_python/models/services/sm/ark_sm_get_session_activities.py,sha256=t4GruuZksfKEOmecHsYPqQfUAFvnBpnPYZyHiYXiyp8,196
 ark_sdk_python/models/services/sm/ark_sm_protocol_type_serializer.py,sha256=6JoQ7sKA6qEuh6J5-JUQAM7Wr4bXLR8u8fxvwLK7lds,812
 ark_sdk_python/models/services/sm/ark_sm_session.py,sha256=GZd3wXM6YEQwNkNONZVkwxswpCR1R94IXZbEUyMj6pY,2195
 ark_sdk_python/models/services/sm/ark_sm_session_activity.py,sha256=4bOJTDFwjHvgN9EBloTgTOqOd_C9QSx9Now8S0hWYSM,1689
@@ -218,15 +221,15 @@
 ark_sdk_python/services/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 ark_sdk_python/services/ark_service.py,sha256=HzO6_qgHDDqMc9bYdQWSr4ErmYn1A9C-ZFEiBgrsIgY,2314
 ark_sdk_python/services/dpa/__init__.py,sha256=-O9w5IkNF-DU3Qccd5-Iva8I_UYGG-tcl1mDhcU9sAE,87
 ark_sdk_python/services/dpa/ark_dpa_api.py,sha256=dF0Au5di0bBoJxsSwO56VNrvcmzcrcla9gcncQLNHMY,3077
 ark_sdk_python/services/dpa/certificates/__init__.py,sha256=qDNBt2FvhbCltfdQogwul4Hi8EGFMIrItTuMlMQdu_Q,149
 ark_sdk_python/services/dpa/certificates/ark_dpa_certificates_service.py,sha256=G0qxEeAmrjfQDNIiHnz32HAfKzrEkYD8yke-N4E9fdU,7989
 ark_sdk_python/services/dpa/db/__init__.py,sha256=wznIh6-QjWLNHGKULu1a1z8HQ0poWlrb9w_vKIjm9W4,116
-ark_sdk_python/services/dpa/db/ark_dpa_db_service.py,sha256=y6LTq6dQKsFwj7mDIXlPHzDzB6qQjZY5SXKeMO3CSXU,9080
+ark_sdk_python/services/dpa/db/ark_dpa_db_service.py,sha256=dBpQabBfYYGHhibAK53DnoNsTt2oWSQ7u6k1UQIe8gM,10634
 ark_sdk_python/services/dpa/k8s/__init__.py,sha256=lb9DrpSJUUhqXhFjd22-7UN4sjiwzV7LXS3Z89ViLjE,113
 ark_sdk_python/services/dpa/k8s/ark_dpa_k8s_service.py,sha256=61fYi26ZnJBAqWU3Rq5DybdYGZ5TKuyNYN1XOsGXXVg,2286
 ark_sdk_python/services/dpa/policies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ark_sdk_python/services/dpa/policies/db/__init__.py,sha256=Oo-NYG3bxGQnw0St260bi859ORve3gS-0YBcbZmIchE,143
 ark_sdk_python/services/dpa/policies/db/ark_dpa_db_policies_service.py,sha256=WnXX1wN4imddv0mXvbHp4RO5w-ZWumERrpnXZKPyH2M,10943
 ark_sdk_python/services/dpa/policies/vm/__init__.py,sha256=9nCR_0LNVcpVQJkyZpkhQ0alWU3Si04bytvnrSKU79g,143
 ark_sdk_python/services/dpa/policies/vm/ark_dpa_vm_policies_service.py,sha256=ba2m2s_UyFeg2mJf1Qh592j43bvM3EFWs4G1o2RVWh0,12681
@@ -236,13 +239,13 @@
 ark_sdk_python/services/dpa/sso/__init__.py,sha256=cHLin78PGJOQjhvESsycXZlcMvnMM00GGDHbeI8awww,120
 ark_sdk_python/services/dpa/sso/ark_dpa_sso_service.py,sha256=otIcdvaEKDk1MveoD1XZQfMAN9YfnDMlPY-DCI5wJIE,15817
 ark_sdk_python/services/dpa/workspaces/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ark_sdk_python/services/dpa/workspaces/db/__init__.py,sha256=KsaQ50bkHsBx0QLUCr6qiQVb9CohGvSeL9Y4-DReWrc,148
 ark_sdk_python/services/dpa/workspaces/db/ark_dpa_db_workspace_service.py,sha256=yT453tQaxe9DeoO9Z0T4cLHX2ANDzNKeBuL5DNxjjdk,11192
 ark_sdk_python/services/sm/__init__.py,sha256=jzKxEkZYOCW9y_byLfd_odae9m2sh1UfjaaKBVySWY0,95
 ark_sdk_python/services/sm/ark_sm_service.py,sha256=8OYHHrIKVDcpcSOomXQBRW2ReNDn7Bd1FY1N_rNsEKA,11400
-ark_sdk_python-1.0.6.dist-info/LICENSE.txt,sha256=tog-p2RGDyKF8f75MfD9FcNnzH4nXVVQpYMrKq8-CTI,11358
-ark_sdk_python-1.0.6.dist-info/METADATA,sha256=KvtTXSNvAWIKejmygkLPYS-AHhxDzHyeAMsyhiu3E8I,17726
-ark_sdk_python-1.0.6.dist-info/NOTICES.md,sha256=5W8-D3unkf27Oz4j86dawLYLkg72KX_R-q4IrHJozbQ,95918
-ark_sdk_python-1.0.6.dist-info/WHEEL,sha256=M4g2KOPqPuBDzs4fXhen7cAP8dzQGHxeSKE5kd7ZmZE,108
-ark_sdk_python-1.0.6.dist-info/entry_points.txt,sha256=v5bcuRn8w42ZKQspfvX3AliKmLVO6f7Zb_bma77p3vQ,47
-ark_sdk_python-1.0.6.dist-info/RECORD,,
+ark_sdk_python-1.0.7.dist-info/LICENSE.txt,sha256=tog-p2RGDyKF8f75MfD9FcNnzH4nXVVQpYMrKq8-CTI,11358
+ark_sdk_python-1.0.7.dist-info/METADATA,sha256=Yys39SDs0DR39PaHgyLxppeGDMUMOUmHLLD4SGIPy24,17728
+ark_sdk_python-1.0.7.dist-info/NOTICES.md,sha256=5W8-D3unkf27Oz4j86dawLYLkg72KX_R-q4IrHJozbQ,95918
+ark_sdk_python-1.0.7.dist-info/WHEEL,sha256=M4g2KOPqPuBDzs4fXhen7cAP8dzQGHxeSKE5kd7ZmZE,108
+ark_sdk_python-1.0.7.dist-info/entry_points.txt,sha256=v5bcuRn8w42ZKQspfvX3AliKmLVO6f7Zb_bma77p3vQ,47
+ark_sdk_python-1.0.7.dist-info/RECORD,,
```

## Comparing `ark_sdk_python-1.0.6.dist-info/METADATA` & `ark_sdk_python-1.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ark-sdk-python
-Version: 1.0.6
+Version: 1.0.7
 Summary: Official Ark SDK / CLI for CyberArk Identity Security Platform
 Home-page: https://github.com/cyberark/ark-sdk-python
 License: Apache-2.0
 Author: CyberArk
 Author-email: cyberark@cyberark.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -20,23 +20,23 @@
 Requires-Dist: aenum
 Requires-Dist: argcomplete
 Requires-Dist: cachetools
 Requires-Dist: colorama
 Requires-Dist: deepdiff
 Requires-Dist: dill
 Requires-Dist: fake-useragent
-Requires-Dist: humps
 Requires-Dist: inquirer
 Requires-Dist: keyring
 Requires-Dist: keyrings.cryptfile
 Requires-Dist: overrides
 Requires-Dist: packaging
 Requires-Dist: progress
 Requires-Dist: pycryptodome
 Requires-Dist: pydantic (==1.10.*)
+Requires-Dist: pyhumps
 Requires-Dist: python-dateutil
 Requires-Dist: python-jose[cryptography]
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: retry
 Requires-Dist: tzlocal
 Requires-Dist: urlextract
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: ark-sdk-python Version: 1.0.6 Summary: Official Ark
+Metadata-Version: 2.1 Name: ark-sdk-python Version: 1.0.7 Summary: Official Ark
 SDK / CLI for CyberArk Identity Security Platform Home-page: https://
 github.com/cyberark/ark-sdk-python License: Apache-2.0 Author: CyberArk Author-
 email: cyberark@cyberark.com Requires-Python: >=3.8,<4.0 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aenum Requires-Dist: argcomplete Requires-Dist:
 cachetools Requires-Dist: colorama Requires-Dist: deepdiff Requires-Dist: dill
-Requires-Dist: fake-useragent Requires-Dist: humps Requires-Dist: inquirer
-Requires-Dist: keyring Requires-Dist: keyrings.cryptfile Requires-Dist:
-overrides Requires-Dist: packaging Requires-Dist: progress Requires-Dist:
-pycryptodome Requires-Dist: pydantic (==1.10.*) Requires-Dist: python-dateutil
+Requires-Dist: fake-useragent Requires-Dist: inquirer Requires-Dist: keyring
+Requires-Dist: keyrings.cryptfile Requires-Dist: overrides Requires-Dist:
+packaging Requires-Dist: progress Requires-Dist: pycryptodome Requires-Dist:
+pydantic (==1.10.*) Requires-Dist: pyhumps Requires-Dist: python-dateutil
 Requires-Dist: python-jose[cryptography] Requires-Dist: pyyaml Requires-Dist:
 requests Requires-Dist: retry Requires-Dist: tzlocal Requires-Dist: urlextract
 Project-URL: Repository, https://github.com/cyberark/ark-sdk-python
 Description-Content-Type: text/markdown ![Ark SDK Python](https://github.com/
 cyberark/ark-sdk-python/blob/main/assets/sdk.png)
         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_a_c_t_i_o_n_s_-
  _b_a_d_g_e_._a_t_r_o_x_._d_e_v_%_2_F_c_y_b_e_r_a_r_k_%_2_F_a_r_k_-_s_d_k_-_p_y_t_h_o_n_%_2_F_b_a_d_g_e_%_3_F_r_e_f_%_3_D_m_a_i_n_&_s_t_y_l_e_=_f_l_a_t_]
```

## Comparing `ark_sdk_python-1.0.6.dist-info/NOTICES.md` & `ark_sdk_python-1.0.7.dist-info/NOTICES.md`

 * *Files identical despite different names*

## Comparing `ark_sdk_python-1.0.6.dist-info/LICENSE.txt` & `ark_sdk_python-1.0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

