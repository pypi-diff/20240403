# Comparing `tmp/imap-tools-1.5.0.tar.gz` & `tmp/imap-tools-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imap-tools-1.5.0.tar", last modified: Mon Nov 13 09:43:21 2023, max compression
+gzip compressed data, was "dist\imap-tools-1.6.0.tar", last modified: Wed Apr  3 18:58:31 2024, max compression
```

## Comparing `imap-tools-1.5.0.tar` & `imap-tools-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-11-13 09:43:21.000000 imap-tools-1.5.0/
-drwxrwxrwx   0        0        0        0 2023-11-13 09:43:21.000000 imap-tools-1.5.0/imap_tools/
--rw-rw-rw-   0        0        0     1251 2023-11-13 09:00:27.000000 imap-tools-1.5.0/imap_tools/consts.py
--rw-rw-rw-   0        0        0     2109 2022-02-15 11:27:46.000000 imap-tools-1.5.0/imap_tools/errors.py
--rw-rw-rw-   0        0        0     7084 2023-08-01 05:51:47.000000 imap-tools-1.5.0/imap_tools/folder.py
--rw-rw-rw-   0        0        0     4465 2022-11-21 11:14:06.000000 imap-tools-1.5.0/imap_tools/idle.py
--rw-rw-rw-   0        0        0     2059 2021-09-20 07:00:52.000000 imap-tools-1.5.0/imap_tools/imap_utf7.py
--rw-rw-rw-   0        0        0    16387 2023-10-04 10:19:33.000000 imap-tools-1.5.0/imap_tools/mailbox.py
--rw-rw-rw-   0        0        0    11302 2023-11-13 09:39:14.000000 imap-tools-1.5.0/imap_tools/message.py
--rw-rw-rw-   0        0        0        0 2023-08-01 05:49:19.000000 imap-tools-1.5.0/imap_tools/py.typed
--rw-rw-rw-   0        0        0    16320 2022-08-31 05:00:37.000000 imap-tools-1.5.0/imap_tools/query.py
--rw-rw-rw-   0        0        0     7878 2023-10-10 04:28:38.000000 imap-tools-1.5.0/imap_tools/utils.py
--rw-rw-rw-   0        0        0      576 2023-11-13 09:15:18.000000 imap-tools-1.5.0/imap_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 09:43:21.000000 imap-tools-1.5.0/imap_tools.egg-info/
--rw-rw-rw-   0        0        0        1 2023-11-13 09:43:21.000000 imap-tools-1.5.0/imap_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    20801 2023-11-13 09:43:21.000000 imap-tools-1.5.0/imap_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2023-11-13 09:43:21.000000 imap-tools-1.5.0/imap_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2023-11-13 09:43:21.000000 imap-tools-1.5.0/imap_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11548 2019-10-23 05:52:39.000000 imap-tools-1.5.0/LICENSE
--rw-rw-rw-   0        0        0       56 2021-01-28 06:25:19.000000 imap-tools-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0    20801 2023-11-13 09:43:21.000000 imap-tools-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    20291 2023-11-13 09:09:21.000000 imap-tools-1.5.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-11-13 09:43:21.000000 imap-tools-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-08-01 05:49:19.000000 imap-tools-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:58:31.000000 imap-tools-1.6.0/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:58:31.000000 imap-tools-1.6.0/imap_tools/
+-rw-rw-rw-   0        0        0     1253 2024-04-03 18:52:27.000000 imap-tools-1.6.0/imap_tools/consts.py
+-rw-rw-rw-   0        0        0     2109 2022-02-15 11:27:46.000000 imap-tools-1.6.0/imap_tools/errors.py
+-rw-rw-rw-   0        0        0     7080 2024-04-03 18:52:27.000000 imap-tools-1.6.0/imap_tools/folder.py
+-rw-rw-rw-   0        0        0     4465 2022-11-21 11:14:06.000000 imap-tools-1.6.0/imap_tools/idle.py
+-rw-rw-rw-   0        0        0     2069 2024-04-03 18:52:27.000000 imap-tools-1.6.0/imap_tools/imap_utf7.py
+-rw-rw-rw-   0        0        0    17611 2024-04-03 18:52:27.000000 imap-tools-1.6.0/imap_tools/mailbox.py
+-rw-rw-rw-   0        0        0    11302 2023-11-13 09:39:14.000000 imap-tools-1.6.0/imap_tools/message.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:49:19.000000 imap-tools-1.6.0/imap_tools/py.typed
+-rw-rw-rw-   0        0        0    16320 2022-08-31 05:00:37.000000 imap-tools-1.6.0/imap_tools/query.py
+-rw-rw-rw-   0        0        0     9617 2024-04-03 18:52:27.000000 imap-tools-1.6.0/imap_tools/utils.py
+-rw-rw-rw-   0        0        0      590 2024-04-03 18:52:27.000000 imap-tools-1.6.0/imap_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:58:31.000000 imap-tools-1.6.0/imap_tools.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-03 18:58:31.000000 imap-tools-1.6.0/imap_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    21233 2024-04-03 18:58:31.000000 imap-tools-1.6.0/imap_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-04-03 18:58:31.000000 imap-tools-1.6.0/imap_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 18:58:31.000000 imap-tools-1.6.0/imap_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11548 2019-10-23 05:52:39.000000 imap-tools-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0       56 2021-01-28 06:25:19.000000 imap-tools-1.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    21233 2024-04-03 18:58:31.000000 imap-tools-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    20723 2024-04-03 18:57:06.000000 imap-tools-1.6.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-03 18:58:31.000000 imap-tools-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-08-01 05:49:19.000000 imap-tools-1.6.0/setup.py
```

### Comparing `imap-tools-1.5.0/imap_tools/consts.py` & `imap-tools-1.6.0/imap_tools/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 SHORT_MONTH_NAMES = ('Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec')
 
 UID_PATTERN = re.compile(r'(^|\s+|\W)UID\s+(?P<uid>\d+)')
 
 CODECS_OFFICIAL_REPLACEMENT_CHAR = '�'
 
+
 class MailMessageFlags:
     """
     System email message flags
     All system flags begin with "\"
     """
     SEEN = '\\Seen'
     ANSWERED = '\\Answered'
```

### Comparing `imap-tools-1.5.0/imap_tools/errors.py` & `imap-tools-1.6.0/imap_tools/errors.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.5.0/imap_tools/folder.py` & `imap-tools-1.6.0/imap_tools/folder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import AnyStr, Optional, Iterable, List, Dict, Tuple
 
-from . import imap_utf7
+from .imap_utf7 import utf7_decode
 from .consts import MailBoxFolderStatusOptions
 from .utils import check_command_status, pairs_to_dict, encode_folder
 from .errors import MailboxFolderStatusValueError, MailboxFolderSelectError, MailboxFolderCreateError, \
     MailboxFolderRenameError, MailboxFolderDeleteError, MailboxFolderStatusError, MailboxFolderSubscribeError
 
 
 class FolderInfo:
@@ -121,28 +121,28 @@
             command, encode_folder(folder), encode_folder(search_args))
         typ, data = self.mailbox.client._untagged_response(typ, data, command)
         result = []
         for folder_item in data:
             if not folder_item:
                 continue
             if type(folder_item) is bytes:
-                folder_match = re.search(folder_item_re, imap_utf7.decode(folder_item))
+                folder_match = re.search(folder_item_re, utf7_decode(folder_item))
                 if not folder_match:
                     continue
                 folder_dict = folder_match.groupdict()
                 name = folder_dict['name']
                 if name.startswith('"') and name.endswith('"'):
                     name = name[1:-1]
             elif type(folder_item) is tuple:
                 # when name has " or \ chars
-                folder_match = re.search(folder_item_re, imap_utf7.decode(folder_item[0]))
+                folder_match = re.search(folder_item_re, utf7_decode(folder_item[0]))
                 if not folder_match:
                     continue
                 folder_dict = folder_match.groupdict()
-                name = imap_utf7.decode(folder_item[1])
+                name = utf7_decode(folder_item[1])
             else:
                 continue
             result.append(FolderInfo(
                 name=name,
                 delim=folder_dict['delim'].replace('"', ''),
                 flags=tuple(folder_dict['flags'].split())  # noqa,
             ))
```

### Comparing `imap-tools-1.5.0/imap_tools/idle.py` & `imap-tools-1.6.0/imap_tools/idle.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.5.0/imap_tools/imap_utf7.py` & `imap-tools-1.6.0/imap_tools/imap_utf7.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def _do_b64(_in: Iterable[str], r: MutableSequence[bytes]):
     if _in:
         r.append(b'&' + _modified_base64(''.join(_in)) + b'-')
     del _in[:]
 
 
-def encode(value: str) -> bytes:
+def utf7_encode(value: str) -> bytes:
     res = []
     _in = []
     for char in value:
         ord_c = ord(char)
         if 0x20 <= ord_c <= 0x25 or 0x27 <= ord_c <= 0x7e:
             _do_b64(_in, res)
             res.append(char.encode())
@@ -42,15 +42,15 @@
 
 # DECODING
 # --------
 def _modified_unbase64(value: bytearray) -> str:
     return binascii.a2b_base64(value.replace(b',', b'/') + b'===').decode('utf-16be')
 
 
-def decode(value: bytes) -> str:
+def utf7_decode(value: bytes) -> str:
     res = []
     decode_arr = bytearray()
     for char in value:
         if char == ord('&') and not decode_arr:
             decode_arr.append(ord('&'))
         elif char == ord('-') and decode_arr:
             if len(decode_arr) == 1:
```

### Comparing `imap-tools-1.5.0/imap_tools/mailbox.py` & `imap-tools-1.6.0/imap_tools/mailbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import datetime
 from collections import UserString
 from typing import AnyStr, Optional, List, Iterable, Sequence, Union, Tuple, Iterator
 
 from .message import MailMessage
 from .folder import MailBoxFolderManager
 from .idle import IdleManager
-from .utils import clean_uids, check_command_status, chunks, encode_folder, clean_flags, check_timeout_arg_support
+from .utils import clean_uids, check_command_status, chunks, encode_folder, clean_flags, check_timeout_arg_support, \
+    chunks_crop
 from .errors import MailboxStarttlsError, MailboxLoginError, MailboxLogoutError, MailboxNumbersError, \
     MailboxFetchError, MailboxExpungeError, MailboxDeleteError, MailboxCopyError, MailboxFlagError, \
     MailboxAppendError, MailboxUidsError, MailboxTaggedResponseError
 
 # Maximal line length when calling readline(). This is to prevent reading arbitrary length lines.
 # 20Mb is enough for search response with about 2 000 000 message numbers
 imaplib._MAXLINE = 20 * 1024 * 1024  # 20Mb
@@ -104,65 +105,90 @@
         :return email message numbers
         """
         encoded_criteria = criteria if type(criteria) is bytes else str(criteria).encode(charset)
         search_result = self.client.search(charset, encoded_criteria)
         check_command_status(search_result, MailboxNumbersError)
         return search_result[1][0].decode().split() if search_result[1][0] else []
 
-    def uids(self, criteria: Criteria = 'ALL', charset: str = 'US-ASCII') -> List[str]:
+    def uids(self, criteria: Criteria = 'ALL', charset: str = 'US-ASCII',
+             sort: Optional[Union[str, Iterable[str]]] = None) -> List[str]:
         """
         Search mailbox for matching message uids in current folder
         :param criteria: message search criteria (see examples at ./doc/imap_search_criteria.txt)
         :param charset: IANA charset, indicates charset of the strings that appear in the search criteria. See rfc2978
+        :param sort: criteria for sort messages on server, use SortCriteria constants. Charset arg is important for sort
         :return: email message uids
         """
         encoded_criteria = criteria if type(criteria) is bytes else str(criteria).encode(charset)
-        uid_result = self.client.uid('SEARCH', 'CHARSET', charset, encoded_criteria)
+        if sort:
+            sort = (sort,) if isinstance(sort, str) else sort
+            uid_result = self.client.uid('SORT', '({})'.format(' '.join(sort)), charset, encoded_criteria)
+        else:
+            uid_result = self.client.uid('SEARCH', 'CHARSET', charset, encoded_criteria)  # *charset are opt here
         check_command_status(uid_result, MailboxUidsError)
         return uid_result[1][0].decode().split() if uid_result[1][0] else []
 
-    def _fetch_by_one(self, uid_list: Sequence[str], message_parts: str, reverse: bool) -> Iterator[list]:  # noqa
+    def _fetch_by_one(self, uid_list: Sequence[str], message_parts: str) -> Iterator[list]:
         for uid in uid_list:
             fetch_result = self.client.uid('fetch', uid, message_parts)
             check_command_status(fetch_result, MailboxFetchError)
             if not fetch_result[1] or fetch_result[1][0] is None:
                 continue
             yield fetch_result[1]
 
-    def _fetch_in_bulk(self, uid_list: Sequence[str], message_parts: str, reverse: bool) -> Iterator[list]:
+    def _fetch_in_bulk(self, uid_list: Sequence[str], message_parts: str, reverse: bool, bulk: int) \
+            -> Iterator[list]:
         if not uid_list:
             return
-        fetch_result = self.client.uid('fetch', ','.join(uid_list), message_parts)
-        check_command_status(fetch_result, MailboxFetchError)
-        if not fetch_result[1] or fetch_result[1][0] is None:
-            return
-        for built_fetch_item in chunks((reversed if reverse else iter)(fetch_result[1]), 2):
-            yield built_fetch_item
+
+        if isinstance(bulk, int) and bulk >= 2:
+            uid_list_seq = chunks_crop(uid_list, bulk)
+        elif isinstance(bulk, bool):
+            uid_list_seq = (uid_list,)
+        else:
+            raise ValueError('bulk arg may be bool or int >= 2')
+
+        for uid_list_i in uid_list_seq:
+            fetch_result = self.client.uid('fetch', ','.join(uid_list_i), message_parts)
+            check_command_status(fetch_result, MailboxFetchError)
+            if not fetch_result[1] or fetch_result[1][0] is None:
+                return
+            for built_fetch_item in chunks((reversed if reverse else iter)(fetch_result[1]), 2):
+                yield built_fetch_item
 
     def fetch(self, criteria: Criteria = 'ALL', charset: str = 'US-ASCII', limit: Optional[Union[int, slice]] = None,
-              mark_seen=True, reverse=False, headers_only=False, bulk=False) -> Iterator[MailMessage]:
+              mark_seen=True, reverse=False, headers_only=False, bulk: Union[bool, int] = False,
+              sort: Optional[Union[str, Iterable[str]]] = None) \
+            -> Iterator[MailMessage]:
         """
         Mail message generator in current folder by search criteria
         :param criteria: message search criteria (see examples at ./doc/imap_search_criteria.txt)
         :param charset: IANA charset, indicates charset of the strings that appear in the search criteria. See rfc2978
         :param limit: int | slice - limit number of read emails | slice emails range for read
                       useful for actions with a large number of messages, like "move" | paging
         :param mark_seen: mark emails as seen on fetch
         :param reverse: in order from the larger date to the smaller
         :param headers_only: get only email headers (without text, html, attachments)
-        :param bulk: False - fetch each message separately per N commands - low memory consumption, slow
-                     True  - fetch all messages per 1 command - high memory consumption, fast
+        :param bulk:
+            False - fetch each message separately per N commands - low memory consumption, slow
+            True  - fetch all messages per 1 command - high memory consumption, fast. Fails on big bulk at server
+            int - fetch messages by bulks of the specified size
+        :param sort: criteria for sort messages on server, use SortCriteria constants. Charset arg is important for sort
         :return generator: MailMessage
         """
         message_parts = "(BODY{}[{}] UID FLAGS RFC822.SIZE)".format(
             '' if mark_seen else '.PEEK', 'HEADER' if headers_only else '')
         limit_range = slice(0, limit) if type(limit) is int else limit or slice(None)
         assert type(limit_range) is slice
-        uids = tuple((reversed if reverse else iter)(self.uids(criteria, charset)))[limit_range]
-        for fetch_item in (self._fetch_in_bulk if bulk else self._fetch_by_one)(uids, message_parts, reverse):  # noqa
+        uids = tuple((reversed if reverse else iter)(self.uids(criteria, charset, sort)))[limit_range]
+        if bulk:
+            message_generator = self._fetch_in_bulk(uids, message_parts, reverse, bulk)
+        else:
+            message_generator = self._fetch_by_one(uids, message_parts)
+        for fetch_item in message_generator:
             yield self.email_message_class(fetch_item)
 
     def expunge(self) -> tuple:
         result = self.client.expunge()
         check_command_status(result, MailboxExpungeError)
         return result
```

### Comparing `imap-tools-1.5.0/imap_tools/message.py` & `imap-tools-1.6.0/imap_tools/message.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.5.0/imap_tools/query.py` & `imap-tools-1.6.0/imap_tools/query.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.5.0/imap_tools/utils.py` & `imap-tools-1.6.0/imap_tools/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime
 from itertools import zip_longest
 from email.utils import getaddresses, parsedate_to_datetime
 from email.header import decode_header, Header
 from typing import AnyStr, Union, Optional, Tuple, Iterable, Any, List, Dict, Iterator
 
 from .consts import SHORT_MONTH_NAMES, MailMessageFlags
-from . import imap_utf7
+from .imap_utf7 import utf7_encode
 
 
 def clean_uids(uid_set: Union[str, Iterable[str]]) -> str:
     """
     Prepare set of uid for use in IMAP commands
     uid RE patterns are not strict and allow invalid combinations, but simple. Example: 2,4:7,9,12:*
     :param uid_set:
@@ -166,15 +166,15 @@
 
 
 def encode_folder(folder: AnyStr) -> bytes:
     """Encode folder name"""
     if isinstance(folder, bytes):
         return folder
     else:
-        return quote(imap_utf7.encode(folder))
+        return quote(utf7_encode(folder))
 
 
 def clean_flags(flag_set: Union[str, Iterable[str]]) -> List[str]:
     """
     Check the correctness of the flags
     :return: list of str - flags
     """
@@ -199,7 +199,59 @@
     """Replace charset in META tag with content-type attribute in HTML text"""
     meta_ct_match = re.search(r'<\s*meta .*?content-type.*?>', html, re.IGNORECASE | re.DOTALL)
     if meta_ct_match:
         meta = meta_ct_match.group(0)
         meta_new = re.sub(r'charset\s*=\s*[a-zA-Z0-9_:.+-]+', 'charset={}'.format(new_charset), meta, 1, re.IGNORECASE)
         html = html.replace(meta, meta_new)
     return html
+
+
+def chunks_crop(lst: iter, n: int) -> iter:
+    """
+    Yield successive n-sized chunks from lst.
+    import pprint
+    pprint.pprint(list(chunks(range(10, 75), 10)))
+    [[10, 11, 12, 13, 14, 15, 16, 17, 18, 19],
+     [20, 21, 22, 23, 24, 25, 26, 27, 28, 29],
+     [30, 31, 32, 33, 34, 35, 36, 37, 38, 39],
+     [40, 41, 42, 43, 44, 45, 46, 47, 48, 49],
+     [50, 51, 52, 53, 54, 55, 56, 57, 58, 59],
+     [60, 61, 62, 63, 64, 65, 66, 67, 68, 69],
+     [70, 71, 72, 73, 74]]
+    """
+    for i in range(0, len(lst), n):
+        yield lst[i:i + n]
+
+
+class SortCriteria:
+    """
+    Sort criteria
+    https://datatracker.ietf.org/doc/html/rfc5256
+    ARRIVAL - Internal date and time of the message.
+        This differs from the ON criteria in SEARCH, which uses just the internal date.
+    CC - [IMAP] addr-mailbox of the first "cc" address.
+    DATE - Sent date and time, as described in section 2.2.
+    FROM - [IMAP] addr-mailbox of the first "From" address.
+    SIZE - Size of the message in octets.
+    SUBJECT - Base subject text.
+    TO - [IMAP] addr-mailbox of the first "To" address.
+    """
+    ARRIVAL_DT_ASC = 'ARRIVAL'
+    CC_ASC = 'CC'
+    DATE_ASC = 'DATE'
+    FROM_ASC = 'FROM'
+    SIZE_ASC = 'SIZE'
+    SUBJECT_ASC = 'SUBJECT'
+    TO_ASC = 'TO'
+
+    ARRIVAL_DT_DESC = 'REVERSE ARRIVAL'
+    CC_DESC = 'REVERSE CC'
+    DATE_DESC = 'REVERSE DATE'
+    FROM_DESC = 'REVERSE FROM'
+    SIZE_DESC = 'REVERSE SIZE'
+    SUBJECT_DESC = 'REVERSE SUBJECT'
+    TO_DESC = 'REVERSE TO'
+
+    all = (
+        ARRIVAL_DT_ASC, CC_ASC, DATE_ASC, FROM_ASC, SIZE_ASC, SUBJECT_ASC, TO_ASC,
+        ARRIVAL_DT_DESC, CC_DESC, DATE_DESC, FROM_DESC, SIZE_DESC, SUBJECT_DESC, TO_DESC,
+    )
```

### Comparing `imap-tools-1.5.0/imap_tools.egg-info/PKG-INFO` & `imap-tools-1.6.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: imap-tools
-Version: 1.5.0
-Summary: Work with email by IMAP
-Home-page: https://github.com/ikvk/imap_tools
-Author: Vladimir Kaukin
-Author-email: KaukinVK@ya.ru
-License: Apache-2.0
-Keywords: imap,imap-client,python3,python,email
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 .. http://docutils.sourceforge.net/docs/user/rst/quickref.html
 
 .. |nbsp| unicode:: 0xA0
    :trim:
 
 imap_tools 📧
 =============
@@ -38,14 +22,15 @@
 ===============  ================================================================================================
 Python version   3.5+
 License          Apache-2.0
 PyPI             https://pypi.python.org/pypi/imap_tools/
 RFC              `IMAP4.1 <https://tools.ietf.org/html/rfc3501>`_,
                  `EMAIL <https://tools.ietf.org/html/rfc2822>`_,
                  `IMAP related RFCs <https://github.com/ikvk/imap_tools/blob/master/docs/IMAP_related_RFCs.txt>`_
+Repo mirror      https://gitflic.ru/project/ikvk/imap-tools
 ===============  ================================================================================================
 
 .. contents::
 
 Installation
 ------------
 ::
@@ -75,19 +60,20 @@
 
 BaseMailBox.<auth> - login, login_utf8, xoauth2, logout - authentication functions, they support context manager.
 
 BaseMailBox.fetch - first searches email uids by criteria in current folder, then fetch and yields `MailMessage <#email-attributes>`_, args:
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
-* *limit* = None, limit on the number of read emails, useful for actions with a large number of messages, like "move"
+* *limit* = None, limit on the number of read emails, useful for actions with a large number of messages, like "move". May be int or slice.
 * *mark_seen* = True, mark emails as seen on fetch
 * *reverse* = False, in order from the larger date to the smaller
 * *headers_only* = False, get only email headers (without text, html, attachments)
-* *bulk* = False, False - fetch each message separately per N commands - low memory consumption, slow; True - fetch all messages per 1 command - high memory consumption, fast
+* *bulk* = False, False - fetch each message separately per N commands - low memory consumption, slow; True - fetch all messages per 1 command - high memory consumption, fast; int - fetch all messages by bulks of the specified size, for 20 messages and bulk=5 -> 4 commands
+* *sort* = None, criteria for sort messages on server, use SortCriteria constants. Charset arg is important for sort
 
 BaseMailBox.uids - search mailbox for matching message uids in current folder, returns [str | None], None when MailMessage.from_bytes used, args:
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
 
 BaseMailBox.<action> - `copy, move, delete, flag, append <#actions-with-emails>`_
@@ -420,17 +406,18 @@
 `NickC-NZ <https://github.com/NickC-NZ>`_,
 `mweinelt <https://github.com/mweinelt>`_,
 `lucbouge <https://github.com/lucbouge>`_,
 `JacquelinCharbonnel <https://github.com/JacquelinCharbonnel>`_,
 `stumpylog <https://github.com/stumpylog>`_,
 `dimitrisstr <https://github.com/dimitrisstr>`_,
 `abionics <https://github.com/abionics>`_,
-`link2xt <https://github.com/link2xt>`_
+`link2xt <https://github.com/link2xt>`_,
+`Docpart <https://github.com/Docpart>`_,
+`meetttttt <https://github.com/meetttttt>`_,
+`sapristi <https://github.com/sapristi>`_
 
 Help the project
 ----------------
 1. Found a bug or figure out how to improve the library - open issue or merge request 🎯
 2. Do not know how to improve library - try to help other open projects that you use ✋
 3. Nowhere to put your money - spend it on your family, friends, loved ones, or people around you 💰
 4. Star the project ⭐
-
-
```

### Comparing `imap-tools-1.5.0/LICENSE` & `imap-tools-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imap-tools-1.5.0/PKG-INFO` & `imap-tools-1.6.0/imap_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap-tools
-Version: 1.5.0
+Version: 1.6.0
 Summary: Work with email by IMAP
 Home-page: https://github.com/ikvk/imap_tools
 Author: Vladimir Kaukin
 Author-email: KaukinVK@ya.ru
 License: Apache-2.0
 Keywords: imap,imap-client,python3,python,email
 Platform: UNKNOWN
@@ -38,14 +38,15 @@
 ===============  ================================================================================================
 Python version   3.5+
 License          Apache-2.0
 PyPI             https://pypi.python.org/pypi/imap_tools/
 RFC              `IMAP4.1 <https://tools.ietf.org/html/rfc3501>`_,
                  `EMAIL <https://tools.ietf.org/html/rfc2822>`_,
                  `IMAP related RFCs <https://github.com/ikvk/imap_tools/blob/master/docs/IMAP_related_RFCs.txt>`_
+Repo mirror      https://gitflic.ru/project/ikvk/imap-tools
 ===============  ================================================================================================
 
 .. contents::
 
 Installation
 ------------
 ::
@@ -75,19 +76,20 @@
 
 BaseMailBox.<auth> - login, login_utf8, xoauth2, logout - authentication functions, they support context manager.
 
 BaseMailBox.fetch - first searches email uids by criteria in current folder, then fetch and yields `MailMessage <#email-attributes>`_, args:
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
-* *limit* = None, limit on the number of read emails, useful for actions with a large number of messages, like "move"
+* *limit* = None, limit on the number of read emails, useful for actions with a large number of messages, like "move". May be int or slice.
 * *mark_seen* = True, mark emails as seen on fetch
 * *reverse* = False, in order from the larger date to the smaller
 * *headers_only* = False, get only email headers (without text, html, attachments)
-* *bulk* = False, False - fetch each message separately per N commands - low memory consumption, slow; True - fetch all messages per 1 command - high memory consumption, fast
+* *bulk* = False, False - fetch each message separately per N commands - low memory consumption, slow; True - fetch all messages per 1 command - high memory consumption, fast; int - fetch all messages by bulks of the specified size, for 20 messages and bulk=5 -> 4 commands
+* *sort* = None, criteria for sort messages on server, use SortCriteria constants. Charset arg is important for sort
 
 BaseMailBox.uids - search mailbox for matching message uids in current folder, returns [str | None], None when MailMessage.from_bytes used, args:
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
 
 BaseMailBox.<action> - `copy, move, delete, flag, append <#actions-with-emails>`_
@@ -420,15 +422,18 @@
 `NickC-NZ <https://github.com/NickC-NZ>`_,
 `mweinelt <https://github.com/mweinelt>`_,
 `lucbouge <https://github.com/lucbouge>`_,
 `JacquelinCharbonnel <https://github.com/JacquelinCharbonnel>`_,
 `stumpylog <https://github.com/stumpylog>`_,
 `dimitrisstr <https://github.com/dimitrisstr>`_,
 `abionics <https://github.com/abionics>`_,
-`link2xt <https://github.com/link2xt>`_
+`link2xt <https://github.com/link2xt>`_,
+`Docpart <https://github.com/Docpart>`_,
+`meetttttt <https://github.com/meetttttt>`_,
+`sapristi <https://github.com/sapristi>`_
 
 Help the project
 ----------------
 1. Found a bug or figure out how to improve the library - open issue or merge request 🎯
 2. Do not know how to improve library - try to help other open projects that you use ✋
 3. Nowhere to put your money - spend it on your family, friends, loved ones, or people around you 💰
 4. Star the project ⭐
```

### Comparing `imap-tools-1.5.0/README.rst` & `imap-tools-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: imap-tools
+Version: 1.6.0
+Summary: Work with email by IMAP
+Home-page: https://github.com/ikvk/imap_tools
+Author: Vladimir Kaukin
+Author-email: KaukinVK@ya.ru
+License: Apache-2.0
+Keywords: imap,imap-client,python3,python,email
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 .. http://docutils.sourceforge.net/docs/user/rst/quickref.html
 
 .. |nbsp| unicode:: 0xA0
    :trim:
 
 imap_tools 📧
 =============
@@ -22,14 +38,15 @@
 ===============  ================================================================================================
 Python version   3.5+
 License          Apache-2.0
 PyPI             https://pypi.python.org/pypi/imap_tools/
 RFC              `IMAP4.1 <https://tools.ietf.org/html/rfc3501>`_,
                  `EMAIL <https://tools.ietf.org/html/rfc2822>`_,
                  `IMAP related RFCs <https://github.com/ikvk/imap_tools/blob/master/docs/IMAP_related_RFCs.txt>`_
+Repo mirror      https://gitflic.ru/project/ikvk/imap-tools
 ===============  ================================================================================================
 
 .. contents::
 
 Installation
 ------------
 ::
@@ -59,19 +76,20 @@
 
 BaseMailBox.<auth> - login, login_utf8, xoauth2, logout - authentication functions, they support context manager.
 
 BaseMailBox.fetch - first searches email uids by criteria in current folder, then fetch and yields `MailMessage <#email-attributes>`_, args:
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
-* *limit* = None, limit on the number of read emails, useful for actions with a large number of messages, like "move"
+* *limit* = None, limit on the number of read emails, useful for actions with a large number of messages, like "move". May be int or slice.
 * *mark_seen* = True, mark emails as seen on fetch
 * *reverse* = False, in order from the larger date to the smaller
 * *headers_only* = False, get only email headers (without text, html, attachments)
-* *bulk* = False, False - fetch each message separately per N commands - low memory consumption, slow; True - fetch all messages per 1 command - high memory consumption, fast
+* *bulk* = False, False - fetch each message separately per N commands - low memory consumption, slow; True - fetch all messages per 1 command - high memory consumption, fast; int - fetch all messages by bulks of the specified size, for 20 messages and bulk=5 -> 4 commands
+* *sort* = None, criteria for sort messages on server, use SortCriteria constants. Charset arg is important for sort
 
 BaseMailBox.uids - search mailbox for matching message uids in current folder, returns [str | None], None when MailMessage.from_bytes used, args:
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
 
 BaseMailBox.<action> - `copy, move, delete, flag, append <#actions-with-emails>`_
@@ -404,15 +422,20 @@
 `NickC-NZ <https://github.com/NickC-NZ>`_,
 `mweinelt <https://github.com/mweinelt>`_,
 `lucbouge <https://github.com/lucbouge>`_,
 `JacquelinCharbonnel <https://github.com/JacquelinCharbonnel>`_,
 `stumpylog <https://github.com/stumpylog>`_,
 `dimitrisstr <https://github.com/dimitrisstr>`_,
 `abionics <https://github.com/abionics>`_,
-`link2xt <https://github.com/link2xt>`_
+`link2xt <https://github.com/link2xt>`_,
+`Docpart <https://github.com/Docpart>`_,
+`meetttttt <https://github.com/meetttttt>`_,
+`sapristi <https://github.com/sapristi>`_
 
 Help the project
 ----------------
 1. Found a bug or figure out how to improve the library - open issue or merge request 🎯
 2. Do not know how to improve library - try to help other open projects that you use ✋
 3. Nowhere to put your money - spend it on your family, friends, loved ones, or people around you 💰
 4. Star the project ⭐
+
+
```

### Comparing `imap-tools-1.5.0/setup.py` & `imap-tools-1.6.0/setup.py`

 * *Files identical despite different names*

