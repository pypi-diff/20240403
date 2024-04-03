# Comparing `tmp/extract_msg-0.48.4.tar.gz` & `tmp/extract_msg-0.48.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extract_msg-0.48.4.tar", last modified: Thu Mar 21 01:02:59 2024, max compression
+gzip compressed data, was "extract_msg-0.48.5.tar", last modified: Wed Apr  3 12:06:21 2024, max compression
```

## Comparing `extract_msg-0.48.4.tar` & `extract_msg-0.48.5.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:59.144220 extract_msg-0.48.4/
--rw-rw-rw-   0        0        0   106419 2024-03-21 01:02:53.000000 extract_msg-0.48.4/CHANGELOG.md
--rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.48.4/LICENSE.txt
--rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.48.4/MANIFEST.in
--rw-rw-rw-   0        0        0    15117 2024-03-21 01:02:59.145216 extract_msg-0.48.4/PKG-INFO
--rw-rw-rw-   0        0        0    14216 2024-03-21 01:02:53.000000 extract_msg-0.48.4/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:58.942294 extract_msg-0.48.4/extract_msg/
--rw-rw-rw-   0        0        0     2012 2024-03-21 01:02:53.000000 extract_msg-0.48.4/extract_msg/__init__.py
--rw-rw-rw-   0        0        0     3683 2024-03-21 01:02:53.000000 extract_msg-0.48.4/extract_msg/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:58.980192 extract_msg-0.48.4/extract_msg/_rtf/
--rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.48.4/extract_msg/_rtf/__init__.py
--rw-rw-rw-   0        0        0      844 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/_rtf/create_doc.py
--rw-rw-rw-   0        0        0     6297 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/_rtf/inject_rtf.py
--rw-rw-rw-   0        0        0      852 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/_rtf/token.py
--rw-rw-rw-   0        0        0     8822 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/_rtf/tokenize_rtf.py
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:58.998144 extract_msg-0.48.4/extract_msg/attachments/
--rw-rw-rw-   0        0        0     5627 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/__init__.py
--rw-rw-rw-   0        0        0     6957 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/attachment.py
--rw-rw-rw-   0        0        0    27802 2024-03-20 18:47:24.000000 extract_msg-0.48.4/extract_msg/attachments/attachment_base.py
--rw-rw-rw-   0        0        0     1063 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/broken_att.py
--rw-rw-rw-   0        0        0     5784 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/custom_att.py
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:59.009115 extract_msg-0.48.4/extract_msg/attachments/custom_att_handler/
--rw-rw-rw-   0        0        0     2704 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/custom_att_handler/__init__.py
--rw-rw-rw-   0        0        0     3988 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/custom_att_handler/custom_handler.py
--rw-rw-rw-   0        0        0     3197 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/custom_att_handler/lnk_obj_att.py
--rw-rw-rw-   0        0        0     4661 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/custom_att_handler/outlook_image_dib.py
--rw-rw-rw-   0        0        0     4760 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/emb_msg_att.py
--rw-rw-rw-   0        0        0    10545 2024-03-20 18:47:24.000000 extract_msg-0.48.4/extract_msg/attachments/signed_att.py
--rw-rw-rw-   0        0        0     1037 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/unsupported_att.py
--rw-rw-rw-   0        0        0     2283 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/attachments/web_att.py
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:59.016096 extract_msg-0.48.4/extract_msg/constants/
--rw-rw-rw-   0        0        0     6489 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/constants/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/constants/ps.py
--rw-rw-rw-   0        0        0     1212 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/constants/re.py
--rw-rw-rw-   0        0        0     3909 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/constants/st.py
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:58.898418 extract_msg-0.48.4/extract_msg/data/
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:59.019088 extract_msg-0.48.4/extract_msg/data/logging-config/
--rw-rw-rw-   0        0        0     2082 2023-07-29 23:17:08.000000 extract_msg-0.48.4/extract_msg/data/logging-config/logging-nt.json
--rw-rw-rw-   0        0        0     2058 2023-07-29 23:17:08.000000 extract_msg-0.48.4/extract_msg/data/logging-config/logging-posix.json
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:59.024074 extract_msg-0.48.4/extract_msg/encoding/
--rw-rw-rw-   0        0        0    12325 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/encoding/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:59.040032 extract_msg-0.48.4/extract_msg/encoding/_dt/
--rw-rw-rw-   0        0        0      113 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/encoding/_dt/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/encoding/_dt/_mac_ce.py
--rw-rw-rw-   0        0        0     2778 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/encoding/_dt/_mac_cyrillic.py
--rw-rw-rw-   0        0        0     2714 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/encoding/_dt/_mac_greek.py
--rw-rw-rw-   0        0        0     2620 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/encoding/_dt/_mac_iceland.py
--rw-rw-rw-   0        0        0     2621 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/encoding/_dt/_mac_turkish.py
--rw-rw-rw-   0        0        0     2415 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/encoding/_dt/_win874_dec.py
--rw-rw-rw-   0        0        0   298017 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/encoding/_dt/_win950_dec.py
--rw-rw-rw-   0        0        0    11783 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/encoding/utils.py
--rw-rw-rw-   0        0        0    66158 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/enums.py
--rw-rw-rw-   0        0        0     4422 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:59.084380 extract_msg-0.48.4/extract_msg/msg_classes/
--rw-rw-rw-   0        0        0     1247 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/msg_classes/__init__.py
--rw-rw-rw-   0        0        0     7164 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/msg_classes/appointment.py
--rw-rw-rw-   0        0        0     2916 2023-08-13 00:04:52.000000 extract_msg-0.48.4/extract_msg/msg_classes/calendar.py
--rw-rw-rw-   0        0        0    17279 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/msg_classes/calendar_base.py
--rw-rw-rw-   0        0        0    45424 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/msg_classes/contact.py
--rw-rw-rw-   0        0        0     4252 2023-11-08 14:33:11.000000 extract_msg-0.48.4/extract_msg/msg_classes/journal.py
--rw-rw-rw-   0        0        0     4025 2023-11-08 14:33:11.000000 extract_msg-0.48.4/extract_msg/msg_classes/meeting_cancellation.py
--rw-rw-rw-   0        0        0     1540 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/msg_classes/meeting_exception.py
--rw-rw-rw-   0        0        0     4183 2023-11-08 14:33:11.000000 extract_msg-0.48.4/extract_msg/msg_classes/meeting_forward.py
--rw-rw-rw-   0        0        0     1889 2023-08-13 00:04:52.000000 extract_msg-0.48.4/extract_msg/msg_classes/meeting_related.py
--rw-rw-rw-   0        0        0     7006 2023-11-08 14:33:11.000000 extract_msg-0.48.4/extract_msg/msg_classes/meeting_request.py
--rw-rw-rw-   0        0        0     2208 2023-08-13 00:04:52.000000 extract_msg-0.48.4/extract_msg/msg_classes/meeting_response.py
--rw-rw-rw-   0        0        0      163 2023-07-29 23:17:08.000000 extract_msg-0.48.4/extract_msg/msg_classes/message.py
--rw-rw-rw-   0        0        0    58720 2024-03-09 17:44:47.000000 extract_msg-0.48.4/extract_msg/msg_classes/message_base.py
--rw-rw-rw-   0        0        0      254 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/msg_classes/message_signed.py
--rw-rw-rw-   0        0        0     6030 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/msg_classes/message_signed_base.py
--rw-rw-rw-   0        0        0    47738 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/msg_classes/msg.py
--rw-rw-rw-   0        0        0     1345 2023-11-08 14:33:11.000000 extract_msg-0.48.4/extract_msg/msg_classes/post.py
--rw-rw-rw-   0        0        0     2021 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/msg_classes/sticky_note.py
--rw-rw-rw-   0        0        0    12418 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/msg_classes/task.py
--rw-rw-rw-   0        0        0     2866 2023-11-08 14:33:11.000000 extract_msg-0.48.4/extract_msg/msg_classes/task_request.py
--rw-rw-rw-   0        0        0      907 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/null_date.py
--rw-rw-rw-   0        0        0    45697 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/ole_writer.py
--rw-rw-rw-   0        0        0     8519 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/open_msg.py
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:59.091361 extract_msg-0.48.4/extract_msg/properties/
--rw-rw-rw-   0        0        0      527 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/properties/__init__.py
--rw-rw-rw-   0        0        0    17572 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/properties/named.py
--rw-rw-rw-   0        0        0    22088 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/properties/prop.py
--rw-rw-rw-   0        0        0    16376 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/properties/properties_store.py
--rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.48.4/extract_msg/py.typed
--rw-rw-rw-   0        0        0    13722 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/recipient.py
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:59.141227 extract_msg-0.48.4/extract_msg/structures/
--rw-rw-rw-   0        0        0      835 2023-11-08 14:33:11.000000 extract_msg-0.48.4/extract_msg/structures/__init__.py
--rw-rw-rw-   0        0        0    11952 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/_helpers.py
--rw-rw-rw-   0        0        0    14764 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/business_card.py
--rw-rw-rw-   0        0        0     3744 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/structures/cfoas.py
--rw-rw-rw-   0        0        0     1400 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/contact_link_entry.py
--rw-rw-rw-   0        0        0    21818 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/dev_mode_a.py
--rw-rw-rw-   0        0        0     5405 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/dv_target_device.py
--rw-rw-rw-   0        0        0    21775 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/structures/entry_id.py
--rw-rw-rw-   0        0        0     6114 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/misc_id.py
--rw-rw-rw-   0        0        0     1367 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/mon_stream.py
--rw-rw-rw-   0        0        0     2131 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/odt.py
--rw-rw-rw-   0        0        0    10406 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/structures/ole_pres.py
--rw-rw-rw-   0        0        0     3943 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/structures/ole_stream_struct.py
--rw-rw-rw-   0        0        0     7329 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/structures/recurrence_pattern.py
--rw-rw-rw-   0        0        0     3278 2024-02-28 16:13:05.000000 extract_msg-0.48.4/extract_msg/structures/report_tag.py
--rw-rw-rw-   0        0        0     4394 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/system_time.py
--rw-rw-rw-   0        0        0     3313 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/time_zone_definition.py
--rw-rw-rw-   0        0        0     2988 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/time_zone_struct.py
--rw-rw-rw-   0        0        0     4327 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/toc_entry.py
--rw-rw-rw-   0        0        0     4465 2023-12-09 19:11:57.000000 extract_msg-0.48.4/extract_msg/structures/tz_rule.py
--rw-rw-rw-   0        0        0    50619 2024-03-08 17:15:10.000000 extract_msg-0.48.4/extract_msg/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-21 01:02:58.968226 extract_msg-0.48.4/extract_msg.egg-info/
--rw-rw-rw-   0        0        0    15117 2024-03-21 01:02:58.000000 extract_msg-0.48.4/extract_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3593 2024-03-21 01:02:58.000000 extract_msg-0.48.4/extract_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 01:02:58.000000 extract_msg-0.48.4/extract_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-03-21 01:02:58.000000 extract_msg-0.48.4/extract_msg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      333 2024-03-21 01:02:58.000000 extract_msg-0.48.4/extract_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-21 01:02:58.000000 extract_msg-0.48.4/extract_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      258 2023-12-09 19:11:57.000000 extract_msg-0.48.4/requirements.txt
--rw-rw-rw-   0        0        0      345 2024-03-21 01:02:59.147212 extract_msg-0.48.4/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.48.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.426564 extract_msg-0.48.5/
+-rw-rw-rw-   0        0        0   106562 2024-04-03 12:06:16.000000 extract_msg-0.48.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.48.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.48.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    15117 2024-04-03 12:06:21.427565 extract_msg-0.48.5/PKG-INFO
+-rw-rw-rw-   0        0        0    14216 2024-04-03 12:06:16.000000 extract_msg-0.48.5/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.274969 extract_msg-0.48.5/extract_msg/
+-rw-rw-rw-   0        0        0     2012 2024-04-03 12:06:16.000000 extract_msg-0.48.5/extract_msg/__init__.py
+-rw-rw-rw-   0        0        0     3683 2024-03-21 01:02:53.000000 extract_msg-0.48.5/extract_msg/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.304893 extract_msg-0.48.5/extract_msg/_rtf/
+-rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.48.5/extract_msg/_rtf/__init__.py
+-rw-rw-rw-   0        0        0      844 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/_rtf/create_doc.py
+-rw-rw-rw-   0        0        0     6297 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/_rtf/inject_rtf.py
+-rw-rw-rw-   0        0        0      852 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/_rtf/token.py
+-rw-rw-rw-   0        0        0     8822 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/_rtf/tokenize_rtf.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.318852 extract_msg-0.48.5/extract_msg/attachments/
+-rw-rw-rw-   0        0        0     5627 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/__init__.py
+-rw-rw-rw-   0        0        0     6957 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/attachment.py
+-rw-rw-rw-   0        0        0    27802 2024-03-20 18:47:24.000000 extract_msg-0.48.5/extract_msg/attachments/attachment_base.py
+-rw-rw-rw-   0        0        0     1063 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/broken_att.py
+-rw-rw-rw-   0        0        0     5784 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/custom_att.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.325835 extract_msg-0.48.5/extract_msg/attachments/custom_att_handler/
+-rw-rw-rw-   0        0        0     2704 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/custom_att_handler/__init__.py
+-rw-rw-rw-   0        0        0     3988 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/custom_att_handler/custom_handler.py
+-rw-rw-rw-   0        0        0     3197 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/custom_att_handler/lnk_obj_att.py
+-rw-rw-rw-   0        0        0     4661 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/custom_att_handler/outlook_image_dib.py
+-rw-rw-rw-   0        0        0     4760 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/emb_msg_att.py
+-rw-rw-rw-   0        0        0    10545 2024-03-20 18:47:24.000000 extract_msg-0.48.5/extract_msg/attachments/signed_att.py
+-rw-rw-rw-   0        0        0     1037 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/unsupported_att.py
+-rw-rw-rw-   0        0        0     2283 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/attachments/web_att.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.331818 extract_msg-0.48.5/extract_msg/constants/
+-rw-rw-rw-   0        0        0     6489 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/constants/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/constants/ps.py
+-rw-rw-rw-   0        0        0     1212 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/constants/re.py
+-rw-rw-rw-   0        0        0     3909 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/constants/st.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.242025 extract_msg-0.48.5/extract_msg/data/
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.334809 extract_msg-0.48.5/extract_msg/data/logging-config/
+-rw-rw-rw-   0        0        0     2082 2023-07-29 23:17:08.000000 extract_msg-0.48.5/extract_msg/data/logging-config/logging-nt.json
+-rw-rw-rw-   0        0        0     2058 2023-07-29 23:17:08.000000 extract_msg-0.48.5/extract_msg/data/logging-config/logging-posix.json
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.338809 extract_msg-0.48.5/extract_msg/encoding/
+-rw-rw-rw-   0        0        0    12325 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/encoding/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.349771 extract_msg-0.48.5/extract_msg/encoding/_dt/
+-rw-rw-rw-   0        0        0      113 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/encoding/_dt/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/encoding/_dt/_mac_ce.py
+-rw-rw-rw-   0        0        0     2778 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/encoding/_dt/_mac_cyrillic.py
+-rw-rw-rw-   0        0        0     2714 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/encoding/_dt/_mac_greek.py
+-rw-rw-rw-   0        0        0     2620 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/encoding/_dt/_mac_iceland.py
+-rw-rw-rw-   0        0        0     2621 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/encoding/_dt/_mac_turkish.py
+-rw-rw-rw-   0        0        0     2415 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/encoding/_dt/_win874_dec.py
+-rw-rw-rw-   0        0        0   298017 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/encoding/_dt/_win950_dec.py
+-rw-rw-rw-   0        0        0    11783 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/encoding/utils.py
+-rw-rw-rw-   0        0        0    66158 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/enums.py
+-rw-rw-rw-   0        0        0     4422 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.384675 extract_msg-0.48.5/extract_msg/msg_classes/
+-rw-rw-rw-   0        0        0     1247 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/msg_classes/__init__.py
+-rw-rw-rw-   0        0        0     7164 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/msg_classes/appointment.py
+-rw-rw-rw-   0        0        0     2916 2023-08-13 00:04:52.000000 extract_msg-0.48.5/extract_msg/msg_classes/calendar.py
+-rw-rw-rw-   0        0        0    17279 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/msg_classes/calendar_base.py
+-rw-rw-rw-   0        0        0    45424 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/msg_classes/contact.py
+-rw-rw-rw-   0        0        0     4252 2023-11-08 14:33:11.000000 extract_msg-0.48.5/extract_msg/msg_classes/journal.py
+-rw-rw-rw-   0        0        0     4025 2023-11-08 14:33:11.000000 extract_msg-0.48.5/extract_msg/msg_classes/meeting_cancellation.py
+-rw-rw-rw-   0        0        0     1540 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/msg_classes/meeting_exception.py
+-rw-rw-rw-   0        0        0     4183 2023-11-08 14:33:11.000000 extract_msg-0.48.5/extract_msg/msg_classes/meeting_forward.py
+-rw-rw-rw-   0        0        0     1889 2023-08-13 00:04:52.000000 extract_msg-0.48.5/extract_msg/msg_classes/meeting_related.py
+-rw-rw-rw-   0        0        0     7006 2023-11-08 14:33:11.000000 extract_msg-0.48.5/extract_msg/msg_classes/meeting_request.py
+-rw-rw-rw-   0        0        0     2208 2023-08-13 00:04:52.000000 extract_msg-0.48.5/extract_msg/msg_classes/meeting_response.py
+-rw-rw-rw-   0        0        0      163 2023-07-29 23:17:08.000000 extract_msg-0.48.5/extract_msg/msg_classes/message.py
+-rw-rw-rw-   0        0        0    58720 2024-03-09 17:44:47.000000 extract_msg-0.48.5/extract_msg/msg_classes/message_base.py
+-rw-rw-rw-   0        0        0      254 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/msg_classes/message_signed.py
+-rw-rw-rw-   0        0        0     6030 2024-04-03 12:06:16.000000 extract_msg-0.48.5/extract_msg/msg_classes/message_signed_base.py
+-rw-rw-rw-   0        0        0    47738 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/msg_classes/msg.py
+-rw-rw-rw-   0        0        0     1345 2023-11-08 14:33:11.000000 extract_msg-0.48.5/extract_msg/msg_classes/post.py
+-rw-rw-rw-   0        0        0     2021 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/msg_classes/sticky_note.py
+-rw-rw-rw-   0        0        0    12418 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/msg_classes/task.py
+-rw-rw-rw-   0        0        0     2866 2023-11-08 14:33:11.000000 extract_msg-0.48.5/extract_msg/msg_classes/task_request.py
+-rw-rw-rw-   0        0        0      907 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/null_date.py
+-rw-rw-rw-   0        0        0    45697 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/ole_writer.py
+-rw-rw-rw-   0        0        0     8519 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/open_msg.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.391660 extract_msg-0.48.5/extract_msg/properties/
+-rw-rw-rw-   0        0        0      527 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/properties/__init__.py
+-rw-rw-rw-   0        0        0    17572 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/properties/named.py
+-rw-rw-rw-   0        0        0    22088 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/properties/prop.py
+-rw-rw-rw-   0        0        0    16376 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/properties/properties_store.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.48.5/extract_msg/py.typed
+-rw-rw-rw-   0        0        0    13722 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/recipient.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.425567 extract_msg-0.48.5/extract_msg/structures/
+-rw-rw-rw-   0        0        0      835 2023-11-08 14:33:11.000000 extract_msg-0.48.5/extract_msg/structures/__init__.py
+-rw-rw-rw-   0        0        0    11952 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/_helpers.py
+-rw-rw-rw-   0        0        0    14764 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/business_card.py
+-rw-rw-rw-   0        0        0     3744 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/structures/cfoas.py
+-rw-rw-rw-   0        0        0     1400 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/contact_link_entry.py
+-rw-rw-rw-   0        0        0    21818 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/dev_mode_a.py
+-rw-rw-rw-   0        0        0     5405 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/dv_target_device.py
+-rw-rw-rw-   0        0        0    21775 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/structures/entry_id.py
+-rw-rw-rw-   0        0        0     6114 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/misc_id.py
+-rw-rw-rw-   0        0        0     1367 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/mon_stream.py
+-rw-rw-rw-   0        0        0     2131 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/odt.py
+-rw-rw-rw-   0        0        0    10406 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/structures/ole_pres.py
+-rw-rw-rw-   0        0        0     3943 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/structures/ole_stream_struct.py
+-rw-rw-rw-   0        0        0     7329 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/structures/recurrence_pattern.py
+-rw-rw-rw-   0        0        0     3278 2024-02-28 16:13:05.000000 extract_msg-0.48.5/extract_msg/structures/report_tag.py
+-rw-rw-rw-   0        0        0     4394 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/system_time.py
+-rw-rw-rw-   0        0        0     3313 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/time_zone_definition.py
+-rw-rw-rw-   0        0        0     2988 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/time_zone_struct.py
+-rw-rw-rw-   0        0        0     4327 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/toc_entry.py
+-rw-rw-rw-   0        0        0     4465 2023-12-09 19:11:57.000000 extract_msg-0.48.5/extract_msg/structures/tz_rule.py
+-rw-rw-rw-   0        0        0    50619 2024-03-08 17:15:10.000000 extract_msg-0.48.5/extract_msg/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:06:21.297909 extract_msg-0.48.5/extract_msg.egg-info/
+-rw-rw-rw-   0        0        0    15117 2024-04-03 12:06:21.000000 extract_msg-0.48.5/extract_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3593 2024-04-03 12:06:21.000000 extract_msg-0.48.5/extract_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 12:06:21.000000 extract_msg-0.48.5/extract_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-03 12:06:21.000000 extract_msg-0.48.5/extract_msg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      333 2024-04-03 12:06:21.000000 extract_msg-0.48.5/extract_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 12:06:21.000000 extract_msg-0.48.5/extract_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      258 2023-12-09 19:11:57.000000 extract_msg-0.48.5/requirements.txt
+-rw-rw-rw-   0        0        0      345 2024-04-03 12:06:21.429556 extract_msg-0.48.5/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.48.5/setup.py
```

### Comparing `extract_msg-0.48.4/CHANGELOG.md` & `extract_msg-0.48.5/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+**v0.48.5**
+* [[TeamMsgExtractor #414](https://github.com/TeamMsgExtractor/msg-extractor/issues/414)] Fixed typo in `message_signed_base.py`.
+
 **v0.48.4**
 * [[TeamMsgExtractor #411](https://github.com/TeamMsgExtractor/msg-extractor/issues/411)] Fix console script throwing error due to changed console args not defaulting.
 
 **v0.48.3**
 * [[TeamMsgExtractor #409](https://github.com/TeamMsgExtractor/msg-extractor/issues/409)] Added missing private method to `SignedAttachment`.
 * Fixed some missing typing information.
```

### Comparing `extract_msg-0.48.4/LICENSE.txt` & `extract_msg-0.48.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/PKG-INFO` & `extract_msg-0.48.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract_msg
-Version: 0.48.4
+Version: 0.48.5
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
@@ -274,16 +274,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.48.4-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.48.4/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.48.5-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.48.5/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3810/
 
 .. |Read the Docs| image:: https://readthedocs.org/projects/msg-extractor/badge/?version=latest
     :target: https://msg-extractor.readthedocs.io/en/stable/?badge=latest
     :alt: Documentation Status
```

### Comparing `extract_msg-0.48.4/README.rst` & `extract_msg-0.48.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -256,16 +256,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.48.4-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.48.4/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.48.5-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.48.5/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3810/
 
 .. |Read the Docs| image:: https://readthedocs.org/projects/msg-extractor/badge/?version=latest
     :target: https://msg-extractor.readthedocs.io/en/stable/?badge=latest
     :alt: Documentation Status
```

### Comparing `extract_msg-0.48.4/extract_msg/__init__.py` & `extract_msg-0.48.5/extract_msg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = 'Destiny Peterson & Matthew Walker'
-__date__ = '2024-03-20'
-__version__ = '0.48.4'
+__date__ = '2024-04-03'
+__version__ = '0.48.5'
 
 __all__ = [
     # Modules:
     'attachments',
     'constants',
     'enums',
     'exceptions',
```

### Comparing `extract_msg-0.48.4/extract_msg/__main__.py` & `extract_msg-0.48.5/extract_msg/__main__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/_rtf/create_doc.py` & `extract_msg-0.48.5/extract_msg/_rtf/create_doc.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/_rtf/inject_rtf.py` & `extract_msg-0.48.5/extract_msg/_rtf/inject_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/_rtf/token.py` & `extract_msg-0.48.5/extract_msg/_rtf/token.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/_rtf/tokenize_rtf.py` & `extract_msg-0.48.5/extract_msg/_rtf/tokenize_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/__init__.py` & `extract_msg-0.48.5/extract_msg/attachments/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/attachment.py` & `extract_msg-0.48.5/extract_msg/attachments/attachment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/attachment_base.py` & `extract_msg-0.48.5/extract_msg/attachments/attachment_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/broken_att.py` & `extract_msg-0.48.5/extract_msg/attachments/broken_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/custom_att.py` & `extract_msg-0.48.5/extract_msg/attachments/custom_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/custom_att_handler/__init__.py` & `extract_msg-0.48.5/extract_msg/attachments/custom_att_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/custom_att_handler/custom_handler.py` & `extract_msg-0.48.5/extract_msg/attachments/custom_att_handler/custom_handler.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/custom_att_handler/lnk_obj_att.py` & `extract_msg-0.48.5/extract_msg/attachments/custom_att_handler/lnk_obj_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/custom_att_handler/outlook_image_dib.py` & `extract_msg-0.48.5/extract_msg/attachments/custom_att_handler/outlook_image_dib.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/emb_msg_att.py` & `extract_msg-0.48.5/extract_msg/attachments/emb_msg_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/signed_att.py` & `extract_msg-0.48.5/extract_msg/attachments/signed_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/unsupported_att.py` & `extract_msg-0.48.5/extract_msg/attachments/unsupported_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/attachments/web_att.py` & `extract_msg-0.48.5/extract_msg/attachments/web_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/constants/__init__.py` & `extract_msg-0.48.5/extract_msg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/constants/ps.py` & `extract_msg-0.48.5/extract_msg/constants/ps.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/constants/re.py` & `extract_msg-0.48.5/extract_msg/constants/re.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/constants/st.py` & `extract_msg-0.48.5/extract_msg/constants/st.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/data/logging-config/logging-nt.json` & `extract_msg-0.48.5/extract_msg/data/logging-config/logging-nt.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/data/logging-config/logging-posix.json` & `extract_msg-0.48.5/extract_msg/data/logging-config/logging-posix.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/encoding/__init__.py` & `extract_msg-0.48.5/extract_msg/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/encoding/_dt/_mac_ce.py` & `extract_msg-0.48.5/extract_msg/encoding/_dt/_mac_ce.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/encoding/_dt/_mac_cyrillic.py` & `extract_msg-0.48.5/extract_msg/encoding/_dt/_mac_cyrillic.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/encoding/_dt/_mac_greek.py` & `extract_msg-0.48.5/extract_msg/encoding/_dt/_mac_greek.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/encoding/_dt/_mac_iceland.py` & `extract_msg-0.48.5/extract_msg/encoding/_dt/_mac_iceland.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/encoding/_dt/_mac_turkish.py` & `extract_msg-0.48.5/extract_msg/encoding/_dt/_mac_turkish.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/encoding/_dt/_win874_dec.py` & `extract_msg-0.48.5/extract_msg/encoding/_dt/_win874_dec.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/encoding/_dt/_win950_dec.py` & `extract_msg-0.48.5/extract_msg/encoding/_dt/_win950_dec.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/encoding/utils.py` & `extract_msg-0.48.5/extract_msg/encoding/utils.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/enums.py` & `extract_msg-0.48.5/extract_msg/enums.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/exceptions.py` & `extract_msg-0.48.5/extract_msg/exceptions.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/__init__.py` & `extract_msg-0.48.5/extract_msg/msg_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/appointment.py` & `extract_msg-0.48.5/extract_msg/msg_classes/appointment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/calendar.py` & `extract_msg-0.48.5/extract_msg/msg_classes/calendar.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/calendar_base.py` & `extract_msg-0.48.5/extract_msg/msg_classes/calendar_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/contact.py` & `extract_msg-0.48.5/extract_msg/msg_classes/contact.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/journal.py` & `extract_msg-0.48.5/extract_msg/msg_classes/journal.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/meeting_cancellation.py` & `extract_msg-0.48.5/extract_msg/msg_classes/meeting_cancellation.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/meeting_exception.py` & `extract_msg-0.48.5/extract_msg/msg_classes/meeting_exception.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/meeting_forward.py` & `extract_msg-0.48.5/extract_msg/msg_classes/meeting_forward.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/meeting_related.py` & `extract_msg-0.48.5/extract_msg/msg_classes/meeting_related.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/meeting_request.py` & `extract_msg-0.48.5/extract_msg/msg_classes/meeting_request.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/meeting_response.py` & `extract_msg-0.48.5/extract_msg/msg_classes/meeting_response.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/message_base.py` & `extract_msg-0.48.5/extract_msg/msg_classes/message_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/message_signed_base.py` & `extract_msg-0.48.5/extract_msg/msg_classes/message_signed_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             htmlBody = self.signedHtmlBody
         elif self.rtfBody:
             logger.info('HTML body was not found, attempting to generate from RTF.')
             htmlBody = self.deencapsulateBody(self.rtfBody, DeencapType.HTML)
         elif self.body:
             # Convert the plain text body to html.
             logger.info('HTML body was not found, attempting to generate from plain text body.')
-            correctedBody = html.escpae(self.body).replace('\r', '').replace('\n', '<br />')
+            correctedBody = html.escape(self.body).replace('\r', '').replace('\n', '<br />')
             htmlBody = f'<html><body>{correctedBody}</body></head>'.encode('utf-8')
         else:
             logger.info('HTML body could not be found nor generated.')
 
         return htmlBody
 
     @functools.cached_property
```

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/msg.py` & `extract_msg-0.48.5/extract_msg/msg_classes/msg.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/post.py` & `extract_msg-0.48.5/extract_msg/msg_classes/post.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/sticky_note.py` & `extract_msg-0.48.5/extract_msg/msg_classes/sticky_note.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/task.py` & `extract_msg-0.48.5/extract_msg/msg_classes/task.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/msg_classes/task_request.py` & `extract_msg-0.48.5/extract_msg/msg_classes/task_request.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/null_date.py` & `extract_msg-0.48.5/extract_msg/null_date.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/ole_writer.py` & `extract_msg-0.48.5/extract_msg/ole_writer.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/open_msg.py` & `extract_msg-0.48.5/extract_msg/open_msg.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/properties/__init__.py` & `extract_msg-0.48.5/extract_msg/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/properties/named.py` & `extract_msg-0.48.5/extract_msg/properties/named.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/properties/prop.py` & `extract_msg-0.48.5/extract_msg/properties/prop.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/properties/properties_store.py` & `extract_msg-0.48.5/extract_msg/properties/properties_store.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/recipient.py` & `extract_msg-0.48.5/extract_msg/recipient.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/__init__.py` & `extract_msg-0.48.5/extract_msg/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/_helpers.py` & `extract_msg-0.48.5/extract_msg/structures/_helpers.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/business_card.py` & `extract_msg-0.48.5/extract_msg/structures/business_card.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/cfoas.py` & `extract_msg-0.48.5/extract_msg/structures/cfoas.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/contact_link_entry.py` & `extract_msg-0.48.5/extract_msg/structures/contact_link_entry.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/dev_mode_a.py` & `extract_msg-0.48.5/extract_msg/structures/dev_mode_a.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/dv_target_device.py` & `extract_msg-0.48.5/extract_msg/structures/dv_target_device.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/entry_id.py` & `extract_msg-0.48.5/extract_msg/structures/entry_id.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/misc_id.py` & `extract_msg-0.48.5/extract_msg/structures/misc_id.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/mon_stream.py` & `extract_msg-0.48.5/extract_msg/structures/mon_stream.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/odt.py` & `extract_msg-0.48.5/extract_msg/structures/odt.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/ole_pres.py` & `extract_msg-0.48.5/extract_msg/structures/ole_pres.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/ole_stream_struct.py` & `extract_msg-0.48.5/extract_msg/structures/ole_stream_struct.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/recurrence_pattern.py` & `extract_msg-0.48.5/extract_msg/structures/recurrence_pattern.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/report_tag.py` & `extract_msg-0.48.5/extract_msg/structures/report_tag.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/system_time.py` & `extract_msg-0.48.5/extract_msg/structures/system_time.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/time_zone_definition.py` & `extract_msg-0.48.5/extract_msg/structures/time_zone_definition.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/time_zone_struct.py` & `extract_msg-0.48.5/extract_msg/structures/time_zone_struct.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/toc_entry.py` & `extract_msg-0.48.5/extract_msg/structures/toc_entry.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/structures/tz_rule.py` & `extract_msg-0.48.5/extract_msg/structures/tz_rule.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg/utils.py` & `extract_msg-0.48.5/extract_msg/utils.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/extract_msg.egg-info/PKG-INFO` & `extract_msg-0.48.5/extract_msg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract-msg
-Version: 0.48.4
+Version: 0.48.5
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
@@ -274,16 +274,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.48.4-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.48.4/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.48.5-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.48.5/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3810/
 
 .. |Read the Docs| image:: https://readthedocs.org/projects/msg-extractor/badge/?version=latest
     :target: https://msg-extractor.readthedocs.io/en/stable/?badge=latest
     :alt: Documentation Status
```

### Comparing `extract_msg-0.48.4/extract_msg.egg-info/SOURCES.txt` & `extract_msg-0.48.5/extract_msg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.48.4/setup.py` & `extract_msg-0.48.5/setup.py`

 * *Files identical despite different names*

