# Comparing `tmp/musicAlgLib-1.0.6.tar.gz` & `tmp/musicAlgLib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicAlgLib-1.0.6.tar", last modified: Tue Apr  2 12:07:27 2024, max compression
+gzip compressed data, was "musicAlgLib-1.0.7.tar", last modified: Wed Apr  3 07:50:47 2024, max compression
```

## Comparing `musicAlgLib-1.0.6.tar` & `musicAlgLib-1.0.7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.722778 musicAlgLib-1.0.6/
--rw-rw-rw-   0        0        0     4676 2024-04-02 12:07:27.722282 musicAlgLib-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.689050 musicAlgLib-1.0.6/musicAlgLib/
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.693018 musicAlgLib-1.0.6/musicAlgLib/AGC_EVALUATION/
--rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/AGC_EVALUATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.693514 musicAlgLib-1.0.6/musicAlgLib/CLIPPING_DETECTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/CLIPPING_DETECTION/__init__.py
--rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.704426 musicAlgLib-1.0.6/musicAlgLib/DLLS/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/__init__.py
--rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/cygwin1.dll
--rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/matchsig.dll
--rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/matchsig.dylib
--rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/matchsig.so
--rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/musicStability.dll
--rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/musicStability.dylib
--rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/musicStability.so
--rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/pcc.dll
--rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/pcc.dylib
--rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/pcc.so
--rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/peaqb.exe
--rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/silero_vad.jit
--rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/snr_music.dll
--rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/snr_music.dylib
--rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/DLLS/snr_music.so
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.704922 musicAlgLib-1.0.6/musicAlgLib/DynmicRange/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.0.6/musicAlgLib/DynmicRange/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.705418 musicAlgLib-1.0.6/musicAlgLib/FUNCTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/FUNCTION/__init__.py
--rw-rw-rw-   0        0        0    19032 2024-04-01 09:34:54.000000 musicAlgLib-1.0.6/musicAlgLib/FUNCTION/audioFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.705914 musicAlgLib-1.0.6/musicAlgLib/FrequencyResponse/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.0.6/musicAlgLib/FrequencyResponse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.706906 musicAlgLib-1.0.6/musicAlgLib/Noise_Suppression/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/Noise_Suppression/__init__.py
--rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/Noise_Suppression/noiseFuction.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.708395 musicAlgLib-1.0.6/musicAlgLib/PCC/
--rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/PCC/Pearson_CC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/PCC/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.710378 musicAlgLib-1.0.6/musicAlgLib/PEAQ/
--rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/PEAQ/PEAQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/PEAQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.710874 musicAlgLib-1.0.6/musicAlgLib/PESQ/
--rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/PESQ/PESQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/PESQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.711370 musicAlgLib-1.0.6/musicAlgLib/PLAY_DELAY/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.0.6/musicAlgLib/PLAY_DELAY/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.713850 musicAlgLib-1.0.6/musicAlgLib/POLQA/
--rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/POLQA/POLQA.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/POLQA/__init__.py
--rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/POLQA/file_server.py
--rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/POLQA/polqa_client.py
--rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/POLQA/polqa_server.py
--rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/POLQA/socketClient.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.714842 musicAlgLib-1.0.6/musicAlgLib/SNR_ESTIMATION/
--rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.0.6/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
--rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/SNR_ESTIMATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.716330 musicAlgLib-1.0.6/musicAlgLib/STI/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/STI/__init__.py
--rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/STI/cal_sti.py
--rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/STI/sti.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.716826 musicAlgLib-1.0.6/musicAlgLib/VAD_NN/
--rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.0.6/musicAlgLib/VAD_NN/__init__.py
--rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.0.6/musicAlgLib/VAD_NN/hubconf.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.717322 musicAlgLib-1.0.6/musicAlgLib/VISQOL/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.0.6/musicAlgLib/VISQOL/__init__.py
--rw-rw-rw-   0        0        0     4832 2024-04-02 06:12:21.000000 musicAlgLib-1.0.6/musicAlgLib/__init__.py
--rw-rw-rw-   0        0        0    14684 2024-01-25 06:27:05.000000 musicAlgLib-1.0.6/musicAlgLib/commFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.718810 musicAlgLib-1.0.6/musicAlgLib/computeAudioQuality/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/computeAudioQuality/__init__.py
--rw-rw-rw-   0        0        0     9563 2024-04-02 11:56:41.000000 musicAlgLib-1.0.6/musicAlgLib/computeAudioQuality/mainProcess.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.719802 musicAlgLib-1.0.6/musicAlgLib/formatConvert/
--rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/formatConvert/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/formatConvert/wav_pcm.py
--rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.720298 musicAlgLib-1.0.6/musicAlgLib/resample/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/resample/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/resample/resampler.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.721290 musicAlgLib-1.0.6/musicAlgLib/tests/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/tests/__init__.py
--rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.0.6/musicAlgLib/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.721786 musicAlgLib-1.0.6/musicAlgLib/timeAligment/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.6/musicAlgLib/timeAligment/__init__.py
--rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.0.6/musicAlgLib/timeAligment/time_align.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:07:27.692026 musicAlgLib-1.0.6/musicAlgLib.egg-info/
--rw-rw-rw-   0        0        0     4676 2024-04-02 12:07:27.000000 musicAlgLib-1.0.6/musicAlgLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2227 2024-04-02 12:07:27.000000 musicAlgLib-1.0.6/musicAlgLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:07:27.000000 musicAlgLib-1.0.6/musicAlgLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-02 12:07:27.000000 musicAlgLib-1.0.6/musicAlgLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 12:07:27.000000 musicAlgLib-1.0.6/musicAlgLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 12:07:27.722778 musicAlgLib-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     5840 2024-04-02 12:07:22.000000 musicAlgLib-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.297806 musicAlgLib-1.0.7/
+-rw-rw-rw-   0        0        0     4676 2024-04-03 07:50:47.297310 musicAlgLib-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.265071 musicAlgLib-1.0.7/musicAlgLib/
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.269038 musicAlgLib-1.0.7/musicAlgLib/AGC_EVALUATION/
+-rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/AGC_EVALUATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.269534 musicAlgLib-1.0.7/musicAlgLib/CLIPPING_DETECTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/CLIPPING_DETECTION/__init__.py
+-rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.280446 musicAlgLib-1.0.7/musicAlgLib/DLLS/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/__init__.py
+-rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/cygwin1.dll
+-rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.dll
+-rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.dylib
+-rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.so
+-rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.dll
+-rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.dylib
+-rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.so
+-rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.dll
+-rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.dylib
+-rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.so
+-rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/peaqb.exe
+-rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/silero_vad.jit
+-rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.dll
+-rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.dylib
+-rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.so
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.280942 musicAlgLib-1.0.7/musicAlgLib/DynmicRange/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.0.7/musicAlgLib/DynmicRange/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.281438 musicAlgLib-1.0.7/musicAlgLib/FUNCTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/FUNCTION/__init__.py
+-rw-rw-rw-   0        0        0    19268 2024-04-03 07:50:07.000000 musicAlgLib-1.0.7/musicAlgLib/FUNCTION/audioFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.281934 musicAlgLib-1.0.7/musicAlgLib/FrequencyResponse/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.0.7/musicAlgLib/FrequencyResponse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.282926 musicAlgLib-1.0.7/musicAlgLib/Noise_Suppression/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/Noise_Suppression/__init__.py
+-rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/Noise_Suppression/noiseFuction.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.283422 musicAlgLib-1.0.7/musicAlgLib/PCC/
+-rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PCC/Pearson_CC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PCC/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.284414 musicAlgLib-1.0.7/musicAlgLib/PEAQ/
+-rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PEAQ/PEAQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PEAQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.285406 musicAlgLib-1.0.7/musicAlgLib/PESQ/
+-rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PESQ/PESQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PESQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.285902 musicAlgLib-1.0.7/musicAlgLib/PLAY_DELAY/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.0.7/musicAlgLib/PLAY_DELAY/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.288382 musicAlgLib-1.0.7/musicAlgLib/POLQA/
+-rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/POLQA.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/__init__.py
+-rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/file_server.py
+-rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/polqa_client.py
+-rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/polqa_server.py
+-rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/socketClient.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.289870 musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/
+-rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
+-rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.290862 musicAlgLib-1.0.7/musicAlgLib/STI/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/STI/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/STI/cal_sti.py
+-rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/STI/sti.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.291854 musicAlgLib-1.0.7/musicAlgLib/VAD_NN/
+-rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.0.7/musicAlgLib/VAD_NN/__init__.py
+-rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.0.7/musicAlgLib/VAD_NN/hubconf.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.292350 musicAlgLib-1.0.7/musicAlgLib/VISQOL/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.0.7/musicAlgLib/VISQOL/__init__.py
+-rw-rw-rw-   0        0        0     4781 2024-04-03 07:50:07.000000 musicAlgLib-1.0.7/musicAlgLib/__init__.py
+-rw-rw-rw-   0        0        0    15523 2024-04-03 07:50:07.000000 musicAlgLib-1.0.7/musicAlgLib/commFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.292846 musicAlgLib-1.0.7/musicAlgLib/computeAudioQuality/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/computeAudioQuality/__init__.py
+-rw-rw-rw-   0        0        0    11369 2024-04-03 07:50:07.000000 musicAlgLib-1.0.7/musicAlgLib/computeAudioQuality/mainProcess.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.294334 musicAlgLib-1.0.7/musicAlgLib/formatConvert/
+-rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/formatConvert/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/formatConvert/wav_pcm.py
+-rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/main.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.295326 musicAlgLib-1.0.7/musicAlgLib/resample/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/resample/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/resample/resampler.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.296318 musicAlgLib-1.0.7/musicAlgLib/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/tests/__init__.py
+-rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.0.7/musicAlgLib/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.296814 musicAlgLib-1.0.7/musicAlgLib/timeAligment/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/timeAligment/__init__.py
+-rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.0.7/musicAlgLib/timeAligment/time_align.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.268046 musicAlgLib-1.0.7/musicAlgLib.egg-info/
+-rw-rw-rw-   0        0        0     4676 2024-04-03 07:50:47.000000 musicAlgLib-1.0.7/musicAlgLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2227 2024-04-03 07:50:47.000000 musicAlgLib-1.0.7/musicAlgLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 07:50:47.000000 musicAlgLib-1.0.7/musicAlgLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-03 07:50:47.000000 musicAlgLib-1.0.7/musicAlgLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 07:50:47.000000 musicAlgLib-1.0.7/musicAlgLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 07:50:47.297806 musicAlgLib-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     5840 2024-04-03 07:50:16.000000 musicAlgLib-1.0.7/setup.py
```

### Comparing `musicAlgLib-1.0.6/PKG-INFO` & `musicAlgLib-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.0.6
+Version: 1.0.7
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.0.6/README.md` & `musicAlgLib-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py` & `musicAlgLib-1.0.7/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py` & `musicAlgLib-1.0.7/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/cygwin1.dll` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/matchsig.dll` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/matchsig.dylib` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/matchsig.so` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/musicStability.dll` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/musicStability.dylib` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/musicStability.so` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/pcc.dll` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/pcc.dylib` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/pcc.so` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/peaqb.exe` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/peaqb.exe`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/silero_vad.jit` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/silero_vad.jit`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/snr_music.dll` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/snr_music.dylib` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/DLLS/snr_music.so` & `musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/FUNCTION/audioFunction.py` & `musicAlgLib-1.0.7/musicAlgLib/FUNCTION/audioFunction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import wave
 import sys,os
 from os import  path
 sys.path.append(path.dirname(__file__))
 sys.path.append(os.path.dirname(path.dirname(__file__)))
 from moviepy.editor import AudioFileClip
-from commFunction import get_rms,get_ave_rms,get_one_channel_data,get_file_duration,get_data_array,get_peak_rms,get_std_rms,get_duration_above_specific_rms
+from commFunction import get_rms,get_ave_rms,get_one_channel_data,get_file_duration,get_data_array,get_peak_rms,get_std_rms,get_duration_above_specific_rms,get_max_rms,get_min_rms
 from formatConvert import pcm2wav
 import numpy as np
 import scipy.signal as signal
 import math
 import librosa
 from PCC.Pearson_CC import get_max_cc_by_dll
 import ctypes,os,platform
@@ -154,14 +154,20 @@
         return get_rms(curdata)
     if rmsMode == 'average':
         return get_ave_rms(curdata)
     if rmsMode == 'peak':
         return  get_peak_rms(curdata)
     if rmsMode == 'std':
         return  get_std_rms(curdata)
+    if rmsMode == 'max':
+        return  get_max_rms(curdata)
+    if rmsMode == 'min':
+        return  get_min_rms(curdata)
+    if rmsMode == 'dynmic':
+        return  get_max_rms(curdata) - get_min_rms(curdata)
     if rmsMode == 'duration':
         return  get_duration_above_specific_rms(curdata)
     return None
 
 
 
 def calculate_band_energy(audio_signal, sample_rate, num_bands,freq_mode='upper'):
```

### Comparing `musicAlgLib-1.0.6/musicAlgLib/Noise_Suppression/noiseFuction.py` & `musicAlgLib-1.0.7/musicAlgLib/Noise_Suppression/noiseFuction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/PCC/Pearson_CC.py` & `musicAlgLib-1.0.7/musicAlgLib/PCC/Pearson_CC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/PESQ/PESQ.py` & `musicAlgLib-1.0.7/musicAlgLib/PESQ/PESQ.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/POLQA/POLQA.py` & `musicAlgLib-1.0.7/musicAlgLib/POLQA/POLQA.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/POLQA/file_server.py` & `musicAlgLib-1.0.7/musicAlgLib/POLQA/file_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/POLQA/polqa_client.py` & `musicAlgLib-1.0.7/musicAlgLib/POLQA/polqa_client.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/POLQA/polqa_server.py` & `musicAlgLib-1.0.7/musicAlgLib/POLQA/polqa_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/POLQA/socketClient.py` & `musicAlgLib-1.0.7/musicAlgLib/POLQA/socketClient.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py` & `musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py` & `musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/STI/cal_sti.py` & `musicAlgLib-1.0.7/musicAlgLib/STI/cal_sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/STI/sti.py` & `musicAlgLib-1.0.7/musicAlgLib/STI/sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/VAD_NN/hubconf.py` & `musicAlgLib-1.0.7/musicAlgLib/VAD_NN/hubconf.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/__init__.py` & `musicAlgLib-1.0.7/musicAlgLib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 from .computeAudioQuality.mainProcess import computeAudioQuality
 
 from ctypes import  *
 
 def compute_music_quality(metrics,testFile=None,refFile=None,outFile=None,audioType=1,
                          rmsCalsection=None,polqaMode=0,pitchLogMode=1,fineDelaySection=None,rmsSpeechOnly=False):
     """
-    :param metrics: POLQA/PESQ/STI/PEAQ/SDR/SII/LOUDNESS/MUSIC/MATCH/
-                    TRANSIENT/GAINTABLE/ATTACKRELEASE/MUSICSTA/AGCDELAY/MATCHAEC/
-                    ERLE/SLIENCE/FORMAT/AECMOS/AIMOS/TRMS/ARMS/PRMS/SRMS/LRATE/NOISE/CLIP/DELAY/ECHO/SPEC/PITCH/EQ，必选项
+    :param metrics: ['ALL','POLQA','PEAQ','LOUDNESS','MUSIC','MATCH','MUSICSTA','SLIENCE','FORMAT','TOTALRMS','AVERMS','PEAKRMS','STDRMS','MAXRMS','MINRMS','DYNMIC','LRATE','CLIP','DELAY','SPEC','PITCH','EQ','MATCH2','MATCH3']
+
     #
     # POLQA 窄带模式  8k  超宽带模式 48k ；WAV/PCM输入 ；双端输入：ref、test；时长 < 20s；
     # PEAQ 无采样率限制；WAV/PCM输入 ；双端输入：ref、test；无时间长度要求；
     # MATCH 无采样率限制; WAV/PCM输入;三端输入：ref、test、out； 无时间长度要求；
     # MUSIC 无采样率限制;WAV/PCM输入;双端输入：ref、test；无时间长度要求；
     # MUSICSTA 无采样率限制,WAV/PCM输入;双端输入：ref、test；无时间长度要求；
     # SLIENCE 无采样率限制 WAV/PCM/MP4输入;单端输入：test；无时间长度要求；
```

### Comparing `musicAlgLib-1.0.6/musicAlgLib/commFunction.py` & `musicAlgLib-1.0.7/musicAlgLib/commFunction.py`

 * *Files 7% similar despite different names*

```diff
@@ -429,33 +429,72 @@
     data = records.astype(np.float32).tolist()
     if len(data) == 0:
         return -99.9
     rms = math.sqrt(sum([(x/32767) * (x/32767) for x in data])/len(data))
     dBrmsValue = 20*math.log10(rms + 1.0E-6)
     return dBrmsValue
 
+
 def get_peak_rms(records):
     '''
     Parameters
     ----------
     records
 
     Returns
     -------
     '''
     #return math.sqrt(sum([x * x for x in records])/len(records))
-    frameLen = 480
+    frameLen = 1
     nFrames = len(records)//frameLen
     maxRms = -99
     for a in range(nFrames):
         curRms = get_rms(records[a*frameLen:(a+1)*frameLen])
         if curRms > maxRms:
             maxRms = curRms
     return maxRms
 
+def get_max_rms(records):
+    '''
+    Parameters
+    ----------
+    records
+
+    Returns
+    -------
+    '''
+    #return math.sqrt(sum([x * x for x in records])/len(records))
+    frameLen = 2400 #50ms
+    nFrames = len(records)//frameLen
+    maxRms = -99
+    for a in range(nFrames):
+        curRms = get_rms(records[a*frameLen:(a+1)*frameLen])
+        if curRms > maxRms:
+            maxRms = curRms
+    return maxRms
+
+def get_min_rms(records):
+    '''
+    Parameters
+    ----------
+    records
+
+    Returns
+    -------
+    '''
+    #return math.sqrt(sum([x * x for x in records])/len(records))
+    frameLen = 2400 #50ms
+    nFrames = len(records)//frameLen
+    minrms = 100
+    for a in range(nFrames):
+        curRms = get_rms(records[a*frameLen:(a+1)*frameLen])
+        if curRms < minrms:
+            minrms = curRms
+    return minrms
+
 def get_one_channel_data(infile):
     """
     :return:
     """
     data, fs, chn = get_data_array(infile)
     if fs == 48000 and chn == 1:
         return data
```

### Comparing `musicAlgLib-1.0.6/musicAlgLib/computeAudioQuality/mainProcess.py` & `musicAlgLib-1.0.7/musicAlgLib/computeAudioQuality/mainProcess.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from SNR_ESTIMATION.MATCH_SIG import match_sig
 from SNR_ESTIMATION.SNR_MUSIC import cal_snr_music
 from AGC_EVALUATION.CAL_MUSIC_STABILITY import cal_music_stablility
 from FUNCTION.audioFunction import isSlience,audioFormat,get_rms_level,get_effective_spectral,cal_pitch,cal_EQ
 from CLIPPING_DETECTION.audio_clip_detection import cal_clip_index
 from commFunction import make_out_file,get_data_array
 
-allMetrics = ['ALL','POLQA','PEAQ','LOUDNESS','MUSIC','MATCH','MUSICSTA','SLIENCE','FORMAT','TRMS','ARMS','PRMS','SRMS','LRATE','CLIP','DELAY','SPEC','PITCH','EQ','MATCH2','MATCH3']
+allMetrics = ['ALL','POLQA','PEAQ','LOUDNESS','MUSIC','MATCH','MUSICSTA','SLIENCE','FORMAT','TOTALRMS','AVERMS','PEAKRMS','STDRMS','MAXRMS','MINRMS','DYNMIC','LRATE','CLIP','DELAY','SPEC','PITCH','EQ','MATCH2','MATCH3']
 
 
 class computeAudioQuality():
     def __init__(self,**kwargs):
         """
         :param kwargs:
         """
@@ -211,52 +211,87 @@
         Returns
         -------
 
         """
         return audioFormat(self.testFile)
 
 
-    def TRMS(self):
+    def TOTALRMS(self):
         """
         Returns
         -------
         # (wavFileName=None,rmsMode='total',startTime=0,endTime=1):
         """
 
 
         return get_rms_level(wavFileName=self.testFile_L, rmsMode='total', section=self.rmsCalsection,
                              speechOnly=self.rmsSpeechOnly), get_rms_level(wavFileName=self.testFile_R, rmsMode='total',
                                                                            section=self.rmsCalsection,
                                                                            speechOnly=self.rmsSpeechOnly)
 
-    def PRMS(self):
+    def PEAKRMS(self):
         """
         Returns
         -------
         # (wavFileName=None,rmsMode='total',startTime=0,endTime=1):
         """
         return get_rms_level(wavFileName=self.testFile_L,rmsMode='peak',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly),get_rms_level(wavFileName=self.testFile_R,rmsMode='peak',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly)
 
-    def SRMS(self):
+    def STDRMS(self):
         """
         Returns
         -------
         # (wavFileName=None,rmsMode='total',startTime=0,endTime=1):
         """
         return get_rms_level(wavFileName=self.testFile_L,rmsMode='std',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly),get_rms_level(wavFileName=self.testFile_R,rmsMode='std',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly)
 
 
-    def ARMS(self):
+    def AVERMS(self):
         """
         Returns
         -------
 
         """
         return get_rms_level(wavFileName=self.testFile_L,rmsMode='average',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly),get_rms_level(wavFileName=self.testFile_R,rmsMode='average',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly)
 
+    def MAXRMS(self):
+        """
+        Returns
+        -------
+
+        """
+        return get_rms_level(wavFileName=self.testFile_L, rmsMode='max', section=self.rmsCalsection,
+                             speechOnly=self.rmsSpeechOnly), get_rms_level(wavFileName=self.testFile_R,
+                                                                           rmsMode='max',
+                                                                           section=self.rmsCalsection,
+                                                                           speechOnly=self.rmsSpeechOnly)
+
+    def MINRMS(self):
+        """
+        Returns
+        -------
+
+        """
+        return get_rms_level(wavFileName=self.testFile_L, rmsMode='min', section=self.rmsCalsection,
+                             speechOnly=self.rmsSpeechOnly), get_rms_level(wavFileName=self.testFile_R,
+                                                                           rmsMode='min',
+                                                                           section=self.rmsCalsection,
+                                                                           speechOnly=self.rmsSpeechOnly)
+    def DYNMIC(self):
+        """
+        Returns
+        -------
+
+        """
+        return get_rms_level(wavFileName=self.testFile_L, rmsMode='dynmic', section=self.rmsCalsection,
+                             speechOnly=self.rmsSpeechOnly), get_rms_level(wavFileName=self.testFile_R,
+                                                                           rmsMode='dynmic',
+                                                                           section=self.rmsCalsection,
+                                                                           speechOnly=self.rmsSpeechOnly)
+
 
 
     def CLIP(self):
         """
         Returns
         -------
```

### Comparing `musicAlgLib-1.0.6/musicAlgLib/formatConvert/wav_pcm.py` & `musicAlgLib-1.0.7/musicAlgLib/formatConvert/wav_pcm.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/main.py` & `musicAlgLib-1.0.7/musicAlgLib/main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/resample/resampler.py` & `musicAlgLib-1.0.7/musicAlgLib/resample/resampler.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/tests/test_main.py` & `musicAlgLib-1.0.7/musicAlgLib/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib/timeAligment/time_align.py` & `musicAlgLib-1.0.7/musicAlgLib/timeAligment/time_align.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/musicAlgLib.egg-info/PKG-INFO` & `musicAlgLib-1.0.7/musicAlgLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.0.6
+Version: 1.0.7
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.0.6/musicAlgLib.egg-info/SOURCES.txt` & `musicAlgLib-1.0.7/musicAlgLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.6/setup.py` & `musicAlgLib-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setup(
     name='musicAlgLib',
-    version='1.0.06',
+    version='1.0.07',
     packages=setuptools.find_packages(),
     url='https://github.com/pypa/sampleproject',
     license='MIT',
     author=' MA JIANLI',
     author_email='majianli@corp.netease.com',
     description='audio algorithms to compute and test music quality',
     long_description="""
```

