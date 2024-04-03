# Comparing `tmp/ass_tg-2.0.1-py3-none-any.whl.zip` & `tmp/ass_tg-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 22299 bytes, number of entries: 22
+Zip file size: 22289 bytes, number of entries: 22
 -rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 ass_tg/__init__.py
 -rw-r--r--  2.0 unx     1849 b- defN 80-Jan-01 00:00 ass_tg/entities.py
 -rw-r--r--  2.0 unx     5144 b- defN 80-Jan-01 00:00 ass_tg/exceptions.py
 -rw-r--r--  2.0 unx      805 b- defN 80-Jan-01 00:00 ass_tg/i18n.py
 -rw-r--r--  2.0 unx     5111 b- defN 80-Jan-01 00:00 ass_tg/middleware.py
 -rw-r--r--  2.0 unx      932 b- defN 80-Jan-01 00:00 ass_tg/types/__init__.py
 -rw-r--r--  2.0 unx      268 b- defN 80-Jan-01 00:00 ass_tg/types/aliases.py
@@ -12,13 +12,13 @@
 -rw-r--r--  2.0 unx     4033 b- defN 80-Jan-01 00:00 ass_tg/types/keyvalue.py
 -rw-r--r--  2.0 unx     8376 b- defN 80-Jan-01 00:00 ass_tg/types/lists.py
 -rw-r--r--  2.0 unx     5108 b- defN 80-Jan-01 00:00 ass_tg/types/logic.py
 -rw-r--r--  2.0 unx     1834 b- defN 80-Jan-01 00:00 ass_tg/types/oneword.py
 -rw-r--r--  2.0 unx     1123 b- defN 80-Jan-01 00:00 ass_tg/types/text.py
 -rw-r--r--  2.0 unx     4587 b- defN 80-Jan-01 00:00 ass_tg/types/text_rules.py
 -rw-r--r--  2.0 unx     2233 b- defN 80-Jan-01 00:00 ass_tg/types/time_arg.py
--rw-r--r--  2.0 unx     4298 b- defN 80-Jan-01 00:00 ass_tg/types/user.py
+-rw-r--r--  2.0 unx     4274 b- defN 80-Jan-01 00:00 ass_tg/types/user.py
 -rw-r--r--  2.0 unx     1574 b- defN 80-Jan-01 00:00 ass_tg/types/wrapped.py
--rw-r--r--  2.0 unx     1652 b- defN 80-Jan-01 00:00 ass_tg-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ass_tg-2.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1693 b- defN 16-Jan-01 00:00 ass_tg-2.0.1.dist-info/RECORD
-22 files, 62657 bytes uncompressed, 19603 bytes compressed:  68.7%
+-rw-r--r--  2.0 unx     1693 b- defN 80-Jan-01 00:00 ass_tg-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ass_tg-2.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1693 b- defN 16-Jan-01 00:00 ass_tg-2.0.2.dist-info/RECORD
+22 files, 62674 bytes uncompressed, 19593 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -51,17 +51,17 @@
 
 Filename: ass_tg/types/user.py
 Comment: 
 
 Filename: ass_tg/types/wrapped.py
 Comment: 
 
-Filename: ass_tg-2.0.1.dist-info/METADATA
+Filename: ass_tg-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: ass_tg-2.0.1.dist-info/WHEEL
+Filename: ass_tg-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: ass_tg-2.0.1.dist-info/RECORD
+Filename: ass_tg-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ass_tg/types/user.py

```diff
@@ -70,15 +70,14 @@
 
     @property
     def examples(self) -> dict[str | StyleFormationCore, Optional[LazyProxy]]:
         return {
             UserLink(
                 user_id=1111224224,
                 name="OrangeFox BOT",
-                link=''
             ): None
         }
 
     @staticmethod
     def check(text: str, entities: ArgEntities) -> bool:
         # It would be nice to check an offset here, but we don't pass it in check()
         return any(x.type == 'mention' for x in entities)
```

## Comparing `ass_tg-2.0.1.dist-info/METADATA` & `ass_tg-2.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: ass-tg
-Version: 2.0.1
+Name: ass_tg
+Version: 2.0.2
 Summary: Arguments Stupendous Searcher (ASS)
 Author: Yacha
 Author-email: yacha@orangefox.tech
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Babel (>=2,<3)
-Requires-Dist: aiogram (>=3.0.0b7,<3.1.0)
+Requires-Dist: aiogram (>=3,<4)
 Requires-Dist: stfu-tg (>=1.4,<2.0)
 Description-Content-Type: text/markdown
 
 # Arguments Stupendous Searcher (ASS)
 
 The library used to parse arguments from the message.
```

## Comparing `ass_tg-2.0.1.dist-info/RECORD` & `ass_tg-2.0.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 ass_tg/types/keyvalue.py,sha256=fUCPUjh2ulUPpmZPHV--GTpOn4QKsOQJdDIIpD05Pe4,4033
 ass_tg/types/lists.py,sha256=_zy9cv2oOTgujdZOTNvxD0tSUijXgN_i6_HRTgwGNjI,8376
 ass_tg/types/logic.py,sha256=IWd1orLBuIU8s4b-vMQ8gLV9jXhqs3AYUFNWnrvvVWM,5108
 ass_tg/types/oneword.py,sha256=pNo3y-DhoAv4WDDg3onqRGwWKIg2GPvUtSUHYHH0QGo,1834
 ass_tg/types/text.py,sha256=sMUmAZknSQ7R0QoNeHad08QAnQFu0JHuA6N2v9bs9PM,1123
 ass_tg/types/text_rules.py,sha256=F4By3SOvIcHJFdxyW3-By3hBOkXmKqZI-ov0jgI4C4k,4587
 ass_tg/types/time_arg.py,sha256=YxM2Z6QwZmmhQYvD-pyWObGXPrXtFHzZM-GNA00rsws,2233
-ass_tg/types/user.py,sha256=OssttqeQMowPT3PluWL92pf9lqEbI38rGiRdMD060ys,4298
+ass_tg/types/user.py,sha256=xwiOaibrnX8nfgH0Mj99rd1JISXviDd6MP3gAU40VLc,4274
 ass_tg/types/wrapped.py,sha256=UO9EtOg080RuIl6ObzkRxjGaPA17805qUFxbqG1Oulk,1574
-ass_tg-2.0.1.dist-info/METADATA,sha256=ZOuCQ89nYi7cErmd0evqlOH5JJY0mLfmesOAOMhVkjc,1652
-ass_tg-2.0.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-ass_tg-2.0.1.dist-info/RECORD,,
+ass_tg-2.0.2.dist-info/METADATA,sha256=0o9r7-W7_wK6ILR4s75RTWNIh4dqyuhqNC2Q0h0Unf8,1693
+ass_tg-2.0.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+ass_tg-2.0.2.dist-info/RECORD,,
```

