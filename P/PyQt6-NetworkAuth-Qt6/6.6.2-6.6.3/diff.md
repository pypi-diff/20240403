# Comparing `tmp/PyQt6_NetworkAuth_Qt6-6.6.2-py3-none-win_amd64.whl.zip` & `tmp/PyQt6_NetworkAuth_Qt6-6.6.3-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 111488 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   222352 b- defN 24-Feb-09 17:18 PyQt6/Qt6/bin/Qt6NetworkAuth.dll
--rw-rw-rw-  2.0 fat    44738 b- defN 24-Feb-17 18:17 PyQt6_NetworkAuth_Qt6-6.6.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      597 b- defN 24-Feb-17 18:17 PyQt6_NetworkAuth_Qt6-6.6.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       95 b- defN 24-Feb-17 18:17 PyQt6_NetworkAuth_Qt6-6.6.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      446 b- defN 24-Feb-17 18:17 PyQt6_NetworkAuth_Qt6-6.6.2.dist-info/RECORD
-5 files, 268228 bytes uncompressed, 110666 bytes compressed:  58.7%
+Zip file size: 111493 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat   222352 b- defN 24-Mar-18 16:58 PyQt6/Qt6/bin/Qt6NetworkAuth.dll
+-rw-rw-rw-  2.0 fat    44738 b- defN 24-Apr-03 18:03 PyQt6_NetworkAuth_Qt6-6.6.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      597 b- defN 24-Apr-03 18:03 PyQt6_NetworkAuth_Qt6-6.6.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       95 b- defN 24-Apr-03 18:03 PyQt6_NetworkAuth_Qt6-6.6.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      446 b- defN 24-Apr-03 18:03 PyQt6_NetworkAuth_Qt6-6.6.3.dist-info/RECORD
+5 files, 268228 bytes uncompressed, 110671 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: PyQt6/Qt6/bin/Qt6NetworkAuth.dll
 Comment: 
 
-Filename: PyQt6_NetworkAuth_Qt6-6.6.2.dist-info/LICENSE
+Filename: PyQt6_NetworkAuth_Qt6-6.6.3.dist-info/LICENSE
 Comment: 
 
-Filename: PyQt6_NetworkAuth_Qt6-6.6.2.dist-info/METADATA
+Filename: PyQt6_NetworkAuth_Qt6-6.6.3.dist-info/METADATA
 Comment: 
 
-Filename: PyQt6_NetworkAuth_Qt6-6.6.2.dist-info/WHEEL
+Filename: PyQt6_NetworkAuth_Qt6-6.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: PyQt6_NetworkAuth_Qt6-6.6.2.dist-info/RECORD
+Filename: PyQt6_NetworkAuth_Qt6-6.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PyQt6/Qt6/bin/Qt6NetworkAuth.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018001f010
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Feb  9 17:18:39 2024
+Time/Date		Mon Mar 18 16:58:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000001ec00
 SizeOfInitializedData	0000000000016000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001f010
@@ -25,15 +25,15 @@
 MajorImageVersion	6
 MinorImageVersion	6
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00038000
 SizeOfHeaders		00000400
-CheckSum		000391f5
+CheckSum		0003c65c
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00004160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 					GUARD_CF
 SizeOfStackReserve	0000000000100000
@@ -42,15 +42,15 @@
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
 NumberOfRvaAndSizes	00000010
 
 The Data Directory
 Entry 0 00000000000282b0 000045b4 Export Directory [.edata (or where ever we found it)]
 Entry 1 000000000002c864 000000c8 Import Directory [parts of .idata]
-Entry 2 0000000000036000 00000598 Resource Directory [.rsrc]
+Entry 2 0000000000036000 00000590 Resource Directory [.rsrc]
 Entry 3 0000000000034000 00001e84 Exception Directory [.pdata]
 Entry 4 0000000000033400 00003090 Security Directory
 Entry 5 0000000000037000 00000470 Base Relocation Directory [.reloc]
 Entry 6 0000000000024958 00000054 Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
 Entry 9 0000000000024b00 00000028 Thread Storage Directory [.tls]
@@ -125,233 +125,233 @@
 	2d998	 1044  ?post@QNetworkAccessManager@@QEAAPEAVQNetworkReply@@AEBVQNetworkRequest@@PEAVQHttpMultiPart@@@Z
 	2da5c	  699  ?finished@QNetworkReply@@QEAAXXZ
 
  0002c878	0002ca20 00000000 00000000 00030470 000200f0
 
 	DLL Name: Qt6Core.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	30442	 3371  ?errorString@QIODevice@@QEBA?AVQString@@XZ
+	30442	 3372  ?errorString@QIODevice@@QEBA?AVQString@@XZ
 	30416	 5636  ?readAll@QIODevice@@QEAA?AVQByteArray@@XZ
-	303e6	 5028  ?object@QJsonDocument@@QEBA?AVQJsonObject@@XZ
-	303c2	 4269  ?isObject@QJsonDocument@@QEBA_NXZ
-	30378	 3621  ?fromJson@QJsonDocument@@SA?AV1@AEBVQByteArray@@PEAUQJsonParseError@@@Z
-	30356	 4136  ?isEmpty@QJsonObject@@QEBA_NXZ
-	30310	 7295  ?toVariantMap@QJsonObject@@QEBA?AV?$QMap@VQString@@VQVariant@@@@XZ
-	302f6	  830  ??1QJsonObject@@QEAA@XZ
-	302d8	 4265  ?isNull@QVariant@@QEBA_NXZ
-	302a8	 6762  ?staticMetaObject@QIODevice@@2UQMetaObject@@B
-	3027e	 3991  ?instance@QCoreApplication@@SAPEAV1@XZ
-	30248	 2125  ?applicationName@QCoreApplication@@SA?AVQString@@XZ
+	303e6	 5029  ?object@QJsonDocument@@QEBA?AVQJsonObject@@XZ
+	303c2	 4270  ?isObject@QJsonDocument@@QEBA_NXZ
+	30378	 3622  ?fromJson@QJsonDocument@@SA?AV1@AEBVQByteArray@@PEAUQJsonParseError@@@Z
+	30356	 4137  ?isEmpty@QJsonObject@@QEBA_NXZ
+	30310	 7296  ?toVariantMap@QJsonObject@@QEBA?AV?$QMap@VQString@@VQVariant@@@@XZ
+	302f6	  831  ??1QJsonObject@@QEAA@XZ
+	302d8	 4266  ?isNull@QVariant@@QEBA_NXZ
+	302a8	 6763  ?staticMetaObject@QIODevice@@2UQMetaObject@@B
+	3027e	 3992  ?instance@QCoreApplication@@SAPEAV1@XZ
+	30248	 2126  ?applicationName@QCoreApplication@@SA?AVQString@@XZ
 	30228	 5673  ?readyRead@QIODevice@@QEAAXXZ
-	30204	 3723  ?getChar@QIODevice@@QEAA_NPEAD@Z
-	301d6	 7660  ?write@QIODevice@@QEAA_JAEBVQByteArray@@@Z
-	301b0	 7343  ?tr@QObject@@SA?AVQString@@PEBD0H@Z
-	30160	 5110  ?path@QUrl@@QEBA?AVQString@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
-	30146	 4459  ?isValid@QUrl@@QEBA_NXZ
-	30110	 6493  ?setUrl@QUrl@@QEAAXAEBVQString@@W4ParsingMode@1@@Z
-	300e2	  532  ??0QString@@QEAA@_JW4Initialization@Qt@@@Z
-	300c2	 5018  ?number@QString@@SA?AV1@HH@Z
-	30084	 6714  ?startsWith@QString@@QEBA_NVQChar@@W4CaseSensitivity@Qt@@@Z
-	30064	 4807  ?mid@QString@@QEBA?AV1@_J0@Z
-	3003c	 2135  ?arg@QString@@QEBA?AV1@GHHVQChar@@@Z
-	2df98	 6772  ?staticMetaObject@QObject@@2UQMetaObject@@B
-	2dfc6	 2613  ?compareMemory@QtPrivate@@YAHVQByteArrayView@@0@Z
+	30204	 3724  ?getChar@QIODevice@@QEAA_NPEAD@Z
+	301d6	 7661  ?write@QIODevice@@QEAA_JAEBVQByteArray@@@Z
+	301b0	 7344  ?tr@QObject@@SA?AVQString@@PEBD0H@Z
+	30160	 5111  ?path@QUrl@@QEBA?AVQString@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
+	30146	 4460  ?isValid@QUrl@@QEBA_NXZ
+	30110	 6494  ?setUrl@QUrl@@QEAAXAEBVQString@@W4ParsingMode@1@@Z
+	300e2	  533  ??0QString@@QEAA@_JW4Initialization@Qt@@@Z
+	300c2	 5019  ?number@QString@@SA?AV1@HH@Z
+	30084	 6715  ?startsWith@QString@@QEBA_NVQChar@@W4CaseSensitivity@Qt@@@Z
+	30064	 4808  ?mid@QString@@QEBA?AV1@_J0@Z
+	3003c	 2136  ?arg@QString@@QEBA?AV1@GHHVQChar@@@Z
+	2df98	 6773  ?staticMetaObject@QObject@@2UQMetaObject@@B
+	2dfc6	 2614  ?compareMemory@QtPrivate@@YAHVQByteArrayView@@0@Z
 	2dffa	   93  ??0QByteArray@@QEAA@XZ
 	2e014	   91  ??0QByteArray@@QEAA@AEBV0@@Z
-	2e034	  765  ??1QByteArray@@QEAA@XZ
+	2e034	  766  ??1QByteArray@@QEAA@XZ
 	2e04e	   89  ??0QByteArray@@QEAA@$$QEAV0@@Z
 	2e070	 5872  ?reserve@QByteArray@@QEAAX_J@Z
-	2e092	 3024  ?data@QByteArray@@QEBAPEBDXZ
-	2e0b2	 2079  ?append@QByteArray@@QEAAAEAV1@PEBD@Z
-	2e0da	 6570  ?size@QByteArray@@QEBA_JXZ
-	2e0f8	 4244  ?isNull@QByteArray@@QEBA_NXZ
-	2e118	 1307  ??6@YAAEAVQDataStream@@AEAV0@AEBVQByteArray@@@Z
-	2e14a	 1189  ??5@YAAEAVQDataStream@@AEAV0@AEAVQByteArray@@@Z
-	2e17c	 2482  ?className@QMetaObject@@QEBAPEBDXZ
-	2e1a2	 7340  ?tr@QMetaObject@@QEBA?AVQString@@PEBD0H@Z
-	2e1ce	 1955  ?activate@QMetaObject@@SAXPEAVQObject@@PEBU1@HPEAPEAX@Z
-	2e208	 2620  ?compareStrings@QtPrivate@@YAHVQStringView@@0W4CaseSensitivity@Qt@@@Z
-	2e250	 3341  ?equalStrings@QtPrivate@@YA_NVQStringView@@0@Z
-	2e282	  530  ??0QString@@QEAA@XZ
-	2e298	  524  ??0QString@@QEAA@AEBV0@@Z
-	2e2b4	  886  ??1QString@@QEAA@XZ
-	2e2ca	  523  ??0QString@@QEAA@$$QEAV0@@Z
-	2e2e8	 1133  ??4QString@@QEAAAEAV0@$$QEAV0@@Z
-	2e30c	 3036  ?data@QString@@QEBAPEBVQChar@@XZ
-	2e330	 4261  ?isNull@QString@@QEBA_NXZ
-	2e34c	 1329  ??6@YAAEAVQDataStream@@AEAV0@AEBVQString@@@Z
-	2e37c	 1213  ??5@YAAEAVQDataStream@@AEAV0@AEAVQString@@@Z
-	2e3ac	  603  ??0QUrl@@QEAA@XZ
-	2e3c0	  601  ??0QUrl@@QEAA@AEBV0@@Z
-	2e3da	 1157  ??4QUrl@@QEAAAEAV0@$$QEAV0@@Z
-	2e3fa	  908  ??1QUrl@@QEAA@XZ
-	2e40e	 1607  ??MQUrl@@QEBA_NAEBV0@@Z
-	2e428	 1441  ??8QUrl@@QEBA_NAEBV0@@Z
-	2e442	 1332  ??6@YAAEAVQDataStream@@AEAV0@AEBVQUrl@@@Z
-	2e46e	 1217  ??5@YAAEAVQDataStream@@AEAV0@AEAVQUrl@@@Z
-	2e49a	 1292  ??6@YA?AVQDebug@@V0@AEBVQUrl@@@Z
-	2e4be	 6806  ?status@QDataStream@@QEBA?AW4Status@1@XZ
-	2e4ea	 6457  ?setStatus@QDataStream@@QEAAXW4Status@1@@Z
+	2e092	 3025  ?data@QByteArray@@QEBAPEBDXZ
+	2e0b2	 2080  ?append@QByteArray@@QEAAAEAV1@PEBD@Z
+	2e0da	 6571  ?size@QByteArray@@QEBA_JXZ
+	2e0f8	 4245  ?isNull@QByteArray@@QEBA_NXZ
+	2e118	 1308  ??6@YAAEAVQDataStream@@AEAV0@AEBVQByteArray@@@Z
+	2e14a	 1190  ??5@YAAEAVQDataStream@@AEAV0@AEAVQByteArray@@@Z
+	2e17c	 2483  ?className@QMetaObject@@QEBAPEBDXZ
+	2e1a2	 7341  ?tr@QMetaObject@@QEBA?AVQString@@PEBD0H@Z
+	2e1ce	 1956  ?activate@QMetaObject@@SAXPEAVQObject@@PEBU1@HPEAPEAX@Z
+	2e208	 2621  ?compareStrings@QtPrivate@@YAHVQStringView@@0W4CaseSensitivity@Qt@@@Z
+	2e250	 3342  ?equalStrings@QtPrivate@@YA_NVQStringView@@0@Z
+	2e282	  531  ??0QString@@QEAA@XZ
+	2e298	  525  ??0QString@@QEAA@AEBV0@@Z
+	2e2b4	  887  ??1QString@@QEAA@XZ
+	2e2ca	  524  ??0QString@@QEAA@$$QEAV0@@Z
+	2e2e8	 1134  ??4QString@@QEAAAEAV0@$$QEAV0@@Z
+	2e30c	 3037  ?data@QString@@QEBAPEBVQChar@@XZ
+	2e330	 4262  ?isNull@QString@@QEBA_NXZ
+	2e34c	 1330  ??6@YAAEAVQDataStream@@AEAV0@AEBVQString@@@Z
+	2e37c	 1214  ??5@YAAEAVQDataStream@@AEAV0@AEAVQString@@@Z
+	2e3ac	  604  ??0QUrl@@QEAA@XZ
+	2e3c0	  602  ??0QUrl@@QEAA@AEBV0@@Z
+	2e3da	 1158  ??4QUrl@@QEAAAEAV0@$$QEAV0@@Z
+	2e3fa	  909  ??1QUrl@@QEAA@XZ
+	2e40e	 1608  ??MQUrl@@QEBA_NAEBV0@@Z
+	2e428	 1442  ??8QUrl@@QEBA_NAEBV0@@Z
+	2e442	 1333  ??6@YAAEAVQDataStream@@AEAV0@AEBVQUrl@@@Z
+	2e46e	 1218  ??5@YAAEAVQDataStream@@AEAV0@AEAVQUrl@@@Z
+	2e49a	 1293  ??6@YA?AVQDebug@@V0@AEBVQUrl@@@Z
+	2e4be	 6807  ?status@QDataStream@@QEBA?AW4Status@1@XZ
+	2e4ea	 6458  ?setStatus@QDataStream@@QEAAXW4Status@1@@Z
 	2e518	 5892  ?resetStatus@QDataStream@@QEAAXXZ
-	2e53c	 1230  ??5QDataStream@@QEAAAEAV0@AEAH@Z
-	2e560	 1349  ??6QDataStream@@QEAAAEAV0@H@Z
-	2e580	 4115  ?isDeviceTransactionStarted@QDataStream@@QEBA_NXZ
+	2e53c	 1231  ??5QDataStream@@QEAAAEAV0@AEAH@Z
+	2e560	 1350  ??6QDataStream@@QEAAAEAV0@H@Z
+	2e580	 4116  ?isDeviceTransactionStarted@QDataStream@@QEBA_NXZ
 	2e5b4	 5707  ?registerNormalizedTypedef@QMetaType@@SAXAEBVQByteArray@@V1@@Z
-	2e5f6	 3851  ?id@QMetaType@@QEBAHH@Z
-	2e610	 3229  ?dynamicMetaObject@QObjectData@@QEBAPEAUQMetaObject@@XZ
-	2e64a	 5502  ?qt_metacast@QObject@@UEAAPEAXPEBD@Z
-	2e672	 5449  ?qt_metacall@QObject@@UEAAHW4Call@QMetaObject@@HPEAPEAX@Z
+	2e5f6	 3852  ?id@QMetaType@@QEBAHH@Z
+	2e610	 3230  ?dynamicMetaObject@QObjectData@@QEBAPEAUQMetaObject@@XZ
+	2e64a	 5503  ?qt_metacast@QObject@@UEAAPEAXPEBD@Z
+	2e672	 5450  ?qt_metacall@QObject@@UEAAHW4Call@QMetaObject@@HPEAPEAX@Z
 	2e6ae	  214  ??0QDebug@@QEAA@$$QEAV0@@Z
-	2e6cc	  790  ??1QDebug@@QEAA@XZ
-	2e6e2	 1363  ??6QDebug@@QEAAAEAV0@D@Z
-	2e6fe	 1373  ??6QDebug@@QEAAAEAV0@PEBD@Z
-	2e71c	 1362  ??6QDebug@@QEAAAEAV0@AEBVQString@@@Z
-	2e744	 1361  ??6QDebug@@QEAAAEAV0@AEBVQByteArray@@@Z
+	2e6cc	  791  ??1QDebug@@QEAA@XZ
+	2e6e2	 1364  ??6QDebug@@QEAAAEAV0@D@Z
+	2e6fe	 1374  ??6QDebug@@QEAAAEAV0@PEBD@Z
+	2e71c	 1363  ??6QDebug@@QEAAAEAV0@AEBVQString@@@Z
+	2e744	 1362  ??6QDebug@@QEAAAEAV0@AEBVQByteArray@@@Z
 	2e76e	  219  ??0QDebugStateSaver@@QEAA@AEAVQDebug@@@Z
-	2e79a	  791  ??1QDebugStateSaver@@QEAA@XZ
-	2e7ba	 5408  ?qt_QMetaEnum_debugOperator@@YA?AVQDebug@@AEAV1@_JPEBUQMetaObject@@PEBD@Z
-	2e806	  669  ??0QVariant@@QEAA@XZ
-	2e81e	  910  ??1QVariant@@QEAA@XZ
-	2e836	  621  ??0QVariant@@QEAA@AEBV0@@Z
-	2e854	 1166  ??4QVariant@@QEAAAEAV0@AEBV0@@Z
-	2e876	 5389  ?qdebugHelper@QVariant@@AEBA?AVQDebug@@V2@@Z
-	2e8a6	 3348  ?equals@QVariant@@IEBA_NAEBV1@@Z
-	2e8ca	 1219  ??5@YAAEAVQDataStream@@AEAV0@AEAVQVariant@@@Z
-	2e8fa	 1334  ??6@YAAEAVQDataStream@@AEAV0@AEBVQVariant@@@Z
-	2e92a	  972  ??4QByteArray@@QEAAAEAV0@$$QEAV0@@Z
-	2e950	 2078  ?append@QByteArray@@QEAAAEAV1@D@Z
-	2e974	 1134  ??4QString@@QEAAAEAV0@AEBV0@@Z
-	2e996	 7278  ?toUtf8@QString@@QEHAA?AVQByteArray@@XZ
-	2e9c0	  522  ??0QString@@QEAA@$$QEAU?$QArrayDataPointer@_S@@@Z
-	2e9f4	 1158  ??4QUrl@@QEAAAEAV0@AEBV0@@Z
-	2ea12	 6396  ?setQuery@QUrl@@QEAAXAEBVQUrlQuery@@@Z
-	2ea3c	 1480  ??9QUrl@@QEBA_NAEBV0@@Z
-	2ea56	  850  ??1QObject@@UEAA@XZ
-	2ea6c	 5088  ?parent@QObject@@QEBAPEAV1@XZ
+	2e79a	  792  ??1QDebugStateSaver@@QEAA@XZ
+	2e7ba	 5409  ?qt_QMetaEnum_debugOperator@@YA?AVQDebug@@AEAV1@_JPEBUQMetaObject@@PEBD@Z
+	2e806	  670  ??0QVariant@@QEAA@XZ
+	2e81e	  911  ??1QVariant@@QEAA@XZ
+	2e836	  622  ??0QVariant@@QEAA@AEBV0@@Z
+	2e854	 1167  ??4QVariant@@QEAAAEAV0@AEBV0@@Z
+	2e876	 5390  ?qdebugHelper@QVariant@@AEBA?AVQDebug@@V2@@Z
+	2e8a6	 3349  ?equals@QVariant@@IEBA_NAEBV1@@Z
+	2e8ca	 1220  ??5@YAAEAVQDataStream@@AEAV0@AEAVQVariant@@@Z
+	2e8fa	 1335  ??6@YAAEAVQDataStream@@AEAV0@AEBVQVariant@@@Z
+	2e92a	  973  ??4QByteArray@@QEAAAEAV0@$$QEAV0@@Z
+	2e950	 2079  ?append@QByteArray@@QEAAAEAV1@D@Z
+	2e974	 1135  ??4QString@@QEAAAEAV0@AEBV0@@Z
+	2e996	 7279  ?toUtf8@QString@@QEHAA?AVQByteArray@@XZ
+	2e9c0	  523  ??0QString@@QEAA@$$QEAU?$QArrayDataPointer@_S@@@Z
+	2e9f4	 1159  ??4QUrl@@QEAAAEAV0@AEBV0@@Z
+	2ea12	 6397  ?setQuery@QUrl@@QEAAXAEBVQUrlQuery@@@Z
+	2ea3c	 1481  ??9QUrl@@QEBA_NAEBV0@@Z
+	2ea56	  851  ??1QObject@@UEAA@XZ
+	2ea6c	 5089  ?parent@QObject@@QEBAPEAV1@XZ
 	2ea8c	  416  ??0QObject@@IEAA@AEAVQObjectPrivate@@PEAV0@@Z
-	2eabc	 3721  ?getAndRef@ExternalRefCountData@QtSharedPointer@@SAPEAU12@PEBVQObject@@@Z
-	2eb08	  625  ??0QVariant@@QEAA@AEBV?$QMap@VQString@@VQVariant@@@@@Z
-	2eb42	  646  ??0QVariant@@QEAA@AEBVQString@@@Z
-	2eb66	 7221  ?toString@QVariant@@QEBA?AVQString@@XZ
+	2eabc	 3722  ?getAndRef@ExternalRefCountData@QtSharedPointer@@SAPEAU12@PEBVQObject@@@Z
+	2eb08	  626  ??0QVariant@@QEAA@AEBV?$QMap@VQString@@VQVariant@@@@@Z
+	2eb42	  647  ??0QVariant@@QEAA@AEBVQString@@@Z
+	2eb66	 7222  ?toString@QVariant@@QEBA?AVQString@@XZ
 	2eb90	  420  ??0QObjectPrivate@@QEAA@H@Z
-	2ebae	  853  ??1QObjectPrivate@@UEAA@XZ
+	2ebae	  854  ??1QObjectPrivate@@UEAA@XZ
 	2ebcc	  367  ??0QLoggingCategory@@QEAA@PEBDW4QtMsgType@@@Z
-	2ebfc	  838  ??1QLoggingCategory@@QEAA@XZ
-	2ec1c	  788  ??1QDateTime@@QEAA@XZ
-	2ec34	 7125  ?toMSecsSinceEpoch@QDateTime@@QEBA_JXZ
-	2ec5e	 2880  ?currentDateTime@QDateTime@@SA?AV1@XZ
-	2ec86	  609  ??0QUrlQuery@@QEAA@XZ
-	2ec9e	  909  ??1QUrlQuery@@QEAA@XZ
-	2ecb6	 7219  ?toString@QUrlQuery@@QEBA?AVQString@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
-	2ed0e	 2019  ?addQueryItem@QUrlQuery@@QEAAXAEBVQString@@0@Z
-	2ed40	  829  ??1QJsonDocument@@QEAA@XZ
-	2ed5c	 3698  ?fromVariant@QJsonDocument@@SA?AV1@AEBVQVariant@@@Z
-	2ed92	 7077  ?toJson@QJsonDocument@@QEBA?AVQByteArray@@W4JsonFormat@1@@Z
-	2edd0	 2464  ?childEvent@QObject@@MEAAXPEAVQChildEvent@@@Z
-	2ee00	 2661  ?connectNotify@QObject@@MEAAXAEBVQMetaMethod@@@Z
-	2ee34	 2910  ?customEvent@QObject@@MEAAXPEAVQEvent@@@Z
-	2ee60	 3184  ?disconnectNotify@QObject@@MEAAXAEBVQMetaMethod@@@Z
-	2ee96	 3393  ?event@QObject@@UEAA_NPEAVQEvent@@@Z
-	2eebe	 3409  ?eventFilter@QObject@@UEAA_NPEAV1@PEAVQEvent@@@Z
-	2eef2	 3584  ?flagsForDumping@QObjectPrivate@@UEBA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@XZ
-	2ef5c	 6961  ?timerEvent@QObject@@MEAAXPEAVQTimerEvent@@@Z
+	2ebfc	  839  ??1QLoggingCategory@@QEAA@XZ
+	2ec1c	  789  ??1QDateTime@@QEAA@XZ
+	2ec34	 7126  ?toMSecsSinceEpoch@QDateTime@@QEBA_JXZ
+	2ec5e	 2881  ?currentDateTime@QDateTime@@SA?AV1@XZ
+	2ec86	  610  ??0QUrlQuery@@QEAA@XZ
+	2ec9e	  910  ??1QUrlQuery@@QEAA@XZ
+	2ecb6	 7220  ?toString@QUrlQuery@@QEBA?AVQString@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
+	2ed0e	 2020  ?addQueryItem@QUrlQuery@@QEAAXAEBVQString@@0@Z
+	2ed40	  830  ??1QJsonDocument@@QEAA@XZ
+	2ed5c	 3699  ?fromVariant@QJsonDocument@@SA?AV1@AEBVQVariant@@@Z
+	2ed92	 7078  ?toJson@QJsonDocument@@QEBA?AVQByteArray@@W4JsonFormat@1@@Z
+	2edd0	 2465  ?childEvent@QObject@@MEAAXPEAVQChildEvent@@@Z
+	2ee00	 2662  ?connectNotify@QObject@@MEAAXAEBVQMetaMethod@@@Z
+	2ee34	 2911  ?customEvent@QObject@@MEAAXPEAVQEvent@@@Z
+	2ee60	 3185  ?disconnectNotify@QObject@@MEAAXAEBVQMetaMethod@@@Z
+	2ee96	 3394  ?event@QObject@@UEAA_NPEAVQEvent@@@Z
+	2eebe	 3410  ?eventFilter@QObject@@UEAA_NPEAV1@PEAVQEvent@@@Z
+	2eef2	 3585  ?flagsForDumping@QObjectPrivate@@UEBA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@XZ
+	2ef5c	 6962  ?timerEvent@QObject@@MEAAXPEAVQTimerEvent@@@Z
 	2ef8c	  371  ??0QMessageLogger@@QEAA@PEBDH00@Z
-	2efb0	 7632  ?warning@QMessageLogger@@QEBAXPEBDZZ
-	2efd8	 4589  ?lengthHelperCharArray@QByteArrayView@@CA_JPEBD_K@Z
+	2efb0	 7633  ?warning@QMessageLogger@@QEBAXPEBDZZ
+	2efd8	 4590  ?lengthHelperCharArray@QByteArrayView@@CA_JPEBD_K@Z
 	2f00e	   92  ??0QByteArray@@QEAA@PEBD_J@Z
-	2f02e	 2132  ?arg@QString@@QEBA?AV1@AEBV1@HVQChar@@@Z
-	2f05a	 7277  ?toUtf8@QString@@QEGBA?AVQByteArray@@XZ
-	2f084	 3696  ?fromUtf8@QString@@SA?AV1@VQByteArrayView@@@Z
-	2f0b4	 4989  ?normalizedType@QMetaObject@@SA?AVQByteArray@@PEBD@Z
-	2f0ec	  736  ??1Connection@QMetaObject@@QEAA@XZ
-	2f112	 2657  ?connectImpl@QObject@@CA?AVConnection@QMetaObject@@PEBV1@PEAPEAX01PEAVQSlotObjectBase@QtPrivate@@W4ConnectionType@Qt@@PEBHPEBU3@@Z
+	2f02e	 2133  ?arg@QString@@QEBA?AV1@AEBV1@HVQChar@@@Z
+	2f05a	 7278  ?toUtf8@QString@@QEGBA?AVQByteArray@@XZ
+	2f084	 3697  ?fromUtf8@QString@@SA?AV1@VQByteArrayView@@@Z
+	2f0b4	 4990  ?normalizedType@QMetaObject@@SA?AVQByteArray@@PEBD@Z
+	2f0ec	  737  ??1Connection@QMetaObject@@QEAA@XZ
+	2f112	 2658  ?connectImpl@QObject@@CA?AVConnection@QMetaObject@@PEBV1@PEAPEAX01PEAVQSlotObjectBase@QtPrivate@@W4ConnectionType@Qt@@PEBHPEBU3@@Z
 	2f198	  207  ??0QDateTime@@QEAA@XZ
 	2f1b0	  203  ??0QDateTime@@QEAA@AEBV0@@Z
 	2f1ce	  202  ??0QDateTime@@QEAA@$$QEAV0@@Z
-	2f1ee	 1006  ??4QDateTime@@QEAAAEAV0@$$QEAV0@@Z
-	2f214	 3344  ?equals@QDateTime@@AEBA_NAEBV1@@Z
-	2f238	 5164  ?precedes@QDateTime@@AEBA_NAEBV1@@Z
-	2f25e	 1311  ??6@YAAEAVQDataStream@@AEAV0@AEBVQDateTime@@@Z
-	2f290	 1195  ??5@YAAEAVQDataStream@@AEAV0@AEAVQDateTime@@@Z
-	2f2c2	 1262  ??6@YA?AVQDebug@@V0@AEBVQDateTime@@@Z
+	2f1ee	 1007  ??4QDateTime@@QEAAAEAV0@$$QEAV0@@Z
+	2f214	 3345  ?equals@QDateTime@@AEBA_NAEBV1@@Z
+	2f238	 5165  ?precedes@QDateTime@@AEBA_NAEBV1@@Z
+	2f25e	 1312  ??6@YAAEAVQDataStream@@AEAV0@AEBVQDateTime@@@Z
+	2f290	 1196  ??5@YAAEAVQDataStream@@AEAV0@AEAVQDateTime@@@Z
+	2f2c2	 1263  ??6@YA?AVQDebug@@V0@AEBVQDateTime@@@Z
 	2f2ea	 5597  ?query@QUrl@@QEBA?AVQString@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
-	2f33a	 4470  ?isWarningEnabled@QLoggingCategory@@QEBA_NXZ
-	2f36a	  606  ??0QUrlQuery@@QEAA@AEBVQString@@@Z
+	2f33a	 4471  ?isWarningEnabled@QLoggingCategory@@QEBA_NXZ
+	2f36a	  607  ??0QUrlQuery@@QEAA@AEBVQString@@@Z
 	2f390	  417  ??0QObject@@QEAA@PEAV0@@Z
 	2f3ac	  372  ??0QMessageLogger@@QEAA@PEBDH0@Z
-	2f3d0	 3458  ?fatal@QMessageLogger@@QEBAXPEBDZZ
-	2f3f6	 2061  ?allocate@QArrayData@@SAPEAXPEAPEAU1@_J11W4AllocationOption@1@@Z
+	2f3d0	 3459  ?fatal@QMessageLogger@@QEBAXPEBDZZ
+	2f3f6	 2062  ?allocate@QArrayData@@SAPEAXPEAPEAU1@_J11W4AllocationOption@1@@Z
 	2f43a	 5684  ?reallocateUnaligned@QArrayData@@SA?AU?$pair@PEAUQArrayData@@PEAX@std@@PEAU1@PEAX_J2W4AllocationOption@1@@Z
-	2f4a8	 2676  ?constData@QByteArray@@QEBAPEBDXZ
-	2f4cc	 6981  ?toBase64@QByteArray@@QEBA?AV1@V?$QFlags@W4Base64Option@QByteArray@@@@@Z
-	2f518	 2421  ?cast@QMetaObject@@QEBAPEBVQObject@@PEBV2@@Z
+	2f4a8	 2677  ?constData@QByteArray@@QEBAPEBDXZ
+	2f4cc	 6982  ?toBase64@QByteArray@@QEBA?AV1@V?$QFlags@W4Base64Option@QByteArray@@@@@Z
+	2f518	 2422  ?cast@QMetaObject@@QEBAPEBVQObject@@PEBV2@@Z
 	2f548	   29  ??0Connection@QMetaObject@@QEAA@XZ
-	2f56e	  947  ??4Connection@QMetaObject@@QEAAAEAV01@$$QEAV01@@Z
+	2f56e	  948  ??4Connection@QMetaObject@@QEAAAEAV01@$$QEAV01@@Z
 	2f5a2	  164  ??0QChar@@QEAA@UQLatin1Char@@@Z
 	2f5c4	 5900  ?resize@QString@@QEAAX_J@Z
-	2f5e2	 2398  ?capacity@QString@@QEBA_JXZ
+	2f5e2	 2399  ?capacity@QString@@QEBA_JXZ
 	2f600	 5874  ?reserve@QString@@QEAAX_J@Z
-	2f61e	 3035  ?data@QString@@QEAAPEAVQChar@@XZ
-	2f642	 2679  ?constData@QString@@QEBAPEBVQChar@@XZ
-	2f66a	 3145  ?detach@QString@@QEAAXXZ
-	2f686	 2501  ?clear@QString@@QEAAXXZ
-	2f6a0	 6713  ?startsWith@QString@@QEBA_NAEBV1@W4CaseSensitivity@Qt@@@Z
-	2f6dc	 2112  ?append@QString@@QEAAAEAV1@VQLatin1String@@@Z
-	2f70c	 7097  ?toLocal8Bit@QString@@QEGBA?AVQByteArray@@XZ
-	2f73c	 5023  ?number@QString@@SA?AV1@_JH@Z
-	2f75c	 2118  ?appendLatin1To@QAbstractConcatenable@@KAXVQLatin1String@@PEAVQChar@@@Z
-	2f7a6	 4145  ?isEmpty@QUrl@@QEBA_NXZ
-	2f7c0	 7142  ?toPercentEncoding@QUrl@@SA?AVQByteArray@@AEBVQString@@AEBV2@1@Z
-	2f804	 3176  ?disconnect@QObject@@SA_NAEBVConnection@QMetaObject@@@Z
-	2f83e	 3117  ?deleteLater@QObject@@QEAAXXZ
-	2f85e	  672  ??0QVariant@@QEAA@_N@Z
-	2f878	  627  ??0QVariant@@QEAA@AEBVQByteArray@@@Z
-	2f8a0	  620  ??0QVariant@@QEAA@$$QEAV0@@Z
-	2f8c0	 6988  ?toBool@QVariant@@QEBA_NXZ
-	2f8de	 6993  ?toByteArray@QVariant@@QEBA?AVQByteArray@@XZ
-	2f90e	 7157  ?toSecsSinceEpoch@QDateTime@@QEBA_JXZ
-	2f936	 2881  ?currentDateTimeUtc@QDateTime@@SA?AV1@XZ
-	2f962	 3716  ?get@QObjectPrivate@@SAPEAV1@PEAVQObject@@@Z
+	2f61e	 3036  ?data@QString@@QEAAPEAVQChar@@XZ
+	2f642	 2680  ?constData@QString@@QEBAPEBVQChar@@XZ
+	2f66a	 3146  ?detach@QString@@QEAAXXZ
+	2f686	 2502  ?clear@QString@@QEAAXXZ
+	2f6a0	 6714  ?startsWith@QString@@QEBA_NAEBV1@W4CaseSensitivity@Qt@@@Z
+	2f6dc	 2113  ?append@QString@@QEAAAEAV1@VQLatin1String@@@Z
+	2f70c	 7098  ?toLocal8Bit@QString@@QEGBA?AVQByteArray@@XZ
+	2f73c	 5024  ?number@QString@@SA?AV1@_JH@Z
+	2f75c	 2119  ?appendLatin1To@QAbstractConcatenable@@KAXVQLatin1String@@PEAVQChar@@@Z
+	2f7a6	 4146  ?isEmpty@QUrl@@QEBA_NXZ
+	2f7c0	 7143  ?toPercentEncoding@QUrl@@SA?AVQByteArray@@AEBVQString@@AEBV2@1@Z
+	2f804	 3177  ?disconnect@QObject@@SA_NAEBVConnection@QMetaObject@@@Z
+	2f83e	 3118  ?deleteLater@QObject@@QEAAXXZ
+	2f85e	  673  ??0QVariant@@QEAA@_N@Z
+	2f878	  628  ??0QVariant@@QEAA@AEBVQByteArray@@@Z
+	2f8a0	  621  ??0QVariant@@QEAA@$$QEAV0@@Z
+	2f8c0	 6989  ?toBool@QVariant@@QEBA_NXZ
+	2f8de	 6994  ?toByteArray@QVariant@@QEBA?AVQByteArray@@XZ
+	2f90e	 7158  ?toSecsSinceEpoch@QDateTime@@QEBA_JXZ
+	2f936	 2882  ?currentDateTimeUtc@QDateTime@@SA?AV1@XZ
+	2f962	 3717  ?get@QObjectPrivate@@SAPEAV1@PEAVQObject@@@Z
 	2f992	 5600  ?queryItems@QUrlQuery@@QEBA?AV?$QList@U?$pair@VQString@@V1@@std@@@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
-	2fa08	 2867  ?critical@QMessageLogger@@QEBAXPEBDZZ
+	2fa08	 2868  ?critical@QMessageLogger@@QEBAXPEBDZZ
 	2fa30	   95  ??0QByteArray@@QEAA@_JW4Initialization@Qt@@@Z
-	2fa60	  973  ??4QByteArray@@QEAAAEAV0@AEBV0@@Z
-	2fa84	 4128  ?isEmpty@QByteArray@@QEBA_NXZ
+	2fa60	  974  ??4QByteArray@@QEAAAEAV0@AEBV0@@Z
+	2fa84	 4129  ?isEmpty@QByteArray@@QEBA_NXZ
 	2faa4	 5895  ?resize@QByteArray@@QEAAX_J@Z
-	2fac4	 2397  ?capacity@QByteArray@@QEBA_JXZ
-	2fae6	 3023  ?data@QByteArray@@QEAAPEADXZ
-	2fb06	 3136  ?detach@QByteArray@@QEAAXXZ
-	2fb24	 2077  ?append@QByteArray@@QEAAAEAV1@AEBV1@@Z
-	2fb4e	 3261  ?end@QByteArray@@QEBAPEBDXZ
+	2fac4	 2398  ?capacity@QByteArray@@QEBA_JXZ
+	2fae6	 3024  ?data@QByteArray@@QEAAPEADXZ
+	2fb06	 3137  ?detach@QByteArray@@QEAAXXZ
+	2fb24	 2078  ?append@QByteArray@@QEAAAEAV1@AEBV1@@Z
+	2fb4e	 3262  ?end@QByteArray@@QEBAPEBDXZ
 	2fb6c	 5854  ?replace@QString@@QEAAAEAV1@VQChar@@0W4CaseSensitivity@Qt@@@Z
-	2fbac	 3630  ?fromLatin1@QString@@SA?AV1@VQByteArrayView@@@Z
-	2fbde	 7218  ?toString@QUrl@@QEBA?AVQString@@V?$QUrlTwoFlags@W4UrlFormattingOption@QUrl@@W4ComponentFormattingOption@2@@@@Z
-	2fc50	 4090  ?isCriticalEnabled@QLoggingCategory@@QEBA_NXZ
-	2fc80	 3823  ?hash@QMessageAuthenticationCode@@SA?AVQByteArray@@VQByteArrayView@@0W4Algorithm@QCryptographicHash@@@Z
-	2fcea	 3092  ?debug@QMessageLogger@@QEBAXPEBDZZ
-	2fd10	 7629  ?warning@QMessageLogger@@QEBA?AVQDebug@@XZ
-	2fd3e	  529  ??0QString@@QEAA@VQLatin1String@@@Z
-	2fd64	 7098  ?toLocal8Bit@QString@@QEHAA?AVQByteArray@@XZ
-	2fd94	 1366  ??6QDebug@@QEAAAEAV0@H@Z
-	2fdb0	 4460  ?isValid@QVariant@@QEBA_NXZ
-	2fdce	 7069  ?toInt@QVariant@@QEBAHPEA_N@Z
-	2fdee	 2024  ?addSecs@QDateTime@@QEBA?AV1@_J@Z
+	2fbac	 3631  ?fromLatin1@QString@@SA?AV1@VQByteArrayView@@@Z
+	2fbde	 7219  ?toString@QUrl@@QEBA?AVQString@@V?$QUrlTwoFlags@W4UrlFormattingOption@QUrl@@W4ComponentFormattingOption@2@@@@Z
+	2fc50	 4091  ?isCriticalEnabled@QLoggingCategory@@QEBA_NXZ
+	2fc80	 3824  ?hash@QMessageAuthenticationCode@@SA?AVQByteArray@@VQByteArrayView@@0W4Algorithm@QCryptographicHash@@@Z
+	2fcea	 3093  ?debug@QMessageLogger@@QEBAXPEBDZZ
+	2fd10	 7630  ?warning@QMessageLogger@@QEBA?AVQDebug@@XZ
+	2fd3e	  530  ??0QString@@QEAA@VQLatin1String@@@Z
+	2fd64	 7099  ?toLocal8Bit@QString@@QEHAA?AVQByteArray@@XZ
+	2fd94	 1367  ??6QDebug@@QEAAAEAV0@H@Z
+	2fdb0	 4461  ?isValid@QVariant@@QEBA_NXZ
+	2fdce	 7070  ?toInt@QVariant@@QEBAHPEA_N@Z
+	2fdee	 2025  ?addSecs@QDateTime@@QEBA?AV1@_J@Z
 	2fe12	 6017  ?secsTo@QDateTime@@QEBA_JAEBV1@@Z
-	2fe36	  602  ??0QUrl@@QEAA@AEBVQString@@W4ParsingMode@0@@Z
-	2fe66	 4099  ?isDebugEnabled@QLoggingCategory@@QEBA_NXZ
-	2fe94	 1160  ??4QUrlQuery@@QEAAAEAV0@$$QEAV0@@Z
-	2feba	 2490  ?clear@QByteArray@@QEAAXXZ
-	2fed8	 2165  ?at@QByteArray@@QEBAD_J@Z
-	2fef4	 3882  ?indexOf@QByteArray@@QEBA_JD_J@Z
-	2ff18	 4804  ?mid@QByteArray@@QEBA?AV1@_J0@Z
-	2ff3a	 6710  ?startsWith@QByteArray@@QEBA_NVQByteArrayView@@@Z
-	2ff6e	 3297  ?endsWith@QByteArray@@QEBA_NVQByteArrayView@@@Z
-	2ffa0	 2469  ?chop@QByteArray@@QEAAX_J@Z
-	2ffbe	 7397  ?trimmed@QByteArray@@QEHAA?AV1@XZ
-	2ffe2	 5016  ?number@QByteArray@@SA?AV1@_JH@Z
+	2fe36	  603  ??0QUrl@@QEAA@AEBVQString@@W4ParsingMode@0@@Z
+	2fe66	 4100  ?isDebugEnabled@QLoggingCategory@@QEBA_NXZ
+	2fe94	 1161  ??4QUrlQuery@@QEAAAEAV0@$$QEAV0@@Z
+	2feba	 2491  ?clear@QByteArray@@QEAAXXZ
+	2fed8	 2166  ?at@QByteArray@@QEBAD_J@Z
+	2fef4	 3883  ?indexOf@QByteArray@@QEBA_JD_J@Z
+	2ff18	 4805  ?mid@QByteArray@@QEBA?AV1@_J0@Z
+	2ff3a	 6711  ?startsWith@QByteArray@@QEBA_NVQByteArrayView@@@Z
+	2ff6e	 3298  ?endsWith@QByteArray@@QEBA_NVQByteArrayView@@@Z
+	2ffa0	 2470  ?chop@QByteArray@@QEAAX_J@Z
+	2ffbe	 7398  ?trimmed@QByteArray@@QEHAA?AV1@XZ
+	2ffe2	 5017  ?number@QByteArray@@SA?AV1@_JH@Z
 	30006	   88  ??0QByteArray@@QEAA@$$QEAU?$QArrayDataPointer@D@@@Z
 
  0002c88c	0002ca08 00000000 00000000 000304c0 000200d8
 
 	DLL Name: MSVCP140.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	3049e	  652  ?_Xbad_function_call@std@@YAXXZ
@@ -7013,601 +7013,601 @@
 	  5d70: 4e 65 74 77 6f 72 6b 45 72 72 6f 72 40 31 40 58
 	  5d80: 5a 00 eb 02 3f 68 65 61 64 65 72 40 51 4e 65 74
 	  5d90: 77 6f 72 6b 52 65 70 6c 79 40 40 51 45 42 41 3f
 	  5da0: 41 56 51 56 61 72 69 61 6e 74 40 40 57 34 4b 6e
 	  5db0: 6f 77 6e 48 65 61 64 65 72 73 40 51 4e 65 74 77
 	  5dc0: 6f 72 6b 52 65 71 75 65 73 74 40 40 40 5a 00 00
 	  5dd0: 51 74 36 4e 65 74 77 6f 72 6b 2e 64 6c 6c 00 00
-	  5de0: 74 1a 3f 73 74 61 74 69 63 4d 65 74 61 4f 62 6a
+	  5de0: 75 1a 3f 73 74 61 74 69 63 4d 65 74 61 4f 62 6a
 	  5df0: 65 63 74 40 51 4f 62 6a 65 63 74 40 40 32 55 51
-	  5e00: 4d 65 74 61 4f 62 6a 65 63 74 40 40 42 00 35 0a
+	  5e00: 4d 65 74 61 4f 62 6a 65 63 74 40 40 42 00 36 0a
 	  5e10: 3f 63 6f 6d 70 61 72 65 4d 65 6d 6f 72 79 40 51
 	  5e20: 74 50 72 69 76 61 74 65 40 40 59 41 48 56 51 42
 	  5e30: 79 74 65 41 72 72 61 79 56 69 65 77 40 40 30 40
 	  5e40: 5a 00 5d 00 3f 3f 30 51 42 79 74 65 41 72 72 61
 	  5e50: 79 40 40 51 45 41 41 40 58 5a 00 00 5b 00 3f 3f
 	  5e60: 30 51 42 79 74 65 41 72 72 61 79 40 40 51 45 41
-	  5e70: 41 40 41 45 42 56 30 40 40 5a 00 00 fd 02 3f 3f
+	  5e70: 41 40 41 45 42 56 30 40 40 5a 00 00 fe 02 3f 3f
 	  5e80: 31 51 42 79 74 65 41 72 72 61 79 40 40 51 45 41
 	  5e90: 41 40 58 5a 00 00 59 00 3f 3f 30 51 42 79 74 65
 	  5ea0: 41 72 72 61 79 40 40 51 45 41 41 40 24 24 51 45
 	  5eb0: 41 56 30 40 40 5a 00 00 f0 16 3f 72 65 73 65 72
 	  5ec0: 76 65 40 51 42 79 74 65 41 72 72 61 79 40 40 51
-	  5ed0: 45 41 41 58 5f 4a 40 5a 00 00 d0 0b 3f 64 61 74
+	  5ed0: 45 41 41 58 5f 4a 40 5a 00 00 d1 0b 3f 64 61 74
 	  5ee0: 61 40 51 42 79 74 65 41 72 72 61 79 40 40 51 45
-	  5ef0: 42 41 50 45 42 44 58 5a 00 00 1f 08 3f 61 70 70
+	  5ef0: 42 41 50 45 42 44 58 5a 00 00 20 08 3f 61 70 70
 	  5f00: 65 6e 64 40 51 42 79 74 65 41 72 72 61 79 40 40
 	  5f10: 51 45 41 41 41 45 41 56 31 40 50 45 42 44 40 5a
-	  5f20: 00 00 aa 19 3f 73 69 7a 65 40 51 42 79 74 65 41
+	  5f20: 00 00 ab 19 3f 73 69 7a 65 40 51 42 79 74 65 41
 	  5f30: 72 72 61 79 40 40 51 45 42 41 5f 4a 58 5a 00 00
-	  5f40: 94 10 3f 69 73 4e 75 6c 6c 40 51 42 79 74 65 41
+	  5f40: 95 10 3f 69 73 4e 75 6c 6c 40 51 42 79 74 65 41
 	  5f50: 72 72 61 79 40 40 51 45 42 41 5f 4e 58 5a 00 00
-	  5f60: 1b 05 3f 3f 36 40 59 41 41 45 41 56 51 44 61 74
+	  5f60: 1c 05 3f 3f 36 40 59 41 41 45 41 56 51 44 61 74
 	  5f70: 61 53 74 72 65 61 6d 40 40 41 45 41 56 30 40 41
 	  5f80: 45 42 56 51 42 79 74 65 41 72 72 61 79 40 40 40
-	  5f90: 5a 00 a5 04 3f 3f 35 40 59 41 41 45 41 56 51 44
+	  5f90: 5a 00 a6 04 3f 3f 35 40 59 41 41 45 41 56 51 44
 	  5fa0: 61 74 61 53 74 72 65 61 6d 40 40 41 45 41 56 30
 	  5fb0: 40 41 45 41 56 51 42 79 74 65 41 72 72 61 79 40
-	  5fc0: 40 40 5a 00 b2 09 3f 63 6c 61 73 73 4e 61 6d 65
+	  5fc0: 40 40 5a 00 b3 09 3f 63 6c 61 73 73 4e 61 6d 65
 	  5fd0: 40 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 51 45
-	  5fe0: 42 41 50 45 42 44 58 5a 00 00 ac 1c 3f 74 72 40
+	  5fe0: 42 41 50 45 42 44 58 5a 00 00 ad 1c 3f 74 72 40
 	  5ff0: 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 51 45 42
 	  6000: 41 3f 41 56 51 53 74 72 69 6e 67 40 40 50 45 42
-	  6010: 44 30 48 40 5a 00 a3 07 3f 61 63 74 69 76 61 74
+	  6010: 44 30 48 40 5a 00 a4 07 3f 61 63 74 69 76 61 74
 	  6020: 65 40 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 53
 	  6030: 41 58 50 45 41 56 51 4f 62 6a 65 63 74 40 40 50
 	  6040: 45 42 55 31 40 48 50 45 41 50 45 41 58 40 5a 00
-	  6050: 3c 0a 3f 63 6f 6d 70 61 72 65 53 74 72 69 6e 67
+	  6050: 3d 0a 3f 63 6f 6d 70 61 72 65 53 74 72 69 6e 67
 	  6060: 73 40 51 74 50 72 69 76 61 74 65 40 40 59 41 48
 	  6070: 56 51 53 74 72 69 6e 67 56 69 65 77 40 40 30 57
 	  6080: 34 43 61 73 65 53 65 6e 73 69 74 69 76 69 74 79
-	  6090: 40 51 74 40 40 40 5a 00 0d 0d 3f 65 71 75 61 6c
+	  6090: 40 51 74 40 40 40 5a 00 0e 0d 3f 65 71 75 61 6c
 	  60a0: 53 74 72 69 6e 67 73 40 51 74 50 72 69 76 61 74
 	  60b0: 65 40 40 59 41 5f 4e 56 51 53 74 72 69 6e 67 56
-	  60c0: 69 65 77 40 40 30 40 5a 00 00 12 02 3f 3f 30 51
+	  60c0: 69 65 77 40 40 30 40 5a 00 00 13 02 3f 3f 30 51
 	  60d0: 53 74 72 69 6e 67 40 40 51 45 41 41 40 58 5a 00
-	  60e0: 0c 02 3f 3f 30 51 53 74 72 69 6e 67 40 40 51 45
-	  60f0: 41 41 40 41 45 42 56 30 40 40 5a 00 76 03 3f 3f
+	  60e0: 0d 02 3f 3f 30 51 53 74 72 69 6e 67 40 40 51 45
+	  60f0: 41 41 40 41 45 42 56 30 40 40 5a 00 77 03 3f 3f
 	  6100: 31 51 53 74 72 69 6e 67 40 40 51 45 41 41 40 58
-	  6110: 5a 00 0b 02 3f 3f 30 51 53 74 72 69 6e 67 40 40
+	  6110: 5a 00 0c 02 3f 3f 30 51 53 74 72 69 6e 67 40 40
 	  6120: 51 45 41 41 40 24 24 51 45 41 56 30 40 40 5a 00
-	  6130: 6d 04 3f 3f 34 51 53 74 72 69 6e 67 40 40 51 45
+	  6130: 6e 04 3f 3f 34 51 53 74 72 69 6e 67 40 40 51 45
 	  6140: 41 41 41 45 41 56 30 40 24 24 51 45 41 56 30 40
-	  6150: 40 5a 00 00 dc 0b 3f 64 61 74 61 40 51 53 74 72
+	  6150: 40 5a 00 00 dd 0b 3f 64 61 74 61 40 51 53 74 72
 	  6160: 69 6e 67 40 40 51 45 42 41 50 45 42 56 51 43 68
-	  6170: 61 72 40 40 58 5a 00 00 a5 10 3f 69 73 4e 75 6c
+	  6170: 61 72 40 40 58 5a 00 00 a6 10 3f 69 73 4e 75 6c
 	  6180: 6c 40 51 53 74 72 69 6e 67 40 40 51 45 42 41 5f
-	  6190: 4e 58 5a 00 31 05 3f 3f 36 40 59 41 41 45 41 56
+	  6190: 4e 58 5a 00 32 05 3f 3f 36 40 59 41 41 45 41 56
 	  61a0: 51 44 61 74 61 53 74 72 65 61 6d 40 40 41 45 41
 	  61b0: 56 30 40 41 45 42 56 51 53 74 72 69 6e 67 40 40
-	  61c0: 40 5a 00 00 bd 04 3f 3f 35 40 59 41 41 45 41 56
+	  61c0: 40 5a 00 00 be 04 3f 3f 35 40 59 41 41 45 41 56
 	  61d0: 51 44 61 74 61 53 74 72 65 61 6d 40 40 41 45 41
 	  61e0: 56 30 40 41 45 41 56 51 53 74 72 69 6e 67 40 40
-	  61f0: 40 5a 00 00 5b 02 3f 3f 30 51 55 72 6c 40 40 51
-	  6200: 45 41 41 40 58 5a 00 00 59 02 3f 3f 30 51 55 72
+	  61f0: 40 5a 00 00 5c 02 3f 3f 30 51 55 72 6c 40 40 51
+	  6200: 45 41 41 40 58 5a 00 00 5a 02 3f 3f 30 51 55 72
 	  6210: 6c 40 40 51 45 41 41 40 41 45 42 56 30 40 40 5a
-	  6220: 00 00 85 04 3f 3f 34 51 55 72 6c 40 40 51 45 41
+	  6220: 00 00 86 04 3f 3f 34 51 55 72 6c 40 40 51 45 41
 	  6230: 41 41 45 41 56 30 40 24 24 51 45 41 56 30 40 40
-	  6240: 5a 00 8c 03 3f 3f 31 51 55 72 6c 40 40 51 45 41
-	  6250: 41 40 58 5a 00 00 47 06 3f 3f 4d 51 55 72 6c 40
+	  6240: 5a 00 8d 03 3f 3f 31 51 55 72 6c 40 40 51 45 41
+	  6250: 41 40 58 5a 00 00 48 06 3f 3f 4d 51 55 72 6c 40
 	  6260: 40 51 45 42 41 5f 4e 41 45 42 56 30 40 40 5a 00
-	  6270: a1 05 3f 3f 38 51 55 72 6c 40 40 51 45 42 41 5f
-	  6280: 4e 41 45 42 56 30 40 40 5a 00 34 05 3f 3f 36 40
+	  6270: a2 05 3f 3f 38 51 55 72 6c 40 40 51 45 42 41 5f
+	  6280: 4e 41 45 42 56 30 40 40 5a 00 35 05 3f 3f 36 40
 	  6290: 59 41 41 45 41 56 51 44 61 74 61 53 74 72 65 61
 	  62a0: 6d 40 40 41 45 41 56 30 40 41 45 42 56 51 55 72
-	  62b0: 6c 40 40 40 5a 00 c1 04 3f 3f 35 40 59 41 41 45
+	  62b0: 6c 40 40 40 5a 00 c2 04 3f 3f 35 40 59 41 41 45
 	  62c0: 41 56 51 44 61 74 61 53 74 72 65 61 6d 40 40 41
 	  62d0: 45 41 56 30 40 41 45 41 56 51 55 72 6c 40 40 40
-	  62e0: 5a 00 0c 05 3f 3f 36 40 59 41 3f 41 56 51 44 65
+	  62e0: 5a 00 0d 05 3f 3f 36 40 59 41 3f 41 56 51 44 65
 	  62f0: 62 75 67 40 40 56 30 40 41 45 42 56 51 55 72 6c
-	  6300: 40 40 40 5a 00 00 96 1a 3f 73 74 61 74 75 73 40
+	  6300: 40 40 40 5a 00 00 97 1a 3f 73 74 61 74 75 73 40
 	  6310: 51 44 61 74 61 53 74 72 65 61 6d 40 40 51 45 42
 	  6320: 41 3f 41 57 34 53 74 61 74 75 73 40 31 40 58 5a
-	  6330: 00 00 39 19 3f 73 65 74 53 74 61 74 75 73 40 51
+	  6330: 00 00 3a 19 3f 73 65 74 53 74 61 74 75 73 40 51
 	  6340: 44 61 74 61 53 74 72 65 61 6d 40 40 51 45 41 41
 	  6350: 58 57 34 53 74 61 74 75 73 40 31 40 40 5a 00 00
 	  6360: 04 17 3f 72 65 73 65 74 53 74 61 74 75 73 40 51
 	  6370: 44 61 74 61 53 74 72 65 61 6d 40 40 51 45 41 41
-	  6380: 58 58 5a 00 ce 04 3f 3f 35 51 44 61 74 61 53 74
+	  6380: 58 58 5a 00 cf 04 3f 3f 35 51 44 61 74 61 53 74
 	  6390: 72 65 61 6d 40 40 51 45 41 41 41 45 41 56 30 40
-	  63a0: 41 45 41 48 40 5a 00 00 45 05 3f 3f 36 51 44 61
+	  63a0: 41 45 41 48 40 5a 00 00 46 05 3f 3f 36 51 44 61
 	  63b0: 74 61 53 74 72 65 61 6d 40 40 51 45 41 41 41 45
-	  63c0: 41 56 30 40 48 40 5a 00 13 10 3f 69 73 44 65 76
+	  63c0: 41 56 30 40 48 40 5a 00 14 10 3f 69 73 44 65 76
 	  63d0: 69 63 65 54 72 61 6e 73 61 63 74 69 6f 6e 53 74
 	  63e0: 61 72 74 65 64 40 51 44 61 74 61 53 74 72 65 61
 	  63f0: 6d 40 40 51 45 42 41 5f 4e 58 5a 00 4b 16 3f 72
 	  6400: 65 67 69 73 74 65 72 4e 6f 72 6d 61 6c 69 7a 65
 	  6410: 64 54 79 70 65 64 65 66 40 51 4d 65 74 61 54 79
 	  6420: 70 65 40 40 53 41 58 41 45 42 56 51 42 79 74 65
-	  6430: 41 72 72 61 79 40 40 56 31 40 40 5a 00 00 0b 0f
+	  6430: 41 72 72 61 79 40 40 56 31 40 40 5a 00 00 0c 0f
 	  6440: 3f 69 64 40 51 4d 65 74 61 54 79 70 65 40 40 51
-	  6450: 45 42 41 48 48 40 5a 00 9d 0c 3f 64 79 6e 61 6d
+	  6450: 45 42 41 48 48 40 5a 00 9e 0c 3f 64 79 6e 61 6d
 	  6460: 69 63 4d 65 74 61 4f 62 6a 65 63 74 40 51 4f 62
 	  6470: 6a 65 63 74 44 61 74 61 40 40 51 45 42 41 50 45
 	  6480: 41 55 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 58
-	  6490: 5a 00 7e 15 3f 71 74 5f 6d 65 74 61 63 61 73 74
+	  6490: 5a 00 7f 15 3f 71 74 5f 6d 65 74 61 63 61 73 74
 	  64a0: 40 51 4f 62 6a 65 63 74 40 40 55 45 41 41 50 45
-	  64b0: 41 58 50 45 42 44 40 5a 00 00 49 15 3f 71 74 5f
+	  64b0: 41 58 50 45 42 44 40 5a 00 00 4a 15 3f 71 74 5f
 	  64c0: 6d 65 74 61 63 61 6c 6c 40 51 4f 62 6a 65 63 74
 	  64d0: 40 40 55 45 41 41 48 57 34 43 61 6c 6c 40 51 4d
 	  64e0: 65 74 61 4f 62 6a 65 63 74 40 40 48 50 45 41 50
 	  64f0: 45 41 58 40 5a 00 d6 00 3f 3f 30 51 44 65 62 75
 	  6500: 67 40 40 51 45 41 41 40 24 24 51 45 41 56 30 40
-	  6510: 40 5a 00 00 16 03 3f 3f 31 51 44 65 62 75 67 40
-	  6520: 40 51 45 41 41 40 58 5a 00 00 53 05 3f 3f 36 51
+	  6510: 40 5a 00 00 17 03 3f 3f 31 51 44 65 62 75 67 40
+	  6520: 40 51 45 41 41 40 58 5a 00 00 54 05 3f 3f 36 51
 	  6530: 44 65 62 75 67 40 40 51 45 41 41 41 45 41 56 30
-	  6540: 40 44 40 5a 00 00 5d 05 3f 3f 36 51 44 65 62 75
+	  6540: 40 44 40 5a 00 00 5e 05 3f 3f 36 51 44 65 62 75
 	  6550: 67 40 40 51 45 41 41 41 45 41 56 30 40 50 45 42
-	  6560: 44 40 5a 00 52 05 3f 3f 36 51 44 65 62 75 67 40
+	  6560: 44 40 5a 00 53 05 3f 3f 36 51 44 65 62 75 67 40
 	  6570: 40 51 45 41 41 41 45 41 56 30 40 41 45 42 56 51
-	  6580: 53 74 72 69 6e 67 40 40 40 5a 00 00 51 05 3f 3f
+	  6580: 53 74 72 69 6e 67 40 40 40 5a 00 00 52 05 3f 3f
 	  6590: 36 51 44 65 62 75 67 40 40 51 45 41 41 41 45 41
 	  65a0: 56 30 40 41 45 42 56 51 42 79 74 65 41 72 72 61
 	  65b0: 79 40 40 40 5a 00 db 00 3f 3f 30 51 44 65 62 75
 	  65c0: 67 53 74 61 74 65 53 61 76 65 72 40 40 51 45 41
 	  65d0: 41 40 41 45 41 56 51 44 65 62 75 67 40 40 40 5a
-	  65e0: 00 00 17 03 3f 3f 31 51 44 65 62 75 67 53 74 61
+	  65e0: 00 00 18 03 3f 3f 31 51 44 65 62 75 67 53 74 61
 	  65f0: 74 65 53 61 76 65 72 40 40 51 45 41 41 40 58 5a
-	  6600: 00 00 20 15 3f 71 74 5f 51 4d 65 74 61 45 6e 75
+	  6600: 00 00 21 15 3f 71 74 5f 51 4d 65 74 61 45 6e 75
 	  6610: 6d 5f 64 65 62 75 67 4f 70 65 72 61 74 6f 72 40
 	  6620: 40 59 41 3f 41 56 51 44 65 62 75 67 40 40 41 45
 	  6630: 41 56 31 40 5f 4a 50 45 42 55 51 4d 65 74 61 4f
-	  6640: 62 6a 65 63 74 40 40 50 45 42 44 40 5a 00 9d 02
+	  6640: 62 6a 65 63 74 40 40 50 45 42 44 40 5a 00 9e 02
 	  6650: 3f 3f 30 51 56 61 72 69 61 6e 74 40 40 51 45 41
-	  6660: 41 40 58 5a 00 00 8e 03 3f 3f 31 51 56 61 72 69
-	  6670: 61 6e 74 40 40 51 45 41 41 40 58 5a 00 00 6d 02
+	  6660: 41 40 58 5a 00 00 8f 03 3f 3f 31 51 56 61 72 69
+	  6670: 61 6e 74 40 40 51 45 41 41 40 58 5a 00 00 6e 02
 	  6680: 3f 3f 30 51 56 61 72 69 61 6e 74 40 40 51 45 41
-	  6690: 41 40 41 45 42 56 30 40 40 5a 00 00 8e 04 3f 3f
+	  6690: 41 40 41 45 42 56 30 40 40 5a 00 00 8f 04 3f 3f
 	  66a0: 34 51 56 61 72 69 61 6e 74 40 40 51 45 41 41 41
-	  66b0: 45 41 56 30 40 41 45 42 56 30 40 40 5a 00 0d 15
+	  66b0: 45 41 56 30 40 41 45 42 56 30 40 40 5a 00 0e 15
 	  66c0: 3f 71 64 65 62 75 67 48 65 6c 70 65 72 40 51 56
 	  66d0: 61 72 69 61 6e 74 40 40 41 45 42 41 3f 41 56 51
-	  66e0: 44 65 62 75 67 40 40 56 32 40 40 5a 00 00 14 0d
+	  66e0: 44 65 62 75 67 40 40 56 32 40 40 5a 00 00 15 0d
 	  66f0: 3f 65 71 75 61 6c 73 40 51 56 61 72 69 61 6e 74
 	  6700: 40 40 49 45 42 41 5f 4e 41 45 42 56 31 40 40 5a
-	  6710: 00 00 c3 04 3f 3f 35 40 59 41 41 45 41 56 51 44
+	  6710: 00 00 c4 04 3f 3f 35 40 59 41 41 45 41 56 51 44
 	  6720: 61 74 61 53 74 72 65 61 6d 40 40 41 45 41 56 30
 	  6730: 40 41 45 41 56 51 56 61 72 69 61 6e 74 40 40 40
-	  6740: 5a 00 36 05 3f 3f 36 40 59 41 41 45 41 56 51 44
+	  6740: 5a 00 37 05 3f 3f 36 40 59 41 41 45 41 56 51 44
 	  6750: 61 74 61 53 74 72 65 61 6d 40 40 41 45 41 56 30
 	  6760: 40 41 45 42 56 51 56 61 72 69 61 6e 74 40 40 40
-	  6770: 5a 00 cc 03 3f 3f 34 51 42 79 74 65 41 72 72 61
+	  6770: 5a 00 cd 03 3f 3f 34 51 42 79 74 65 41 72 72 61
 	  6780: 79 40 40 51 45 41 41 41 45 41 56 30 40 24 24 51
-	  6790: 45 41 56 30 40 40 5a 00 1e 08 3f 61 70 70 65 6e
+	  6790: 45 41 56 30 40 40 5a 00 1f 08 3f 61 70 70 65 6e
 	  67a0: 64 40 51 42 79 74 65 41 72 72 61 79 40 40 51 45
-	  67b0: 41 41 41 45 41 56 31 40 44 40 5a 00 6e 04 3f 3f
+	  67b0: 41 41 41 45 41 56 31 40 44 40 5a 00 6f 04 3f 3f
 	  67c0: 34 51 53 74 72 69 6e 67 40 40 51 45 41 41 41 45
-	  67d0: 41 56 30 40 41 45 42 56 30 40 40 5a 00 00 6e 1c
+	  67d0: 41 56 30 40 41 45 42 56 30 40 40 5a 00 00 6f 1c
 	  67e0: 3f 74 6f 55 74 66 38 40 51 53 74 72 69 6e 67 40
 	  67f0: 40 51 45 48 41 41 3f 41 56 51 42 79 74 65 41 72
-	  6800: 72 61 79 40 40 58 5a 00 0a 02 3f 3f 30 51 53 74
+	  6800: 72 61 79 40 40 58 5a 00 0b 02 3f 3f 30 51 53 74
 	  6810: 72 69 6e 67 40 40 51 45 41 41 40 24 24 51 45 41
 	  6820: 55 3f 24 51 41 72 72 61 79 44 61 74 61 50 6f 69
-	  6830: 6e 74 65 72 40 5f 53 40 40 40 5a 00 86 04 3f 3f
+	  6830: 6e 74 65 72 40 5f 53 40 40 40 5a 00 87 04 3f 3f
 	  6840: 34 51 55 72 6c 40 40 51 45 41 41 41 45 41 56 30
-	  6850: 40 41 45 42 56 30 40 40 5a 00 fc 18 3f 73 65 74
+	  6850: 40 41 45 42 56 30 40 40 5a 00 fd 18 3f 73 65 74
 	  6860: 51 75 65 72 79 40 51 55 72 6c 40 40 51 45 41 41
 	  6870: 58 41 45 42 56 51 55 72 6c 51 75 65 72 79 40 40
-	  6880: 40 5a 00 00 c8 05 3f 3f 39 51 55 72 6c 40 40 51
-	  6890: 45 42 41 5f 4e 41 45 42 56 30 40 40 5a 00 52 03
+	  6880: 40 5a 00 00 c9 05 3f 3f 39 51 55 72 6c 40 40 51
+	  6890: 45 42 41 5f 4e 41 45 42 56 30 40 40 5a 00 53 03
 	  68a0: 3f 3f 31 51 4f 62 6a 65 63 74 40 40 55 45 41 41
-	  68b0: 40 58 5a 00 e0 13 3f 70 61 72 65 6e 74 40 51 4f
+	  68b0: 40 58 5a 00 e1 13 3f 70 61 72 65 6e 74 40 51 4f
 	  68c0: 62 6a 65 63 74 40 40 51 45 42 41 50 45 41 56 31
 	  68d0: 40 58 5a 00 a0 01 3f 3f 30 51 4f 62 6a 65 63 74
 	  68e0: 40 40 49 45 41 41 40 41 45 41 56 51 4f 62 6a 65
 	  68f0: 63 74 50 72 69 76 61 74 65 40 40 50 45 41 56 30
-	  6900: 40 40 5a 00 89 0e 3f 67 65 74 41 6e 64 52 65 66
+	  6900: 40 40 5a 00 8a 0e 3f 67 65 74 41 6e 64 52 65 66
 	  6910: 40 45 78 74 65 72 6e 61 6c 52 65 66 43 6f 75 6e
 	  6920: 74 44 61 74 61 40 51 74 53 68 61 72 65 64 50 6f
 	  6930: 69 6e 74 65 72 40 40 53 41 50 45 41 55 31 32 40
 	  6940: 50 45 42 56 51 4f 62 6a 65 63 74 40 40 40 5a 00
-	  6950: 71 02 3f 3f 30 51 56 61 72 69 61 6e 74 40 40 51
+	  6950: 72 02 3f 3f 30 51 56 61 72 69 61 6e 74 40 40 51
 	  6960: 45 41 41 40 41 45 42 56 3f 24 51 4d 61 70 40 56
 	  6970: 51 53 74 72 69 6e 67 40 40 56 51 56 61 72 69 61
-	  6980: 6e 74 40 40 40 40 40 5a 00 00 86 02 3f 3f 30 51
+	  6980: 6e 74 40 40 40 40 40 5a 00 00 87 02 3f 3f 30 51
 	  6990: 56 61 72 69 61 6e 74 40 40 51 45 41 41 40 41 45
-	  69a0: 42 56 51 53 74 72 69 6e 67 40 40 40 5a 00 35 1c
+	  69a0: 42 56 51 53 74 72 69 6e 67 40 40 40 5a 00 36 1c
 	  69b0: 3f 74 6f 53 74 72 69 6e 67 40 51 56 61 72 69 61
 	  69c0: 6e 74 40 40 51 45 42 41 3f 41 56 51 53 74 72 69
 	  69d0: 6e 67 40 40 58 5a 00 00 a4 01 3f 3f 30 51 4f 62
 	  69e0: 6a 65 63 74 50 72 69 76 61 74 65 40 40 51 45 41
-	  69f0: 41 40 48 40 5a 00 55 03 3f 3f 31 51 4f 62 6a 65
+	  69f0: 41 40 48 40 5a 00 56 03 3f 3f 31 51 4f 62 6a 65
 	  6a00: 63 74 50 72 69 76 61 74 65 40 40 55 45 41 41 40
 	  6a10: 58 5a 00 00 6f 01 3f 3f 30 51 4c 6f 67 67 69 6e
 	  6a20: 67 43 61 74 65 67 6f 72 79 40 40 51 45 41 41 40
 	  6a30: 50 45 42 44 57 34 51 74 4d 73 67 54 79 70 65 40
-	  6a40: 40 40 5a 00 46 03 3f 3f 31 51 4c 6f 67 67 69 6e
+	  6a40: 40 40 5a 00 47 03 3f 3f 31 51 4c 6f 67 67 69 6e
 	  6a50: 67 43 61 74 65 67 6f 72 79 40 40 51 45 41 41 40
-	  6a60: 58 5a 00 00 14 03 3f 3f 31 51 44 61 74 65 54 69
-	  6a70: 6d 65 40 40 51 45 41 41 40 58 5a 00 d5 1b 3f 74
+	  6a60: 58 5a 00 00 15 03 3f 3f 31 51 44 61 74 65 54 69
+	  6a70: 6d 65 40 40 51 45 41 41 40 58 5a 00 d6 1b 3f 74
 	  6a80: 6f 4d 53 65 63 73 53 69 6e 63 65 45 70 6f 63 68
 	  6a90: 40 51 44 61 74 65 54 69 6d 65 40 40 51 45 42 41
-	  6aa0: 5f 4a 58 5a 00 00 40 0b 3f 63 75 72 72 65 6e 74
+	  6aa0: 5f 4a 58 5a 00 00 41 0b 3f 63 75 72 72 65 6e 74
 	  6ab0: 44 61 74 65 54 69 6d 65 40 51 44 61 74 65 54 69
-	  6ac0: 6d 65 40 40 53 41 3f 41 56 31 40 58 5a 00 61 02
+	  6ac0: 6d 65 40 40 53 41 3f 41 56 31 40 58 5a 00 62 02
 	  6ad0: 3f 3f 30 51 55 72 6c 51 75 65 72 79 40 40 51 45
-	  6ae0: 41 41 40 58 5a 00 8d 03 3f 3f 31 51 55 72 6c 51
-	  6af0: 75 65 72 79 40 40 51 45 41 41 40 58 5a 00 33 1c
+	  6ae0: 41 41 40 58 5a 00 8e 03 3f 3f 31 51 55 72 6c 51
+	  6af0: 75 65 72 79 40 40 51 45 41 41 40 58 5a 00 34 1c
 	  6b00: 3f 74 6f 53 74 72 69 6e 67 40 51 55 72 6c 51 75
 	  6b10: 65 72 79 40 40 51 45 42 41 3f 41 56 51 53 74 72
 	  6b20: 69 6e 67 40 40 56 3f 24 51 46 6c 61 67 73 40 57
 	  6b30: 34 43 6f 6d 70 6f 6e 65 6e 74 46 6f 72 6d 61 74
 	  6b40: 74 69 6e 67 4f 70 74 69 6f 6e 40 51 55 72 6c 40
-	  6b50: 40 40 40 40 5a 00 e3 07 3f 61 64 64 51 75 65 72
+	  6b50: 40 40 40 40 5a 00 e4 07 3f 61 64 64 51 75 65 72
 	  6b60: 79 49 74 65 6d 40 51 55 72 6c 51 75 65 72 79 40
 	  6b70: 40 51 45 41 41 58 41 45 42 56 51 53 74 72 69 6e
-	  6b80: 67 40 40 30 40 5a 00 00 3d 03 3f 3f 31 51 4a 73
+	  6b80: 67 40 40 30 40 5a 00 00 3e 03 3f 3f 31 51 4a 73
 	  6b90: 6f 6e 44 6f 63 75 6d 65 6e 74 40 40 51 45 41 41
-	  6ba0: 40 58 5a 00 72 0e 3f 66 72 6f 6d 56 61 72 69 61
+	  6ba0: 40 58 5a 00 73 0e 3f 66 72 6f 6d 56 61 72 69 61
 	  6bb0: 6e 74 40 51 4a 73 6f 6e 44 6f 63 75 6d 65 6e 74
 	  6bc0: 40 40 53 41 3f 41 56 31 40 41 45 42 56 51 56 61
-	  6bd0: 72 69 61 6e 74 40 40 40 5a 00 a5 1b 3f 74 6f 4a
+	  6bd0: 72 69 61 6e 74 40 40 40 5a 00 a6 1b 3f 74 6f 4a
 	  6be0: 73 6f 6e 40 51 4a 73 6f 6e 44 6f 63 75 6d 65 6e
 	  6bf0: 74 40 40 51 45 42 41 3f 41 56 51 42 79 74 65 41
 	  6c00: 72 72 61 79 40 40 57 34 4a 73 6f 6e 46 6f 72 6d
-	  6c10: 61 74 40 31 40 40 5a 00 a0 09 3f 63 68 69 6c 64
+	  6c10: 61 74 40 31 40 40 5a 00 a1 09 3f 63 68 69 6c 64
 	  6c20: 45 76 65 6e 74 40 51 4f 62 6a 65 63 74 40 40 4d
 	  6c30: 45 41 41 58 50 45 41 56 51 43 68 69 6c 64 45 76
-	  6c40: 65 6e 74 40 40 40 5a 00 65 0a 3f 63 6f 6e 6e 65
+	  6c40: 65 6e 74 40 40 40 5a 00 66 0a 3f 63 6f 6e 6e 65
 	  6c50: 63 74 4e 6f 74 69 66 79 40 51 4f 62 6a 65 63 74
 	  6c60: 40 40 4d 45 41 41 58 41 45 42 56 51 4d 65 74 61
-	  6c70: 4d 65 74 68 6f 64 40 40 40 5a 00 00 5e 0b 3f 63
+	  6c70: 4d 65 74 68 6f 64 40 40 40 5a 00 00 5f 0b 3f 63
 	  6c80: 75 73 74 6f 6d 45 76 65 6e 74 40 51 4f 62 6a 65
 	  6c90: 63 74 40 40 4d 45 41 41 58 50 45 41 56 51 45 76
-	  6ca0: 65 6e 74 40 40 40 5a 00 70 0c 3f 64 69 73 63 6f
+	  6ca0: 65 6e 74 40 40 40 5a 00 71 0c 3f 64 69 73 63 6f
 	  6cb0: 6e 6e 65 63 74 4e 6f 74 69 66 79 40 51 4f 62 6a
 	  6cc0: 65 63 74 40 40 4d 45 41 41 58 41 45 42 56 51 4d
-	  6cd0: 65 74 61 4d 65 74 68 6f 64 40 40 40 5a 00 41 0d
+	  6cd0: 65 74 61 4d 65 74 68 6f 64 40 40 40 5a 00 42 0d
 	  6ce0: 3f 65 76 65 6e 74 40 51 4f 62 6a 65 63 74 40 40
 	  6cf0: 55 45 41 41 5f 4e 50 45 41 56 51 45 76 65 6e 74
-	  6d00: 40 40 40 5a 00 00 51 0d 3f 65 76 65 6e 74 46 69
+	  6d00: 40 40 40 5a 00 00 52 0d 3f 65 76 65 6e 74 46 69
 	  6d10: 6c 74 65 72 40 51 4f 62 6a 65 63 74 40 40 55 45
 	  6d20: 41 41 5f 4e 50 45 41 56 31 40 50 45 41 56 51 45
-	  6d30: 76 65 6e 74 40 40 40 5a 00 00 00 0e 3f 66 6c 61
+	  6d30: 76 65 6e 74 40 40 40 5a 00 00 01 0e 3f 66 6c 61
 	  6d40: 67 73 46 6f 72 44 75 6d 70 69 6e 67 40 51 4f 62
 	  6d50: 6a 65 63 74 50 72 69 76 61 74 65 40 40 55 45 42
 	  6d60: 41 3f 41 56 3f 24 62 61 73 69 63 5f 73 74 72 69
 	  6d70: 6e 67 40 44 55 3f 24 63 68 61 72 5f 74 72 61 69
 	  6d80: 74 73 40 44 40 73 74 64 40 40 56 3f 24 61 6c 6c
 	  6d90: 6f 63 61 74 6f 72 40 44 40 32 40 40 73 74 64 40
-	  6da0: 40 58 5a 00 31 1b 3f 74 69 6d 65 72 45 76 65 6e
+	  6da0: 40 58 5a 00 32 1b 3f 74 69 6d 65 72 45 76 65 6e
 	  6db0: 74 40 51 4f 62 6a 65 63 74 40 40 4d 45 41 41 58
 	  6dc0: 50 45 41 56 51 54 69 6d 65 72 45 76 65 6e 74 40
 	  6dd0: 40 40 5a 00 73 01 3f 3f 30 51 4d 65 73 73 61 67
 	  6de0: 65 4c 6f 67 67 65 72 40 40 51 45 41 41 40 50 45
-	  6df0: 42 44 48 30 30 40 5a 00 d0 1d 3f 77 61 72 6e 69
+	  6df0: 42 44 48 30 30 40 5a 00 d1 1d 3f 77 61 72 6e 69
 	  6e00: 6e 67 40 51 4d 65 73 73 61 67 65 4c 6f 67 67 65
 	  6e10: 72 40 40 51 45 42 41 58 50 45 42 44 5a 5a 00 00
-	  6e20: ed 11 3f 6c 65 6e 67 74 68 48 65 6c 70 65 72 43
+	  6e20: ee 11 3f 6c 65 6e 67 74 68 48 65 6c 70 65 72 43
 	  6e30: 68 61 72 41 72 72 61 79 40 51 42 79 74 65 41 72
 	  6e40: 72 61 79 56 69 65 77 40 40 43 41 5f 4a 50 45 42
 	  6e50: 44 5f 4b 40 5a 00 5c 00 3f 3f 30 51 42 79 74 65
 	  6e60: 41 72 72 61 79 40 40 51 45 41 41 40 50 45 42 44
-	  6e70: 5f 4a 40 5a 00 00 54 08 3f 61 72 67 40 51 53 74
+	  6e70: 5f 4a 40 5a 00 00 55 08 3f 61 72 67 40 51 53 74
 	  6e80: 72 69 6e 67 40 40 51 45 42 41 3f 41 56 31 40 41
 	  6e90: 45 42 56 31 40 48 56 51 43 68 61 72 40 40 40 5a
-	  6ea0: 00 00 6d 1c 3f 74 6f 55 74 66 38 40 51 53 74 72
+	  6ea0: 00 00 6e 1c 3f 74 6f 55 74 66 38 40 51 53 74 72
 	  6eb0: 69 6e 67 40 40 51 45 47 42 41 3f 41 56 51 42 79
-	  6ec0: 74 65 41 72 72 61 79 40 40 58 5a 00 70 0e 3f 66
+	  6ec0: 74 65 41 72 72 61 79 40 40 58 5a 00 71 0e 3f 66
 	  6ed0: 72 6f 6d 55 74 66 38 40 51 53 74 72 69 6e 67 40
 	  6ee0: 40 53 41 3f 41 56 31 40 56 51 42 79 74 65 41 72
-	  6ef0: 72 61 79 56 69 65 77 40 40 40 5a 00 7d 13 3f 6e
+	  6ef0: 72 61 79 56 69 65 77 40 40 40 5a 00 7e 13 3f 6e
 	  6f00: 6f 72 6d 61 6c 69 7a 65 64 54 79 70 65 40 51 4d
 	  6f10: 65 74 61 4f 62 6a 65 63 74 40 40 53 41 3f 41 56
 	  6f20: 51 42 79 74 65 41 72 72 61 79 40 40 50 45 42 44
-	  6f30: 40 5a 00 00 e0 02 3f 3f 31 43 6f 6e 6e 65 63 74
+	  6f30: 40 5a 00 00 e1 02 3f 3f 31 43 6f 6e 6e 65 63 74
 	  6f40: 69 6f 6e 40 51 4d 65 74 61 4f 62 6a 65 63 74 40
-	  6f50: 40 51 45 41 41 40 58 5a 00 00 61 0a 3f 63 6f 6e
+	  6f50: 40 51 45 41 41 40 58 5a 00 00 62 0a 3f 63 6f 6e
 	  6f60: 6e 65 63 74 49 6d 70 6c 40 51 4f 62 6a 65 63 74
 	  6f70: 40 40 43 41 3f 41 56 43 6f 6e 6e 65 63 74 69 6f
 	  6f80: 6e 40 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 50
 	  6f90: 45 42 56 31 40 50 45 41 50 45 41 58 30 31 50 45
 	  6fa0: 41 56 51 53 6c 6f 74 4f 62 6a 65 63 74 42 61 73
 	  6fb0: 65 40 51 74 50 72 69 76 61 74 65 40 40 57 34 43
 	  6fc0: 6f 6e 6e 65 63 74 69 6f 6e 54 79 70 65 40 51 74
 	  6fd0: 40 40 50 45 42 48 50 45 42 55 33 40 40 5a 00 00
 	  6fe0: cf 00 3f 3f 30 51 44 61 74 65 54 69 6d 65 40 40
 	  6ff0: 51 45 41 41 40 58 5a 00 cb 00 3f 3f 30 51 44 61
 	  7000: 74 65 54 69 6d 65 40 40 51 45 41 41 40 41 45 42
 	  7010: 56 30 40 40 5a 00 ca 00 3f 3f 30 51 44 61 74 65
 	  7020: 54 69 6d 65 40 40 51 45 41 41 40 24 24 51 45 41
-	  7030: 56 30 40 40 5a 00 ee 03 3f 3f 34 51 44 61 74 65
+	  7030: 56 30 40 40 5a 00 ef 03 3f 3f 34 51 44 61 74 65
 	  7040: 54 69 6d 65 40 40 51 45 41 41 41 45 41 56 30 40
-	  7050: 24 24 51 45 41 56 30 40 40 5a 00 00 10 0d 3f 65
+	  7050: 24 24 51 45 41 56 30 40 40 5a 00 00 11 0d 3f 65
 	  7060: 71 75 61 6c 73 40 51 44 61 74 65 54 69 6d 65 40
 	  7070: 40 41 45 42 41 5f 4e 41 45 42 56 31 40 40 5a 00
-	  7080: 2c 14 3f 70 72 65 63 65 64 65 73 40 51 44 61 74
+	  7080: 2d 14 3f 70 72 65 63 65 64 65 73 40 51 44 61 74
 	  7090: 65 54 69 6d 65 40 40 41 45 42 41 5f 4e 41 45 42
-	  70a0: 56 31 40 40 5a 00 1f 05 3f 3f 36 40 59 41 41 45
+	  70a0: 56 31 40 40 5a 00 20 05 3f 3f 36 40 59 41 41 45
 	  70b0: 41 56 51 44 61 74 61 53 74 72 65 61 6d 40 40 41
 	  70c0: 45 41 56 30 40 41 45 42 56 51 44 61 74 65 54 69
-	  70d0: 6d 65 40 40 40 5a 00 00 ab 04 3f 3f 35 40 59 41
+	  70d0: 6d 65 40 40 40 5a 00 00 ac 04 3f 3f 35 40 59 41
 	  70e0: 41 45 41 56 51 44 61 74 61 53 74 72 65 61 6d 40
 	  70f0: 40 41 45 41 56 30 40 41 45 41 56 51 44 61 74 65
-	  7100: 54 69 6d 65 40 40 40 5a 00 00 ee 04 3f 3f 36 40
+	  7100: 54 69 6d 65 40 40 40 5a 00 00 ef 04 3f 3f 36 40
 	  7110: 59 41 3f 41 56 51 44 65 62 75 67 40 40 56 30 40
 	  7120: 41 45 42 56 51 44 61 74 65 54 69 6d 65 40 40 40
 	  7130: 5a 00 dd 15 3f 71 75 65 72 79 40 51 55 72 6c 40
 	  7140: 40 51 45 42 41 3f 41 56 51 53 74 72 69 6e 67 40
 	  7150: 40 56 3f 24 51 46 6c 61 67 73 40 57 34 43 6f 6d
 	  7160: 70 6f 6e 65 6e 74 46 6f 72 6d 61 74 74 69 6e 67
 	  7170: 4f 70 74 69 6f 6e 40 51 55 72 6c 40 40 40 40 40
-	  7180: 5a 00 76 11 3f 69 73 57 61 72 6e 69 6e 67 45 6e
+	  7180: 5a 00 77 11 3f 69 73 57 61 72 6e 69 6e 67 45 6e
 	  7190: 61 62 6c 65 64 40 51 4c 6f 67 67 69 6e 67 43 61
 	  71a0: 74 65 67 6f 72 79 40 40 51 45 42 41 5f 4e 58 5a
-	  71b0: 00 00 5e 02 3f 3f 30 51 55 72 6c 51 75 65 72 79
+	  71b0: 00 00 5f 02 3f 3f 30 51 55 72 6c 51 75 65 72 79
 	  71c0: 40 40 51 45 41 41 40 41 45 42 56 51 53 74 72 69
 	  71d0: 6e 67 40 40 40 5a 00 00 a1 01 3f 3f 30 51 4f 62
 	  71e0: 6a 65 63 74 40 40 51 45 41 41 40 50 45 41 56 30
 	  71f0: 40 40 5a 00 74 01 3f 3f 30 51 4d 65 73 73 61 67
 	  7200: 65 4c 6f 67 67 65 72 40 40 51 45 41 41 40 50 45
-	  7210: 42 44 48 30 40 5a 00 00 82 0d 3f 66 61 74 61 6c
+	  7210: 42 44 48 30 40 5a 00 00 83 0d 3f 66 61 74 61 6c
 	  7220: 40 51 4d 65 73 73 61 67 65 4c 6f 67 67 65 72 40
-	  7230: 40 51 45 42 41 58 50 45 42 44 5a 5a 00 00 0d 08
+	  7230: 40 51 45 42 41 58 50 45 42 44 5a 5a 00 00 0e 08
 	  7240: 3f 61 6c 6c 6f 63 61 74 65 40 51 41 72 72 61 79
 	  7250: 44 61 74 61 40 40 53 41 50 45 41 58 50 45 41 50
 	  7260: 45 41 55 31 40 5f 4a 31 31 57 34 41 6c 6c 6f 63
 	  7270: 61 74 69 6f 6e 4f 70 74 69 6f 6e 40 31 40 40 5a
 	  7280: 00 00 34 16 3f 72 65 61 6c 6c 6f 63 61 74 65 55
 	  7290: 6e 61 6c 69 67 6e 65 64 40 51 41 72 72 61 79 44
 	  72a0: 61 74 61 40 40 53 41 3f 41 55 3f 24 70 61 69 72
 	  72b0: 40 50 45 41 55 51 41 72 72 61 79 44 61 74 61 40
 	  72c0: 40 50 45 41 58 40 73 74 64 40 40 50 45 41 55 31
 	  72d0: 40 50 45 41 58 5f 4a 32 57 34 41 6c 6c 6f 63 61
 	  72e0: 74 69 6f 6e 4f 70 74 69 6f 6e 40 31 40 40 5a 00
-	  72f0: 74 0a 3f 63 6f 6e 73 74 44 61 74 61 40 51 42 79
+	  72f0: 75 0a 3f 63 6f 6e 73 74 44 61 74 61 40 51 42 79
 	  7300: 74 65 41 72 72 61 79 40 40 51 45 42 41 50 45 42
-	  7310: 44 58 5a 00 45 1b 3f 74 6f 42 61 73 65 36 34 40
+	  7310: 44 58 5a 00 46 1b 3f 74 6f 42 61 73 65 36 34 40
 	  7320: 51 42 79 74 65 41 72 72 61 79 40 40 51 45 42 41
 	  7330: 3f 41 56 31 40 56 3f 24 51 46 6c 61 67 73 40 57
 	  7340: 34 42 61 73 65 36 34 4f 70 74 69 6f 6e 40 51 42
 	  7350: 79 74 65 41 72 72 61 79 40 40 40 40 40 5a 00 00
-	  7360: 75 09 3f 63 61 73 74 40 51 4d 65 74 61 4f 62 6a
+	  7360: 76 09 3f 63 61 73 74 40 51 4d 65 74 61 4f 62 6a
 	  7370: 65 63 74 40 40 51 45 42 41 50 45 42 56 51 4f 62
 	  7380: 6a 65 63 74 40 40 50 45 42 56 32 40 40 5a 00 00
 	  7390: 1d 00 3f 3f 30 43 6f 6e 6e 65 63 74 69 6f 6e 40
 	  73a0: 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 51 45 41
-	  73b0: 41 40 58 5a 00 00 b3 03 3f 3f 34 43 6f 6e 6e 65
+	  73b0: 41 40 58 5a 00 00 b4 03 3f 3f 34 43 6f 6e 6e 65
 	  73c0: 63 74 69 6f 6e 40 51 4d 65 74 61 4f 62 6a 65 63
 	  73d0: 74 40 40 51 45 41 41 41 45 41 56 30 31 40 24 24
 	  73e0: 51 45 41 56 30 31 40 40 5a 00 a4 00 3f 3f 30 51
 	  73f0: 43 68 61 72 40 40 51 45 41 41 40 55 51 4c 61 74
 	  7400: 69 6e 31 43 68 61 72 40 40 40 5a 00 0c 17 3f 72
 	  7410: 65 73 69 7a 65 40 51 53 74 72 69 6e 67 40 40 51
-	  7420: 45 41 41 58 5f 4a 40 5a 00 00 5e 09 3f 63 61 70
+	  7420: 45 41 41 58 5f 4a 40 5a 00 00 5f 09 3f 63 61 70
 	  7430: 61 63 69 74 79 40 51 53 74 72 69 6e 67 40 40 51
 	  7440: 45 42 41 5f 4a 58 5a 00 f2 16 3f 72 65 73 65 72
 	  7450: 76 65 40 51 53 74 72 69 6e 67 40 40 51 45 41 41
-	  7460: 58 5f 4a 40 5a 00 db 0b 3f 64 61 74 61 40 51 53
+	  7460: 58 5f 4a 40 5a 00 dc 0b 3f 64 61 74 61 40 51 53
 	  7470: 74 72 69 6e 67 40 40 51 45 41 41 50 45 41 56 51
-	  7480: 43 68 61 72 40 40 58 5a 00 00 77 0a 3f 63 6f 6e
+	  7480: 43 68 61 72 40 40 58 5a 00 00 78 0a 3f 63 6f 6e
 	  7490: 73 74 44 61 74 61 40 51 53 74 72 69 6e 67 40 40
 	  74a0: 51 45 42 41 50 45 42 56 51 43 68 61 72 40 40 58
-	  74b0: 5a 00 49 0c 3f 64 65 74 61 63 68 40 51 53 74 72
-	  74c0: 69 6e 67 40 40 51 45 41 41 58 58 5a 00 00 c5 09
+	  74b0: 5a 00 4a 0c 3f 64 65 74 61 63 68 40 51 53 74 72
+	  74c0: 69 6e 67 40 40 51 45 41 41 58 58 5a 00 00 c6 09
 	  74d0: 3f 63 6c 65 61 72 40 51 53 74 72 69 6e 67 40 40
-	  74e0: 51 45 41 41 58 58 5a 00 39 1a 3f 73 74 61 72 74
+	  74e0: 51 45 41 41 58 58 5a 00 3a 1a 3f 73 74 61 72 74
 	  74f0: 73 57 69 74 68 40 51 53 74 72 69 6e 67 40 40 51
 	  7500: 45 42 41 5f 4e 41 45 42 56 31 40 57 34 43 61 73
 	  7510: 65 53 65 6e 73 69 74 69 76 69 74 79 40 51 74 40
-	  7520: 40 40 5a 00 40 08 3f 61 70 70 65 6e 64 40 51 53
+	  7520: 40 40 5a 00 41 08 3f 61 70 70 65 6e 64 40 51 53
 	  7530: 74 72 69 6e 67 40 40 51 45 41 41 41 45 41 56 31
 	  7540: 40 56 51 4c 61 74 69 6e 31 53 74 72 69 6e 67 40
-	  7550: 40 40 5a 00 b9 1b 3f 74 6f 4c 6f 63 61 6c 38 42
+	  7550: 40 40 5a 00 ba 1b 3f 74 6f 4c 6f 63 61 6c 38 42
 	  7560: 69 74 40 51 53 74 72 69 6e 67 40 40 51 45 47 42
 	  7570: 41 3f 41 56 51 42 79 74 65 41 72 72 61 79 40 40
-	  7580: 58 5a 00 00 9f 13 3f 6e 75 6d 62 65 72 40 51 53
+	  7580: 58 5a 00 00 a0 13 3f 6e 75 6d 62 65 72 40 51 53
 	  7590: 74 72 69 6e 67 40 40 53 41 3f 41 56 31 40 5f 4a
-	  75a0: 48 40 5a 00 46 08 3f 61 70 70 65 6e 64 4c 61 74
+	  75a0: 48 40 5a 00 47 08 3f 61 70 70 65 6e 64 4c 61 74
 	  75b0: 69 6e 31 54 6f 40 51 41 62 73 74 72 61 63 74 43
 	  75c0: 6f 6e 63 61 74 65 6e 61 62 6c 65 40 40 4b 41 58
 	  75d0: 56 51 4c 61 74 69 6e 31 53 74 72 69 6e 67 40 40
-	  75e0: 50 45 41 56 51 43 68 61 72 40 40 40 5a 00 31 10
+	  75e0: 50 45 41 56 51 43 68 61 72 40 40 40 5a 00 32 10
 	  75f0: 3f 69 73 45 6d 70 74 79 40 51 55 72 6c 40 40 51
-	  7600: 45 42 41 5f 4e 58 5a 00 e6 1b 3f 74 6f 50 65 72
+	  7600: 45 42 41 5f 4e 58 5a 00 e7 1b 3f 74 6f 50 65 72
 	  7610: 63 65 6e 74 45 6e 63 6f 64 69 6e 67 40 51 55 72
 	  7620: 6c 40 40 53 41 3f 41 56 51 42 79 74 65 41 72 72
 	  7630: 61 79 40 40 41 45 42 56 51 53 74 72 69 6e 67 40
-	  7640: 40 41 45 42 56 32 40 31 40 5a 00 00 68 0c 3f 64
+	  7640: 40 41 45 42 56 32 40 31 40 5a 00 00 69 0c 3f 64
 	  7650: 69 73 63 6f 6e 6e 65 63 74 40 51 4f 62 6a 65 63
 	  7660: 74 40 40 53 41 5f 4e 41 45 42 56 43 6f 6e 6e 65
 	  7670: 63 74 69 6f 6e 40 51 4d 65 74 61 4f 62 6a 65 63
-	  7680: 74 40 40 40 5a 00 2d 0c 3f 64 65 6c 65 74 65 4c
+	  7680: 74 40 40 40 5a 00 2e 0c 3f 64 65 6c 65 74 65 4c
 	  7690: 61 74 65 72 40 51 4f 62 6a 65 63 74 40 40 51 45
-	  76a0: 41 41 58 58 5a 00 a0 02 3f 3f 30 51 56 61 72 69
+	  76a0: 41 41 58 58 5a 00 a1 02 3f 3f 30 51 56 61 72 69
 	  76b0: 61 6e 74 40 40 51 45 41 41 40 5f 4e 40 5a 00 00
-	  76c0: 73 02 3f 3f 30 51 56 61 72 69 61 6e 74 40 40 51
+	  76c0: 74 02 3f 3f 30 51 56 61 72 69 61 6e 74 40 40 51
 	  76d0: 45 41 41 40 41 45 42 56 51 42 79 74 65 41 72 72
-	  76e0: 61 79 40 40 40 5a 00 00 6c 02 3f 3f 30 51 56 61
+	  76e0: 61 79 40 40 40 5a 00 00 6d 02 3f 3f 30 51 56 61
 	  76f0: 72 69 61 6e 74 40 40 51 45 41 41 40 24 24 51 45
-	  7700: 41 56 30 40 40 5a 00 00 4c 1b 3f 74 6f 42 6f 6f
+	  7700: 41 56 30 40 40 5a 00 00 4d 1b 3f 74 6f 42 6f 6f
 	  7710: 6c 40 51 56 61 72 69 61 6e 74 40 40 51 45 42 41
-	  7720: 5f 4e 58 5a 00 00 51 1b 3f 74 6f 42 79 74 65 41
+	  7720: 5f 4e 58 5a 00 00 52 1b 3f 74 6f 42 79 74 65 41
 	  7730: 72 72 61 79 40 51 56 61 72 69 61 6e 74 40 40 51
 	  7740: 45 42 41 3f 41 56 51 42 79 74 65 41 72 72 61 79
-	  7750: 40 40 58 5a 00 00 f5 1b 3f 74 6f 53 65 63 73 53
+	  7750: 40 40 58 5a 00 00 f6 1b 3f 74 6f 53 65 63 73 53
 	  7760: 69 6e 63 65 45 70 6f 63 68 40 51 44 61 74 65 54
-	  7770: 69 6d 65 40 40 51 45 42 41 5f 4a 58 5a 00 41 0b
+	  7770: 69 6d 65 40 40 51 45 42 41 5f 4a 58 5a 00 42 0b
 	  7780: 3f 63 75 72 72 65 6e 74 44 61 74 65 54 69 6d 65
 	  7790: 55 74 63 40 51 44 61 74 65 54 69 6d 65 40 40 53
-	  77a0: 41 3f 41 56 31 40 58 5a 00 00 84 0e 3f 67 65 74
+	  77a0: 41 3f 41 56 31 40 58 5a 00 00 85 0e 3f 67 65 74
 	  77b0: 40 51 4f 62 6a 65 63 74 50 72 69 76 61 74 65 40
 	  77c0: 40 53 41 50 45 41 56 31 40 50 45 41 56 51 4f 62
 	  77d0: 6a 65 63 74 40 40 40 5a 00 00 e0 15 3f 71 75 65
 	  77e0: 72 79 49 74 65 6d 73 40 51 55 72 6c 51 75 65 72
 	  77f0: 79 40 40 51 45 42 41 3f 41 56 3f 24 51 4c 69 73
 	  7800: 74 40 55 3f 24 70 61 69 72 40 56 51 53 74 72 69
 	  7810: 6e 67 40 40 56 31 40 40 73 74 64 40 40 40 40 56
 	  7820: 3f 24 51 46 6c 61 67 73 40 57 34 43 6f 6d 70 6f
 	  7830: 6e 65 6e 74 46 6f 72 6d 61 74 74 69 6e 67 4f 70
 	  7840: 74 69 6f 6e 40 51 55 72 6c 40 40 40 40 40 5a 00
-	  7850: 33 0b 3f 63 72 69 74 69 63 61 6c 40 51 4d 65 73
+	  7850: 34 0b 3f 63 72 69 74 69 63 61 6c 40 51 4d 65 73
 	  7860: 73 61 67 65 4c 6f 67 67 65 72 40 40 51 45 42 41
 	  7870: 58 50 45 42 44 5a 5a 00 5f 00 3f 3f 30 51 42 79
 	  7880: 74 65 41 72 72 61 79 40 40 51 45 41 41 40 5f 4a
 	  7890: 57 34 49 6e 69 74 69 61 6c 69 7a 61 74 69 6f 6e
-	  78a0: 40 51 74 40 40 40 5a 00 cd 03 3f 3f 34 51 42 79
+	  78a0: 40 51 74 40 40 40 5a 00 ce 03 3f 3f 34 51 42 79
 	  78b0: 74 65 41 72 72 61 79 40 40 51 45 41 41 41 45 41
-	  78c0: 56 30 40 41 45 42 56 30 40 40 5a 00 20 10 3f 69
+	  78c0: 56 30 40 41 45 42 56 30 40 40 5a 00 21 10 3f 69
 	  78d0: 73 45 6d 70 74 79 40 51 42 79 74 65 41 72 72 61
 	  78e0: 79 40 40 51 45 42 41 5f 4e 58 5a 00 07 17 3f 72
 	  78f0: 65 73 69 7a 65 40 51 42 79 74 65 41 72 72 61 79
-	  7900: 40 40 51 45 41 41 58 5f 4a 40 5a 00 5d 09 3f 63
+	  7900: 40 40 51 45 41 41 58 5f 4a 40 5a 00 5e 09 3f 63
 	  7910: 61 70 61 63 69 74 79 40 51 42 79 74 65 41 72 72
-	  7920: 61 79 40 40 51 45 42 41 5f 4a 58 5a 00 00 cf 0b
+	  7920: 61 79 40 40 51 45 42 41 5f 4a 58 5a 00 00 d0 0b
 	  7930: 3f 64 61 74 61 40 51 42 79 74 65 41 72 72 61 79
-	  7940: 40 40 51 45 41 41 50 45 41 44 58 5a 00 00 40 0c
+	  7940: 40 40 51 45 41 41 50 45 41 44 58 5a 00 00 41 0c
 	  7950: 3f 64 65 74 61 63 68 40 51 42 79 74 65 41 72 72
-	  7960: 61 79 40 40 51 45 41 41 58 58 5a 00 1d 08 3f 61
+	  7960: 61 79 40 40 51 45 41 41 58 58 5a 00 1e 08 3f 61
 	  7970: 70 70 65 6e 64 40 51 42 79 74 65 41 72 72 61 79
 	  7980: 40 40 51 45 41 41 41 45 41 56 31 40 41 45 42 56
-	  7990: 31 40 40 5a 00 00 bd 0c 3f 65 6e 64 40 51 42 79
+	  7990: 31 40 40 5a 00 00 be 0c 3f 65 6e 64 40 51 42 79
 	  79a0: 74 65 41 72 72 61 79 40 40 51 45 42 41 50 45 42
 	  79b0: 44 58 5a 00 de 16 3f 72 65 70 6c 61 63 65 40 51
 	  79c0: 53 74 72 69 6e 67 40 40 51 45 41 41 41 45 41 56
 	  79d0: 31 40 56 51 43 68 61 72 40 40 30 57 34 43 61 73
 	  79e0: 65 53 65 6e 73 69 74 69 76 69 74 79 40 51 74 40
-	  79f0: 40 40 5a 00 2e 0e 3f 66 72 6f 6d 4c 61 74 69 6e
+	  79f0: 40 40 5a 00 2f 0e 3f 66 72 6f 6d 4c 61 74 69 6e
 	  7a00: 31 40 51 53 74 72 69 6e 67 40 40 53 41 3f 41 56
 	  7a10: 31 40 56 51 42 79 74 65 41 72 72 61 79 56 69 65
-	  7a20: 77 40 40 40 5a 00 32 1c 3f 74 6f 53 74 72 69 6e
+	  7a20: 77 40 40 40 5a 00 33 1c 3f 74 6f 53 74 72 69 6e
 	  7a30: 67 40 51 55 72 6c 40 40 51 45 42 41 3f 41 56 51
 	  7a40: 53 74 72 69 6e 67 40 40 56 3f 24 51 55 72 6c 54
 	  7a50: 77 6f 46 6c 61 67 73 40 57 34 55 72 6c 46 6f 72
 	  7a60: 6d 61 74 74 69 6e 67 4f 70 74 69 6f 6e 40 51 55
 	  7a70: 72 6c 40 40 57 34 43 6f 6d 70 6f 6e 65 6e 74 46
 	  7a80: 6f 72 6d 61 74 74 69 6e 67 4f 70 74 69 6f 6e 40
-	  7a90: 32 40 40 40 40 5a 00 00 fa 0f 3f 69 73 43 72 69
+	  7a90: 32 40 40 40 40 5a 00 00 fb 0f 3f 69 73 43 72 69
 	  7aa0: 74 69 63 61 6c 45 6e 61 62 6c 65 64 40 51 4c 6f
 	  7ab0: 67 67 69 6e 67 43 61 74 65 67 6f 72 79 40 40 51
-	  7ac0: 45 42 41 5f 4e 58 5a 00 ef 0e 3f 68 61 73 68 40
+	  7ac0: 45 42 41 5f 4e 58 5a 00 f0 0e 3f 68 61 73 68 40
 	  7ad0: 51 4d 65 73 73 61 67 65 41 75 74 68 65 6e 74 69
 	  7ae0: 63 61 74 69 6f 6e 43 6f 64 65 40 40 53 41 3f 41
 	  7af0: 56 51 42 79 74 65 41 72 72 61 79 40 40 56 51 42
 	  7b00: 79 74 65 41 72 72 61 79 56 69 65 77 40 40 30 57
 	  7b10: 34 41 6c 67 6f 72 69 74 68 6d 40 51 43 72 79 70
 	  7b20: 74 6f 67 72 61 70 68 69 63 48 61 73 68 40 40 40
-	  7b30: 5a 00 14 0c 3f 64 65 62 75 67 40 51 4d 65 73 73
+	  7b30: 5a 00 15 0c 3f 64 65 62 75 67 40 51 4d 65 73 73
 	  7b40: 61 67 65 4c 6f 67 67 65 72 40 40 51 45 42 41 58
-	  7b50: 50 45 42 44 5a 5a 00 00 cd 1d 3f 77 61 72 6e 69
+	  7b50: 50 45 42 44 5a 5a 00 00 ce 1d 3f 77 61 72 6e 69
 	  7b60: 6e 67 40 51 4d 65 73 73 61 67 65 4c 6f 67 67 65
 	  7b70: 72 40 40 51 45 42 41 3f 41 56 51 44 65 62 75 67
-	  7b80: 40 40 58 5a 00 00 11 02 3f 3f 30 51 53 74 72 69
+	  7b80: 40 40 58 5a 00 00 12 02 3f 3f 30 51 53 74 72 69
 	  7b90: 6e 67 40 40 51 45 41 41 40 56 51 4c 61 74 69 6e
-	  7ba0: 31 53 74 72 69 6e 67 40 40 40 5a 00 ba 1b 3f 74
+	  7ba0: 31 53 74 72 69 6e 67 40 40 40 5a 00 bb 1b 3f 74
 	  7bb0: 6f 4c 6f 63 61 6c 38 42 69 74 40 51 53 74 72 69
 	  7bc0: 6e 67 40 40 51 45 48 41 41 3f 41 56 51 42 79 74
-	  7bd0: 65 41 72 72 61 79 40 40 58 5a 00 00 56 05 3f 3f
+	  7bd0: 65 41 72 72 61 79 40 40 58 5a 00 00 57 05 3f 3f
 	  7be0: 36 51 44 65 62 75 67 40 40 51 45 41 41 41 45 41
-	  7bf0: 56 30 40 48 40 5a 00 00 6c 11 3f 69 73 56 61 6c
+	  7bf0: 56 30 40 48 40 5a 00 00 6d 11 3f 69 73 56 61 6c
 	  7c00: 69 64 40 51 56 61 72 69 61 6e 74 40 40 51 45 42
-	  7c10: 41 5f 4e 58 5a 00 9d 1b 3f 74 6f 49 6e 74 40 51
+	  7c10: 41 5f 4e 58 5a 00 9e 1b 3f 74 6f 49 6e 74 40 51
 	  7c20: 56 61 72 69 61 6e 74 40 40 51 45 42 41 48 50 45
-	  7c30: 41 5f 4e 40 5a 00 e8 07 3f 61 64 64 53 65 63 73
+	  7c30: 41 5f 4e 40 5a 00 e9 07 3f 61 64 64 53 65 63 73
 	  7c40: 40 51 44 61 74 65 54 69 6d 65 40 40 51 45 42 41
 	  7c50: 3f 41 56 31 40 5f 4a 40 5a 00 81 17 3f 73 65 63
 	  7c60: 73 54 6f 40 51 44 61 74 65 54 69 6d 65 40 40 51
-	  7c70: 45 42 41 5f 4a 41 45 42 56 31 40 40 5a 00 5a 02
+	  7c70: 45 42 41 5f 4a 41 45 42 56 31 40 40 5a 00 5b 02
 	  7c80: 3f 3f 30 51 55 72 6c 40 40 51 45 41 41 40 41 45
 	  7c90: 42 56 51 53 74 72 69 6e 67 40 40 57 34 50 61 72
-	  7ca0: 73 69 6e 67 4d 6f 64 65 40 30 40 40 5a 00 03 10
+	  7ca0: 73 69 6e 67 4d 6f 64 65 40 30 40 40 5a 00 04 10
 	  7cb0: 3f 69 73 44 65 62 75 67 45 6e 61 62 6c 65 64 40
 	  7cc0: 51 4c 6f 67 67 69 6e 67 43 61 74 65 67 6f 72 79
-	  7cd0: 40 40 51 45 42 41 5f 4e 58 5a 00 00 88 04 3f 3f
+	  7cd0: 40 40 51 45 42 41 5f 4e 58 5a 00 00 89 04 3f 3f
 	  7ce0: 34 51 55 72 6c 51 75 65 72 79 40 40 51 45 41 41
 	  7cf0: 41 45 41 56 30 40 24 24 51 45 41 56 30 40 40 5a
-	  7d00: 00 00 ba 09 3f 63 6c 65 61 72 40 51 42 79 74 65
+	  7d00: 00 00 bb 09 3f 63 6c 65 61 72 40 51 42 79 74 65
 	  7d10: 41 72 72 61 79 40 40 51 45 41 41 58 58 5a 00 00
-	  7d20: 75 08 3f 61 74 40 51 42 79 74 65 41 72 72 61 79
-	  7d30: 40 40 51 45 42 41 44 5f 4a 40 5a 00 2a 0f 3f 69
+	  7d20: 76 08 3f 61 74 40 51 42 79 74 65 41 72 72 61 79
+	  7d30: 40 40 51 45 42 41 44 5f 4a 40 5a 00 2b 0f 3f 69
 	  7d40: 6e 64 65 78 4f 66 40 51 42 79 74 65 41 72 72 61
 	  7d50: 79 40 40 51 45 42 41 5f 4a 44 5f 4a 40 5a 00 00
-	  7d60: c4 12 3f 6d 69 64 40 51 42 79 74 65 41 72 72 61
+	  7d60: c5 12 3f 6d 69 64 40 51 42 79 74 65 41 72 72 61
 	  7d70: 79 40 40 51 45 42 41 3f 41 56 31 40 5f 4a 30 40
-	  7d80: 5a 00 36 1a 3f 73 74 61 72 74 73 57 69 74 68 40
+	  7d80: 5a 00 37 1a 3f 73 74 61 72 74 73 57 69 74 68 40
 	  7d90: 51 42 79 74 65 41 72 72 61 79 40 40 51 45 42 41
 	  7da0: 5f 4e 56 51 42 79 74 65 41 72 72 61 79 56 69 65
-	  7db0: 77 40 40 40 5a 00 e1 0c 3f 65 6e 64 73 57 69 74
+	  7db0: 77 40 40 40 5a 00 e2 0c 3f 65 6e 64 73 57 69 74
 	  7dc0: 68 40 51 42 79 74 65 41 72 72 61 79 40 40 51 45
 	  7dd0: 42 41 5f 4e 56 51 42 79 74 65 41 72 72 61 79 56
-	  7de0: 69 65 77 40 40 40 5a 00 a5 09 3f 63 68 6f 70 40
+	  7de0: 69 65 77 40 40 40 5a 00 a6 09 3f 63 68 6f 70 40
 	  7df0: 51 42 79 74 65 41 72 72 61 79 40 40 51 45 41 41
-	  7e00: 58 5f 4a 40 5a 00 e5 1c 3f 74 72 69 6d 6d 65 64
+	  7e00: 58 5f 4a 40 5a 00 e6 1c 3f 74 72 69 6d 6d 65 64
 	  7e10: 40 51 42 79 74 65 41 72 72 61 79 40 40 51 45 48
-	  7e20: 41 41 3f 41 56 31 40 58 5a 00 98 13 3f 6e 75 6d
+	  7e20: 41 41 3f 41 56 31 40 58 5a 00 99 13 3f 6e 75 6d
 	  7e30: 62 65 72 40 51 42 79 74 65 41 72 72 61 79 40 40
 	  7e40: 53 41 3f 41 56 31 40 5f 4a 48 40 5a 00 00 58 00
 	  7e50: 3f 3f 30 51 42 79 74 65 41 72 72 61 79 40 40 51
 	  7e60: 45 41 41 40 24 24 51 45 41 55 3f 24 51 41 72 72
 	  7e70: 61 79 44 61 74 61 50 6f 69 6e 74 65 72 40 44 40
-	  7e80: 40 40 5a 00 57 08 3f 61 72 67 40 51 53 74 72 69
+	  7e80: 40 40 5a 00 58 08 3f 61 72 67 40 51 53 74 72 69
 	  7e90: 6e 67 40 40 51 45 42 41 3f 41 56 31 40 47 48 48
-	  7ea0: 56 51 43 68 61 72 40 40 40 5a 00 00 c7 12 3f 6d
+	  7ea0: 56 51 43 68 61 72 40 40 40 5a 00 00 c8 12 3f 6d
 	  7eb0: 69 64 40 51 53 74 72 69 6e 67 40 40 51 45 42 41
-	  7ec0: 3f 41 56 31 40 5f 4a 30 40 5a 00 00 3a 1a 3f 73
+	  7ec0: 3f 41 56 31 40 5f 4a 30 40 5a 00 00 3b 1a 3f 73
 	  7ed0: 74 61 72 74 73 57 69 74 68 40 51 53 74 72 69 6e
 	  7ee0: 67 40 40 51 45 42 41 5f 4e 56 51 43 68 61 72 40
 	  7ef0: 40 57 34 43 61 73 65 53 65 6e 73 69 74 69 76 69
-	  7f00: 74 79 40 51 74 40 40 40 5a 00 9a 13 3f 6e 75 6d
+	  7f00: 74 79 40 51 74 40 40 40 5a 00 9b 13 3f 6e 75 6d
 	  7f10: 62 65 72 40 51 53 74 72 69 6e 67 40 40 53 41 3f
-	  7f20: 41 56 31 40 48 48 40 5a 00 00 14 02 3f 3f 30 51
+	  7f20: 41 56 31 40 48 48 40 5a 00 00 15 02 3f 3f 30 51
 	  7f30: 53 74 72 69 6e 67 40 40 51 45 41 41 40 5f 4a 57
 	  7f40: 34 49 6e 69 74 69 61 6c 69 7a 61 74 69 6f 6e 40
-	  7f50: 51 74 40 40 40 5a 00 00 5d 19 3f 73 65 74 55 72
+	  7f50: 51 74 40 40 40 5a 00 00 5e 19 3f 73 65 74 55 72
 	  7f60: 6c 40 51 55 72 6c 40 40 51 45 41 41 58 41 45 42
 	  7f70: 56 51 53 74 72 69 6e 67 40 40 57 34 50 61 72 73
-	  7f80: 69 6e 67 4d 6f 64 65 40 31 40 40 5a 00 00 6b 11
+	  7f80: 69 6e 67 4d 6f 64 65 40 31 40 40 5a 00 00 6c 11
 	  7f90: 3f 69 73 56 61 6c 69 64 40 51 55 72 6c 40 40 51
-	  7fa0: 45 42 41 5f 4e 58 5a 00 f6 13 3f 70 61 74 68 40
+	  7fa0: 45 42 41 5f 4e 58 5a 00 f7 13 3f 70 61 74 68 40
 	  7fb0: 51 55 72 6c 40 40 51 45 42 41 3f 41 56 51 53 74
 	  7fc0: 72 69 6e 67 40 40 56 3f 24 51 46 6c 61 67 73 40
 	  7fd0: 57 34 43 6f 6d 70 6f 6e 65 6e 74 46 6f 72 6d 61
 	  7fe0: 74 74 69 6e 67 4f 70 74 69 6f 6e 40 51 55 72 6c
-	  7ff0: 40 40 40 40 40 5a 00 00 af 1c 3f 74 72 40 51 4f
+	  7ff0: 40 40 40 40 40 5a 00 00 b0 1c 3f 74 72 40 51 4f
 	  8000: 62 6a 65 63 74 40 40 53 41 3f 41 56 51 53 74 72
-	  8010: 69 6e 67 40 40 50 45 42 44 30 48 40 5a 00 ec 1d
+	  8010: 69 6e 67 40 40 50 45 42 44 30 48 40 5a 00 ed 1d
 	  8020: 3f 77 72 69 74 65 40 51 49 4f 44 65 76 69 63 65
 	  8030: 40 40 51 45 41 41 5f 4a 41 45 42 56 51 42 79 74
-	  8040: 65 41 72 72 61 79 40 40 40 5a 00 00 8b 0e 3f 67
+	  8040: 65 41 72 72 61 79 40 40 40 5a 00 00 8c 0e 3f 67
 	  8050: 65 74 43 68 61 72 40 51 49 4f 44 65 76 69 63 65
 	  8060: 40 40 51 45 41 41 5f 4e 50 45 41 44 40 5a 00 00
 	  8070: 29 16 3f 72 65 61 64 79 52 65 61 64 40 51 49 4f
 	  8080: 44 65 76 69 63 65 40 40 51 45 41 41 58 58 5a 00
-	  8090: 4d 08 3f 61 70 70 6c 69 63 61 74 69 6f 6e 4e 61
+	  8090: 4e 08 3f 61 70 70 6c 69 63 61 74 69 6f 6e 4e 61
 	  80a0: 6d 65 40 51 43 6f 72 65 41 70 70 6c 69 63 61 74
 	  80b0: 69 6f 6e 40 40 53 41 3f 41 56 51 53 74 72 69 6e
-	  80c0: 67 40 40 58 5a 00 97 0f 3f 69 6e 73 74 61 6e 63
+	  80c0: 67 40 40 58 5a 00 98 0f 3f 69 6e 73 74 61 6e 63
 	  80d0: 65 40 51 43 6f 72 65 41 70 70 6c 69 63 61 74 69
 	  80e0: 6f 6e 40 40 53 41 50 45 41 56 31 40 58 5a 00 00
-	  80f0: 6a 1a 3f 73 74 61 74 69 63 4d 65 74 61 4f 62 6a
+	  80f0: 6b 1a 3f 73 74 61 74 69 63 4d 65 74 61 4f 62 6a
 	  8100: 65 63 74 40 51 49 4f 44 65 76 69 63 65 40 40 32
 	  8110: 55 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 42 00
-	  8120: a9 10 3f 69 73 4e 75 6c 6c 40 51 56 61 72 69 61
-	  8130: 6e 74 40 40 51 45 42 41 5f 4e 58 5a 00 00 3e 03
+	  8120: aa 10 3f 69 73 4e 75 6c 6c 40 51 56 61 72 69 61
+	  8130: 6e 74 40 40 51 45 42 41 5f 4e 58 5a 00 00 3f 03
 	  8140: 3f 3f 31 51 4a 73 6f 6e 4f 62 6a 65 63 74 40 40
-	  8150: 51 45 41 41 40 58 5a 00 7f 1c 3f 74 6f 56 61 72
+	  8150: 51 45 41 41 40 58 5a 00 80 1c 3f 74 6f 56 61 72
 	  8160: 69 61 6e 74 4d 61 70 40 51 4a 73 6f 6e 4f 62 6a
 	  8170: 65 63 74 40 40 51 45 42 41 3f 41 56 3f 24 51 4d
 	  8180: 61 70 40 56 51 53 74 72 69 6e 67 40 40 56 51 56
-	  8190: 61 72 69 61 6e 74 40 40 40 40 58 5a 00 00 28 10
+	  8190: 61 72 69 61 6e 74 40 40 40 40 58 5a 00 00 29 10
 	  81a0: 3f 69 73 45 6d 70 74 79 40 51 4a 73 6f 6e 4f 62
 	  81b0: 6a 65 63 74 40 40 51 45 42 41 5f 4e 58 5a 00 00
-	  81c0: 25 0e 3f 66 72 6f 6d 4a 73 6f 6e 40 51 4a 73 6f
+	  81c0: 26 0e 3f 66 72 6f 6d 4a 73 6f 6e 40 51 4a 73 6f
 	  81d0: 6e 44 6f 63 75 6d 65 6e 74 40 40 53 41 3f 41 56
 	  81e0: 31 40 41 45 42 56 51 42 79 74 65 41 72 72 61 79
 	  81f0: 40 40 50 45 41 55 51 4a 73 6f 6e 50 61 72 73 65
-	  8200: 45 72 72 6f 72 40 40 40 5a 00 ad 10 3f 69 73 4f
+	  8200: 45 72 72 6f 72 40 40 40 5a 00 ae 10 3f 69 73 4f
 	  8210: 62 6a 65 63 74 40 51 4a 73 6f 6e 44 6f 63 75 6d
-	  8220: 65 6e 74 40 40 51 45 42 41 5f 4e 58 5a 00 a4 13
+	  8220: 65 6e 74 40 40 51 45 42 41 5f 4e 58 5a 00 a5 13
 	  8230: 3f 6f 62 6a 65 63 74 40 51 4a 73 6f 6e 44 6f 63
 	  8240: 75 6d 65 6e 74 40 40 51 45 42 41 3f 41 56 51 4a
 	  8250: 73 6f 6e 4f 62 6a 65 63 74 40 40 58 5a 00 04 16
 	  8260: 3f 72 65 61 64 41 6c 6c 40 51 49 4f 44 65 76 69
 	  8270: 63 65 40 40 51 45 41 41 3f 41 56 51 42 79 74 65
-	  8280: 41 72 72 61 79 40 40 58 5a 00 2b 0d 3f 65 72 72
+	  8280: 41 72 72 61 79 40 40 58 5a 00 2c 0d 3f 65 72 72
 	  8290: 6f 72 53 74 72 69 6e 67 40 51 49 4f 44 65 76 69
 	  82a0: 63 65 40 40 51 45 42 41 3f 41 56 51 53 74 72 69
 	  82b0: 6e 67 40 40 58 5a 00 00 51 74 36 43 6f 72 65 2e
 	  82c0: 64 6c 6c 00 8e 02 3f 5f 58 6c 65 6e 67 74 68 5f
 	  82d0: 65 72 72 6f 72 40 73 74 64 40 40 59 41 58 50 45
 	  82e0: 42 44 40 5a 00 00 8c 02 3f 5f 58 62 61 64 5f 66
 	  82f0: 75 6e 63 74 69 6f 6e 5f 63 61 6c 6c 40 73 74 64
@@ -8296,45 +8296,45 @@
 	reloc  134 offset  d00 [31d00] DIR64
 	reloc  135 offset    0 [31000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x180024958
 
 Type                Size     Rva      Offset
   2        CodeView 00000057 00025b58 00024b58
-(format RSDS signature 43ea780ec4f94ad38c2eecfad4efa459 age 1 pdb C:\Users\qt\work\qt\qtnetworkauth_build\bin\Qt6NetworkAuth.pdb)
+(format RSDS signature 4913789a82a643578e5a1b0f5f5d1719 age 1 pdb C:\Users\qt\work\qt\qtnetworkauth_build\bin\Qt6NetworkAuth.pdb)
  12         Feature 00000014 00025bb0 00024bb0
  13         CoffGrp 00000384 00025bc4 00024bc4
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 2
 010   Entry: ID: 0x000010, Value: 0x80000020
 020    Name Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 030     Entry: ID: 0x000001, Value: 0x80000050
 050      Language Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 060       Entry: ID: 0x000409, Value: 0x000080
-080        Leaf: Addr: 0x0360a0, Size: 0x000374, Codepage: 0
+080        Leaf: Addr: 0x0360a0, Size: 0x00036c, Codepage: 0
 018   Entry: ID: 0x000018, Value: 0x80000038
 038    Name Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 048     Entry: ID: 0x000002, Value: 0x80000068
 068      Language Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 078       Entry: ID: 0x000409, Value: 0x000090
-090        Leaf: Addr: 0x036418, Size: 0x00017d, Codepage: 0
+090        Leaf: Addr: 0x036410, Size: 0x00017d, Codepage: 0
  Resources start at offset: 0xa0
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
   0 .text         0001eb5e  0000000180001000  0000000180001000  00000400  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE
   1 .rdata        00010988  0000000180020000  0000000180020000  0001f000  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   2 .data         00000e00  0000000180031000  0000000180031000  0002fa00  2**4
                   CONTENTS, ALLOC, LOAD, DATA
   3 .pdata        00001e84  0000000180034000  0000000180034000  00030800  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  4 .rsrc         00000598  0000000180036000  0000000180036000  00032800  2**2
+  4 .rsrc         00000590  0000000180036000  0000000180036000  00032800  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   5 .reloc        00000470  0000000180037000  0000000180037000  00032e00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
 SYMBOL TABLE:
 no symbols
 
 
@@ -12871,15 +12871,15 @@
    180004c70:	mov    %rbx,0x8(%rsp)
    180004c75:	mov    %rsi,0x10(%rsp)
    180004c7a:	mov    %rdi,0x18(%rsp)
    180004c7f:	push   %r14
    180004c81:	sub    $0x20,%rsp
    180004c85:	mov    %rdx,%rbx
    180004c88:	mov    %r9,%rdi
-   180004c8b:	mov    $0x60602,%edx
+   180004c8b:	mov    $0x60603,%edx
    180004c90:	mov    %r8,%rsi
    180004c93:	mov    %rcx,%r14
    180004c96:	call   *0x1b78c(%rip)        # 0x180020428
    180004c9c:	lea    0x1dc3d(%rip),%rax        # 0x1800228e0
    180004ca3:	xor    %r8d,%r8d
    180004ca6:	lea    0x78(%r14),%rcx
    180004caa:	mov    %rax,(%r14)
@@ -49245,47 +49245,41 @@
    180024943:	imul   $0x34500000,0x6e(%rdi),%ebp
    18002494a:	add    0x1(%rax),%eax
    180024950:	lock xor $0x3,%al
    180024953:	addb   $0x0,(%rcx)
    180024956:	add    %al,(%rax)
    180024958:	add    %al,(%rax)
    18002495a:	add    %al,(%rax)
-   18002495c:	outsl  %ds:(%rsi),(%dx)
-   18002495d:	pop    %rsi
-   18002495e:	(bad)
+   18002495c:	(bad)
    18002495f:	add    %al,%gs:(%rax)
    180024962:	add    %al,(%rax)
    180024964:	add    (%rax),%al
    180024966:	add    %al,(%rax)
    180024968:	push   %rdi
    180024969:	add    %al,(%rax)
    18002496b:	add    %bl,0x5b(%rax)
    18002496e:	add    (%rax),%al
    180024970:	pop    %rax
    180024971:	rex.WXB add (%r8),%al
    180024974:	add    %al,(%rax)
    180024976:	add    %al,(%rax)
-   180024978:	outsl  %ds:(%rsi),(%dx)
-   180024979:	pop    %rsi
-   18002497a:	(bad)
+   180024978:	(bad)
    18002497b:	add    %al,%gs:(%rax)
    18002497e:	add    %al,(%rax)
    180024980:	or     $0x0,%al
    180024982:	add    %al,(%rax)
    180024984:	adc    $0x0,%al
    180024986:	add    %al,(%rax)
    180024988:	mov    $0x5b,%al
    18002498a:	add    (%rax),%al
    18002498c:	mov    $0x4b,%al
    18002498e:	add    (%rax),%al
    180024990:	add    %al,(%rax)
    180024992:	add    %al,(%rax)
-   180024994:	outsl  %ds:(%rsi),(%dx)
-   180024995:	pop    %rsi
-   180024996:	(bad)
+   180024994:	(bad)
    180024997:	add    %al,%gs:(%rax)
    18002499a:	add    %al,(%rax)
    18002499c:	or     $0x84000000,%eax
    1800249a1:	add    (%rax),%eax
    1800249a3:	add    %al,%ah
    1800249a5:	pop    %rbx
    1800249a6:	add    (%rax),%al
@@ -50654,28 +50648,27 @@
    180025b4e:	add    %al,(%rax)
    180025b50:	and    %bh,%cl
    180025b52:	add    %eax,(%rax)
    180025b54:	ds add (%rax),%al
    180025b57:	add    %dl,0x53(%rdx)
    180025b5a:	rex.R push %rbx
    180025b5c:	(bad)
-   180025b5d:	js     0x180025b49
-   180025b5f:	rex.XB stc
+   180025b5d:	js     0x180025b72
+   180025b5f:	rex.WB cmpsb %es:(%rdi),%ds:(%rsi)
    180025b61:	(bad)
-   180025b62:	rorl   %cl,-0x74(%rdx)
-   180025b65:	cs in  (%dx),%al
-   180025b67:	cli
-   180025b68:	(bad)
-   180025b69:	out    %eax,(%dx)
-   180025b6a:	movsb  %ds:(%rsi),%es:(%rdi)
-   180025b6b:	pop    %rcx
-   180025b6c:	add    %eax,(%rax)
-   180025b6e:	add    %al,(%rax)
-   180025b70:	cmp    0x73(%r13,%r10,2),%bl
-   180025b75:	gs jb  0x180025beb
+   180025b62:	push   %rdi
+   180025b63:	rex.XB mov 0x1b(%r10),%ds
+   180025b67:	maxps  0x17(%rbp),%xmm3
+   180025b6b:	sbb    %eax,(%rcx)
+   180025b6d:	add    %al,(%rax)
+   180025b6f:	add    %al,0x3a(%rbx)
+   180025b72:	pop    %rsp
+   180025b73:	push   %rbp
+   180025b74:	jae    0x180025bdb
+   180025b76:	jb     0x180025beb
    180025b78:	pop    %rsp
    180025b79:	jno    0x180025bef
    180025b7b:	pop    %rsp
    180025b7c:	ja     0x180025bed
    180025b7e:	jb     0x180025beb
    180025b80:	pop    %rsp
    180025b81:	jno    0x180025bf7
@@ -51089,15 +51082,15 @@
    180025f20:	add    %ah,0x3(%rax)
    180025f23:	add    %ah,0x2e000000(%rax)
    180025f29:	jb     0x180025f9e
    180025f2b:	jb     0x180025f90
    180025f2d:	and    $0x30,%al
    180025f2f:	xor    %eax,(%rax)
    180025f31:	add    %al,(%rax)
-   180025f33:	add    %ah,-0x7fffca0(%rax)
+   180025f33:	add    %ah,-0xffffca0(%rax)
    180025f39:	add    $0x0,%al
    180025f3b:	add    %ch,(%rsi)
    180025f3d:	jb     0x180025fb2
    180025f3f:	jb     0x180025fa4
    180025f41:	and    $0x30,%al
    180025f43:	xor    (%rax),%al
 	...
@@ -66000,15 +65993,15 @@
    18002df8b:	rex.WRX
    18002df8c:	gs je  0x18002e006
    18002df8f:	outsl  %ds:(%rsi),(%dx)
    18002df90:	jb     0x18002dffd
    18002df92:	cs fs insb (%dx),%es:(%rdi)
    18002df95:	insb   (%dx),%es:(%rdi)
    18002df96:	add    %al,(%rax)
-   18002df98:	je     0x18002dfb4
+   18002df98:	jne    0x18002dfb4
    18002df9a:	(bad)
    18002df9b:	jae    0x18002e011
    18002df9d:	(bad)
    18002df9e:	je     0x18002e009
    18002dfa0:	movsxd 0x65(%rbp),%ecx
    18002dfa3:	je     0x18002e006
    18002dfa5:	(bad)
@@ -66017,16 +66010,17 @@
    18002dfb3:	rex
    18002dfb4:	rex xor 0x51(%rbp),%dl
    18002dfb8:	rex.WRB
    18002dfb9:	gs je  0x18002e01d
    18002dfbc:	(bad)
    18002dfc2:	rex
    18002dfc3:	rex
-   18002dfc4:	rex.X add %sil,0x6f633f0a(%rip)        # 0x1ef661ed5
-   18002dfcb:	insl   (%dx),%es:(%rdi)
+   18002dfc4:	rex.X add %sil,(%rsi)
+   18002dfc7:	or     (%rdi),%bh
+   18002dfc9:	movsxd 0x6d(%rdi),%ebp
    18002dfcc:	jo     0x18002e02f
    18002dfce:	jb     0x18002e035
    18002dfd0:	rex.WRB
    18002dfd1:	gs insl (%dx),%es:(%rdi)
    18002dfd3:	outsl  %ds:(%rsi),(%dx)
    18002dfd4:	jb     0x18002e04f
    18002dfd6:	rex push %rcx
@@ -66075,16 +66069,16 @@
    18002e029:	rex
    18002e02a:	rex.B
    18002e02b:	rex.RB
    18002e02c:	rex.X push %rsi
    18002e02e:	xor    %al,0x40(%rax)
    18002e031:	pop    %rdx
    18002e032:	add    %al,(%rax)
-   18002e034:	std
-   18002e035:	add    (%rdi),%bh
+   18002e034:	incb   (%rdx)
+   18002e036:	(bad)
    18002e037:	(bad)
    18002e038:	xor    %edx,0x42(%rcx)
    18002e03b:	jns    0x18002e0b1
    18002e03d:	gs rex.B jb 0x18002e0b3
    18002e041:	(bad)
    18002e042:	jns    0x18002e084
    18002e044:	rex push %rcx
@@ -66127,15 +66121,15 @@
    18002e088:	rex.RB
    18002e089:	rex.B
    18002e08a:	pop    %r8
    18002e08c:	pop    %rdi
    18002e08d:	rex.WX
    18002e08e:	rex pop %rdx
    18002e090:	add    %al,(%rax)
-   18002e092:	rorb   $1,(%rbx)
+   18002e092:	rorl   $1,(%rbx)
    18002e094:	(bad)
    18002e095:	fs (bad)
    18002e097:	je     0x18002e0fa
    18002e099:	rex push %rcx
    18002e09b:	rex.X jns 0x18002e112
    18002e09e:	gs rex.B jb 0x18002e114
    18002e0a2:	(bad)
@@ -66145,16 +66139,16 @@
    18002e0a8:	rex.X
    18002e0a9:	push   %r8
    18002e0ab:	rex.RB
    18002e0ac:	rex.X
    18002e0ad:	rex.R pop %rax
    18002e0af:	pop    %rdx
    18002e0b0:	add    %al,(%rax)
-   18002e0b2:	(bad)
-   18002e0b3:	or     %bh,(%rdi)
+   18002e0b2:	and    %cl,(%rax)
+   18002e0b4:	(bad)
    18002e0b5:	(bad)
    18002e0b6:	jo     0x18002e128
    18002e0b8:	outsb  %gs:(%rsi),(%dx)
    18002e0ba:	fs rex push %rcx
    18002e0bd:	rex.X jns 0x18002e134
    18002e0c0:	gs rex.B jb 0x18002e136
    18002e0c4:	(bad)
@@ -66168,15 +66162,15 @@
    18002e0ce:	push   %r14
    18002e0d0:	xor    %eax,0x50(%rax)
    18002e0d3:	rex.RB
    18002e0d4:	rex.X
    18002e0d5:	rex.R
    18002e0d6:	rex pop %rdx
    18002e0d8:	add    %al,(%rax)
-   18002e0da:	stos   %al,%es:(%rdi)
+   18002e0da:	stos   %eax,%es:(%rdi)
    18002e0db:	sbb    %edi,(%rdi)
    18002e0dd:	jae    0x18002e148
    18002e0df:	jp     0x18002e146
    18002e0e1:	rex push %rcx
    18002e0e3:	rex.X jns 0x18002e15a
    18002e0e6:	gs rex.B jb 0x18002e15c
    18002e0ea:	(bad)
@@ -66184,31 +66178,33 @@
    18002e0ed:	rex push %rcx
    18002e0ef:	rex.RB
    18002e0f0:	rex.X
    18002e0f1:	pop    %r15
    18002e0f3:	rex.WX pop %rax
    18002e0f5:	pop    %rdx
    18002e0f6:	add    %al,(%rax)
-   18002e0f8:	xchg   %eax,%esp
+   18002e0f8:	xchg   %eax,%ebp
    18002e0f9:	adc    %bh,(%rdi)
    18002e0fb:	imul   $0x406c6c75,0x4e(%rbx),%esi
    18002e102:	push   %rcx
    18002e103:	rex.X jns 0x18002e17a
    18002e106:	gs rex.B jb 0x18002e17c
    18002e10a:	(bad)
    18002e10b:	jns    0x18002e14d
    18002e10d:	rex push %rcx
    18002e10f:	rex.RB
    18002e110:	rex.X
    18002e111:	pop    %r15
    18002e113:	rex.WRX pop %rax
    18002e115:	pop    %rdx
    18002e116:	add    %al,(%rax)
-   18002e118:	sbb    0x40363f3f(%rip),%eax        # 0x1c039205d
-   18002e11e:	pop    %rcx
+   18002e118:	sbb    $0x5,%al
+   18002e11a:	(bad)
+   18002e11b:	(bad)
+   18002e11c:	ss rex pop %rcx
    18002e11f:	rex.B
    18002e120:	rex.B
    18002e121:	rex.RB
    18002e122:	push   %r14
    18002e124:	push   %rcx
    18002e125:	rex.R (bad)
    18002e127:	je     0x18002e18a
@@ -66227,15 +66223,15 @@
    18002e13b:	push   %rcx
    18002e13c:	rex.X jns 0x18002e1b3
    18002e13f:	gs rex.B jb 0x18002e1b5
    18002e143:	(bad)
    18002e144:	jns    0x18002e186
    18002e146:	rex
    18002e147:	rex pop %rdx
-   18002e149:	add    %ah,0x353f3f04(%rbp)
+   18002e149:	add    %ah,0x353f3f04(%rsi)
    18002e14f:	rex pop %rcx
    18002e151:	rex.B
    18002e152:	rex.B
    18002e153:	rex.RB
    18002e154:	push   %r14
    18002e156:	push   %rcx
    18002e157:	rex.R (bad)
@@ -66255,15 +66251,15 @@
    18002e16d:	push   %rcx
    18002e16e:	rex.X jns 0x18002e1e5
    18002e171:	gs rex.B jb 0x18002e1e7
    18002e175:	(bad)
    18002e176:	jns    0x18002e1b8
    18002e178:	rex
    18002e179:	rex pop %rdx
-   18002e17b:	add    %dh,0x6c633f09(%rdx)
+   18002e17b:	add    %dh,0x6c633f09(%rbx)
    18002e181:	(bad)
    18002e182:	jae    0x18002e1f7
    18002e184:	rex.WRX (bad)
    18002e186:	insl   (%dx),%es:(%rdi)
    18002e187:	gs rex push %rcx
    18002e18a:	rex.WRB
    18002e18b:	gs je  0x18002e1ef
@@ -66274,15 +66270,15 @@
    18002e198:	rex.X
    18002e199:	push   %r8
    18002e19b:	rex.RB
    18002e19c:	rex.X
    18002e19d:	rex.R pop %rax
    18002e19f:	pop    %rdx
    18002e1a0:	add    %al,(%rax)
-   18002e1a2:	lods   %ds:(%rsi),%al
+   18002e1a2:	lods   %ds:(%rsi),%eax
    18002e1a3:	sbb    $0x3f,%al
    18002e1a5:	je     0x18002e219
    18002e1a7:	rex push %rcx
    18002e1a9:	rex.WRB
    18002e1aa:	gs je  0x18002e20e
    18002e1ad:	(bad)
    18002e1b3:	rex
@@ -66294,19 +66290,16 @@
    18002e1bc:	push   %rcx
    18002e1bd:	push   %rbx
    18002e1be:	je     0x18002e232
    18002e1c0:	imul   $0x45504040,0x67(%rsi),%ebp
    18002e1c7:	rex.X
    18002e1c8:	xor    %r9b,0x40(%rax)
    18002e1cc:	pop    %rdx
-   18002e1cd:	add    %ah,0x63613f07(%rbx)
-   18002e1d3:	je     0x18002e23e
-   18002e1d5:	jbe    0x18002e238
-   18002e1d7:	je     0x18002e23e
-   18002e1d9:	rex push %rcx
+   18002e1cd:	add    %ah,0x7463613f(%rdi,%rax,1)
+   18002e1d4:	imul   $0x51406574,0x61(%rsi),%esi
    18002e1db:	rex.WRB
    18002e1dc:	gs je  0x18002e240
    18002e1df:	(bad)
    18002e1e5:	rex
    18002e1e6:	rex push %rbx
    18002e1e8:	pop    %r8
    18002e1ea:	push   %rax
@@ -66321,17 +66314,16 @@
    18002e1fb:	xor    %eax,0x48(%rax)
    18002e1fe:	push   %rax
    18002e1ff:	rex.RB
    18002e200:	push   %r8
    18002e202:	rex.RB
    18002e203:	pop    %r8
    18002e205:	rex pop %rdx
-   18002e207:	add    %bh,(%rdx,%rcx,1)
-   18002e20a:	(bad)
-   18002e20b:	movsxd 0x6d(%rdi),%ebp
+   18002e207:	add    %bh,0x6f633f0a(%rip)        # 0x1ef662117
+   18002e20d:	insl   (%dx),%es:(%rdi)
    18002e20e:	jo     0x18002e271
    18002e210:	jb     0x18002e277
    18002e212:	push   %rbx
    18002e213:	je     0x18002e287
    18002e215:	imul   $0x74514073,0x67(%rsi),%ebp
    18002e21c:	push   %rax
    18002e21d:	jb     0x18002e288
@@ -66355,16 +66347,17 @@
    18002e242:	je     0x18002e2ad
    18002e244:	jbe    0x18002e2af
    18002e246:	je     0x18002e2c1
    18002e248:	rex push %rcx
    18002e24a:	je     0x18002e28c
    18002e24c:	rex
    18002e24d:	rex pop %rdx
-   18002e24f:	add    %cl,0x71653f0d(%rip)        # 0x1f1682162
-   18002e255:	jne    0x18002e2b8
+   18002e24f:	add    %cl,(%rsi)
+   18002e251:	or     $0x7571653f,%eax
+   18002e256:	(bad)
    18002e257:	insb   (%dx),%es:(%rdi)
    18002e258:	push   %rbx
    18002e259:	je     0x18002e2cd
    18002e25b:	imul   $0x74514073,0x67(%rsi),%ebp
    18002e262:	push   %rax
    18002e263:	jb     0x18002e2ce
    18002e265:	jbe    0x18002e2c8
@@ -66376,63 +66369,62 @@
    18002e270:	push   %rcx
    18002e271:	push   %rbx
    18002e272:	je     0x18002e2e6
    18002e274:	imul   $0x77656956,0x67(%rsi),%ebp
    18002e27b:	rex
    18002e27c:	rex xor %al,0x5a(%rax)
    18002e280:	add    %al,(%rax)
-   18002e282:	adc    (%rdx),%al
+   18002e282:	adc    (%rdx),%eax
    18002e284:	(bad)
    18002e285:	(bad)
    18002e286:	xor    %dl,0x53(%rcx)
    18002e289:	je     0x18002e2fd
    18002e28b:	imul   $0x45514040,0x67(%rsi),%ebp
    18002e292:	rex.B
    18002e293:	rex.B
    18002e294:	rex pop %rax
    18002e296:	pop    %rdx
-   18002e297:	add    %cl,(%rdx,%rax,1)
-   18002e29a:	(bad)
-   18002e29b:	(bad)
-   18002e29c:	xor    %dl,0x53(%rcx)
+   18002e297:	add    %cl,0x303f3f02(%rip)        # 0x1b042219f
+   18002e29d:	push   %rcx
+   18002e29e:	push   %rbx
    18002e29f:	je     0x18002e313
    18002e2a1:	imul   $0x45514040,0x67(%rsi),%ebp
    18002e2a8:	rex.B
    18002e2a9:	rex.B
    18002e2aa:	rex
    18002e2ab:	rex.B
    18002e2ac:	rex.RB
    18002e2ad:	rex.X push %rsi
    18002e2af:	xor    %al,0x40(%rax)
    18002e2b2:	pop    %rdx
-   18002e2b3:	add    %dh,0x3(%rsi)
+   18002e2b3:	add    %dh,0x3(%rdi)
    18002e2b6:	(bad)
    18002e2b7:	(bad)
    18002e2b8:	xor    %edx,0x53(%rcx)
    18002e2bb:	je     0x18002e32f
    18002e2bd:	imul   $0x45514040,0x67(%rsi),%ebp
    18002e2c4:	rex.B
    18002e2c5:	rex.B
    18002e2c6:	rex pop %rax
    18002e2c8:	pop    %rdx
-   18002e2c9:	add    %cl,(%rbx)
-   18002e2cb:	add    (%rdi),%bh
+   18002e2c9:	add    %cl,(%rdx,%rax,1)
+   18002e2cc:	(bad)
    18002e2cd:	(bad)
    18002e2ce:	xor    %dl,0x53(%rcx)
    18002e2d1:	je     0x18002e345
    18002e2d3:	imul   $0x45514040,0x67(%rsi),%ebp
    18002e2da:	rex.B
    18002e2db:	rex.B
    18002e2dc:	rex and $0x24,%al
    18002e2df:	push   %rcx
    18002e2e0:	rex.RB
    18002e2e1:	push   %r14
    18002e2e3:	xor    %al,0x40(%rax)
    18002e2e6:	pop    %rdx
-   18002e2e7:	add    %ch,0x4(%rbp)
+   18002e2e7:	add    %ch,0x4(%rsi)
    18002e2ea:	(bad)
    18002e2eb:	(bad)
    18002e2ec:	xor    $0x51,%al
    18002e2ee:	push   %rbx
    18002e2ef:	je     0x18002e363
    18002e2f1:	imul   $0x45514040,0x67(%rsi),%ebp
    18002e2f8:	rex.B
@@ -66443,15 +66435,15 @@
    18002e2fe:	xor    %al,0x24(%rax)
    18002e301:	and    $0x51,%al
    18002e303:	rex.RB
    18002e304:	push   %r14
    18002e306:	xor    %al,0x40(%rax)
    18002e309:	pop    %rdx
    18002e30a:	add    %al,(%rax)
-   18002e30c:	fmull  (%rbx)
+   18002e30c:	fisttpll (%rbx)
    18002e30e:	(bad)
    18002e30f:	fs (bad)
    18002e311:	je     0x18002e374
    18002e313:	rex push %rcx
    18002e315:	push   %rbx
    18002e316:	je     0x18002e38a
    18002e318:	imul   $0x45514040,0x67(%rsi),%ebp
@@ -66460,26 +66452,26 @@
    18002e322:	rex.RB
    18002e323:	rex.X push %rsi
    18002e325:	push   %rcx
    18002e326:	rex.XB push $0x40407261
    18002e32c:	pop    %rax
    18002e32d:	pop    %rdx
    18002e32e:	add    %al,(%rax)
-   18002e330:	movsl  %ds:(%rsi),%es:(%rdi)
+   18002e330:	cmpsb  %es:(%rdi),%ds:(%rsi)
    18002e331:	adc    %bh,(%rdi)
    18002e333:	imul   $0x406c6c75,0x4e(%rbx),%esi
    18002e33a:	push   %rcx
    18002e33b:	push   %rbx
    18002e33c:	je     0x18002e3b0
    18002e33e:	imul   $0x45514040,0x67(%rsi),%ebp
    18002e345:	rex.X
    18002e346:	pop    %r15
    18002e348:	rex.WRX pop %rax
    18002e34a:	pop    %rdx
-   18002e34b:	add    %dh,(%rcx)
+   18002e34b:	add    %dh,(%rdx)
    18002e34d:	add    $0x40363f3f,%eax
    18002e352:	pop    %rcx
    18002e353:	rex.B
    18002e354:	rex.B
    18002e355:	rex.RB
    18002e356:	push   %r14
    18002e358:	push   %rcx
@@ -66498,15 +66490,15 @@
    18002e36c:	rex.RB
    18002e36d:	rex.X push %rsi
    18002e36f:	push   %rcx
    18002e370:	push   %rbx
    18002e371:	je     0x18002e3e5
    18002e373:	imul   $0x5a404040,0x67(%rsi),%ebp
    18002e37a:	add    %al,(%rax)
-   18002e37c:	mov    $0x353f3f04,%ebp
+   18002e37c:	mov    $0x353f3f04,%esi
    18002e381:	rex pop %rcx
    18002e383:	rex.B
    18002e384:	rex.B
    18002e385:	rex.RB
    18002e386:	push   %r14
    18002e388:	push   %rcx
    18002e389:	rex.R (bad)
@@ -66524,28 +66516,28 @@
    18002e39c:	rex.RB
    18002e39d:	push   %r14
    18002e39f:	push   %rcx
    18002e3a0:	push   %rbx
    18002e3a1:	je     0x18002e415
    18002e3a3:	imul   $0x5a404040,0x67(%rsi),%ebp
    18002e3aa:	add    %al,(%rax)
-   18002e3ac:	pop    %rbx
+   18002e3ac:	pop    %rsp
    18002e3ad:	add    (%rdi),%bh
    18002e3af:	(bad)
    18002e3b0:	xor    %dl,0x55(%rcx)
    18002e3b3:	jb     0x18002e421
    18002e3b5:	rex
    18002e3b6:	rex push %rcx
    18002e3b8:	rex.RB
    18002e3b9:	rex.B
    18002e3ba:	rex.B
    18002e3bb:	rex pop %rax
    18002e3bd:	pop    %rdx
    18002e3be:	add    %al,(%rax)
-   18002e3c0:	pop    %rcx
+   18002e3c0:	pop    %rdx
    18002e3c1:	add    (%rdi),%bh
    18002e3c3:	(bad)
    18002e3c4:	xor    %dl,0x55(%rcx)
    18002e3c7:	jb     0x18002e435
    18002e3c9:	rex
    18002e3ca:	rex push %rcx
    18002e3cc:	rex.RB
@@ -66554,15 +66546,15 @@
    18002e3cf:	rex
    18002e3d0:	rex.B
    18002e3d1:	rex.RB
    18002e3d2:	rex.X push %rsi
    18002e3d4:	xor    %al,0x40(%rax)
    18002e3d7:	pop    %rdx
    18002e3d8:	add    %al,(%rax)
-   18002e3da:	test   %eax,(%rdi,%rdi,1)
+   18002e3da:	xchg   %al,(%rdi,%rdi,1)
    18002e3dd:	(bad)
    18002e3de:	xor    $0x51,%al
    18002e3e0:	push   %rbp
    18002e3e1:	jb     0x18002e44f
    18002e3e3:	rex
    18002e3e4:	rex push %rcx
    18002e3e6:	rex.RB
@@ -66573,26 +66565,27 @@
    18002e3eb:	push   %r14
    18002e3ed:	xor    %al,0x24(%rax)
    18002e3f0:	and    $0x51,%al
    18002e3f2:	rex.RB
    18002e3f3:	push   %r14
    18002e3f5:	xor    %al,0x40(%rax)
    18002e3f8:	pop    %rdx
-   18002e3f9:	add    %cl,0x51313f3f(%rbx,%rax,1)
+   18002e3f9:	add    %cl,0x313f3f03(%rbp)
+   18002e3ff:	push   %rcx
    18002e400:	push   %rbp
    18002e401:	jb     0x18002e46f
    18002e403:	rex
    18002e404:	rex push %rcx
    18002e406:	rex.RB
    18002e407:	rex.B
    18002e408:	rex.B
    18002e409:	rex pop %rax
    18002e40b:	pop    %rdx
    18002e40c:	add    %al,(%rax)
-   18002e40e:	rex.RXB (bad)
+   18002e40e:	rex.W (bad)
    18002e410:	(bad)
    18002e411:	(bad)
    18002e412:	rex.WRB push %r9
    18002e414:	push   %rbp
    18002e415:	jb     0x18002e483
    18002e417:	rex
    18002e418:	rex push %rcx
@@ -66601,31 +66594,31 @@
    18002e41c:	pop    %r15
    18002e41e:	rex.WRX
    18002e41f:	rex.B
    18002e420:	rex.RB
    18002e421:	rex.X push %rsi
    18002e423:	xor    %al,0x40(%rax)
    18002e426:	pop    %rdx
-   18002e427:	add    %ah,0x383f3f05(%rcx)
+   18002e427:	add    %ah,0x383f3f05(%rdx)
    18002e42d:	push   %rcx
    18002e42e:	push   %rbp
    18002e42f:	jb     0x18002e49d
    18002e431:	rex
    18002e432:	rex push %rcx
    18002e434:	rex.RB
    18002e435:	rex.X
    18002e436:	pop    %r15
    18002e438:	rex.WRX
    18002e439:	rex.B
    18002e43a:	rex.RB
    18002e43b:	rex.X push %rsi
    18002e43d:	xor    %al,0x40(%rax)
    18002e440:	pop    %rdx
-   18002e441:	add    %dh,0x40363f3f(,%rax,1)
-   18002e448:	pop    %rcx
+   18002e441:	add    %dh,0x363f3f05(%rip)        # 0x1b642234c
+   18002e447:	rex pop %rcx
    18002e449:	rex.B
    18002e44a:	rex.B
    18002e44b:	rex.RB
    18002e44c:	push   %r14
    18002e44e:	push   %rcx
    18002e44f:	rex.R (bad)
    18002e451:	je     0x18002e4b4
@@ -66643,15 +66636,15 @@
    18002e463:	rex.X push %rsi
    18002e465:	push   %rcx
    18002e466:	push   %rbp
    18002e467:	jb     0x18002e4d5
    18002e469:	rex
    18002e46a:	rex
    18002e46b:	rex pop %rdx
-   18002e46d:	add    %al,%cl
+   18002e46d:	add    %al,%dl
    18002e46f:	add    $0x3f,%al
    18002e471:	(bad)
    18002e472:	xor    $0x41415940,%eax
    18002e477:	rex.RB
    18002e478:	push   %r14
    18002e47a:	push   %rcx
    18002e47b:	rex.R (bad)
@@ -66670,16 +66663,16 @@
    18002e48f:	push   %r14
    18002e491:	push   %rcx
    18002e492:	push   %rbp
    18002e493:	jb     0x18002e501
    18002e495:	rex
    18002e496:	rex
    18002e497:	rex pop %rdx
-   18002e499:	add    %cl,0x40363f3f(,%rax,1)
-   18002e4a0:	pop    %rcx
+   18002e499:	add    %cl,0x363f3f05(%rip)        # 0x1b64223a4
+   18002e49f:	rex pop %rcx
    18002e4a1:	rex.B (bad)
    18002e4a3:	push   %r14
    18002e4a5:	push   %rcx
    18002e4a6:	rex.R
    18002e4a7:	(bad)
    18002e4ad:	push   %rsi
    18002e4ae:	xor    %al,0x41(%rax)
@@ -66688,15 +66681,15 @@
    18002e4b4:	push   %rcx
    18002e4b5:	push   %rbp
    18002e4b6:	jb     0x18002e524
    18002e4b8:	rex
    18002e4b9:	rex
    18002e4ba:	rex pop %rdx
    18002e4bc:	add    %al,(%rax)
-   18002e4be:	xchg   %eax,%esi
+   18002e4be:	xchg   %eax,%edi
    18002e4bf:	sbb    (%rdi),%bh
    18002e4c1:	jae    0x18002e537
    18002e4c3:	(bad)
    18002e4c4:	je     0x18002e53b
    18002e4c6:	jae    0x18002e508
    18002e4c8:	push   %rcx
    18002e4c9:	rex.R (bad)
@@ -66714,15 +66707,15 @@
    18002e4dc:	xor    $0x53,%al
    18002e4de:	je     0x18002e541
    18002e4e0:	je     0x18002e557
    18002e4e2:	jae    0x18002e524
    18002e4e4:	xor    %eax,0x58(%rax)
    18002e4e7:	pop    %rdx
    18002e4e8:	add    %al,(%rax)
-   18002e4ea:	cmp    %ebx,(%rcx)
+   18002e4ea:	cmp    (%rcx),%bl
    18002e4ec:	(bad)
    18002e4ed:	jae    0x18002e554
    18002e4ef:	je     0x18002e544
    18002e4f1:	je     0x18002e554
    18002e4f3:	je     0x18002e56a
    18002e4f5:	jae    0x18002e537
    18002e4f7:	push   %rcx
@@ -66763,15 +66756,15 @@
    18002e532:	rex
    18002e533:	rex push %rcx
    18002e535:	rex.RB
    18002e536:	rex.B
    18002e537:	pop    %r8
    18002e539:	pop    %rax
    18002e53a:	pop    %rdx
-   18002e53b:	add    %cl,%dh
+   18002e53b:	add    %cl,%bh
    18002e53d:	add    $0x3f,%al
    18002e53f:	(bad)
    18002e540:	xor    $0x74614451,%eax
    18002e545:	(bad)
    18002e546:	push   %rbx
    18002e547:	je     0x18002e5bb
    18002e549:	gs (bad)
@@ -66786,15 +66779,15 @@
    18002e554:	push   %r14
    18002e556:	xor    %al,0x41(%rax)
    18002e559:	rex.RB
    18002e55a:	rex.B
    18002e55b:	rex.W
    18002e55c:	rex pop %rdx
    18002e55e:	add    %al,(%rax)
-   18002e560:	rex.RB add $0x51363f3f,%eax
+   18002e560:	rex.RX add $0x51363f3f,%eax
    18002e566:	rex.R (bad)
    18002e568:	je     0x18002e5cb
    18002e56a:	push   %rbx
    18002e56b:	je     0x18002e5df
    18002e56d:	gs (bad)
    18002e56f:	insl   (%dx),%es:(%rdi)
    18002e570:	rex
@@ -66803,16 +66796,16 @@
    18002e574:	rex.B
    18002e575:	rex.B
    18002e576:	rex.B
    18002e577:	rex.RB
    18002e578:	push   %r14
    18002e57a:	xor    %al,0x48(%rax)
    18002e57d:	rex pop %rdx
-   18002e57f:	add    %dl,(%rbx)
-   18002e581:	adc    %bh,(%rdi)
+   18002e57f:	add    %dl,(%rax,%rdx,1)
+   18002e582:	(bad)
    18002e583:	imul   $0x63697665,0x44(%rbx),%esi
    18002e58a:	gs push %rsp
    18002e58c:	jb     0x18002e5ef
    18002e58e:	outsb  %ds:(%rsi),(%dx)
    18002e58f:	jae    0x18002e5f2
    18002e591:	movsxd 0x6f(%rcx,%rbp,2),%esi
    18002e595:	outsb  %ds:(%rsi),(%dx)
@@ -66857,28 +66850,28 @@
    18002e5e7:	gs rex.B jb 0x18002e65d
    18002e5eb:	(bad)
    18002e5ec:	jns    0x18002e62e
    18002e5ee:	rex push %rsi
    18002e5f0:	xor    %eax,0x40(%rax)
    18002e5f3:	pop    %rdx
    18002e5f4:	add    %al,(%rax)
-   18002e5f6:	or     (%rdi),%ecx
+   18002e5f6:	or     $0xf,%al
    18002e5f8:	(bad)
    18002e5f9:	imul   $0x6174654d,0x51(%rax,%rax,2),%esp
    18002e601:	push   %rsp
    18002e602:	jns    0x18002e674
    18002e604:	gs rex
    18002e606:	rex push %rcx
    18002e608:	rex.RB
    18002e609:	rex.X
    18002e60a:	rex.B
    18002e60b:	rex.W
    18002e60c:	rex.W
    18002e60d:	rex pop %rdx
-   18002e60f:	add    %bl,0x79643f0c(%rbp)
+   18002e60f:	add    %bl,0x79643f0c(%rsi)
    18002e615:	outsb  %ds:(%rsi),(%dx)
    18002e616:	(bad)
    18002e617:	insl   (%dx),%es:(%rdi)
    18002e618:	imul   $0x4f617465,0x4d(%rbx),%esp
    18002e61f:	(bad)
    18002e624:	rex push %rcx
    18002e626:	(bad)
@@ -66894,15 +66887,15 @@
    18002e63a:	push   %rcx
    18002e63b:	rex.WRB
    18002e63c:	gs je  0x18002e6a0
    18002e63f:	(bad)
    18002e645:	rex
    18002e646:	rex pop %rax
    18002e648:	pop    %rdx
-   18002e649:	add    %bh,0x15(%rsi)
+   18002e649:	add    %bh,0x15(%rdi)
    18002e64c:	(bad)
    18002e64d:	jno    0x18002e6c3
    18002e64f:	pop    %rdi
    18002e650:	insl   (%dx),%es:(%rdi)
    18002e651:	gs je  0x18002e6b5
    18002e654:	movsxd 0x73(%rcx),%esp
    18002e657:	je     0x18002e699
@@ -66917,15 +66910,15 @@
    18002e668:	pop    %r8
    18002e66a:	push   %rax
    18002e66b:	rex.RB
    18002e66c:	rex.X
    18002e66d:	rex.R
    18002e66e:	rex pop %rdx
    18002e670:	add    %al,(%rax)
-   18002e672:	rex.WB adc $0x5f74713f,%rax
+   18002e672:	rex.WX adc $0x5f74713f,%rax
    18002e678:	insl   (%dx),%es:(%rdi)
    18002e679:	gs je  0x18002e6dd
    18002e67c:	movsxd 0x6c(%rcx),%esp
    18002e67f:	insb   (%dx),%es:(%rdi)
    18002e680:	rex push %rcx
    18002e682:	(bad)
    18002e688:	rex
@@ -66974,29 +66967,29 @@
    18002e6d9:	push   %rcx
    18002e6da:	rex.RB
    18002e6db:	rex.B
    18002e6dc:	rex.B
    18002e6dd:	rex pop %rax
    18002e6df:	pop    %rdx
    18002e6e0:	add    %al,(%rax)
-   18002e6e2:	push   %rbx
+   18002e6e2:	push   %rsp
    18002e6e3:	add    $0x51363f3f,%eax
    18002e6e8:	rex.R
    18002e6e9:	(bad)
    18002e6ef:	push   %rcx
    18002e6f0:	rex.RB
    18002e6f1:	rex.B
    18002e6f2:	rex.B
    18002e6f3:	rex.B
    18002e6f4:	rex.RB
    18002e6f5:	push   %r14
    18002e6f7:	xor    %al,0x44(%rax)
    18002e6fa:	rex pop %rdx
    18002e6fc:	add    %al,(%rax)
-   18002e6fe:	pop    %rbp
+   18002e6fe:	pop    %rsi
    18002e6ff:	add    $0x51363f3f,%eax
    18002e704:	rex.R
    18002e705:	(bad)
    18002e70b:	push   %rcx
    18002e70c:	rex.RB
    18002e70d:	rex.B
    18002e70e:	rex.B
@@ -67004,15 +66997,15 @@
    18002e710:	rex.RB
    18002e711:	push   %r14
    18002e713:	xor    %al,0x50(%rax)
    18002e716:	rex.RB
    18002e717:	rex.X
    18002e718:	rex.R
    18002e719:	rex pop %rdx
-   18002e71b:	add    %dl,0x5(%rdx)
+   18002e71b:	add    %dl,0x5(%rbx)
    18002e71e:	(bad)
    18002e71f:	(bad)
    18002e720:	ss push %rcx
    18002e722:	rex.R
    18002e723:	(bad)
    18002e729:	push   %rcx
    18002e72a:	rex.RB
@@ -67025,15 +67018,15 @@
    18002e734:	rex.RB
    18002e735:	rex.X push %rsi
    18002e737:	push   %rcx
    18002e738:	push   %rbx
    18002e739:	je     0x18002e7ad
    18002e73b:	imul   $0x5a404040,0x67(%rsi),%ebp
    18002e742:	add    %al,(%rax)
-   18002e744:	push   %rcx
+   18002e744:	push   %rdx
    18002e745:	add    $0x51363f3f,%eax
    18002e74a:	rex.R
    18002e74b:	(bad)
    18002e751:	push   %rcx
    18002e752:	rex.RB
    18002e753:	rex.B
    18002e754:	rex.B
@@ -67070,16 +67063,16 @@
    18002e78b:	rex.RB
    18002e78c:	push   %r14
    18002e78e:	push   %rcx
    18002e78f:	rex.R
    18002e790:	(bad)
    18002e796:	rex pop %rdx
    18002e798:	add    %al,(%rax)
-   18002e79a:	(bad)
-   18002e79b:	add    (%rdi),%edi
+   18002e79a:	sbb    %al,(%rbx)
+   18002e79c:	(bad)
    18002e79d:	(bad)
    18002e79e:	xor    %edx,0x44(%rcx)
    18002e7a1:	(bad)
    18002e7a7:	(bad)
    18002e7a8:	je     0x18002e80f
    18002e7aa:	push   %rbx
    18002e7ab:	(bad)
@@ -67088,15 +67081,15 @@
    18002e7b0:	rex push %rcx
    18002e7b2:	rex.RB
    18002e7b3:	rex.B
    18002e7b4:	rex.B
    18002e7b5:	rex pop %rax
    18002e7b7:	pop    %rdx
    18002e7b8:	add    %al,(%rax)
-   18002e7ba:	and    %dl,0x5f74713f(%rip)        # 0x1df7758ff
+   18002e7ba:	and    %edx,0x5f74713f(%rip)        # 0x1df7758ff
    18002e7c0:	push   %rcx
    18002e7c1:	rex.WRB
    18002e7c2:	gs je  0x18002e826
    18002e7c5:	rex.RB outsb %ds:(%rsi),(%dx)
    18002e7c7:	jne    0x18002e836
    18002e7c9:	pop    %rdi
    18002e7ca:	(bad)
@@ -67122,30 +67115,30 @@
    18002e7f7:	(bad)
    18002e7fd:	rex
    18002e7fe:	rex push %rax
    18002e800:	rex.RB
    18002e801:	rex.X
    18002e802:	rex.R
    18002e803:	rex pop %rdx
-   18002e805:	add    %bl,0x303f3f02(%rbp)
+   18002e805:	add    %bl,0x303f3f02(%rsi)
    18002e80b:	push   %rcx
    18002e80c:	push   %rsi
    18002e80d:	(bad)
    18002e80e:	jb     0x18002e879
    18002e810:	(bad)
    18002e811:	outsb  %ds:(%rsi),(%dx)
    18002e812:	je     0x18002e854
    18002e814:	rex push %rcx
    18002e816:	rex.RB
    18002e817:	rex.B
    18002e818:	rex.B
    18002e819:	rex pop %rax
    18002e81b:	pop    %rdx
    18002e81c:	add    %al,(%rax)
-   18002e81e:	mov    (%rbx),%es
+   18002e81e:	pop    (%rbx)
    18002e820:	(bad)
    18002e821:	(bad)
    18002e822:	xor    %edx,0x56(%rcx)
    18002e825:	(bad)
    18002e826:	jb     0x18002e891
    18002e828:	(bad)
    18002e829:	outsb  %ds:(%rsi),(%dx)
@@ -67153,15 +67146,15 @@
    18002e82c:	rex push %rcx
    18002e82e:	rex.RB
    18002e82f:	rex.B
    18002e830:	rex.B
    18002e831:	rex pop %rax
    18002e833:	pop    %rdx
    18002e834:	add    %al,(%rax)
-   18002e836:	insl   (%dx),%es:(%rdi)
+   18002e836:	outsb  %ds:(%rsi),(%dx)
    18002e837:	add    (%rdi),%bh
    18002e839:	(bad)
    18002e83a:	xor    %dl,0x56(%rcx)
    18002e83d:	(bad)
    18002e83e:	jb     0x18002e8a9
    18002e840:	(bad)
    18002e841:	outsb  %ds:(%rsi),(%dx)
@@ -67173,15 +67166,15 @@
    18002e849:	rex
    18002e84a:	rex.B
    18002e84b:	rex.RB
    18002e84c:	rex.X push %rsi
    18002e84e:	xor    %al,0x40(%rax)
    18002e851:	pop    %rdx
    18002e852:	add    %al,(%rax)
-   18002e854:	mov    (%rdi,%rdi,1),%es
+   18002e854:	pop    (%rdi,%rdi,1)
    18002e857:	(bad)
    18002e858:	xor    $0x51,%al
    18002e85a:	push   %rsi
    18002e85b:	(bad)
    18002e85c:	jb     0x18002e8c7
    18002e85e:	(bad)
    18002e85f:	outsb  %ds:(%rsi),(%dx)
@@ -67194,16 +67187,17 @@
    18002e868:	rex.RB
    18002e869:	push   %r14
    18002e86b:	xor    %al,0x41(%rax)
    18002e86e:	rex.RB
    18002e86f:	rex.X push %rsi
    18002e871:	xor    %al,0x40(%rax)
    18002e874:	pop    %rdx
-   18002e875:	add    %cl,0x64713f15(%rip)        # 0x1e4742790
-   18002e87b:	(bad)
+   18002e875:	add    %cl,(%rsi)
+   18002e877:	adc    $0x6564713f,%eax
+   18002e87c:	(bad)
    18002e881:	insb   (%dx),%es:(%rdi)
    18002e882:	jo     0x18002e8e9
    18002e884:	jb     0x18002e8c6
    18002e886:	push   %rcx
    18002e887:	push   %rsi
    18002e888:	(bad)
    18002e889:	jb     0x18002e8f4
@@ -67219,18 +67213,16 @@
    18002e897:	push   %rcx
    18002e898:	rex.R
    18002e899:	(bad)
    18002e89f:	push   %rsi
    18002e8a0:	xor    0x40(%rax),%al
    18002e8a3:	pop    %rdx
    18002e8a4:	add    %al,(%rax)
-   18002e8a6:	adc    $0xd,%al
-   18002e8a8:	(bad)
-   18002e8a9:	gs jno 0x18002e921
-   18002e8ac:	(bad)
+   18002e8a6:	adc    $0x71653f0d,%eax
+   18002e8ab:	jne    0x18002e90e
    18002e8ad:	insb   (%dx),%es:(%rdi)
    18002e8ae:	jae    0x18002e8f0
    18002e8b0:	push   %rcx
    18002e8b1:	push   %rsi
    18002e8b2:	(bad)
    18002e8b3:	jb     0x18002e91e
    18002e8b5:	(bad)
@@ -67244,15 +67236,15 @@
    18002e8bf:	rex.WRX
    18002e8c0:	rex.B
    18002e8c1:	rex.RB
    18002e8c2:	rex.X push %rsi
    18002e8c4:	xor    %eax,0x40(%rax)
    18002e8c7:	pop    %rdx
    18002e8c8:	add    %al,(%rax)
-   18002e8ca:	ret
+   18002e8ca:	(bad)
    18002e8cb:	add    $0x3f,%al
    18002e8cd:	(bad)
    18002e8ce:	xor    $0x41415940,%eax
    18002e8d3:	rex.RB
    18002e8d4:	push   %r14
    18002e8d6:	push   %rcx
    18002e8d7:	rex.R (bad)
@@ -67274,15 +67266,15 @@
    18002e8ef:	(bad)
    18002e8f0:	jb     0x18002e95b
    18002e8f2:	(bad)
    18002e8f3:	outsb  %ds:(%rsi),(%dx)
    18002e8f4:	je     0x18002e936
    18002e8f6:	rex
    18002e8f7:	rex pop %rdx
-   18002e8f9:	add    %dh,(%rsi)
+   18002e8f9:	add    %dh,(%rdi)
    18002e8fb:	add    $0x40363f3f,%eax
    18002e900:	pop    %rcx
    18002e901:	rex.B
    18002e902:	rex.B
    18002e903:	rex.RB
    18002e904:	push   %r14
    18002e906:	push   %rcx
@@ -67305,15 +67297,15 @@
    18002e91f:	(bad)
    18002e920:	jb     0x18002e98b
    18002e922:	(bad)
    18002e923:	outsb  %ds:(%rsi),(%dx)
    18002e924:	je     0x18002e966
    18002e926:	rex
    18002e927:	rex pop %rdx
-   18002e929:	add    %cl,%ah
+   18002e929:	add    %cl,%ch
    18002e92b:	add    (%rdi),%edi
    18002e92d:	(bad)
    18002e92e:	xor    $0x51,%al
    18002e930:	rex.X jns 0x18002e9a7
    18002e933:	gs rex.B jb 0x18002e9a9
    18002e937:	(bad)
    18002e938:	jns    0x18002e97a
@@ -67326,15 +67318,15 @@
    18002e941:	push   %r14
    18002e943:	xor    %al,0x24(%rax)
    18002e946:	and    $0x51,%al
    18002e948:	rex.RB
    18002e949:	push   %r14
    18002e94b:	xor    %al,0x40(%rax)
    18002e94e:	pop    %rdx
-   18002e94f:	add    %bl,(%rsi)
+   18002e94f:	add    %bl,(%rdi)
    18002e951:	or     %bh,(%rdi)
    18002e953:	(bad)
    18002e954:	jo     0x18002e9c6
    18002e956:	outsb  %gs:(%rsi),(%dx)
    18002e958:	fs rex push %rcx
    18002e95b:	rex.X jns 0x18002e9d2
    18002e95e:	gs rex.B jb 0x18002e9d4
@@ -67345,15 +67337,15 @@
    18002e968:	rex.B
    18002e969:	rex.B
    18002e96a:	rex.B
    18002e96b:	rex.RB
    18002e96c:	push   %r14
    18002e96e:	xor    %eax,0x44(%rax)
    18002e971:	rex pop %rdx
-   18002e973:	add    %ch,0x4(%rsi)
+   18002e973:	add    %ch,0x4(%rdi)
    18002e976:	(bad)
    18002e977:	(bad)
    18002e978:	xor    $0x51,%al
    18002e97a:	push   %rbx
    18002e97b:	je     0x18002e9ef
    18002e97d:	imul   $0x45514040,0x67(%rsi),%ebp
    18002e984:	rex.B
@@ -67363,15 +67355,15 @@
    18002e988:	push   %r14
    18002e98a:	xor    %al,0x41(%rax)
    18002e98d:	rex.RB
    18002e98e:	rex.X push %rsi
    18002e990:	xor    %al,0x40(%rax)
    18002e993:	pop    %rdx
    18002e994:	add    %al,(%rax)
-   18002e996:	outsb  %ds:(%rsi),(%dx)
+   18002e996:	outsl  %ds:(%rsi),(%dx)
    18002e997:	sbb    $0x3f,%al
    18002e999:	je     0x18002ea0a
    18002e99b:	push   %rbp
    18002e99c:	je     0x18002ea04
    18002e99e:	cmp    %al,0x51(%rax)
    18002e9a1:	push   %rbx
    18002e9a2:	je     0x18002ea16
@@ -67383,15 +67375,15 @@
    18002e9b1:	push   %rcx
    18002e9b2:	rex.X jns 0x18002ea29
    18002e9b5:	gs rex.B jb 0x18002ea2b
    18002e9b9:	(bad)
    18002e9ba:	jns    0x18002e9fc
    18002e9bc:	rex pop %rax
    18002e9be:	pop    %rdx
-   18002e9bf:	add    %cl,(%rdx)
+   18002e9bf:	add    %cl,(%rbx)
    18002e9c1:	add    (%rdi),%bh
    18002e9c3:	(bad)
    18002e9c4:	xor    %dl,0x53(%rcx)
    18002e9c7:	je     0x18002ea3b
    18002e9c9:	imul   $0x45514040,0x67(%rsi),%ebp
    18002e9d0:	rex.B
    18002e9d1:	rex.B
@@ -67409,15 +67401,15 @@
    18002e9e5:	push   %rax
    18002e9e6:	outsl  %ds:(%rsi),(%dx)
    18002e9e7:	imul   $0x5f407265,0x74(%rsi),%ebp
    18002e9ee:	push   %rbx
    18002e9ef:	rex
    18002e9f0:	rex
    18002e9f1:	rex pop %rdx
-   18002e9f3:	add    %al,0x343f3f04(%rsi)
+   18002e9f3:	add    %al,0x343f3f04(%rdi)
    18002e9f9:	push   %rcx
    18002e9fa:	push   %rbp
    18002e9fb:	jb     0x18002ea69
    18002e9fd:	rex
    18002e9fe:	rex push %rcx
    18002ea00:	rex.RB
    18002ea01:	rex.B
@@ -67426,15 +67418,15 @@
    18002ea04:	rex.RB
    18002ea05:	push   %r14
    18002ea07:	xor    %al,0x41(%rax)
    18002ea0a:	rex.RB
    18002ea0b:	rex.X push %rsi
    18002ea0d:	xor    %al,0x40(%rax)
    18002ea10:	pop    %rdx
-   18002ea11:	add    %bh,%ah
+   18002ea11:	add    %bh,%ch
    18002ea13:	sbb    %bh,(%rdi)
    18002ea15:	jae    0x18002ea7c
    18002ea17:	je     0x18002ea6a
    18002ea19:	jne    0x18002ea80
    18002ea1b:	jb     0x18002ea96
    18002ea1d:	rex push %rcx
    18002ea1f:	push   %rbp
@@ -67453,41 +67445,42 @@
    18002ea31:	push   %rcx
    18002ea32:	jne    0x18002ea99
    18002ea34:	jb     0x18002eaaf
    18002ea36:	rex
    18002ea37:	rex
    18002ea38:	rex pop %rdx
    18002ea3a:	add    %al,(%rax)
-   18002ea3c:	enter  $0x3f05,$0x3f
-   18002ea40:	cmp    %edx,0x55(%rcx)
+   18002ea3c:	leave
+   18002ea3d:	add    $0x51393f3f,%eax
+   18002ea42:	push   %rbp
    18002ea43:	jb     0x18002eab1
    18002ea45:	rex
    18002ea46:	rex push %rcx
    18002ea48:	rex.RB
    18002ea49:	rex.X
    18002ea4a:	pop    %r15
    18002ea4c:	rex.WRX
    18002ea4d:	rex.B
    18002ea4e:	rex.RB
    18002ea4f:	rex.X push %rsi
    18002ea51:	xor    %al,0x40(%rax)
    18002ea54:	pop    %rdx
-   18002ea55:	add    %dl,0x3(%rdx)
+   18002ea55:	add    %dl,0x3(%rbx)
    18002ea58:	(bad)
    18002ea59:	(bad)
    18002ea5a:	xor    %edx,0x4f(%rcx)
    18002ea5d:	(bad)
    18002ea62:	rex
    18002ea63:	rex push %rbp
    18002ea65:	rex.RB
    18002ea66:	rex.B
    18002ea67:	rex.B
    18002ea68:	rex pop %rax
    18002ea6a:	pop    %rdx
-   18002ea6b:	add    %ah,%al
+   18002ea6b:	add    %ah,%cl
    18002ea6d:	adc    (%rdi),%edi
    18002ea6f:	jo     0x18002ead2
    18002ea71:	jb     0x18002ead8
    18002ea73:	outsb  %ds:(%rsi),(%dx)
    18002ea74:	je     0x18002eab6
    18002ea76:	push   %rcx
    18002ea77:	(bad)
@@ -67521,15 +67514,15 @@
    18002eaaf:	je     0x18002eb16
    18002eab1:	rex
    18002eab2:	rex push %rax
    18002eab4:	rex.RB
    18002eab5:	push   %r14
    18002eab7:	xor    %al,0x40(%rax)
    18002eaba:	pop    %rdx
-   18002eabb:	add    %cl,0x65673f0e(%rcx)
+   18002eabb:	add    %cl,0x65673f0e(%rdx)
    18002eac1:	je     0x18002eb04
    18002eac3:	outsb  %ds:(%rsi),(%dx)
    18002eac4:	fs push %rdx
    18002eac6:	gs data16 rex
    18002eac9:	rex.RB js 0x18002eb40
    18002eacc:	gs jb  0x18002eb3d
    18002eacf:	(bad)
@@ -67555,15 +67548,15 @@
    18002eaf9:	rex.RB
    18002eafa:	rex.X push %rsi
    18002eafc:	push   %rcx
    18002eafd:	(bad)
    18002eb03:	rex
    18002eb04:	rex
    18002eb05:	rex pop %rdx
-   18002eb07:	add    %dh,0x2(%rcx)
+   18002eb07:	add    %dh,0x2(%rdx)
    18002eb0a:	(bad)
    18002eb0b:	(bad)
    18002eb0c:	xor    %dl,0x56(%rcx)
    18002eb0f:	(bad)
    18002eb10:	jb     0x18002eb7b
    18002eb12:	(bad)
    18002eb13:	outsb  %ds:(%rsi),(%dx)
@@ -67592,15 +67585,15 @@
    18002eb38:	outsb  %ds:(%rsi),(%dx)
    18002eb39:	je     0x18002eb7b
    18002eb3b:	rex
    18002eb3c:	rex
    18002eb3d:	rex
    18002eb3e:	rex pop %rdx
    18002eb40:	add    %al,(%rax)
-   18002eb42:	xchg   %al,(%rdx)
+   18002eb42:	xchg   %eax,(%rdx)
    18002eb44:	(bad)
    18002eb45:	(bad)
    18002eb46:	xor    %dl,0x56(%rcx)
    18002eb49:	(bad)
    18002eb4a:	jb     0x18002ebb5
    18002eb4c:	(bad)
    18002eb4d:	outsb  %ds:(%rsi),(%dx)
@@ -67613,15 +67606,17 @@
    18002eb56:	rex.B
    18002eb57:	rex.RB
    18002eb58:	rex.X push %rsi
    18002eb5a:	push   %rcx
    18002eb5b:	push   %rbx
    18002eb5c:	je     0x18002ebd0
    18002eb5e:	imul   $0x5a404040,0x67(%rsi),%ebp
-   18002eb65:	add    %dh,0x6f743f1c(%rip)        # 0x1ef772a87
+   18002eb65:	add    %dh,(%rsi)
+   18002eb67:	sbb    $0x3f,%al
+   18002eb69:	je     0x18002ebda
    18002eb6b:	push   %rbx
    18002eb6c:	je     0x18002ebe0
    18002eb6e:	imul   $0x61565140,0x67(%rsi),%ebp
    18002eb75:	jb     0x18002ebe0
    18002eb77:	(bad)
    18002eb78:	outsb  %ds:(%rsi),(%dx)
    18002eb79:	je     0x18002ebbb
@@ -67648,15 +67643,15 @@
    18002eba4:	rex push %rcx
    18002eba6:	rex.RB
    18002eba7:	rex.B
    18002eba8:	rex.B
    18002eba9:	rex
    18002ebaa:	rex.W
    18002ebab:	rex pop %rdx
-   18002ebad:	add    %dl,0x3(%rbp)
+   18002ebad:	add    %dl,0x3(%rsi)
    18002ebb0:	(bad)
    18002ebb1:	(bad)
    18002ebb2:	xor    %edx,0x4f(%rcx)
    18002ebb5:	(bad)
    18002ebba:	push   %rax
    18002ebbb:	jb     0x18002ec26
    18002ebbd:	jbe    0x18002ec20
@@ -67690,15 +67685,15 @@
    18002ebef:	je     0x18002ec3e
    18002ebf1:	jae    0x18002ec5a
    18002ebf3:	push   %rsp
    18002ebf4:	jns    0x18002ec66
    18002ebf6:	gs rex
    18002ebf8:	rex
    18002ebf9:	rex pop %rdx
-   18002ebfb:	add    %al,0x3(%rsi)
+   18002ebfb:	add    %al,0x3(%rdi)
    18002ebfe:	(bad)
    18002ebff:	(bad)
    18002ec00:	xor    %edx,0x4c(%rcx)
    18002ec03:	outsl  %ds:(%rsi),(%dx)
    18002ec04:	addr32 imul $0x65746143,0x67(%esi),%ebp
    18002ec0d:	outsl  %ds:(%esi),(%dx)
    18002ec0f:	jb     0x18002ec8a
@@ -67706,27 +67701,25 @@
    18002ec12:	rex push %rcx
    18002ec14:	rex.RB
    18002ec15:	rex.B
    18002ec16:	rex.B
    18002ec17:	rex pop %rax
    18002ec19:	pop    %rdx
    18002ec1a:	add    %al,(%rax)
-   18002ec1c:	adc    $0x3,%al
-   18002ec1e:	(bad)
-   18002ec1f:	(bad)
-   18002ec20:	xor    %edx,0x44(%rcx)
-   18002ec23:	(bad)
+   18002ec1c:	adc    $0x313f3f03,%eax
+   18002ec21:	push   %rcx
+   18002ec22:	rex.R (bad)
    18002ec24:	je     0x18002ec8b
    18002ec26:	push   %rsp
    18002ec27:	imul   $0x45514040,0x65(%rbp),%ebp
    18002ec2e:	rex.B
    18002ec2f:	rex.B
    18002ec30:	rex pop %rax
    18002ec32:	pop    %rdx
-   18002ec33:	add    %dl,%ch
+   18002ec33:	add    %dl,%dh
    18002ec35:	sbb    (%rdi),%edi
    18002ec37:	je     0x18002eca8
    18002ec39:	rex.WRB push %r11
    18002ec3b:	movsxd %gs:0x53(%rbx),%esi
    18002ec3f:	imul   $0x6f704565,0x63(%rsi),%ebp
    18002ec46:	movsxd 0x40(%rax),%ebp
    18002ec49:	push   %rcx
@@ -67735,15 +67728,15 @@
    18002ec4e:	push   %rsp
    18002ec4f:	imul   $0x45514040,0x65(%rbp),%ebp
    18002ec56:	rex.X
    18002ec57:	pop    %r15
    18002ec59:	rex.WX pop %rax
    18002ec5b:	pop    %rdx
    18002ec5c:	add    %al,(%rax)
-   18002ec5e:	rex or (%rdi),%edi
+   18002ec5e:	or     (%r15),%edi
    18002ec61:	movsxd 0x72(%rbp),%esi
    18002ec64:	jb     0x18002eccb
    18002ec66:	outsb  %ds:(%rsi),(%dx)
    18002ec67:	je     0x18002ecad
    18002ec69:	(bad)
    18002ec6a:	je     0x18002ecd1
    18002ec6c:	push   %rsp
@@ -67751,45 +67744,45 @@
    18002ec74:	je     0x18002ecdb
    18002ec76:	push   %rsp
    18002ec77:	imul   $0x41534040,0x65(%rbp),%ebp
    18002ec7e:	(bad)
    18002ec7f:	push   %r14
    18002ec81:	xor    %eax,0x58(%rax)
    18002ec84:	pop    %rdx
-   18002ec85:	add    %ah,0x2(%rcx)
+   18002ec85:	add    %ah,0x2(%rdx)
    18002ec88:	(bad)
    18002ec89:	(bad)
    18002ec8a:	xor    %dl,0x55(%rcx)
    18002ec8d:	jb     0x18002ecfb
    18002ec8f:	push   %rcx
    18002ec90:	jne    0x18002ecf7
    18002ec92:	jb     0x18002ed0d
    18002ec94:	rex
    18002ec95:	rex push %rcx
    18002ec97:	rex.RB
    18002ec98:	rex.B
    18002ec99:	rex.B
    18002ec9a:	rex pop %rax
    18002ec9c:	pop    %rdx
-   18002ec9d:	add    %cl,0x313f3f03(%rbp)
+   18002ec9d:	add    %cl,0x313f3f03(%rsi)
    18002eca3:	push   %rcx
    18002eca4:	push   %rbp
    18002eca5:	jb     0x18002ed13
    18002eca7:	push   %rcx
    18002eca8:	jne    0x18002ed0f
    18002ecaa:	jb     0x18002ed25
    18002ecac:	rex
    18002ecad:	rex push %rcx
    18002ecaf:	rex.RB
    18002ecb0:	rex.B
    18002ecb1:	rex.B
    18002ecb2:	rex pop %rax
    18002ecb4:	pop    %rdx
-   18002ecb5:	add    %dh,(%rbx)
-   18002ecb7:	sbb    $0x3f,%al
+   18002ecb5:	add    %dh,(%rsp,%rbx,1)
+   18002ecb8:	(bad)
    18002ecb9:	je     0x18002ed2a
    18002ecbb:	push   %rbx
    18002ecbc:	je     0x18002ed30
    18002ecbe:	imul   $0x72555140,0x67(%rsi),%ebp
    18002ecc5:	insb   (%dx),%es:(%rdi)
    18002ecc6:	push   %rcx
    18002ecc7:	jne    0x18002ed2e
@@ -67827,15 +67820,15 @@
    18002ed04:	push   %rbp
    18002ed05:	jb     0x18002ed73
    18002ed07:	rex
    18002ed08:	rex
    18002ed09:	rex
    18002ed0a:	rex
    18002ed0b:	rex pop %rdx
-   18002ed0d:	add    %ah,%bl
+   18002ed0d:	add    %ah,%ah
    18002ed0f:	(bad)
    18002ed10:	(bad)
    18002ed11:	(bad)
    18002ed12:	fs fs push %rcx
    18002ed15:	jne    0x18002ed7c
    18002ed17:	jb     0x18002ed92
    18002ed19:	rex.WB je 0x18002ed81
@@ -67856,29 +67849,30 @@
    18002ed30:	rex.X push %rsi
    18002ed32:	push   %rcx
    18002ed33:	push   %rbx
    18002ed34:	je     0x18002eda8
    18002ed36:	imul   $0x40304040,0x67(%rsi),%ebp
    18002ed3d:	pop    %rdx
    18002ed3e:	add    %al,(%rax)
-   18002ed40:	cmp    $0x313f3f03,%eax
-   18002ed45:	push   %rcx
-   18002ed46:	rex.WX jae 0x18002edb8
+   18002ed40:	ds add (%rdi),%edi
+   18002ed43:	(bad)
+   18002ed44:	xor    %edx,0x4a(%rcx)
+   18002ed47:	jae    0x18002edb8
    18002ed49:	outsb  %ds:(%rsi),(%dx)
    18002ed4a:	rex.R outsl %ds:(%rsi),(%dx)
    18002ed4c:	movsxd 0x6d(%rbp),%esi
    18002ed4f:	outsb  %gs:(%rsi),(%dx)
    18002ed51:	je     0x18002ed93
    18002ed53:	rex push %rcx
    18002ed55:	rex.RB
    18002ed56:	rex.B
    18002ed57:	rex.B
    18002ed58:	rex pop %rax
    18002ed5a:	pop    %rdx
-   18002ed5b:	add    %dh,0xe(%rdx)
+   18002ed5b:	add    %dh,0xe(%rbx)
    18002ed5e:	(bad)
    18002ed5f:	data16 jb 0x18002edd1
    18002ed62:	insl   (%dx),%es:(%rdi)
    18002ed63:	push   %rsi
    18002ed64:	(bad)
    18002ed65:	jb     0x18002edd0
    18002ed67:	(bad)
@@ -67902,15 +67896,15 @@
    18002ed87:	(bad)
    18002ed88:	jb     0x18002edf3
    18002ed8a:	(bad)
    18002ed8b:	outsb  %ds:(%rsi),(%dx)
    18002ed8c:	je     0x18002edce
    18002ed8e:	rex
    18002ed8f:	rex pop %rdx
-   18002ed91:	add    %ah,0x6f743f1b(%rbp)
+   18002ed91:	add    %ah,0x6f743f1b(%rsi)
    18002ed97:	rex.WX jae 0x18002ee09
    18002ed9a:	outsb  %ds:(%rsi),(%dx)
    18002ed9b:	rex push %rcx
    18002ed9d:	rex.WX jae 0x18002ee0f
    18002eda0:	outsb  %ds:(%rsi),(%dx)
    18002eda1:	rex.R outsl %ds:(%rsi),(%dx)
    18002eda3:	movsxd 0x6d(%rbp),%esi
@@ -67932,15 +67926,15 @@
    18002edc3:	outsb  %ds:(%rsi),(%dx)
    18002edc4:	rex.RX outsl %ds:(%rsi),(%dx)
    18002edc6:	jb     0x18002ee35
    18002edc8:	(bad)
    18002edc9:	je     0x18002ee0b
    18002edcb:	xor    %eax,0x40(%rax)
    18002edce:	pop    %rdx
-   18002edcf:	add    %ah,0x68633f09(%rax)
+   18002edcf:	add    %ah,0x68633f09(%rcx)
    18002edd5:	imul   $0x746e6576,0x45(%rsp,%riz,2),%ebp
    18002eddd:	rex push %rcx
    18002eddf:	(bad)
    18002ede5:	rex
    18002ede6:	rex
    18002ede7:	rex.WRB
    18002ede8:	rex.RB
@@ -67952,15 +67946,15 @@
    18002edf0:	push   %rcx
    18002edf1:	rex.XB push $0x45646c69
    18002edf7:	jbe    0x18002ee5e
    18002edf9:	outsb  %ds:(%rsi),(%dx)
    18002edfa:	je     0x18002ee3c
    18002edfc:	rex
    18002edfd:	rex pop %rdx
-   18002edff:	add    %ah,0xa(%rbp)
+   18002edff:	add    %ah,0xa(%rsi)
    18002ee02:	(bad)
    18002ee03:	movsxd 0x6e(%rdi),%ebp
    18002ee06:	outsb  %ds:(%rsi),(%dx)
    18002ee07:	movsxd %gs:0x6f(%rsi,%rcx,2),%esi
    18002ee0c:	je     0x18002ee77
    18002ee0e:	data16 jns 0x18002ee51
    18002ee11:	push   %rcx
@@ -67980,15 +67974,15 @@
    18002ee28:	rex.WRB
    18002ee29:	gs je  0x18002ee94
    18002ee2c:	outsl  %ds:(%rsi),(%dx)
    18002ee2d:	fs rex
    18002ee2f:	rex
    18002ee30:	rex pop %rdx
    18002ee32:	add    %al,(%rax)
-   18002ee34:	pop    %rsi
+   18002ee34:	pop    %rdi
    18002ee35:	or     (%rdi),%edi
    18002ee37:	movsxd 0x73(%rbp),%esi
    18002ee3a:	je     0x18002eeab
    18002ee3c:	insl   (%dx),%es:(%rdi)
    18002ee3d:	rex.RB jbe 0x18002eea5
    18002ee40:	outsb  %ds:(%rsi),(%dx)
    18002ee41:	je     0x18002ee83
@@ -68005,15 +67999,15 @@
    18002ee53:	push   %r14
    18002ee55:	push   %rcx
    18002ee56:	rex.RB jbe 0x18002eebe
    18002ee59:	outsb  %ds:(%rsi),(%dx)
    18002ee5a:	je     0x18002ee9c
    18002ee5c:	rex
    18002ee5d:	rex pop %rdx
-   18002ee5f:	add    %dh,0xc(%rax)
+   18002ee5f:	add    %dh,0xc(%rcx)
    18002ee62:	(bad)
    18002ee63:	imul   $0x656e6e6f,%fs:0x63(%rbx),%esi
    18002ee6b:	movsxd 0x6f(%rsi,%rcx,2),%esi
    18002ee6f:	je     0x18002eeda
    18002ee71:	data16 jns 0x18002eeb4
    18002ee74:	push   %rcx
    18002ee75:	(bad)
@@ -68031,15 +68025,15 @@
    18002ee88:	gs je  0x18002eeec
    18002ee8b:	rex.WRB
    18002ee8c:	gs je  0x18002eef7
    18002ee8f:	outsl  %ds:(%rsi),(%dx)
    18002ee90:	fs rex
    18002ee92:	rex
    18002ee93:	rex pop %rdx
-   18002ee95:	add    %al,0xd(%rcx)
+   18002ee95:	add    %al,0xd(%rdx)
    18002ee98:	(bad)
    18002ee99:	gs jbe 0x18002ef01
    18002ee9c:	outsb  %ds:(%rsi),(%dx)
    18002ee9d:	je     0x18002eedf
    18002ee9f:	push   %rcx
    18002eea0:	(bad)
    18002eea6:	rex
@@ -68053,15 +68047,15 @@
    18002eeb2:	push   %rcx
    18002eeb3:	rex.RB jbe 0x18002ef1b
    18002eeb6:	outsb  %ds:(%rsi),(%dx)
    18002eeb7:	je     0x18002eef9
    18002eeb9:	rex
    18002eeba:	rex pop %rdx
    18002eebc:	add    %al,(%rax)
-   18002eebe:	push   %rcx
+   18002eebe:	push   %rdx
    18002eebf:	or     $0x6576653f,%eax
    18002eec4:	outsb  %ds:(%rsi),(%dx)
    18002eec5:	je     0x18002ef0d
    18002eec7:	imul   $0x4f514072,0x65(%rsp,%rsi,2),%ebp
    18002eecf:	(bad)
    18002eed4:	rex
    18002eed5:	rex push %rbp
@@ -68077,15 +68071,15 @@
    18002eee6:	push   %rcx
    18002eee7:	rex.RB jbe 0x18002ef4f
    18002eeea:	outsb  %ds:(%rsi),(%dx)
    18002eeeb:	je     0x18002ef2d
    18002eeed:	rex
    18002eeee:	rex pop %rdx
    18002eef0:	add    %al,(%rax)
-   18002eef2:	add    %cl,(%rsi)
+   18002eef2:	add    %ecx,(%rsi)
    18002eef4:	(bad)
    18002eef5:	data16 insb (%dx),%es:(%rdi)
    18002eef7:	(bad)
    18002eef8:	addr32 jae 0x18002ef41
    18002eefb:	outsl  %ds:(%rsi),(%dx)
    18002eefc:	jb     0x18002ef42
    18002eefe:	jne    0x18002ef6d
@@ -68126,15 +68120,15 @@
    18002ef4d:	jb     0x18002ef8f
    18002ef4f:	rex.R
    18002ef50:	rex xor 0x40(%rax),%al
    18002ef54:	jae    0x18002efca
    18002ef56:	fs rex
    18002ef58:	rex pop %rax
    18002ef5a:	pop    %rdx
-   18002ef5b:	add    %dh,(%rcx)
+   18002ef5b:	add    %dh,(%rdx)
    18002ef5d:	sbb    (%rdi),%edi
    18002ef5f:	je     0x18002efca
    18002ef61:	insl   (%dx),%es:(%rdi)
    18002ef62:	gs jb  0x18002efaa
    18002ef65:	jbe    0x18002efcc
    18002ef67:	outsb  %ds:(%rsi),(%dx)
    18002ef68:	je     0x18002efaa
@@ -68170,15 +68164,15 @@
    18002efa4:	rex.B
    18002efa5:	rex push %rax
    18002efa7:	rex.RB
    18002efa8:	rex.X
    18002efa9:	rex.R
    18002efaa:	rex.W xor %sil,(%rax)
    18002efad:	rex pop %rdx
-   18002efaf:	add    %dl,%al
+   18002efaf:	add    %dl,%cl
    18002efb1:	sbb    $0x7261773f,%eax
    18002efb6:	outsb  %ds:(%rsi),(%dx)
    18002efb7:	imul   $0x654d5140,0x67(%rsi),%ebp
    18002efbe:	jae    0x18002f033
    18002efc0:	(bad)
    18002efc1:	rex.WR outsl %gs:(%esi),(%dx)
    18002efc5:	addr32 addr32 gs jb 0x18002f00a
@@ -68188,15 +68182,15 @@
    18002efce:	pop    %r8
    18002efd0:	push   %rax
    18002efd1:	rex.RB
    18002efd2:	rex.X
    18002efd3:	rex.R pop %rdx
    18002efd5:	pop    %rdx
    18002efd6:	add    %al,(%rax)
-   18002efd8:	in     (%dx),%eax
+   18002efd8:	out    %al,(%dx)
    18002efd9:	adc    %edi,(%rdi)
    18002efdb:	insb   (%dx),%es:(%rdi)
    18002efdc:	outsb  %gs:(%rsi),(%dx)
    18002efde:	addr32 je 0x18002f049
    18002efe1:	rex.W
    18002efe2:	gs insb (%dx),%es:(%rdi)
    18002efe4:	jo     0x18002f04b
@@ -68231,15 +68225,15 @@
    18002f023:	rex push %rax
    18002f025:	rex.RB
    18002f026:	rex.X
    18002f027:	rex.R pop %rdi
    18002f029:	rex.WX
    18002f02a:	rex pop %rdx
    18002f02c:	add    %al,(%rax)
-   18002f02e:	push   %rsp
+   18002f02e:	push   %rbp
    18002f02f:	or     %bh,(%rdi)
    18002f031:	(bad)
    18002f032:	jb     0x18002f09b
    18002f034:	rex push %rcx
    18002f036:	push   %rbx
    18002f037:	je     0x18002f0ab
    18002f039:	imul   $0x45514040,0x67(%rsi),%ebp
@@ -68251,15 +68245,15 @@
    18002f049:	rex.X push %rsi
    18002f04b:	xor    %eax,0x48(%rax)
    18002f04e:	push   %rsi
    18002f04f:	push   %rcx
    18002f050:	rex.XB push $0x40407261
    18002f056:	rex pop %rdx
    18002f058:	add    %al,(%rax)
-   18002f05a:	insl   (%dx),%es:(%rdi)
+   18002f05a:	outsb  %ds:(%rsi),(%dx)
    18002f05b:	sbb    $0x3f,%al
    18002f05d:	je     0x18002f0ce
    18002f05f:	push   %rbp
    18002f060:	je     0x18002f0c8
    18002f062:	cmp    %al,0x51(%rax)
    18002f065:	push   %rbx
    18002f066:	je     0x18002f0da
@@ -68271,15 +68265,15 @@
    18002f075:	push   %rcx
    18002f076:	rex.X jns 0x18002f0ed
    18002f079:	gs rex.B jb 0x18002f0ef
    18002f07d:	(bad)
    18002f07e:	jns    0x18002f0c0
    18002f080:	rex pop %rax
    18002f082:	pop    %rdx
-   18002f083:	add    %dh,0xe(%rax)
+   18002f083:	add    %dh,0xe(%rcx)
    18002f086:	(bad)
    18002f087:	data16 jb 0x18002f0f9
    18002f08a:	insl   (%dx),%es:(%rdi)
    18002f08b:	push   %rbp
    18002f08c:	je     0x18002f0f4
    18002f08e:	cmp    %al,0x51(%rax)
    18002f091:	push   %rbx
@@ -68290,15 +68284,15 @@
    18002f09e:	xor    %eax,0x56(%rax)
    18002f0a1:	push   %rcx
    18002f0a2:	rex.X jns 0x18002f119
    18002f0a5:	gs rex.B jb 0x18002f11b
    18002f0a9:	(bad)
    18002f0aa:	jns    0x18002f102
    18002f0ac:	imul   $0x5a404040,0x77(%rbp),%esp
-   18002f0b3:	add    %bh,0x13(%rbp)
+   18002f0b3:	add    %bh,0x13(%rsi)
    18002f0b6:	(bad)
    18002f0b7:	outsb  %ds:(%rsi),(%dx)
    18002f0b8:	outsl  %ds:(%rsi),(%dx)
    18002f0b9:	jb     0x18002f128
    18002f0bb:	(bad)
    18002f0bc:	insb   (%dx),%es:(%rdi)
    18002f0bd:	imul   $0x70795464,0x65(%rdx),%edi
@@ -68317,15 +68311,15 @@
    18002f0e1:	jns    0x18002f123
    18002f0e3:	rex push %rax
    18002f0e5:	rex.RB
    18002f0e6:	rex.X
    18002f0e7:	rex.R
    18002f0e8:	rex pop %rdx
    18002f0ea:	add    %al,(%rax)
-   18002f0ec:	loopne 0x18002f0f0
+   18002f0ec:	loope  0x18002f0f0
    18002f0ee:	(bad)
    18002f0ef:	(bad)
    18002f0f0:	xor    %eax,0x6f(%rbx)
    18002f0f3:	outsb  %ds:(%rsi),(%dx)
    18002f0f4:	outsb  %ds:(%rsi),(%dx)
    18002f0f5:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    18002f0fa:	outsb  %ds:(%rsi),(%dx)
@@ -68338,16 +68332,15 @@
    18002f10a:	rex.RB
    18002f10b:	rex.B
    18002f10c:	rex.B
    18002f10d:	rex pop %rax
    18002f10f:	pop    %rdx
    18002f110:	add    %al,(%rax)
    18002f112:	(bad)
-   18002f113:	or     (%rdi),%bh
-   18002f115:	movsxd 0x6e(%rdi),%ebp
+   18002f117:	outsb  %ds:(%rsi),(%dx)
    18002f118:	outsb  %ds:(%rsi),(%dx)
    18002f119:	movsxd %gs:0x6d(%rcx,%rcx,2),%esi
    18002f11e:	jo     0x18002f18c
    18002f120:	rex push %rcx
    18002f122:	(bad)
    18002f128:	rex
    18002f129:	rex
@@ -68450,15 +68443,15 @@
    18002f1e1:	rex.B
    18002f1e2:	rex and $0x24,%al
    18002f1e5:	push   %rcx
    18002f1e6:	rex.RB
    18002f1e7:	push   %r14
    18002f1e9:	xor    %al,0x40(%rax)
    18002f1ec:	pop    %rdx
-   18002f1ed:	add    %ch,%dh
+   18002f1ed:	add    %ch,%bh
    18002f1ef:	add    (%rdi),%edi
    18002f1f1:	(bad)
    18002f1f2:	xor    $0x51,%al
    18002f1f4:	rex.R (bad)
    18002f1f6:	je     0x18002f25d
    18002f1f8:	push   %rsp
    18002f1f9:	imul   $0x45514040,0x65(%rbp),%ebp
@@ -68470,15 +68463,15 @@
    18002f206:	xor    %al,0x24(%rax)
    18002f209:	and    $0x51,%al
    18002f20b:	rex.RB
    18002f20c:	push   %r14
    18002f20e:	xor    %al,0x40(%rax)
    18002f211:	pop    %rdx
    18002f212:	add    %al,(%rax)
-   18002f214:	adc    %cl,0x7571653f(%rip)        # 0x1f5745759
+   18002f214:	adc    %ecx,0x7571653f(%rip)        # 0x1f5745759
    18002f21a:	(bad)
    18002f21b:	insb   (%dx),%es:(%rdi)
    18002f21c:	jae    0x18002f25e
    18002f21e:	push   %rcx
    18002f21f:	rex.R (bad)
    18002f221:	je     0x18002f288
    18002f223:	push   %rsp
@@ -68487,17 +68480,15 @@
    18002f22c:	pop    %r15
    18002f22e:	rex.WRX
    18002f22f:	rex.B
    18002f230:	rex.RB
    18002f231:	rex.X push %rsi
    18002f233:	xor    %eax,0x40(%rax)
    18002f236:	pop    %rdx
-   18002f237:	add    %ch,(%rsp,%rdx,1)
-   18002f23a:	(bad)
-   18002f23b:	jo     0x18002f2af
+   18002f237:	add    %ch,0x72703f14(%rip)        # 0x1f2733151
    18002f23d:	movsxd %gs:0x64(%rbp),%esp
    18002f241:	gs jae 0x18002f284
    18002f244:	push   %rcx
    18002f245:	rex.R (bad)
    18002f247:	je     0x18002f2ae
    18002f249:	push   %rsp
    18002f24a:	imul   $0x45414040,0x65(%rbp),%ebp
@@ -68505,15 +68496,15 @@
    18002f252:	pop    %r15
    18002f254:	rex.WRX
    18002f255:	rex.B
    18002f256:	rex.RB
    18002f257:	rex.X push %rsi
    18002f259:	xor    %eax,0x40(%rax)
    18002f25c:	pop    %rdx
-   18002f25d:	add    %bl,(%rdi)
+   18002f25d:	add    %ah,(%rax)
    18002f25f:	add    $0x40363f3f,%eax
    18002f264:	pop    %rcx
    18002f265:	rex.B
    18002f266:	rex.B
    18002f267:	rex.RB
    18002f268:	push   %r14
    18002f26a:	push   %rcx
@@ -68533,15 +68524,15 @@
    18002f27f:	rex.X push %rsi
    18002f281:	push   %rcx
    18002f282:	rex.R (bad)
    18002f284:	je     0x18002f2eb
    18002f286:	push   %rsp
    18002f287:	imul   $0x5a404040,0x65(%rbp),%ebp
    18002f28e:	add    %al,(%rax)
-   18002f290:	stos   %eax,%es:(%rdi)
+   18002f290:	lods   %ds:(%rsi),%al
    18002f291:	add    $0x3f,%al
    18002f293:	(bad)
    18002f294:	xor    $0x41415940,%eax
    18002f299:	rex.RB
    18002f29a:	push   %r14
    18002f29c:	push   %rcx
    18002f29d:	rex.R (bad)
@@ -68560,15 +68551,15 @@
    18002f2b1:	push   %r14
    18002f2b3:	push   %rcx
    18002f2b4:	rex.R (bad)
    18002f2b6:	je     0x18002f31d
    18002f2b8:	push   %rsp
    18002f2b9:	imul   $0x5a404040,0x65(%rbp),%ebp
    18002f2c0:	add    %al,(%rax)
-   18002f2c2:	out    %al,(%dx)
+   18002f2c2:	out    %eax,(%dx)
    18002f2c3:	add    $0x3f,%al
    18002f2c5:	(bad)
    18002f2c6:	ss rex pop %rcx
    18002f2c9:	rex.B (bad)
    18002f2cb:	push   %r14
    18002f2cd:	push   %rcx
    18002f2ce:	rex.R
@@ -68621,15 +68612,15 @@
    18002f330:	push   %rbp
    18002f331:	jb     0x18002f39f
    18002f333:	rex
    18002f334:	rex
    18002f335:	rex
    18002f336:	rex
    18002f337:	rex pop %rdx
-   18002f339:	add    %dh,0x11(%rsi)
+   18002f339:	add    %dh,0x11(%rdi)
    18002f33c:	(bad)
    18002f33d:	imul   $0x696e7261,0x57(%rbx),%esi
    18002f344:	outsb  %ds:(%rsi),(%dx)
    18002f345:	rex.RB outsb %ds:(%esi),(%dx)
    18002f348:	(bad)
    18002f349:	(bad)  {%k4}
    18002f34c:	fs rex push %rcx
@@ -68641,15 +68632,15 @@
    18002f35f:	rex push %rcx
    18002f361:	rex.RB
    18002f362:	rex.X
    18002f363:	pop    %r15
    18002f365:	rex.WRX pop %rax
    18002f367:	pop    %rdx
    18002f368:	add    %al,(%rax)
-   18002f36a:	pop    %rsi
+   18002f36a:	pop    %rdi
    18002f36b:	add    (%rdi),%bh
    18002f36d:	(bad)
    18002f36e:	xor    %dl,0x55(%rcx)
    18002f371:	jb     0x18002f3df
    18002f373:	push   %rcx
    18002f374:	jne    0x18002f3db
    18002f376:	jb     0x18002f3f1
@@ -68691,17 +68682,15 @@
    18002f3c4:	rex.B
    18002f3c5:	rex push %rax
    18002f3c7:	rex.RB
    18002f3c8:	rex.X
    18002f3c9:	rex.R
    18002f3ca:	rex.W xor %al,0x5a(%rax)
    18002f3ce:	add    %al,(%rax)
-   18002f3d0:	(bad)
-   18002f3d1:	or     $0x7461663f,%eax
-   18002f3d6:	(bad)
+   18002f3d0:	orl    $0x61,0x7461663f(%rip)        # 0x1f4645a16
    18002f3d7:	insb   (%dx),%es:(%rdi)
    18002f3d8:	rex push %rcx
    18002f3da:	rex.WRB
    18002f3db:	gs jae 0x18002f451
    18002f3de:	(bad)
    18002f3df:	rex.WR outsl %gs:(%esi),(%dx)
    18002f3e3:	addr32 addr32 gs jb 0x18002f428
@@ -68711,15 +68700,18 @@
    18002f3ec:	pop    %r8
    18002f3ee:	push   %rax
    18002f3ef:	rex.RB
    18002f3f0:	rex.X
    18002f3f1:	rex.R pop %rdx
    18002f3f3:	pop    %rdx
    18002f3f4:	add    %al,(%rax)
-   18002f3f6:	or     $0x6c613f08,%eax
+   18002f3f6:	(bad)
+   18002f3f7:	or     %bh,(%rdi)
+   18002f3f9:	(bad)
+   18002f3fa:	insb   (%dx),%es:(%rdi)
    18002f3fb:	insb   (%dx),%es:(%rdi)
    18002f3fc:	outsl  %ds:(%rsi),(%dx)
    18002f3fd:	movsxd 0x74(%rcx),%esp
    18002f400:	gs rex push %rcx
    18002f403:	rex.B jb 0x18002f478
    18002f406:	(bad)
    18002f407:	jns    0x18002f44d
@@ -68800,15 +68792,16 @@
    18002f495:	outsl  %ds:(%rsi),(%dx)
    18002f496:	movsxd 0x74(%rcx),%esp
    18002f499:	imul   $0x6974704f,0x6e(%rdi),%ebp
    18002f4a0:	outsl  %ds:(%rsi),(%dx)
    18002f4a1:	outsb  %ds:(%rsi),(%dx)
    18002f4a2:	rex xor %eax,0x40(%rax)
    18002f4a6:	pop    %rdx
-   18002f4a7:	add    %dh,0x3f(%rdx,%rcx,1)
+   18002f4a7:	add    %dh,0xa(%rbp)
+   18002f4aa:	(bad)
    18002f4ab:	movsxd 0x6e(%rdi),%ebp
    18002f4ae:	jae    0x18002f524
    18002f4b0:	rex.R (bad)
    18002f4b2:	je     0x18002f515
    18002f4b4:	rex push %rcx
    18002f4b6:	rex.X jns 0x18002f52d
    18002f4b9:	gs rex.B jb 0x18002f52f
@@ -68818,15 +68811,15 @@
    18002f4c2:	rex.RB
    18002f4c3:	rex.X
    18002f4c4:	push   %r8
    18002f4c6:	rex.RB
    18002f4c7:	rex.X
    18002f4c8:	rex.R pop %rax
    18002f4ca:	pop    %rdx
-   18002f4cb:	add    %al,0x1b(%rbp)
+   18002f4cb:	add    %al,0x1b(%rsi)
    18002f4ce:	(bad)
    18002f4cf:	je     0x18002f540
    18002f4d1:	rex.X (bad)
    18002f4d3:	jae    0x18002f53a
    18002f4d5:	ss xor $0x40,%al
    18002f4d8:	push   %rcx
    18002f4d9:	rex.X jns 0x18002f550
@@ -68856,15 +68849,15 @@
    18002f50e:	(bad)
    18002f50f:	jns    0x18002f551
    18002f511:	rex
    18002f512:	rex
    18002f513:	rex
    18002f514:	rex pop %rdx
    18002f516:	add    %al,(%rax)
-   18002f518:	jne    0x18002f523
+   18002f518:	jbe    0x18002f523
    18002f51a:	(bad)
    18002f51b:	movsxd 0x73(%rcx),%esp
    18002f51e:	je     0x18002f560
    18002f520:	push   %rcx
    18002f521:	rex.WRB
    18002f522:	gs je  0x18002f586
    18002f525:	(bad)
@@ -68898,15 +68891,15 @@
    18002f564:	rex push %rcx
    18002f566:	rex.RB
    18002f567:	rex.B
    18002f568:	rex.B
    18002f569:	rex pop %rax
    18002f56b:	pop    %rdx
    18002f56c:	add    %al,(%rax)
-   18002f56e:	mov    $0x3,%bl
+   18002f56e:	mov    $0x3,%ah
    18002f570:	(bad)
    18002f571:	(bad)
    18002f572:	xor    $0x43,%al
    18002f574:	outsl  %ds:(%rsi),(%dx)
    18002f575:	outsb  %ds:(%rsi),(%dx)
    18002f576:	outsb  %ds:(%rsi),(%dx)
    18002f577:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
@@ -68958,15 +68951,15 @@
    18002f5d2:	imul   $0x45514040,0x67(%rsi),%ebp
    18002f5d9:	rex.B
    18002f5da:	pop    %r8
    18002f5dc:	pop    %rdi
    18002f5dd:	rex.WX
    18002f5de:	rex pop %rdx
    18002f5e0:	add    %al,(%rax)
-   18002f5e2:	pop    %rsi
+   18002f5e2:	pop    %rdi
    18002f5e3:	or     %edi,(%rdi)
    18002f5e5:	movsxd 0x70(%rcx),%esp
    18002f5e8:	(bad)
    18002f5e9:	movsxd 0x74(%rcx),%ebp
    18002f5ec:	jns    0x18002f62e
    18002f5ee:	push   %rcx
    18002f5ef:	push   %rbx
@@ -68987,15 +68980,15 @@
    18002f60d:	je     0x18002f681
    18002f60f:	imul   $0x45514040,0x67(%rsi),%ebp
    18002f616:	rex.B
    18002f617:	pop    %r8
    18002f619:	pop    %rdi
    18002f61a:	rex.WX
    18002f61b:	rex pop %rdx
-   18002f61d:	add    %bl,%bl
+   18002f61d:	add    %bl,%ah
    18002f61f:	or     (%rdi),%edi
    18002f621:	fs (bad)
    18002f623:	je     0x18002f686
    18002f625:	rex push %rcx
    18002f627:	push   %rbx
    18002f628:	je     0x18002f69c
    18002f62a:	imul   $0x45514040,0x67(%rsi),%ebp
@@ -69004,15 +68997,15 @@
    18002f634:	rex.RB
    18002f635:	push   %r14
    18002f637:	push   %rcx
    18002f638:	rex.XB push $0x40407261
    18002f63e:	pop    %rax
    18002f63f:	pop    %rdx
    18002f640:	add    %al,(%rax)
-   18002f642:	ja     0x18002f64e
+   18002f642:	js     0x18002f64e
    18002f644:	(bad)
    18002f645:	movsxd 0x6e(%rdi),%ebp
    18002f648:	jae    0x18002f6be
    18002f64a:	rex.R (bad)
    18002f64c:	je     0x18002f6af
    18002f64e:	rex push %rcx
    18002f650:	push   %rbx
@@ -69022,39 +69015,40 @@
    18002f65b:	push   %r8
    18002f65d:	rex.RB
    18002f65e:	rex.X push %rsi
    18002f660:	push   %rcx
    18002f661:	rex.XB push $0x40407261
    18002f667:	pop    %rax
    18002f668:	pop    %rdx
-   18002f669:	add    %cl,0xc(%rcx)
+   18002f669:	add    %cl,0xc(%rdx)
    18002f66c:	(bad)
    18002f66d:	fs gs je 0x18002f6d2
    18002f671:	movsxd 0x40(%rax),%ebp
    18002f674:	push   %rcx
    18002f675:	push   %rbx
    18002f676:	je     0x18002f6ea
    18002f678:	imul   $0x45514040,0x67(%rsi),%ebp
    18002f67f:	rex.B
    18002f680:	pop    %r8
    18002f682:	pop    %rax
    18002f683:	pop    %rdx
    18002f684:	add    %al,(%rax)
    18002f686:	(bad)
+   18002f687:	or     %edi,(%rdi)
    18002f689:	movsxd 0x61(%rbp,%riz,2),%ebp
    18002f68d:	jb     0x18002f6cf
    18002f68f:	push   %rcx
    18002f690:	push   %rbx
    18002f691:	je     0x18002f705
    18002f693:	imul   $0x45514040,0x67(%rsi),%ebp
    18002f69a:	rex.B
    18002f69b:	pop    %r8
    18002f69d:	pop    %rax
    18002f69e:	pop    %rdx
-   18002f69f:	add    %bh,(%rcx)
+   18002f69f:	add    %bh,(%rdx)
    18002f6a1:	sbb    (%rdi),%bh
    18002f6a3:	jae    0x18002f719
    18002f6a5:	(bad)
    18002f6a6:	jb     0x18002f71c
    18002f6a8:	jae    0x18002f701
    18002f6aa:	imul   $0x72745351,0x40(%rax,%rbp,2),%esi
    18002f6b2:	imul   $0x45514040,0x67(%rsi),%ebp
@@ -69074,15 +69068,15 @@
    18002f6ce:	je     0x18002f739
    18002f6d0:	jbe    0x18002f73b
    18002f6d2:	je     0x18002f74d
    18002f6d4:	rex push %rcx
    18002f6d6:	je     0x18002f718
    18002f6d8:	rex
    18002f6d9:	rex pop %rdx
-   18002f6db:	add    %al,0x8(%rax)
+   18002f6db:	add    %al,0x8(%rcx)
    18002f6de:	(bad)
    18002f6df:	(bad)
    18002f6e0:	jo     0x18002f752
    18002f6e2:	outsb  %gs:(%rsi),(%dx)
    18002f6e4:	fs rex push %rcx
    18002f6e7:	push   %rbx
    18002f6e8:	je     0x18002f75c
@@ -69099,15 +69093,15 @@
    18002f6ff:	outsb  %ds:(%rsi),(%dx)
    18002f700:	xor    %edx,0x74(%rbx)
    18002f703:	jb     0x18002f76e
    18002f705:	outsb  %ds:(%rsi),(%dx)
    18002f706:	addr32 rex
    18002f708:	rex
    18002f709:	rex pop %rdx
-   18002f70b:	add    %bh,0x6f743f1b(%rcx)
+   18002f70b:	add    %bh,0x6f743f1b(%rdx)
    18002f711:	rex.WR outsl %ds:(%rsi),(%dx)
    18002f713:	movsxd 0x6c(%rcx),%esp
    18002f716:	cmp    %al,0x69(%rdx)
    18002f719:	je     0x18002f75b
    18002f71b:	push   %rcx
    18002f71c:	push   %rbx
    18002f71d:	je     0x18002f791
@@ -69120,30 +69114,26 @@
    18002f72d:	rex.X jns 0x18002f7a4
    18002f730:	gs rex.B jb 0x18002f7a6
    18002f734:	(bad)
    18002f735:	jns    0x18002f777
    18002f737:	rex pop %rax
    18002f739:	pop    %rdx
    18002f73a:	add    %al,(%rax)
-   18002f73c:	lahf
-   18002f73d:	adc    (%rdi),%edi
-   18002f73f:	outsb  %ds:(%rsi),(%dx)
-   18002f740:	jne    0x18002f7af
-   18002f742:	vsqrtsh 0xe8(%rbx),%xmm17,%xmm26
-   18002f749:	jb     0x18002f7b4
-   18002f74b:	outsb  %ds:(%rsi),(%dx)
-   18002f74c:	addr32 rex
-   18002f74e:	rex push %rbx
-   18002f750:	rex.B (bad)
+   18002f73c:	movabs 0x7265626d756e3f13,%al
+   18002f745:	rex push %rcx
+   18002f747:	push   %rbx
+   18002f748:	je     0x18002f7bc
+   18002f74a:	imul   $0x41534040,0x67(%rsi),%ebp
+   18002f751:	(bad)
    18002f752:	push   %r14
    18002f754:	xor    %eax,0x5f(%rax)
    18002f757:	rex.WX
    18002f758:	rex.W
    18002f759:	rex pop %rdx
-   18002f75b:	add    %al,0x8(%rsi)
+   18002f75b:	add    %al,0x8(%rdi)
    18002f75e:	(bad)
    18002f75f:	(bad)
    18002f760:	jo     0x18002f7d2
    18002f762:	outsb  %gs:(%rsi),(%dx)
    18002f764:	fs rex.WR (bad)
    18002f767:	je     0x18002f7d2
    18002f769:	outsb  %ds:(%rsi),(%dx)
@@ -69171,28 +69161,28 @@
    18002f795:	addr32 rex
    18002f797:	rex push %rax
    18002f799:	rex.RB
    18002f79a:	push   %r14
    18002f79c:	push   %rcx
    18002f79d:	rex.XB push $0x40407261
    18002f7a3:	rex pop %rdx
-   18002f7a5:	add    %dh,(%rcx)
+   18002f7a5:	add    %dh,(%rdx)
    18002f7a7:	adc    %bh,(%rdi)
    18002f7a9:	imul   $0x7974706d,0x45(%rbx),%esi
    18002f7b0:	rex push %rcx
    18002f7b2:	push   %rbp
    18002f7b3:	jb     0x18002f821
    18002f7b5:	rex
    18002f7b6:	rex push %rcx
    18002f7b8:	rex.RB
    18002f7b9:	rex.X
    18002f7ba:	pop    %r15
    18002f7bc:	rex.WRX pop %rax
    18002f7be:	pop    %rdx
-   18002f7bf:	add    %ah,%dh
+   18002f7bf:	add    %ah,%bh
    18002f7c1:	sbb    (%rdi),%edi
    18002f7c3:	je     0x18002f834
    18002f7c5:	push   %rax
    18002f7c6:	gs jb  0x18002f82c
    18002f7c9:	outsb  %gs:(%rsi),(%dx)
    18002f7cb:	je     0x18002f812
    18002f7cd:	outsb  %ds:(%rsi),(%dx)
@@ -69216,16 +69206,15 @@
    18002f7f1:	push   %rbx
    18002f7f2:	je     0x18002f866
    18002f7f4:	imul   $0x45414040,0x67(%rsi),%ebp
    18002f7fb:	rex.X push %rsi
    18002f7fd:	xor    0x31(%rax),%al
    18002f800:	rex pop %rdx
    18002f802:	add    %al,(%rax)
-   18002f804:	push   $0x69643f0c
-   18002f809:	jae    0x18002f86e
+   18002f804:	imul   $0x63736964,(%rdi,%rdi,1),%ecx
    18002f80b:	outsl  %ds:(%rsi),(%dx)
    18002f80c:	outsb  %ds:(%rsi),(%dx)
    18002f80d:	outsb  %ds:(%rsi),(%dx)
    18002f80e:	movsxd %gs:0x51(%rax,%rax,2),%esi
    18002f813:	(bad)
    18002f819:	rex
    18002f81a:	rex push %rbx
@@ -69242,30 +69231,31 @@
    18002f82d:	rex push %rcx
    18002f82f:	rex.WRB
    18002f830:	gs je  0x18002f894
    18002f833:	(bad)
    18002f839:	rex
    18002f83a:	rex
    18002f83b:	rex pop %rdx
-   18002f83d:	add    %ch,0x65643f0c(%rip)        # 0x1e567374f
-   18002f843:	insb   (%dx),%es:(%rdi)
+   18002f83d:	add    %ch,(%rsi)
+   18002f83f:	or     $0x3f,%al
+   18002f841:	fs gs insb (%dx),%es:(%rdi)
    18002f844:	gs je  0x18002f8ac
    18002f847:	rex.WR (bad)
    18002f849:	je     0x18002f8b0
    18002f84b:	jb     0x18002f88d
    18002f84d:	push   %rcx
    18002f84e:	(bad)
    18002f854:	rex
    18002f855:	rex push %rcx
    18002f857:	rex.RB
    18002f858:	rex.B
    18002f859:	pop    %r8
    18002f85b:	pop    %rax
    18002f85c:	pop    %rdx
-   18002f85d:	add    %ah,0x303f3f02(%rax)
+   18002f85d:	add    %ah,0x303f3f02(%rcx)
    18002f863:	push   %rcx
    18002f864:	push   %rsi
    18002f865:	(bad)
    18002f866:	jb     0x18002f8d1
    18002f868:	(bad)
    18002f869:	outsb  %ds:(%rsi),(%dx)
    18002f86a:	je     0x18002f8ac
@@ -69273,15 +69263,15 @@
    18002f86e:	rex.RB
    18002f86f:	rex.B
    18002f870:	rex.B
    18002f871:	rex pop %rdi
    18002f873:	rex.WRX
    18002f874:	rex pop %rdx
    18002f876:	add    %al,(%rax)
-   18002f878:	jae    0x18002f87c
+   18002f878:	je     0x18002f87c
    18002f87a:	(bad)
    18002f87b:	(bad)
    18002f87c:	xor    %dl,0x56(%rcx)
    18002f87f:	(bad)
    18002f880:	jb     0x18002f8eb
    18002f882:	(bad)
    18002f883:	outsb  %ds:(%rsi),(%dx)
@@ -69298,15 +69288,15 @@
    18002f891:	rex.X jns 0x18002f908
    18002f894:	gs rex.B jb 0x18002f90a
    18002f898:	(bad)
    18002f899:	jns    0x18002f8db
    18002f89b:	rex
    18002f89c:	rex pop %rdx
    18002f89e:	add    %al,(%rax)
-   18002f8a0:	insb   (%dx),%es:(%rdi)
+   18002f8a0:	insl   (%dx),%es:(%rdi)
    18002f8a1:	add    (%rdi),%bh
    18002f8a3:	(bad)
    18002f8a4:	xor    %dl,0x56(%rcx)
    18002f8a7:	(bad)
    18002f8a8:	jb     0x18002f913
    18002f8aa:	(bad)
    18002f8ab:	outsb  %ds:(%rsi),(%dx)
@@ -69318,15 +69308,15 @@
    18002f8b3:	rex and $0x24,%al
    18002f8b6:	push   %rcx
    18002f8b7:	rex.RB
    18002f8b8:	push   %r14
    18002f8ba:	xor    %al,0x40(%rax)
    18002f8bd:	pop    %rdx
    18002f8be:	add    %al,(%rax)
-   18002f8c0:	sbb    (%rdi),%r15
+   18002f8c0:	sbb    (%r15),%r15
    18002f8c3:	je     0x18002f934
    18002f8c5:	rex.X outsl %ds:(%rsi),(%dx)
    18002f8c7:	outsl  %ds:(%rsi),(%dx)
    18002f8c8:	insb   (%dx),%es:(%rdi)
    18002f8c9:	rex push %rcx
    18002f8cb:	push   %rsi
    18002f8cc:	(bad)
@@ -69337,15 +69327,15 @@
    18002f8d3:	rex push %rcx
    18002f8d5:	rex.RB
    18002f8d6:	rex.X
    18002f8d7:	pop    %r15
    18002f8d9:	rex.WRX pop %rax
    18002f8db:	pop    %rdx
    18002f8dc:	add    %al,(%rax)
-   18002f8de:	push   %rcx
+   18002f8de:	push   %rdx
    18002f8df:	sbb    (%rdi),%edi
    18002f8e1:	je     0x18002f952
    18002f8e3:	rex.X jns 0x18002f95a
    18002f8e6:	gs rex.B jb 0x18002f95c
    18002f8ea:	(bad)
    18002f8eb:	jns    0x18002f92d
    18002f8ed:	push   %rcx
@@ -69364,31 +69354,31 @@
    18002f8ff:	rex.X jns 0x18002f976
    18002f902:	gs rex.B jb 0x18002f978
    18002f906:	(bad)
    18002f907:	jns    0x18002f949
    18002f909:	rex pop %rax
    18002f90b:	pop    %rdx
    18002f90c:	add    %al,(%rax)
-   18002f90e:	cmc
-   18002f90f:	sbb    (%rdi),%edi
+   18002f90e:	negb   (%rbx)
+   18002f910:	(bad)
    18002f911:	je     0x18002f982
    18002f913:	push   %rbx
    18002f914:	movsxd %gs:0x53(%rbx),%esi
    18002f918:	imul   $0x6f704565,0x63(%rsi),%ebp
    18002f91f:	movsxd 0x40(%rax),%ebp
    18002f922:	push   %rcx
    18002f923:	rex.R (bad)
    18002f925:	je     0x18002f98c
    18002f927:	push   %rsp
    18002f928:	imul   $0x45514040,0x65(%rbp),%ebp
    18002f92f:	rex.X
    18002f930:	pop    %r15
    18002f932:	rex.WX pop %rax
    18002f934:	pop    %rdx
-   18002f935:	add    %al,0xb(%rcx)
+   18002f935:	add    %al,0xb(%rdx)
    18002f938:	(bad)
    18002f939:	movsxd 0x72(%rbp),%esi
    18002f93c:	jb     0x18002f9a3
    18002f93e:	outsb  %ds:(%rsi),(%dx)
    18002f93f:	je     0x18002f985
    18002f941:	(bad)
    18002f942:	je     0x18002f9a9
@@ -69400,15 +69390,15 @@
    18002f951:	push   %rsp
    18002f952:	imul   $0x41534040,0x65(%rbp),%ebp
    18002f959:	(bad)
    18002f95a:	push   %r14
    18002f95c:	xor    %eax,0x58(%rax)
    18002f95f:	pop    %rdx
    18002f960:	add    %al,(%rax)
-   18002f962:	test   %cl,(%rsi)
+   18002f962:	test   %ecx,(%rsi)
    18002f964:	(bad)
    18002f965:	addr32 gs je 0x18002f9a9
    18002f969:	push   %rcx
    18002f96a:	(bad)
    18002f970:	push   %rax
    18002f971:	jb     0x18002f9dc
    18002f973:	jbe    0x18002f9d6
@@ -69485,16 +69475,16 @@
    18002f9fe:	push   %rbp
    18002f9ff:	jb     0x18002fa6d
    18002fa01:	rex
    18002fa02:	rex
    18002fa03:	rex
    18002fa04:	rex
    18002fa05:	rex pop %rdx
-   18002fa07:	add    %dh,(%rbx)
-   18002fa09:	or     (%rdi),%edi
+   18002fa07:	add    %dh,(%rbx,%rcx,1)
+   18002fa0a:	(bad)
    18002fa0b:	movsxd 0x69(%rdx),%esi
    18002fa0e:	je     0x18002fa79
    18002fa10:	movsxd 0x6c(%rcx),%esp
    18002fa13:	rex push %rcx
    18002fa15:	rex.WRB
    18002fa16:	gs jae 0x18002fa8c
    18002fa19:	(bad)
@@ -69529,15 +69519,15 @@
    18002fa54:	je     0x18002fabf
    18002fa56:	outsl  %ds:(%rsi),(%dx)
    18002fa57:	outsb  %ds:(%rsi),(%dx)
    18002fa58:	rex push %rcx
    18002fa5a:	je     0x18002fa9c
    18002fa5c:	rex
    18002fa5d:	rex pop %rdx
-   18002fa5f:	add    %cl,%ch
+   18002fa5f:	add    %cl,%dh
    18002fa61:	add    (%rdi),%edi
    18002fa63:	(bad)
    18002fa64:	xor    $0x51,%al
    18002fa66:	rex.X jns 0x18002fadd
    18002fa69:	gs rex.B jb 0x18002fadf
    18002fa6d:	(bad)
    18002fa6e:	jns    0x18002fab0
@@ -69549,15 +69539,15 @@
    18002fa76:	rex.RB
    18002fa77:	push   %r14
    18002fa79:	xor    %al,0x41(%rax)
    18002fa7c:	rex.RB
    18002fa7d:	rex.X push %rsi
    18002fa7f:	xor    %al,0x40(%rax)
    18002fa82:	pop    %rdx
-   18002fa83:	add    %ah,(%rax)
+   18002fa83:	add    %ah,(%rcx)
    18002fa85:	adc    %bh,(%rdi)
    18002fa87:	imul   $0x7974706d,0x45(%rbx),%esi
    18002fa8e:	rex push %rcx
    18002fa90:	rex.X jns 0x18002fb07
    18002fa93:	gs rex.B jb 0x18002fb09
    18002fa97:	(bad)
    18002fa98:	jns    0x18002fada
@@ -69581,15 +69571,15 @@
    18002fab9:	rex push %rcx
    18002fabb:	rex.RB
    18002fabc:	rex.B
    18002fabd:	pop    %r8
    18002fabf:	pop    %rdi
    18002fac0:	rex.WX
    18002fac1:	rex pop %rdx
-   18002fac3:	add    %bl,0x9(%rbp)
+   18002fac3:	add    %bl,0x9(%rsi)
    18002fac6:	(bad)
    18002fac7:	movsxd 0x70(%rcx),%esp
    18002faca:	(bad)
    18002facb:	movsxd 0x74(%rcx),%ebp
    18002face:	jns    0x18002fb10
    18002fad0:	push   %rcx
    18002fad1:	rex.X jns 0x18002fb48
@@ -69599,16 +69589,16 @@
    18002fadb:	rex push %rcx
    18002fadd:	rex.RB
    18002fade:	rex.X
    18002fadf:	pop    %r15
    18002fae1:	rex.WX pop %rax
    18002fae3:	pop    %rdx
    18002fae4:	add    %al,(%rax)
-   18002fae6:	iret
-   18002fae7:	or     (%rdi),%edi
+   18002fae6:	rorb   $1,(%rbx)
+   18002fae8:	(bad)
    18002fae9:	fs (bad)
    18002faeb:	je     0x18002fb4e
    18002faed:	rex push %rcx
    18002faef:	rex.X jns 0x18002fb66
    18002faf2:	gs rex.B jb 0x18002fb68
    18002faf6:	(bad)
    18002faf7:	jns    0x18002fb39
@@ -69617,31 +69607,33 @@
    18002fafc:	rex.B
    18002fafd:	push   %r8
    18002faff:	rex.RB
    18002fb00:	rex.B
    18002fb01:	rex.R pop %rax
    18002fb03:	pop    %rdx
    18002fb04:	add    %al,(%rax)
-   18002fb06:	rex or $0x3f,%al
+   18002fb06:	rex.B or $0x3f,%al
    18002fb09:	fs gs je 0x18002fb6e
    18002fb0d:	movsxd 0x40(%rax),%ebp
    18002fb10:	push   %rcx
    18002fb11:	rex.X jns 0x18002fb88
    18002fb14:	gs rex.B jb 0x18002fb8a
    18002fb18:	(bad)
    18002fb19:	jns    0x18002fb5b
    18002fb1b:	rex push %rcx
    18002fb1d:	rex.RB
    18002fb1e:	rex.B
    18002fb1f:	pop    %r8
    18002fb21:	pop    %rax
    18002fb22:	pop    %rdx
-   18002fb23:	add    %bl,0x70613f08(%rip)        # 0x1f0643a31
-   18002fb29:	jo     0x18002fb90
-   18002fb2b:	outsb  %ds:(%rsi),(%dx)
+   18002fb23:	add    %bl,(%rsi)
+   18002fb25:	or     %bh,(%rdi)
+   18002fb27:	(bad)
+   18002fb28:	jo     0x18002fb9a
+   18002fb2a:	outsb  %gs:(%rsi),(%dx)
    18002fb2c:	fs rex push %rcx
    18002fb2f:	rex.X jns 0x18002fba6
    18002fb32:	gs rex.B jb 0x18002fba8
    18002fb36:	(bad)
    18002fb37:	jns    0x18002fb79
    18002fb39:	rex push %rcx
    18002fb3b:	rex.RB
@@ -69652,15 +69644,15 @@
    18002fb40:	push   %r14
    18002fb42:	xor    %eax,0x41(%rax)
    18002fb45:	rex.RB
    18002fb46:	rex.X push %rsi
    18002fb48:	xor    %eax,0x40(%rax)
    18002fb4b:	pop    %rdx
    18002fb4c:	add    %al,(%rax)
-   18002fb4e:	mov    $0x6e653f0c,%ebp
+   18002fb4e:	mov    $0x6e653f0c,%esi
    18002fb53:	fs rex push %rcx
    18002fb56:	rex.X jns 0x18002fbcd
    18002fb59:	gs rex.B jb 0x18002fbcf
    18002fb5d:	(bad)
    18002fb5e:	jns    0x18002fba0
    18002fb60:	rex push %rcx
    18002fb62:	rex.RB
@@ -69698,15 +69690,15 @@
    18002fb9e:	je     0x18002fc09
    18002fba0:	jbe    0x18002fc0b
    18002fba2:	je     0x18002fc1d
    18002fba4:	rex push %rcx
    18002fba6:	je     0x18002fbe8
    18002fba8:	rex
    18002fba9:	rex pop %rdx
-   18002fbab:	add    %ch,(%rsi)
+   18002fbab:	add    %ch,(%rdi)
    18002fbad:	(bad)
    18002fbae:	(bad)
    18002fbaf:	data16 jb 0x18002fc21
    18002fbb2:	insl   (%dx),%es:(%rdi)
    18002fbb3:	rex.WR (bad)
    18002fbb5:	je     0x18002fc20
    18002fbb7:	outsb  %ds:(%rsi),(%dx)
@@ -69719,15 +69711,15 @@
    18002fbc8:	xor    %eax,0x56(%rax)
    18002fbcb:	push   %rcx
    18002fbcc:	rex.X jns 0x18002fc43
    18002fbcf:	gs rex.B jb 0x18002fc45
    18002fbd3:	(bad)
    18002fbd4:	jns    0x18002fc2c
    18002fbd6:	imul   $0x5a404040,0x77(%rbp),%esp
-   18002fbdd:	add    %dh,(%rdx)
+   18002fbdd:	add    %dh,(%rbx)
    18002fbdf:	sbb    $0x3f,%al
    18002fbe1:	je     0x18002fc52
    18002fbe3:	push   %rbx
    18002fbe4:	je     0x18002fc58
    18002fbe6:	imul   $0x72555140,0x67(%rsi),%ebp
    18002fbed:	insb   (%dx),%es:(%rdi)
    18002fbee:	rex
@@ -69777,15 +69769,15 @@
    18002fc3e:	imul   $0x6974704f,0x67(%rsi),%ebp
    18002fc45:	outsl  %ds:(%rsi),(%dx)
    18002fc46:	outsb  %ds:(%rsi),(%dx)
    18002fc47:	rex xor 0x40(%rax),%al
    18002fc4b:	rex
    18002fc4c:	rex pop %rdx
    18002fc4e:	add    %al,(%rax)
-   18002fc50:	cli
+   18002fc50:	sti
    18002fc51:	(bad)
    18002fc53:	imul   $0x69746972,0x43(%rbx),%esi
    18002fc5a:	movsxd 0x6c(%rcx),%esp
    18002fc5d:	rex.RB outsb %ds:(%rsi),(%dx)
    18002fc5f:	(bad)
    18002fc60:	(bad)  {%k4}
    18002fc63:	fs rex push %rcx
@@ -69796,15 +69788,15 @@
    18002fc75:	rex
    18002fc76:	rex push %rcx
    18002fc78:	rex.RB
    18002fc79:	rex.X
    18002fc7a:	pop    %r15
    18002fc7c:	rex.WRX pop %rax
    18002fc7e:	pop    %rdx
-   18002fc7f:	add    %ch,%bh
+   18002fc7f:	add    %dh,%al
    18002fc81:	(bad)
    18002fc82:	(bad)
    18002fc83:	push   $0x40687361
    18002fc88:	push   %rcx
    18002fc89:	rex.WRB
    18002fc8a:	gs jae 0x18002fd00
    18002fc8d:	(bad)
@@ -69839,17 +69831,16 @@
    18002fcd7:	jo     0x18002fd4d
    18002fcd9:	outsl  %ds:(%rsi),(%dx)
    18002fcda:	addr32 jb 0x18002fd3e
    18002fcdd:	jo     0x18002fd47
    18002fcdf:	imul   $0x40687361,0x48(%rbx),%esp
    18002fce6:	rex
    18002fce7:	rex pop %rdx
-   18002fce9:	add    %dl,(%rsp,%rcx,1)
-   18002fcec:	(bad)
-   18002fced:	(bad)
+   18002fce9:	add    %dl,0x65643f0c(%rip)        # 0x1e5673bfb
+   18002fcef:	(bad)
    18002fcf4:	rex.WRB
    18002fcf5:	gs jae 0x18002fd6b
    18002fcf8:	(bad)
    18002fcf9:	rex.WR outsl %gs:(%esi),(%dx)
    18002fcfd:	addr32 addr32 gs jb 0x18002fd42
    18002fd02:	rex push %rcx
    18002fd04:	rex.RB
@@ -69857,18 +69848,17 @@
    18002fd06:	pop    %r8
    18002fd08:	push   %rax
    18002fd09:	rex.RB
    18002fd0a:	rex.X
    18002fd0b:	rex.R pop %rdx
    18002fd0d:	pop    %rdx
    18002fd0e:	add    %al,(%rax)
-   18002fd10:	int    $0x1d
-   18002fd12:	(bad)
-   18002fd13:	ja     0x18002fd76
-   18002fd15:	jb     0x18002fd85
+   18002fd10:	(bad)
+   18002fd11:	sbb    $0x7261773f,%eax
+   18002fd16:	outsb  %ds:(%rsi),(%dx)
    18002fd17:	imul   $0x654d5140,0x67(%rsi),%ebp
    18002fd1e:	jae    0x18002fd93
    18002fd20:	(bad)
    18002fd21:	rex.WR outsl %gs:(%esi),(%dx)
    18002fd25:	addr32 addr32 gs jb 0x18002fd6a
    18002fd2a:	rex push %rcx
    18002fd2c:	rex.RB
@@ -69877,15 +69867,15 @@
    18002fd30:	push   %r14
    18002fd32:	push   %rcx
    18002fd33:	rex.R
    18002fd34:	(bad)
    18002fd3a:	pop    %rax
    18002fd3b:	pop    %rdx
    18002fd3c:	add    %al,(%rax)
-   18002fd3e:	adc    %eax,(%rdx)
+   18002fd3e:	adc    (%rdx),%al
    18002fd40:	(bad)
    18002fd41:	(bad)
    18002fd42:	xor    %dl,0x53(%rcx)
    18002fd45:	je     0x18002fdb9
    18002fd47:	imul   $0x45514040,0x67(%rsi),%ebp
    18002fd4e:	rex.B
    18002fd4f:	rex.B
@@ -69896,15 +69886,15 @@
    18002fd57:	outsb  %ds:(%rsi),(%dx)
    18002fd58:	xor    %edx,0x74(%rbx)
    18002fd5b:	jb     0x18002fdc6
    18002fd5d:	outsb  %ds:(%rsi),(%dx)
    18002fd5e:	addr32 rex
    18002fd60:	rex
    18002fd61:	rex pop %rdx
-   18002fd63:	add    %bh,0x6f743f1b(%rdx)
+   18002fd63:	add    %bh,0x6f743f1b(%rbx)
    18002fd69:	rex.WR outsl %ds:(%rsi),(%dx)
    18002fd6b:	movsxd 0x6c(%rcx),%esp
    18002fd6e:	cmp    %al,0x69(%rdx)
    18002fd71:	je     0x18002fdb3
    18002fd73:	push   %rcx
    18002fd74:	push   %rbx
    18002fd75:	je     0x18002fde9
@@ -69917,29 +69907,29 @@
    18002fd85:	rex.X jns 0x18002fdfc
    18002fd88:	gs rex.B jb 0x18002fdfe
    18002fd8c:	(bad)
    18002fd8d:	jns    0x18002fdcf
    18002fd8f:	rex pop %rax
    18002fd91:	pop    %rdx
    18002fd92:	add    %al,(%rax)
-   18002fd94:	push   %rsi
+   18002fd94:	push   %rdi
    18002fd95:	add    $0x51363f3f,%eax
    18002fd9a:	rex.R
    18002fd9b:	(bad)
    18002fda1:	push   %rcx
    18002fda2:	rex.RB
    18002fda3:	rex.B
    18002fda4:	rex.B
    18002fda5:	rex.B
    18002fda6:	rex.RB
    18002fda7:	push   %r14
    18002fda9:	xor    %al,0x48(%rax)
    18002fdac:	rex pop %rdx
    18002fdae:	add    %al,(%rax)
-   18002fdb0:	insb   (%dx),%es:(%rdi)
+   18002fdb0:	insl   (%dx),%es:(%rdi)
    18002fdb1:	adc    %edi,(%rdi)
    18002fdb3:	imul   $0x64696c61,0x56(%rbx),%esi
    18002fdba:	rex push %rcx
    18002fdbc:	push   %rsi
    18002fdbd:	(bad)
    18002fdbe:	jb     0x18002fe29
    18002fdc0:	(bad)
@@ -69947,15 +69937,15 @@
    18002fdc2:	je     0x18002fe04
    18002fdc4:	rex push %rcx
    18002fdc6:	rex.RB
    18002fdc7:	rex.X
    18002fdc8:	pop    %r15
    18002fdca:	rex.WRX pop %rax
    18002fdcc:	pop    %rdx
-   18002fdcd:	add    %bl,0x6f743f1b(%rbp)
+   18002fdcd:	add    %bl,0x6f743f1b(%rsi)
    18002fdd3:	rex.WB outsb %ds:(%rsi),(%dx)
    18002fdd5:	je     0x18002fe17
    18002fdd7:	push   %rcx
    18002fdd8:	push   %rsi
    18002fdd9:	(bad)
    18002fdda:	jb     0x18002fe45
    18002fddc:	(bad)
@@ -69966,15 +69956,15 @@
    18002fde3:	rex.X
    18002fde4:	rex.B
    18002fde5:	rex.W push %rax
    18002fde7:	rex.RB
    18002fde8:	pop    %r15
    18002fdea:	rex.WRX
    18002fdeb:	rex pop %rdx
-   18002fded:	add    %ch,%al
+   18002fded:	add    %ch,%cl
    18002fdef:	(bad)
    18002fdf0:	(bad)
    18002fdf1:	(bad)
    18002fdf2:	fs fs push %rbx
    18002fdf5:	movsxd %gs:0x40(%rbx),%esi
    18002fdf9:	push   %rcx
    18002fdfa:	rex.R (bad)
@@ -69999,15 +69989,15 @@
    18002fe2a:	pop    %r15
    18002fe2c:	rex.WX
    18002fe2d:	rex.B
    18002fe2e:	rex.RB
    18002fe2f:	rex.X push %rsi
    18002fe31:	xor    %eax,0x40(%rax)
    18002fe34:	pop    %rdx
-   18002fe35:	add    %bl,0x2(%rdx)
+   18002fe35:	add    %bl,0x2(%rbx)
    18002fe38:	(bad)
    18002fe39:	(bad)
    18002fe3a:	xor    %dl,0x55(%rcx)
    18002fe3d:	jb     0x18002feab
    18002fe3f:	rex
    18002fe40:	rex push %rcx
    18002fe42:	rex.RB
@@ -70023,16 +70013,16 @@
    18002fe4e:	imul   $0x34574040,0x67(%rsi),%ebp
    18002fe55:	push   %rax
    18002fe56:	(bad)
    18002fe57:	jb     0x18002fecc
    18002fe59:	imul   $0x65646f4d,0x67(%rsi),%ebp
    18002fe60:	rex xor %al,0x40(%rax)
    18002fe64:	pop    %rdx
-   18002fe65:	add    %al,(%rbx)
-   18002fe67:	adc    %bh,(%rdi)
+   18002fe65:	add    %al,(%rax,%rdx,1)
+   18002fe68:	(bad)
    18002fe69:	imul   $0x67756265,0x44(%rbx),%esi
    18002fe70:	rex.RB outsb %ds:(%rsi),(%dx)
    18002fe72:	(bad)
    18002fe73:	(bad)  {%k4}
    18002fe76:	fs rex push %rcx
    18002fe79:	rex.WR outsl %ds:(%rsi),(%dx)
    18002fe7b:	addr32 imul $0x65746143,0x67(%esi),%ebp
@@ -70042,15 +70032,15 @@
    18002fe89:	rex push %rcx
    18002fe8b:	rex.RB
    18002fe8c:	rex.X
    18002fe8d:	pop    %r15
    18002fe8f:	rex.WRX pop %rax
    18002fe91:	pop    %rdx
    18002fe92:	add    %al,(%rax)
-   18002fe94:	mov    %al,(%rdi,%rdi,1)
+   18002fe94:	mov    %eax,(%rdi,%rdi,1)
    18002fe97:	(bad)
    18002fe98:	xor    $0x51,%al
    18002fe9a:	push   %rbp
    18002fe9b:	jb     0x18002ff09
    18002fe9d:	push   %rcx
    18002fe9e:	jne    0x18002ff05
    18002fea0:	jb     0x18002ff1b
@@ -70065,30 +70055,30 @@
    18002feac:	xor    %al,0x24(%rax)
    18002feaf:	and    $0x51,%al
    18002feb1:	rex.RB
    18002feb2:	push   %r14
    18002feb4:	xor    %al,0x40(%rax)
    18002feb7:	pop    %rdx
    18002feb8:	add    %al,(%rax)
-   18002feba:	mov    $0x6c633f09,%edx
+   18002feba:	mov    $0x6c633f09,%ebx
    18002febf:	gs (bad)
    18002fec1:	jb     0x18002ff03
    18002fec3:	push   %rcx
    18002fec4:	rex.X jns 0x18002ff3b
    18002fec7:	gs rex.B jb 0x18002ff3d
    18002fecb:	(bad)
    18002fecc:	jns    0x18002ff0e
    18002fece:	rex push %rcx
    18002fed0:	rex.RB
    18002fed1:	rex.B
    18002fed2:	pop    %r8
    18002fed4:	pop    %rax
    18002fed5:	pop    %rdx
    18002fed6:	add    %al,(%rax)
-   18002fed8:	jne    0x18002fee2
+   18002fed8:	jbe    0x18002fee2
    18002feda:	(bad)
    18002fedb:	(bad)
    18002fedc:	je     0x18002ff1e
    18002fede:	push   %rcx
    18002fedf:	rex.X jns 0x18002ff56
    18002fee2:	gs rex.B jb 0x18002ff58
    18002fee6:	(bad)
@@ -70096,15 +70086,15 @@
    18002fee9:	rex push %rcx
    18002feeb:	rex.RB
    18002feec:	rex.X
    18002feed:	rex.B
    18002feee:	rex.R pop %rdi
    18002fef0:	rex.WX
    18002fef1:	rex pop %rdx
-   18002fef3:	add    %ch,(%rdx)
+   18002fef3:	add    %ch,(%rbx)
    18002fef5:	(bad)
    18002fef7:	imul   $0x664f7865,0x64(%rsi),%ebp
    18002fefe:	rex push %rcx
    18002ff00:	rex.X jns 0x18002ff77
    18002ff03:	gs rex.B jb 0x18002ff79
    18002ff07:	(bad)
    18002ff08:	jns    0x18002ff4a
@@ -70114,28 +70104,27 @@
    18002ff0e:	pop    %r15
    18002ff10:	rex.WX
    18002ff11:	rex.R pop %rdi
    18002ff13:	rex.WX
    18002ff14:	rex pop %rdx
    18002ff16:	add    %al,(%rax)
    18002ff18:	(bad)
-   18002ff19:	adc    (%rdi),%bh
    18002ff1b:	insl   (%dx),%es:(%rdi)
    18002ff1c:	imul   $0x65747942,0x51(%rax,%rax,2),%esp
    18002ff24:	rex.B jb 0x18002ff99
    18002ff27:	(bad)
    18002ff28:	jns    0x18002ff6a
    18002ff2a:	rex push %rcx
    18002ff2c:	rex.RB
    18002ff2d:	rex.X
    18002ff2e:	rex.B (bad)
    18002ff30:	push   %r14
    18002ff32:	xor    %eax,0x5f(%rax)
    18002ff35:	rex.WX xor %al,0x5a(%rax)
-   18002ff39:	add    %dh,(%rsi)
+   18002ff39:	add    %dh,(%rdi)
    18002ff3b:	sbb    (%rdi),%bh
    18002ff3d:	jae    0x18002ffb3
    18002ff3f:	(bad)
    18002ff40:	jb     0x18002ffb6
    18002ff42:	jae    0x18002ff9b
    18002ff44:	imul   $0x74794251,0x40(%rax,%rbp,2),%esi
    18002ff4c:	gs rex.B jb 0x18002ffc2
@@ -70148,15 +70137,15 @@
    18002ff59:	rex.WRX push %rsi
    18002ff5b:	push   %rcx
    18002ff5c:	rex.X jns 0x18002ffd3
    18002ff5f:	gs rex.B jb 0x18002ffd5
    18002ff63:	(bad)
    18002ff64:	jns    0x18002ffbc
    18002ff66:	imul   $0x5a404040,0x77(%rbp),%esp
-   18002ff6d:	add    %ah,%cl
+   18002ff6d:	add    %ah,%dl
    18002ff6f:	or     $0x3f,%al
    18002ff71:	outsb  %gs:(%rsi),(%dx)
    18002ff73:	fs jae 0x18002ffcd
    18002ff76:	imul   $0x74794251,0x40(%rax,%rbp,2),%esi
    18002ff7e:	gs rex.B jb 0x18002fff4
    18002ff82:	(bad)
    18002ff83:	jns    0x18002ffc5
@@ -70167,30 +70156,30 @@
    18002ff8b:	rex.WRX push %rsi
    18002ff8d:	push   %rcx
    18002ff8e:	rex.X jns 0x180030005
    18002ff91:	gs rex.B jb 0x180030007
    18002ff95:	(bad)
    18002ff96:	jns    0x18002ffee
    18002ff98:	imul   $0x5a404040,0x77(%rbp),%esp
-   18002ff9f:	add    %ah,0x68633f09(%rbp)
+   18002ff9f:	add    %ah,0x68633f09(%rsi)
    18002ffa5:	outsl  %ds:(%rsi),(%dx)
    18002ffa6:	jo     0x18002ffe8
    18002ffa8:	push   %rcx
    18002ffa9:	rex.X jns 0x180030020
    18002ffac:	gs rex.B jb 0x180030022
    18002ffb0:	(bad)
    18002ffb1:	jns    0x18002fff3
    18002ffb3:	rex push %rcx
    18002ffb5:	rex.RB
    18002ffb6:	rex.B
    18002ffb7:	pop    %r8
    18002ffb9:	pop    %rdi
    18002ffba:	rex.WX
    18002ffbb:	rex pop %rdx
-   18002ffbd:	add    %ah,%ch
+   18002ffbd:	add    %ah,%dh
    18002ffbf:	sbb    $0x3f,%al
    18002ffc1:	je     0x180030035
    18002ffc3:	imul   $0x51406465,0x6d(%rbp),%ebp
    18002ffca:	rex.X jns 0x180030041
    18002ffcd:	gs rex.B jb 0x180030043
    18002ffd1:	(bad)
    18002ffd2:	jns    0x180030014
@@ -70198,15 +70187,15 @@
    18002ffd6:	rex.RB
    18002ffd7:	rex.W
    18002ffd8:	rex.B
    18002ffd9:	rex.B (bad)
    18002ffdb:	push   %r14
    18002ffdd:	xor    %eax,0x58(%rax)
    18002ffe0:	pop    %rdx
-   18002ffe1:	add    %bl,0x756e3f13(%rax)
+   18002ffe1:	add    %bl,0x756e3f13(%rcx)
    18002ffe7:	insl   (%dx),%es:(%rdi)
    18002ffe8:	vsqrtsh 0xf2(%rdx),%xmm17,%xmm24
    18002ffef:	je     0x180030056
    18002fff1:	rex.B jb 0x180030066
    18002fff4:	(bad)
    18002fff5:	jns    0x180030037
    18002fff7:	rex push %rbx
@@ -70242,15 +70231,15 @@
    18003002c:	je     0x18003008f
    18003002e:	push   %rax
    18003002f:	outsl  %ds:(%rsi),(%dx)
    180030030:	imul   $0x44407265,0x74(%rsi),%ebp
    180030037:	rex
    180030038:	rex
    180030039:	rex pop %rdx
-   18003003b:	add    %dl,0x8(%rdi)
+   18003003b:	add    %bl,0x8(%rax)
    18003003e:	(bad)
    18003003f:	(bad)
    180030040:	jb     0x1800300a9
    180030042:	rex push %rcx
    180030044:	push   %rbx
    180030045:	je     0x1800300b9
    180030047:	imul   $0x45514040,0x67(%rsi),%ebp
@@ -70260,29 +70249,27 @@
    180030053:	xor    %eax,0x47(%rax)
    180030056:	rex.W
    180030057:	rex.W push %rsi
    180030059:	push   %rcx
    18003005a:	rex.XB push $0x40407261
    180030060:	rex pop %rdx
    180030062:	add    %al,(%rax)
-   180030064:	(bad)
-   180030065:	adc    (%rdi),%bh
-   180030067:	insl   (%dx),%es:(%rdi)
+   180030064:	enter  $0x3f12,$0x6d
    180030068:	imul   $0x69727453,0x51(%rax,%rax,2),%esp
    180030070:	outsb  %ds:(%rsi),(%dx)
    180030071:	addr32 rex
    180030073:	rex push %rcx
    180030075:	rex.RB
    180030076:	rex.X
    180030077:	rex.B (bad)
    180030079:	push   %r14
    18003007b:	xor    %eax,0x5f(%rax)
    18003007e:	rex.WX xor %al,0x5a(%rax)
    180030082:	add    %al,(%rax)
-   180030084:	cmp    (%rdx),%bl
+   180030084:	cmp    (%rdx),%ebx
    180030086:	(bad)
    180030087:	jae    0x1800300fd
    180030089:	(bad)
    18003008a:	jb     0x180030100
    18003008c:	jae    0x1800300e5
    18003008e:	imul   $0x72745351,0x40(%rax,%rbp,2),%esi
    180030096:	imul   $0x45514040,0x67(%rsi),%ebp
@@ -70301,31 +70288,30 @@
    1800300b4:	je     0x18003011f
    1800300b6:	jbe    0x180030121
    1800300b8:	je     0x180030133
    1800300ba:	rex push %rcx
    1800300bc:	je     0x1800300fe
    1800300be:	rex
    1800300bf:	rex pop %rdx
-   1800300c1:	add    %bl,0x756e3f13(%rdx)
+   1800300c1:	add    %bl,0x756e3f13(%rbx)
    1800300c7:	insl   (%dx),%es:(%rdi)
    1800300c8:	vsqrtsh 0xe8(%rbx),%xmm17,%xmm26
    1800300cf:	jb     0x18003013a
    1800300d1:	outsb  %ds:(%rsi),(%dx)
    1800300d2:	addr32 rex
    1800300d4:	rex push %rbx
    1800300d6:	rex.B (bad)
    1800300d8:	push   %r14
    1800300da:	xor    %eax,0x48(%rax)
    1800300dd:	rex.W
    1800300de:	rex pop %rdx
    1800300e0:	add    %al,(%rax)
-   1800300e2:	adc    $0x2,%al
-   1800300e4:	(bad)
-   1800300e5:	(bad)
-   1800300e6:	xor    %dl,0x53(%rcx)
+   1800300e2:	adc    $0x303f3f02,%eax
+   1800300e7:	push   %rcx
+   1800300e8:	push   %rbx
    1800300e9:	je     0x18003015d
    1800300eb:	imul   $0x45514040,0x67(%rsi),%ebp
    1800300f2:	rex.B
    1800300f3:	rex.B
    1800300f4:	rex pop %rdi
    1800300f6:	rex.WX push %rdi
    1800300f8:	xor    $0x49,%al
@@ -70335,15 +70321,15 @@
    180030105:	outsl  %ds:(%rsi),(%dx)
    180030106:	outsb  %ds:(%rsi),(%dx)
    180030107:	rex push %rcx
    180030109:	je     0x18003014b
    18003010b:	rex
    18003010c:	rex pop %rdx
    18003010e:	add    %al,(%rax)
-   180030110:	pop    %rbp
+   180030110:	pop    %rsi
    180030111:	sbb    %edi,(%rdi)
    180030113:	jae    0x18003017a
    180030115:	je     0x18003016c
    180030117:	jb     0x180030185
    180030119:	rex push %rcx
    18003011b:	push   %rbp
    18003011c:	jb     0x18003018a
@@ -70362,27 +70348,28 @@
    180030134:	push   %rax
    180030135:	(bad)
    180030136:	jb     0x1800301ab
    180030138:	imul   $0x65646f4d,0x67(%rsi),%ebp
    18003013f:	rex xor %eax,0x40(%rax)
    180030143:	pop    %rdx
    180030144:	add    %al,(%rax)
-   180030146:	imul   $0x3f,(%rcx),%edx
+   180030146:	insb   (%dx),%es:(%rdi)
+   180030147:	adc    %edi,(%rdi)
    180030149:	imul   $0x64696c61,0x56(%rbx),%esi
    180030150:	rex push %rcx
    180030152:	push   %rbp
    180030153:	jb     0x1800301c1
    180030155:	rex
    180030156:	rex push %rcx
    180030158:	rex.RB
    180030159:	rex.X
    18003015a:	pop    %r15
    18003015c:	rex.WRX pop %rax
    18003015e:	pop    %rdx
-   18003015f:	add    %dh,%dh
+   18003015f:	add    %dh,%bh
    180030161:	adc    (%rdi),%edi
    180030163:	jo     0x1800301c6
    180030165:	je     0x1800301cf
    180030167:	rex push %rcx
    180030169:	push   %rbp
    18003016a:	jb     0x1800301d8
    18003016c:	rex
@@ -70419,31 +70406,31 @@
    1800301a6:	jb     0x180030214
    1800301a8:	rex
    1800301a9:	rex
    1800301aa:	rex
    1800301ab:	rex
    1800301ac:	rex pop %rdx
    1800301ae:	add    %al,(%rax)
-   1800301b0:	scas   %es:(%rdi),%eax
-   1800301b1:	sbb    $0x3f,%al
+   1800301b0:	mov    $0x1c,%al
+   1800301b2:	(bad)
    1800301b3:	je     0x180030227
    1800301b5:	rex push %rcx
    1800301b7:	(bad)
    1800301bd:	rex
    1800301be:	rex push %rbx
    1800301c0:	rex.B (bad)
    1800301c2:	push   %r14
    1800301c4:	push   %rcx
    1800301c5:	push   %rbx
    1800301c6:	je     0x18003023a
    1800301c8:	imul   $0x45504040,0x67(%rsi),%ebp
    1800301cf:	rex.X
    1800301d0:	xor    %r9b,0x40(%rax)
    1800301d4:	pop    %rdx
-   1800301d5:	add    %ch,%ah
+   1800301d5:	add    %ch,%ch
    1800301d7:	sbb    $0x6972773f,%eax
    1800301dc:	je     0x180030243
    1800301de:	rex push %rcx
    1800301e0:	rex.WB
    1800301e1:	rex.WRXB
    1800301e2:	rex.R
    1800301e3:	gs jbe 0x18003024f
@@ -70460,15 +70447,15 @@
    1800301f5:	rex.X jns 0x18003026c
    1800301f8:	gs rex.B jb 0x18003026e
    1800301fc:	(bad)
    1800301fd:	jns    0x18003023f
    1800301ff:	rex
    180030200:	rex pop %rdx
    180030202:	add    %al,(%rax)
-   180030204:	mov    (%rsi),%ecx
+   180030204:	mov    %cs,(%rsi)
    180030206:	(bad)
    180030207:	addr32 gs je 0x18003024e
    18003020b:	push   $0x51407261
    180030210:	rex.WB
    180030211:	rex.WRXB
    180030212:	rex.R
    180030213:	gs jbe 0x18003027f
@@ -70497,15 +70484,15 @@
    18003023c:	movsxd 0x40(%rbp),%esp
    18003023f:	rex push %rcx
    180030241:	rex.RB
    180030242:	rex.B
    180030243:	pop    %r8
    180030245:	pop    %rax
    180030246:	pop    %rdx
-   180030247:	add    %cl,0x8(%rbp)
+   180030247:	add    %cl,0x8(%rsi)
    18003024a:	(bad)
    18003024b:	(bad)
    18003024c:	jo     0x1800302be
    18003024e:	insb   (%dx),%es:(%rdi)
    18003024f:	imul   $0x6e6f6974,0x61(%rbx),%esp
    180030256:	rex.WRX (bad)
    180030258:	insl   (%dx),%es:(%rdi)
@@ -70519,15 +70506,15 @@
    18003026c:	rex push %rbx
    18003026e:	rex.B (bad)
    180030270:	push   %r14
    180030272:	push   %rcx
    180030273:	push   %rbx
    180030274:	je     0x1800302e8
    180030276:	imul   $0x5a584040,0x67(%rsi),%ebp
-   18003027d:	add    %dl,0x6e693f0f(%rdi)
+   18003027d:	add    %bl,0x6e693f0f(%rax)
    180030283:	jae    0x1800302f9
    180030285:	(bad)
    180030286:	outsb  %ds:(%rsi),(%dx)
    180030287:	movsxd 0x40(%rbp),%esp
    18003028a:	push   %rcx
    18003028b:	rex.XB outsl %ds:(%rsi),(%dx)
    18003028d:	jb     0x1800302f4
@@ -70538,16 +70525,15 @@
    18003029b:	rex push %rbx
    18003029d:	push   %r8
    18003029f:	rex.RB
    1800302a0:	push   %r14
    1800302a2:	xor    %eax,0x58(%rax)
    1800302a5:	pop    %rdx
    1800302a6:	add    %al,(%rax)
-   1800302a8:	push   $0x1a
-   1800302aa:	(bad)
+   1800302a8:	imul   $0x3f,(%rdx),%ebx
    1800302ab:	jae    0x180030321
    1800302ad:	(bad)
    1800302ae:	je     0x180030319
    1800302b0:	movsxd 0x65(%rbp),%ecx
    1800302b3:	je     0x180030316
    1800302b5:	(bad)
    1800302bb:	rex push %rcx
@@ -70558,15 +70544,15 @@
    1800302c3:	movsxd 0x40(%rbp),%esp
    1800302c6:	rex xor 0x51(%rbp),%dl
    1800302ca:	rex.WRB
    1800302cb:	gs je  0x18003032f
    1800302ce:	(bad)
    1800302d4:	rex
    1800302d5:	rex
-   1800302d6:	rex.X add %bpl,0x73693f10(%rcx)
+   1800302d6:	rex.X add %bpl,0x73693f10(%rdx)
    1800302dd:	rex.WRX jne 0x18003034c
    1800302e0:	insb   (%dx),%es:(%rdi)
    1800302e1:	rex push %rcx
    1800302e3:	push   %rsi
    1800302e4:	(bad)
    1800302e5:	jb     0x180030350
    1800302e7:	(bad)
@@ -70575,30 +70561,29 @@
    1800302eb:	rex push %rcx
    1800302ed:	rex.RB
    1800302ee:	rex.X
    1800302ef:	pop    %r15
    1800302f1:	rex.WRX pop %rax
    1800302f3:	pop    %rdx
    1800302f4:	add    %al,(%rax)
-   1800302f6:	ds add (%rdi),%edi
+   1800302f6:	(bad)
+   1800302f7:	add    (%rdi),%edi
    1800302f9:	(bad)
    1800302fa:	xor    %edx,0x4a(%rcx)
    1800302fd:	jae    0x18003036e
    1800302ff:	outsb  %ds:(%rsi),(%dx)
    180030300:	(bad)
    180030306:	rex
    180030307:	rex push %rcx
    180030309:	rex.RB
    18003030a:	rex.B
    18003030b:	rex.B
    18003030c:	rex pop %rax
    18003030e:	pop    %rdx
-   18003030f:	add    %bh,0x1c(%rdi)
-   180030312:	(bad)
-   180030313:	je     0x180030384
+   18003030f:	add    %al,0x6f743f1c(%rax)
    180030315:	push   %rsi
    180030316:	(bad)
    180030317:	jb     0x180030382
    180030319:	(bad)
    18003031a:	outsb  %ds:(%rsi),(%dx)
    18003031b:	je     0x18003036a
    18003031d:	(bad)
@@ -70629,31 +70614,32 @@
    18003034c:	outsb  %ds:(%rsi),(%dx)
    18003034d:	je     0x18003038f
    18003034f:	rex
    180030350:	rex
    180030351:	rex pop %rax
    180030353:	pop    %rdx
    180030354:	add    %al,(%rax)
-   180030356:	sub    %dl,(%rax)
+   180030356:	sub    %edx,(%rax)
    180030358:	(bad)
    180030359:	imul   $0x7974706d,0x45(%rbx),%esi
    180030360:	rex push %rcx
    180030362:	rex.WX jae 0x1800303d4
    180030365:	outsb  %ds:(%rsi),(%dx)
    180030366:	(bad)
    18003036c:	rex
    18003036d:	rex push %rcx
    18003036f:	rex.RB
    180030370:	rex.X
    180030371:	pop    %r15
    180030373:	rex.WRX pop %rax
    180030375:	pop    %rdx
    180030376:	add    %al,(%rax)
-   180030378:	and    $0x72663f0e,%eax
-   18003037d:	outsl  %ds:(%rsi),(%dx)
+   180030378:	es (bad)
+   18003037a:	(bad)
+   18003037b:	data16 jb 0x1800303ed
    18003037e:	insl   (%dx),%es:(%rdi)
    18003037f:	rex.WX jae 0x1800303f1
    180030382:	outsb  %ds:(%rsi),(%dx)
    180030383:	rex push %rcx
    180030385:	rex.WX jae 0x1800303f7
    180030388:	outsb  %ds:(%rsi),(%dx)
    180030389:	rex.R outsl %ds:(%rsi),(%dx)
@@ -70681,31 +70667,32 @@
    1800303b4:	(bad)
    1800303b5:	jb     0x18003042a
    1800303b7:	gs rex.RB jb 0x18003042d
    1800303bb:	outsl  %ds:(%rsi),(%dx)
    1800303bc:	jb     0x1800303fe
    1800303be:	rex
    1800303bf:	rex pop %rdx
-   1800303c1:	add    %ch,0x73693f10(%rbp)
+   1800303c1:	add    %ch,0x73693f10(%rsi)
    1800303c7:	(bad)
    1800303cd:	rex push %rcx
    1800303cf:	rex.WX jae 0x180030441
    1800303d2:	outsb  %ds:(%rsi),(%dx)
    1800303d3:	rex.R outsl %ds:(%rsi),(%dx)
    1800303d5:	movsxd 0x6d(%rbp),%esi
    1800303d8:	outsb  %gs:(%rsi),(%dx)
    1800303da:	je     0x18003041c
    1800303dc:	rex push %rcx
    1800303de:	rex.RB
    1800303df:	rex.X
    1800303e0:	pop    %r15
    1800303e2:	rex.WRX pop %rax
    1800303e4:	pop    %rdx
-   1800303e5:	add    %ah,0x6a626f3f(%rbx,%rdx,1)
-   1800303ec:	movsxd %gs:0x51(%rax,%rax,2),%esi
+   1800303e5:	add    %ah,0x626f3f13(%rbp)
+   1800303eb:	push   $0x65
+   1800303ed:	movsxd 0x51(%rax,%rax,2),%esi
    1800303f1:	rex.WX jae 0x180030463
    1800303f4:	outsb  %ds:(%rsi),(%dx)
    1800303f5:	rex.R outsl %ds:(%rsi),(%dx)
    1800303f7:	movsxd 0x6d(%rbp),%esi
    1800303fa:	outsb  %gs:(%rsi),(%dx)
    1800303fc:	je     0x18003043e
    1800303fe:	rex push %rcx
@@ -70740,16 +70727,15 @@
    180030433:	push   %rcx
    180030434:	rex.X jns 0x1800304ab
    180030437:	gs rex.B jb 0x1800304ad
    18003043b:	(bad)
    18003043c:	jns    0x18003047e
    18003043e:	rex pop %rax
    180030440:	pop    %rdx
-   180030441:	add    %ch,(%rbx)
-   180030443:	or     $0x7272653f,%eax
+   180030441:	add    %ch,0x7272653f(,%rcx,1)
    180030448:	outsl  %ds:(%rsi),(%dx)
    180030449:	jb     0x18003049e
    18003044b:	je     0x1800304bf
    18003044d:	imul   $0x4f495140,0x67(%rsi),%ebp
    180030454:	rex.R
    180030455:	gs jbe 0x1800304c1
    180030458:	movsxd 0x40(%rbp),%esp
@@ -75274,23 +75260,24 @@
 	...
    180036075:	add    %al,(%rcx)
    180036077:	add    %cl,(%rcx)
    180036079:	add    $0x0,%al
    18003607b:	add    %dl,-0x60000000(%rax)
    180036081:	(bad)
    180036082:	add    (%rax),%eax
-   180036084:	je     0x180036089
+   180036084:	insb   (%dx),%es:(%rdi)
+   180036085:	add    (%rax),%eax
 	...
-   18003608e:	add    %al,(%rax)
-   180036090:	sbb    %ah,0x0(%rbx,%rax,1)
+   18003608f:	add    %dl,(%rax)
+   180036091:	add    %fs:(%rax),%eax
    180036094:	jge    0x180036097
 	...
    18003609e:	add    %al,(%rax)
-   1800360a0:	je     0x1800360a5
-   1800360a2:	xor    $0x0,%al
+   1800360a0:	insb   (%dx),%es:(%rdi)
+   1800360a1:	add    (%rax,%rax,1),%esi
    1800360a4:	add    %al,(%rax)
    1800360a6:	push   %rsi
    1800360a7:	add    %dl,0x0(%rbx)
    1800360aa:	pop    %rdi
    1800360ab:	add    %dl,0x0(%rsi)
    1800360ae:	add    %r10b,0x0(%r10)
    1800360b2:	push   %rbx
@@ -75302,42 +75289,42 @@
    1800360c2:	rex.WRXB add %r8b,(%r8)
    1800360c5:	add    %al,(%rax)
    1800360c7:	add    %bh,0xfeef04(%rbp)
    1800360cd:	add    %al,(%rcx)
    1800360cf:	add    %al,(%rsi)
    1800360d1:	add    %al,(%rsi)
    1800360d3:	add    %al,(%rax)
-   1800360d5:	add    %al,(%rdx)
+   1800360d5:	add    %al,(%rbx)
    1800360d7:	add    %al,(%rsi)
    1800360d9:	add    %al,(%rsi)
    1800360db:	add    %al,(%rax)
-   1800360dd:	add    %al,(%rdx)
+   1800360dd:	add    %al,(%rbx)
    1800360df:	add    %bh,(%rdi)
    1800360e1:	add    %al,(%rax)
    1800360e3:	add    %al,(%rax)
    1800360e5:	add    %al,(%rax)
    1800360e7:	add    %al,(%rax,%rax,1)
    1800360ea:	add    $0x0,%al
    1800360ec:	add    (%rax),%al
 	...
    1800360fa:	add    %al,(%rax)
-   1800360fc:	(bad)
+   1800360fc:	int3
    1800360fd:	add    (%rax),%al
    1800360ff:	add    %al,(%rcx)
    180036101:	add    %dl,0x0(%rbx)
    180036104:	je     0x180036106
    180036106:	jb     0x180036108
    180036108:	imul   $0x67006e,(%rax),%eax
    18003610e:	rex.RX add %r13b,0x0(%rcx)
    180036112:	insb   (%dx),%es:(%rdi)
    180036113:	add    %ah,0x0(%rbp)
    180036116:	rex.WB add %bpl,0x0(%r14)
    18003611a:	data16 add %ch,0x0(%rdi)
    18003611e:	add    %al,(%rax)
-   180036120:	mov    $0x2,%al
+   180036120:	test   $0x2,%al
    180036122:	add    %al,(%rax)
    180036124:	add    %eax,(%rax)
    180036126:	xor    %al,(%rax)
    180036128:	xor    $0x0,%al
    18003612a:	xor    %al,(%rax)
    18003612c:	cmp    %eax,(%rax)
    18003612e:	xor    %al,(%rax)
@@ -75428,19 +75415,19 @@
    180036208:	jae    0x18003620a
    18003620a:	imul   $0x6e006f,(%rax),%eax
    180036210:	add    %al,(%rax)
    180036212:	add    %al,(%rax)
    180036214:	ss add %ch,(%rsi)
    180036217:	add    %dh,(%rsi)
    180036219:	add    %ch,(%rsi)
-   18003621b:	add    %dh,(%rdx)
+   18003621b:	add    %dh,(%rbx)
    18003621d:	add    %ch,(%rsi)
    18003621f:	add    %dh,(%rax)
    180036221:	add    %al,(%rax)
-   180036223:	add    %ah,0x1003e00(%rax)
+   180036223:	add    %bl,0x1003a00(%rax)
    180036229:	add    %cl,0x65(%rax,%rax,1)
    18003622d:	add    %ah,0x0(%rdi)
    180036230:	(bad)
    180036231:	add    %ch,0x43(%rax,%rax,1)
    180036235:	add    %ch,0x0(%rdi)
    180036238:	jo     0x18003623a
    18003623a:	jns    0x18003623c
@@ -75454,324 +75441,320 @@
    180036250:	jb     0x180036252
    180036252:	imul   $0x680067,(%rax),%eax
    180036258:	je     0x18003625a
    18003625a:	and    %al,(%rax)
    18003625c:	sub    %al,(%rax)
    18003625e:	rex.XB add %bpl,(%r9)
    180036261:	add    %ah,(%rax)
-   180036263:	add    %dh,(%rdx)
-   180036265:	add    %dh,(%rax)
-   180036267:	add    %dh,(%rdx)
-   180036269:	add    %dh,(%rbx)
-   18003626b:	add    %ah,(%rax)
-   18003626d:	add    %dl,0x68(%rax,%rax,1)
-   180036271:	add    %ah,0x0(%rbp)
-   180036274:	and    %al,(%rax)
-   180036276:	push   %rcx
-   180036277:	add    %dh,0x20(%rax,%rax,1)
-   18003627b:	add    %al,0x0(%rbx)
-   18003627e:	outsl  %ds:(%rsi),(%dx)
-   18003627f:	add    %ch,0x0(%rbp)
-   180036282:	jo     0x180036284
-   180036284:	(bad)
-   180036285:	add    %ch,0x0(%rsi)
-   180036288:	jns    0x18003628a
-   18003628a:	and    %al,(%rax)
-   18003628c:	rex.WR add %r14b,0x64(%rax,%rax,1)
-   180036291:	add    %ah,(%rax)
-   180036293:	add    %ah,0x0(%rcx)
-   180036296:	outsb  %ds:(%rsi),(%dx)
-   180036297:	add    %ah,0x20(%rax,%rax,1)
-   18003629b:	add    %ch,0x0(%rdi)
-   18003629e:	je     0x1800362a0
-   1800362a0:	push   $0x72006500
-   1800362a5:	add    %ah,(%rax)
-   1800362a7:	add    %ah,0x0(%rbx)
-   1800362aa:	outsl  %ds:(%rsi),(%dx)
-   1800362ab:	add    %ch,0x0(%rsi)
-   1800362ae:	je     0x1800362b0
-   1800362b0:	jb     0x1800362b2
-   1800362b2:	imul   $0x750062,(%rax),%eax
-   1800362b8:	je     0x1800362ba
-   1800362ba:	outsl  %ds:(%rsi),(%dx)
-   1800362bb:	add    %dh,0x0(%rdx)
-   1800362be:	jae    0x1800362c0
-   1800362c0:	cs add %al,(%rax)
-   1800362c3:	add    %cl,0x0(%rsi)
-   1800362c6:	adc    (%rax),%eax
-   1800362c8:	add    %eax,(%rax)
-   1800362ca:	rex.WRXB add %r14b,0x0(%r10)
-   1800362ce:	imul   $0x690067,(%rax),%eax
-   1800362d4:	outsb  %ds:(%rsi),(%dx)
-   1800362d5:	add    %ah,0x0(%rcx)
-   1800362d8:	insb   (%dx),%es:(%rdi)
-   1800362d9:	add    %al,0x0(%rsi)
-   1800362dc:	imul   $0x65006c,(%rax),%eax
-   1800362e2:	outsb  %ds:(%rsi),(%dx)
-   1800362e3:	add    %ah,0x0(%rcx)
-   1800362e6:	insl   (%dx),%es:(%rdi)
-   1800362e7:	add    %ah,0x0(%rbp)
-   1800362ea:	add    %al,(%rax)
-   1800362ec:	push   %rcx
-   1800362ed:	add    %dh,0x36(%rax,%rax,1)
-   1800362f1:	add    %cl,0x0(%rsi)
-   1800362f4:	add    %dh,%gs:0x77(%rax,%rax,1)
-   1800362f9:	add    %ch,0x0(%rdi)
-   1800362fc:	jb     0x1800362fe
-   1800362fe:	imul   $0x41,(%rax),%eax
-   180036301:	add    %dh,0x0(%rbp)
-   180036304:	je     0x180036306
-   180036306:	push   $0x64002e00
-   18003630b:	add    %ch,0x6c(%rax,%rax,1)
-   18003630f:	add    %al,(%rax)
-   180036311:	add    %al,(%rax)
-   180036313:	add    %ch,(%rax)
-   180036315:	add    %al,(%rax,%rax,1)
-   180036318:	add    %eax,(%rax)
-   18003631a:	push   %rax
-   18003631b:	add    %dh,0x0(%rdx)
-   18003631e:	outsl  %ds:(%rsi),(%dx)
-   18003631f:	add    %ah,0x75(%rax,%rax,1)
-   180036323:	add    %ah,0x0(%rbx)
-   180036326:	je     0x180036328
-   180036328:	rex.WRX add %r12b,0x0(%rcx)
-   18003632c:	insl   (%dx),%es:(%rdi)
-   18003632d:	add    %ah,0x0(%rbp)
-   180036330:	add    %al,(%rax)
-   180036332:	add    %al,(%rax)
-   180036334:	push   %rcx
-   180036335:	add    %dh,0x36(%rax,%rax,1)
-   180036339:	add    %al,(%rax)
-   18003633b:	add    %dh,(%rax,%rax,1)
-   18003633e:	or     %al,(%rax)
-   180036340:	add    %eax,(%rax)
-   180036342:	push   %rax
-   180036343:	add    %dh,0x0(%rdx)
-   180036346:	outsl  %ds:(%rsi),(%dx)
-   180036347:	add    %ah,0x75(%rax,%rax,1)
-   18003634b:	add    %ah,0x0(%rbx)
-   18003634e:	je     0x180036350
-   180036350:	push   %rsi
-   180036351:	add    %ah,0x0(%rbp)
-   180036354:	jb     0x180036356
-   180036356:	jae    0x180036358
-   180036358:	imul   $0x6e006f,(%rax),%eax
-   18003635e:	add    %al,(%rax)
-   180036360:	ss add %ch,(%rsi)
-   180036363:	add    %dh,(%rsi)
-   180036365:	add    %ch,(%rsi)
-   180036367:	add    %dh,(%rdx)
-   180036369:	add    %ch,(%rsi)
-   18003636b:	add    %dh,(%rax)
-   18003636d:	add    %al,(%rax)
-   18003636f:	add    %bl,(%rax)
-   180036371:	add    %al,(%rax)
-   180036373:	add    %al,(%rcx)
-   180036375:	add    %al,0x0(%rbx)
-   180036378:	outsl  %ds:(%rsi),(%dx)
-   180036379:	add    %ch,0x0(%rbp)
-   18003637c:	insl   (%dx),%es:(%rdi)
-   18003637d:	add    %ah,0x0(%rbp)
-   180036380:	outsb  %ds:(%rsi),(%dx)
-   180036381:	add    %dh,0x73(%rax,%rax,1)
-   180036385:	add    %al,(%rax)
-   180036387:	add    %ch,(%rax)
-   180036389:	add    %al,(%rax)
-   18003638b:	add    %al,(%rcx)
-   18003638d:	add    %cl,0x65(%rax,%rax,1)
-   180036391:	add    %ah,0x0(%rdi)
+   180036263:	add    %dl,0x68(%rax,%rax,1)
+   180036267:	add    %ah,0x0(%rbp)
+   18003626a:	and    %al,(%rax)
+   18003626c:	push   %rcx
+   18003626d:	add    %dh,0x20(%rax,%rax,1)
+   180036271:	add    %al,0x0(%rbx)
+   180036274:	outsl  %ds:(%rsi),(%dx)
+   180036275:	add    %ch,0x0(%rbp)
+   180036278:	jo     0x18003627a
+   18003627a:	(bad)
+   18003627b:	add    %ch,0x0(%rsi)
+   18003627e:	jns    0x180036280
+   180036280:	and    %al,(%rax)
+   180036282:	rex.WR add %r14b,0x64(%rax,%rax,1)
+   180036287:	add    %ch,(%rsi)
+   180036289:	add    %ah,(%rax)
+   18003628b:	add    %ah,0x0(%rcx)
+   18003628e:	outsb  %ds:(%rsi),(%dx)
+   18003628f:	add    %ah,0x20(%rax,%rax,1)
+   180036293:	add    %ch,0x0(%rdi)
+   180036296:	je     0x180036298
+   180036298:	push   $0x72006500
+   18003629d:	add    %ah,(%rax)
+   18003629f:	add    %ah,0x0(%rbx)
+   1800362a2:	outsl  %ds:(%rsi),(%dx)
+   1800362a3:	add    %ch,0x0(%rsi)
+   1800362a6:	je     0x1800362a8
+   1800362a8:	jb     0x1800362aa
+   1800362aa:	imul   $0x750062,(%rax),%eax
+   1800362b0:	je     0x1800362b2
+   1800362b2:	outsl  %ds:(%rsi),(%dx)
+   1800362b3:	add    %dh,0x0(%rdx)
+   1800362b6:	jae    0x1800362b8
+   1800362b8:	cs add %al,(%rax)
+   1800362bb:	add    %cl,0x0(%rsi)
+   1800362be:	adc    (%rax),%eax
+   1800362c0:	add    %eax,(%rax)
+   1800362c2:	rex.WRXB add %r14b,0x0(%r10)
+   1800362c6:	imul   $0x690067,(%rax),%eax
+   1800362cc:	outsb  %ds:(%rsi),(%dx)
+   1800362cd:	add    %ah,0x0(%rcx)
+   1800362d0:	insb   (%dx),%es:(%rdi)
+   1800362d1:	add    %al,0x0(%rsi)
+   1800362d4:	imul   $0x65006c,(%rax),%eax
+   1800362da:	outsb  %ds:(%rsi),(%dx)
+   1800362db:	add    %ah,0x0(%rcx)
+   1800362de:	insl   (%dx),%es:(%rdi)
+   1800362df:	add    %ah,0x0(%rbp)
+   1800362e2:	add    %al,(%rax)
+   1800362e4:	push   %rcx
+   1800362e5:	add    %dh,0x36(%rax,%rax,1)
+   1800362e9:	add    %cl,0x0(%rsi)
+   1800362ec:	add    %dh,%gs:0x77(%rax,%rax,1)
+   1800362f1:	add    %ch,0x0(%rdi)
+   1800362f4:	jb     0x1800362f6
+   1800362f6:	imul   $0x41,(%rax),%eax
+   1800362f9:	add    %dh,0x0(%rbp)
+   1800362fc:	je     0x1800362fe
+   1800362fe:	push   $0x64002e00
+   180036303:	add    %ch,0x6c(%rax,%rax,1)
+   180036307:	add    %al,(%rax)
+   180036309:	add    %al,(%rax)
+   18003630b:	add    %ch,(%rax)
+   18003630d:	add    %al,(%rax,%rax,1)
+   180036310:	add    %eax,(%rax)
+   180036312:	push   %rax
+   180036313:	add    %dh,0x0(%rdx)
+   180036316:	outsl  %ds:(%rsi),(%dx)
+   180036317:	add    %ah,0x75(%rax,%rax,1)
+   18003631b:	add    %ah,0x0(%rbx)
+   18003631e:	je     0x180036320
+   180036320:	rex.WRX add %r12b,0x0(%rcx)
+   180036324:	insl   (%dx),%es:(%rdi)
+   180036325:	add    %ah,0x0(%rbp)
+   180036328:	add    %al,(%rax)
+   18003632a:	add    %al,(%rax)
+   18003632c:	push   %rcx
+   18003632d:	add    %dh,0x36(%rax,%rax,1)
+   180036331:	add    %al,(%rax)
+   180036333:	add    %dh,(%rax,%rax,1)
+   180036336:	or     %al,(%rax)
+   180036338:	add    %eax,(%rax)
+   18003633a:	push   %rax
+   18003633b:	add    %dh,0x0(%rdx)
+   18003633e:	outsl  %ds:(%rsi),(%dx)
+   18003633f:	add    %ah,0x75(%rax,%rax,1)
+   180036343:	add    %ah,0x0(%rbx)
+   180036346:	je     0x180036348
+   180036348:	push   %rsi
+   180036349:	add    %ah,0x0(%rbp)
+   18003634c:	jb     0x18003634e
+   18003634e:	jae    0x180036350
+   180036350:	imul   $0x6e006f,(%rax),%eax
+   180036356:	add    %al,(%rax)
+   180036358:	ss add %ch,(%rsi)
+   18003635b:	add    %dh,(%rsi)
+   18003635d:	add    %ch,(%rsi)
+   18003635f:	add    %dh,(%rbx)
+   180036361:	add    %ch,(%rsi)
+   180036363:	add    %dh,(%rax)
+   180036365:	add    %al,(%rax)
+   180036367:	add    %bl,(%rax)
+   180036369:	add    %al,(%rax)
+   18003636b:	add    %al,(%rcx)
+   18003636d:	add    %al,0x0(%rbx)
+   180036370:	outsl  %ds:(%rsi),(%dx)
+   180036371:	add    %ch,0x0(%rbp)
+   180036374:	insl   (%dx),%es:(%rdi)
+   180036375:	add    %ah,0x0(%rbp)
+   180036378:	outsb  %ds:(%rsi),(%dx)
+   180036379:	add    %dh,0x73(%rax,%rax,1)
+   18003637d:	add    %al,(%rax)
+   18003637f:	add    %ch,(%rax)
+   180036381:	add    %al,(%rax)
+   180036383:	add    %al,(%rcx)
+   180036385:	add    %cl,0x65(%rax,%rax,1)
+   180036389:	add    %ah,0x0(%rdi)
+   18003638c:	(bad)
+   18003638d:	add    %ch,0x54(%rax,%rax,1)
+   180036391:	add    %dh,0x0(%rdx)
    180036394:	(bad)
-   180036395:	add    %ch,0x54(%rax,%rax,1)
-   180036399:	add    %dh,0x0(%rdx)
+   180036395:	add    %ah,0x65(%rax,%rax,1)
+   180036399:	add    %ch,0x0(%rbp)
    18003639c:	(bad)
-   18003639d:	add    %ah,0x65(%rax,%rax,1)
-   1800363a1:	add    %ch,0x0(%rbp)
-   1800363a4:	(bad)
-   1800363a5:	add    %dh,0x0(%rdx)
-   1800363a8:	imul   $0x73,(%rax),%eax
-   1800363ab:	add    %al,(%rax)
-   1800363ad:	add    %al,(%rax)
-   1800363af:	add    %ah,(%rax)
-   1800363b1:	add    %al,(%rax)
-   1800363b3:	add    %al,(%rcx)
-   1800363b5:	add    %cl,0x0(%rcx)
+   18003639d:	add    %dh,0x0(%rdx)
+   1800363a0:	imul   $0x73,(%rax),%eax
+   1800363a3:	add    %al,(%rax)
+   1800363a5:	add    %al,(%rax)
+   1800363a7:	add    %ah,(%rax)
+   1800363a9:	add    %al,(%rax)
+   1800363ab:	add    %al,(%rcx)
+   1800363ad:	add    %cl,0x0(%rcx)
+   1800363b0:	outsb  %ds:(%rsi),(%dx)
+   1800363b1:	add    %dh,0x65(%rax,%rax,1)
+   1800363b5:	add    %dh,0x0(%rdx)
    1800363b8:	outsb  %ds:(%rsi),(%dx)
-   1800363b9:	add    %dh,0x65(%rax,%rax,1)
-   1800363bd:	add    %dh,0x0(%rdx)
-   1800363c0:	outsb  %ds:(%rsi),(%dx)
-   1800363c1:	add    %ah,0x0(%rcx)
-   1800363c4:	insb   (%dx),%es:(%rdi)
-   1800363c5:	add    %cl,0x0(%rsi)
-   1800363c8:	(bad)
-   1800363c9:	add    %ch,0x0(%rbp)
-   1800363cc:	add    %al,%gs:(%rax)
-   1800363cf:	add    %al,0x0(%rax,%rax,1)
-   1800363d3:	add    %al,(%rcx)
-   1800363d5:	add    %dl,0x0(%rsi)
-   1800363d8:	(bad)
-   1800363d9:	add    %dh,0x0(%rdx)
-   1800363dc:	rex.RX add %r13b,0x0(%rcx)
-   1800363e0:	insb   (%dx),%es:(%rdi)
-   1800363e1:	add    %ah,0x0(%rbp)
-   1800363e4:	rex.WB add %bpl,0x0(%r14)
-   1800363e8:	data16 add %ch,0x0(%rdi)
+   1800363b9:	add    %ah,0x0(%rcx)
+   1800363bc:	insb   (%dx),%es:(%rdi)
+   1800363bd:	add    %cl,0x0(%rsi)
+   1800363c0:	(bad)
+   1800363c1:	add    %ch,0x0(%rbp)
+   1800363c4:	add    %al,%gs:(%rax)
+   1800363c7:	add    %al,0x0(%rax,%rax,1)
+   1800363cb:	add    %al,(%rcx)
+   1800363cd:	add    %dl,0x0(%rsi)
+   1800363d0:	(bad)
+   1800363d1:	add    %dh,0x0(%rdx)
+   1800363d4:	rex.RX add %r13b,0x0(%rcx)
+   1800363d8:	insb   (%dx),%es:(%rdi)
+   1800363d9:	add    %ah,0x0(%rbp)
+   1800363dc:	rex.WB add %bpl,0x0(%r14)
+   1800363e0:	data16 add %ch,0x0(%rdi)
+   1800363e4:	add    %al,(%rax)
+   1800363e6:	add    %al,(%rax)
+   1800363e8:	and    $0x0,%al
+   1800363ea:	add    $0x0,%al
    1800363ec:	add    %al,(%rax)
-   1800363ee:	add    %al,(%rax)
-   1800363f0:	and    $0x0,%al
-   1800363f2:	add    $0x0,%al
-   1800363f4:	add    %al,(%rax)
-   1800363f6:	push   %rsp
-   1800363f7:	add    %dh,0x0(%rdx)
-   1800363fa:	(bad)
-   1800363fb:	add    %ch,0x0(%rsi)
-   1800363fe:	jae    0x180036400
-   180036400:	insb   (%dx),%es:(%rdi)
-   180036401:	add    %ah,0x0(%rcx)
-   180036404:	je     0x180036406
-   180036406:	imul   $0x6e006f,(%rax),%eax
-   18003640c:	add    %al,(%rax)
-   18003640e:	add    %al,(%rax)
-   180036410:	or     %eax,(%rax,%rsi,4)
-   180036413:	add    $0x0,%al
-   180036415:	add    %al,(%rax)
-   180036417:	add    %bh,(%rdi,%rdi,1)
-   18003641a:	js     0x180036489
-   18003641c:	insb   (%dx),%es:(%rdi)
-   18003641d:	and    %dh,0x65(%rsi)
-   180036420:	jb     0x180036495
-   180036422:	imul   $0x2e31273d,0x6e(%rdi),%ebp
-   180036429:	xor    %ah,(%rdi)
-   18003642b:	and    %ah,0x6e(%rbp)
-   18003642e:	movsxd 0x64(%rdi),%ebp
-   180036431:	imul   $0x5455273d,0x67(%rsi),%ebp
-   180036438:	rex.RX sub $0x73202738,%eax
-   18003643e:	je     0x1800364a1
-   180036440:	outsb  %ds:(%rsi),(%dx)
-   180036441:	fs (bad)
-   180036443:	insb   (%dx),%es:(%rdi)
-   180036444:	outsl  %ds:(%rsi),(%dx)
-   180036445:	outsb  %ds:(%rsi),(%dx)
-   180036446:	gs cmp $0x73657927,%eax
-   18003644c:	(bad)
-   18003644d:	(bad)
-   18003644e:	ds or  $0x73613c0a,%eax
-   180036454:	jae    0x1800364bb
-   180036456:	insl   (%dx),%es:(%rdi)
-   180036457:	(bad)
-   18003645a:	and    %bh,0x6d(%rax)
-   18003645d:	insb   (%dx),%es:(%rdi)
-   18003645e:	outsb  %ds:(%rsi),(%dx)
-   18003645f:	jae    0x18003649e
-   180036461:	(bad)
-   180036462:	jne    0x1800364d6
-   180036464:	outsb  %ds:(%rsi),(%dx)
-   180036465:	cmp    0x63(%rbx),%dh
-   180036468:	push   $0x73616d65
-   18003646d:	sub    $0x7263696d,%eax
-   180036472:	outsl  %ds:(%rsi),(%dx)
-   180036473:	jae    0x1800364e4
-   180036475:	data16 je 0x1800364a5
-   180036478:	movsxd 0x6d(%rdi),%ebp
-   18003647b:	cmp    0x73(%rcx),%ah
-   18003647e:	insl   (%dx),%es:(%rdi)
-   18003647f:	jbe,pn 0x1800364b3
-   180036482:	(bad)
-   180036483:	and    %ch,0x61(%rbp)
-   180036486:	outsb  %ds:(%rsi),(%dx)
-   180036487:	imul   $0x65567473,0x65(%rsi),%esp
-   18003648e:	jb     0x180036503
-   180036490:	imul   $0x2e31273d,0x6e(%rdi),%ebp
-   180036497:	xor    %ah,(%rdi)
-   180036499:	ds or  $0x3c20200a,%eax
-   18003649f:	je     0x180036513
-   1800364a1:	jne    0x180036516
-   1800364a3:	je     0x1800364ee
-   1800364a5:	outsb  %ds:(%rsi),(%dx)
-   1800364a6:	outsw  %ds:(%rsi),(%dx)
-   1800364a8:	and    %bh,0x6d(%rax)
-   1800364ab:	insb   (%dx),%es:(%rdi)
-   1800364ac:	outsb  %ds:(%rsi),(%dx)
-   1800364ad:	jae    0x1800364ec
-   1800364af:	and    0x72(%rbp),%dh
-   1800364b2:	outsb  %ds:(%rsi),(%dx)
-   1800364b3:	cmp    0x63(%rbx),%dh
-   1800364b6:	push   $0x73616d65
-   1800364bb:	sub    $0x7263696d,%eax
-   1800364c0:	outsl  %ds:(%rsi),(%dx)
-   1800364c1:	jae    0x180036532
-   1800364c3:	data16 je 0x1800364f3
-   1800364c6:	movsxd 0x6d(%rdi),%ebp
-   1800364c9:	cmp    0x73(%rcx),%ah
-   1800364cc:	insl   (%dx),%es:(%rdi)
-   1800364cd:	jbe,pn 0x180036503
-   1800364d0:	and    (%rsi),%bh
-   1800364d2:	or     $0x2020200a,%eax
-   1800364d7:	and    %bh,(%rbx,%rsi,2)
-   1800364da:	movsxd %gs:0x72(%rbp),%esi
-   1800364de:	imul   $0x20200a0d,0x3e(%rcx,%rdi,2),%esi
-   1800364e6:	and    %ah,(%rax)
-   1800364e8:	and    %ah,(%rax)
-   1800364ea:	cmp    $0x72,%al
-   1800364ec:	gs jno 0x180036564
-   1800364ef:	gs jae 0x180036566
-   1800364f2:	gs fs push %rax
-   1800364f5:	jb     0x180036560
-   1800364f7:	jbe    0x180036562
-   1800364f9:	insb   (%dx),%es:(%rdi)
-   1800364fa:	gs addr32 gs jae 0x18003653d
-   1800364ff:	or     $0x2020200a,%eax
-   180036504:	and    %ah,(%rax)
-   180036506:	and    %ah,(%rax)
-   180036508:	and    %bh,(%rdx,%rsi,2)
-   18003650b:	gs jno 0x180036583
-   18003650e:	gs jae 0x180036585
-   180036511:	gs fs rex.RB js 0x18003657b
-   180036516:	movsxd 0x74(%rbp),%esi
-   180036519:	imul   $0x6576654c,0x6e(%rdi),%ebp
-   180036520:	insb   (%dx),%es:(%rdi)
-   180036521:	and    %ch,0x76(%rbp,%riz,2)
-   180036525:	gs insb (%dx),%es:(%rdi)
-   180036527:	cmp    $0x49736127,%eax
-   18003652c:	outsb  %ds:(%rsi),(%dx)
-   18003652d:	jbe    0x18003659e
-   18003652f:	imul   $0x27,0x72(%rbp),%esp
-   180036533:	and    %dh,0x69(%rbp)
-   180036536:	movsxd 0x65(%r11),%esp
-   18003653a:	jae    0x1800365af
-   18003653c:	cmp    $0x6c616627,%eax
-   180036541:	jae    0x1800365a8
-   180036543:	(bad)
-   180036544:	and    %ch,(%rdi)
-   180036546:	ds or  $0x2020200a,%eax
-   18003654c:	and    %ah,(%rax)
-   18003654e:	and    %bh,(%rdi,%rbp,1)
-   180036551:	jb     0x1800365b8
-   180036553:	jno    0x1800365ca
-   180036555:	gs jae 0x1800365cc
-   180036558:	gs fs push %rax
-   18003655b:	jb     0x1800365c6
-   18003655d:	jbe    0x1800365c8
-   18003655f:	insb   (%dx),%es:(%rdi)
-   180036560:	gs addr32 gs jae 0x1800365a3
-   180036565:	or     $0x2020200a,%eax
-   18003656a:	and    %bh,(%rdi,%rbp,1)
-   18003656d:	jae    0x1800365d4
-   18003656f:	movsxd 0x72(%rbp),%esi
-   180036572:	imul   $0x20200a0d,0x3e(%rcx,%rdi,2),%esi
-   18003657a:	cmp    $0x2f,%al
-   18003657c:	je     0x1800365f0
-   18003657e:	jne    0x1800365f3
-   180036580:	je     0x1800365cb
-   180036582:	outsb  %ds:(%rsi),(%dx)
-   180036583:	outsw  %ds:(%rsi),(%dx)
-   180036585:	ds or  $0x612f3c0a,%eax
-   18003658b:	jae    0x180036600
-   18003658d:	gs insl (%dx),%es:(%rdi)
-   18003658f:	(bad)  {%k6}
-   180036592:	ds or  $0xa,%eax
+   1800363ee:	push   %rsp
+   1800363ef:	add    %dh,0x0(%rdx)
+   1800363f2:	(bad)
+   1800363f3:	add    %ch,0x0(%rsi)
+   1800363f6:	jae    0x1800363f8
+   1800363f8:	insb   (%dx),%es:(%rdi)
+   1800363f9:	add    %ah,0x0(%rcx)
+   1800363fc:	je     0x1800363fe
+   1800363fe:	imul   $0x6e006f,(%rax),%eax
+   180036404:	add    %al,(%rax)
+   180036406:	add    %al,(%rax)
+   180036408:	or     %eax,(%rax,%rsi,4)
+   18003640b:	add    $0x0,%al
+   18003640d:	add    %al,(%rax)
+   18003640f:	add    %bh,(%rdi,%rdi,1)
+   180036412:	js     0x180036481
+   180036414:	insb   (%dx),%es:(%rdi)
+   180036415:	and    %dh,0x65(%rsi)
+   180036418:	jb     0x18003648d
+   18003641a:	imul   $0x2e31273d,0x6e(%rdi),%ebp
+   180036421:	xor    %ah,(%rdi)
+   180036423:	and    %ah,0x6e(%rbp)
+   180036426:	movsxd 0x64(%rdi),%ebp
+   180036429:	imul   $0x5455273d,0x67(%rsi),%ebp
+   180036430:	rex.RX sub $0x73202738,%eax
+   180036436:	je     0x180036499
+   180036438:	outsb  %ds:(%rsi),(%dx)
+   180036439:	fs (bad)
+   18003643b:	insb   (%dx),%es:(%rdi)
+   18003643c:	outsl  %ds:(%rsi),(%dx)
+   18003643d:	outsb  %ds:(%rsi),(%dx)
+   18003643e:	gs cmp $0x73657927,%eax
+   180036444:	(bad)
+   180036445:	(bad)
+   180036446:	ds or  $0x73613c0a,%eax
+   18003644c:	jae    0x1800364b3
+   18003644e:	insl   (%dx),%es:(%rdi)
+   18003644f:	(bad)
+   180036452:	and    %bh,0x6d(%rax)
+   180036455:	insb   (%dx),%es:(%rdi)
+   180036456:	outsb  %ds:(%rsi),(%dx)
+   180036457:	jae    0x180036496
+   180036459:	(bad)
+   18003645a:	jne    0x1800364ce
+   18003645c:	outsb  %ds:(%rsi),(%dx)
+   18003645d:	cmp    0x63(%rbx),%dh
+   180036460:	push   $0x73616d65
+   180036465:	sub    $0x7263696d,%eax
+   18003646a:	outsl  %ds:(%rsi),(%dx)
+   18003646b:	jae    0x1800364dc
+   18003646d:	data16 je 0x18003649d
+   180036470:	movsxd 0x6d(%rdi),%ebp
+   180036473:	cmp    0x73(%rcx),%ah
+   180036476:	insl   (%dx),%es:(%rdi)
+   180036477:	jbe,pn 0x1800364ab
+   18003647a:	(bad)
+   18003647b:	and    %ch,0x61(%rbp)
+   18003647e:	outsb  %ds:(%rsi),(%dx)
+   18003647f:	imul   $0x65567473,0x65(%rsi),%esp
+   180036486:	jb     0x1800364fb
+   180036488:	imul   $0x2e31273d,0x6e(%rdi),%ebp
+   18003648f:	xor    %ah,(%rdi)
+   180036491:	ds or  $0x3c20200a,%eax
+   180036497:	je     0x18003650b
+   180036499:	jne    0x18003650e
+   18003649b:	je     0x1800364e6
+   18003649d:	outsb  %ds:(%rsi),(%dx)
+   18003649e:	outsw  %ds:(%rsi),(%dx)
+   1800364a0:	and    %bh,0x6d(%rax)
+   1800364a3:	insb   (%dx),%es:(%rdi)
+   1800364a4:	outsb  %ds:(%rsi),(%dx)
+   1800364a5:	jae    0x1800364e4
+   1800364a7:	and    0x72(%rbp),%dh
+   1800364aa:	outsb  %ds:(%rsi),(%dx)
+   1800364ab:	cmp    0x63(%rbx),%dh
+   1800364ae:	push   $0x73616d65
+   1800364b3:	sub    $0x7263696d,%eax
+   1800364b8:	outsl  %ds:(%rsi),(%dx)
+   1800364b9:	jae    0x18003652a
+   1800364bb:	data16 je 0x1800364eb
+   1800364be:	movsxd 0x6d(%rdi),%ebp
+   1800364c1:	cmp    0x73(%rcx),%ah
+   1800364c4:	insl   (%dx),%es:(%rdi)
+   1800364c5:	jbe,pn 0x1800364fb
+   1800364c8:	and    (%rsi),%bh
+   1800364ca:	or     $0x2020200a,%eax
+   1800364cf:	and    %bh,(%rbx,%rsi,2)
+   1800364d2:	movsxd %gs:0x72(%rbp),%esi
+   1800364d6:	imul   $0x20200a0d,0x3e(%rcx,%rdi,2),%esi
+   1800364de:	and    %ah,(%rax)
+   1800364e0:	and    %ah,(%rax)
+   1800364e2:	cmp    $0x72,%al
+   1800364e4:	gs jno 0x18003655c
+   1800364e7:	gs jae 0x18003655e
+   1800364ea:	gs fs push %rax
+   1800364ed:	jb     0x180036558
+   1800364ef:	jbe    0x18003655a
+   1800364f1:	insb   (%dx),%es:(%rdi)
+   1800364f2:	gs addr32 gs jae 0x180036535
+   1800364f7:	or     $0x2020200a,%eax
+   1800364fc:	and    %ah,(%rax)
+   1800364fe:	and    %ah,(%rax)
+   180036500:	and    %bh,(%rdx,%rsi,2)
+   180036503:	gs jno 0x18003657b
+   180036506:	gs jae 0x18003657d
+   180036509:	gs fs rex.RB js 0x180036573
+   18003650e:	movsxd 0x74(%rbp),%esi
+   180036511:	imul   $0x6576654c,0x6e(%rdi),%ebp
+   180036518:	insb   (%dx),%es:(%rdi)
+   180036519:	and    %ch,0x76(%rbp,%riz,2)
+   18003651d:	gs insb (%dx),%es:(%rdi)
+   18003651f:	cmp    $0x49736127,%eax
+   180036524:	outsb  %ds:(%rsi),(%dx)
+   180036525:	jbe    0x180036596
+   180036527:	imul   $0x27,0x72(%rbp),%esp
+   18003652b:	and    %dh,0x69(%rbp)
+   18003652e:	movsxd 0x65(%r11),%esp
+   180036532:	jae    0x1800365a7
+   180036534:	cmp    $0x6c616627,%eax
+   180036539:	jae    0x1800365a0
+   18003653b:	(bad)
+   18003653c:	and    %ch,(%rdi)
+   18003653e:	ds or  $0x2020200a,%eax
+   180036544:	and    %ah,(%rax)
+   180036546:	and    %bh,(%rdi,%rbp,1)
+   180036549:	jb     0x1800365b0
+   18003654b:	jno    0x1800365c2
+   18003654d:	gs jae 0x1800365c4
+   180036550:	gs fs push %rax
+   180036553:	jb     0x1800365be
+   180036555:	jbe    0x1800365c0
+   180036557:	insb   (%dx),%es:(%rdi)
+   180036558:	gs addr32 gs jae 0x18003659b
+   18003655d:	or     $0x2020200a,%eax
+   180036562:	and    %bh,(%rdi,%rbp,1)
+   180036565:	jae    0x1800365cc
+   180036567:	movsxd 0x72(%rbp),%esi
+   18003656a:	imul   $0x20200a0d,0x3e(%rcx,%rdi,2),%esi
+   180036572:	cmp    $0x2f,%al
+   180036574:	je     0x1800365e8
+   180036576:	jne    0x1800365eb
+   180036578:	je     0x1800365c3
+   18003657a:	outsb  %ds:(%rsi),(%dx)
+   18003657b:	outsw  %ds:(%rsi),(%dx)
+   18003657d:	ds or  $0x612f3c0a,%eax
+   180036583:	jae    0x1800365f8
+   180036585:	gs insl (%dx),%es:(%rdi)
+   180036587:	(bad)  {%k6}
+   18003658a:	ds or  $0xa,%eax
 
 Disassembly of section .reloc:
 
 0000000180037000 <.reloc>:
    180037000:	add    %al,(%rax)
    180037002:	add    (%rax),%al
    180037004:	rex.WR add %r8b,(%rax)
```

## Comparing `PyQt6_NetworkAuth_Qt6-6.6.2.dist-info/LICENSE` & `PyQt6_NetworkAuth_Qt6-6.6.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `PyQt6_NetworkAuth_Qt6-6.6.2.dist-info/METADATA` & `PyQt6_NetworkAuth_Qt6-6.6.3.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-NetworkAuth-Qt6
-Version: 6.6.2
+Version: 6.6.3
 Summary: The subset of a Qt installation needed by PyQt6-NetworkAuth.
 Home-page: https://www.riverbankcomputing.com/software/pyqt/
 Author: Riverbank Computing Limited
 Author-email: info@riverbankcomputing.com
 License: GPL v3
 Platform: Linux
 Platform: macOS
```

