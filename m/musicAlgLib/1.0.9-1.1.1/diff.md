# Comparing `tmp/musicAlgLib-1.0.9.tar.gz` & `tmp/musicAlgLib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicAlgLib-1.0.9.tar", last modified: Wed Apr  3 08:15:20 2024, max compression
+gzip compressed data, was "musicAlgLib-1.1.1.tar", last modified: Wed Apr  3 08:35:19 2024, max compression
```

## Comparing `musicAlgLib-1.0.9.tar` & `musicAlgLib-1.1.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.809568 musicAlgLib-1.0.9/
--rw-rw-rw-   0        0        0     4676 2024-04-03 08:15:20.809072 musicAlgLib-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.776336 musicAlgLib-1.0.9/musicAlgLib/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.779808 musicAlgLib-1.0.9/musicAlgLib/AGC_EVALUATION/
--rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/AGC_EVALUATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.780800 musicAlgLib-1.0.9/musicAlgLib/CLIPPING_DETECTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/CLIPPING_DETECTION/__init__.py
--rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.791712 musicAlgLib-1.0.9/musicAlgLib/DLLS/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/__init__.py
--rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/cygwin1.dll
--rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/matchsig.dll
--rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/matchsig.dylib
--rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/matchsig.so
--rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/musicStability.dll
--rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/musicStability.dylib
--rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/musicStability.so
--rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/pcc.dll
--rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/pcc.dylib
--rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/pcc.so
--rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/peaqb.exe
--rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/silero_vad.jit
--rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/snr_music.dll
--rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/snr_music.dylib
--rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/DLLS/snr_music.so
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.792208 musicAlgLib-1.0.9/musicAlgLib/DynmicRange/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.0.9/musicAlgLib/DynmicRange/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.793200 musicAlgLib-1.0.9/musicAlgLib/FUNCTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/FUNCTION/__init__.py
--rw-rw-rw-   0        0        0    19268 2024-04-03 07:50:07.000000 musicAlgLib-1.0.9/musicAlgLib/FUNCTION/audioFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.793696 musicAlgLib-1.0.9/musicAlgLib/FrequencyResponse/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.0.9/musicAlgLib/FrequencyResponse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.794192 musicAlgLib-1.0.9/musicAlgLib/Noise_Suppression/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/Noise_Suppression/__init__.py
--rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/Noise_Suppression/noiseFuction.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.795184 musicAlgLib-1.0.9/musicAlgLib/PCC/
--rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/PCC/Pearson_CC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/PCC/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.795680 musicAlgLib-1.0.9/musicAlgLib/PEAQ/
--rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/PEAQ/PEAQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/PEAQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.797168 musicAlgLib-1.0.9/musicAlgLib/PESQ/
--rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/PESQ/PESQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/PESQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.797704 musicAlgLib-1.0.9/musicAlgLib/PLAY_DELAY/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.0.9/musicAlgLib/PLAY_DELAY/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.800144 musicAlgLib-1.0.9/musicAlgLib/POLQA/
--rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/POLQA/POLQA.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/POLQA/__init__.py
--rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/POLQA/file_server.py
--rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/POLQA/polqa_client.py
--rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/POLQA/polqa_server.py
--rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/POLQA/socketClient.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.801632 musicAlgLib-1.0.9/musicAlgLib/SNR_ESTIMATION/
--rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.0.9/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
--rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/SNR_ESTIMATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.802624 musicAlgLib-1.0.9/musicAlgLib/STI/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/STI/__init__.py
--rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/STI/cal_sti.py
--rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/STI/sti.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.803616 musicAlgLib-1.0.9/musicAlgLib/VAD_NN/
--rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.0.9/musicAlgLib/VAD_NN/__init__.py
--rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.0.9/musicAlgLib/VAD_NN/hubconf.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.804112 musicAlgLib-1.0.9/musicAlgLib/VISQOL/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.0.9/musicAlgLib/VISQOL/__init__.py
--rw-rw-rw-   0        0        0     4781 2024-04-03 07:50:07.000000 musicAlgLib-1.0.9/musicAlgLib/__init__.py
--rw-rw-rw-   0        0        0    15385 2024-04-03 08:14:53.000000 musicAlgLib-1.0.9/musicAlgLib/commFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.804608 musicAlgLib-1.0.9/musicAlgLib/computeAudioQuality/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/computeAudioQuality/__init__.py
--rw-rw-rw-   0        0        0    11334 2024-04-03 08:07:32.000000 musicAlgLib-1.0.9/musicAlgLib/computeAudioQuality/mainProcess.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.806096 musicAlgLib-1.0.9/musicAlgLib/formatConvert/
--rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/formatConvert/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/formatConvert/wav_pcm.py
--rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/main.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.807088 musicAlgLib-1.0.9/musicAlgLib/resample/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/resample/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/resample/resampler.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.808080 musicAlgLib-1.0.9/musicAlgLib/tests/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/tests/__init__.py
--rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.0.9/musicAlgLib/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.808576 musicAlgLib-1.0.9/musicAlgLib/timeAligment/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.9/musicAlgLib/timeAligment/__init__.py
--rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.0.9/musicAlgLib/timeAligment/time_align.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:15:20.779312 musicAlgLib-1.0.9/musicAlgLib.egg-info/
--rw-rw-rw-   0        0        0     4676 2024-04-03 08:15:20.000000 musicAlgLib-1.0.9/musicAlgLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2227 2024-04-03 08:15:20.000000 musicAlgLib-1.0.9/musicAlgLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:15:20.000000 musicAlgLib-1.0.9/musicAlgLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-03 08:15:20.000000 musicAlgLib-1.0.9/musicAlgLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 08:15:20.000000 musicAlgLib-1.0.9/musicAlgLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:15:20.809568 musicAlgLib-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     5840 2024-04-03 08:15:12.000000 musicAlgLib-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.712098 musicAlgLib-1.1.1/
+-rw-rw-rw-   0        0        0     4676 2024-04-03 08:35:19.712098 musicAlgLib-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.678369 musicAlgLib-1.1.1/musicAlgLib/
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.682337 musicAlgLib-1.1.1/musicAlgLib/AGC_EVALUATION/
+-rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/AGC_EVALUATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.682833 musicAlgLib-1.1.1/musicAlgLib/CLIPPING_DETECTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/CLIPPING_DETECTION/__init__.py
+-rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.693745 musicAlgLib-1.1.1/musicAlgLib/DLLS/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/__init__.py
+-rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/cygwin1.dll
+-rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/matchsig.dll
+-rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/matchsig.dylib
+-rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/matchsig.so
+-rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/musicStability.dll
+-rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/musicStability.dylib
+-rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/musicStability.so
+-rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/pcc.dll
+-rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/pcc.dylib
+-rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/pcc.so
+-rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/peaqb.exe
+-rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/silero_vad.jit
+-rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/snr_music.dll
+-rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/snr_music.dylib
+-rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/DLLS/snr_music.so
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.693745 musicAlgLib-1.1.1/musicAlgLib/DynmicRange/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.1.1/musicAlgLib/DynmicRange/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.694738 musicAlgLib-1.1.1/musicAlgLib/FUNCTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/FUNCTION/__init__.py
+-rw-rw-rw-   0        0        0    19295 2024-04-03 08:34:31.000000 musicAlgLib-1.1.1/musicAlgLib/FUNCTION/audioFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.695233 musicAlgLib-1.1.1/musicAlgLib/FrequencyResponse/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.1.1/musicAlgLib/FrequencyResponse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.695729 musicAlgLib-1.1.1/musicAlgLib/Noise_Suppression/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/Noise_Suppression/__init__.py
+-rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/Noise_Suppression/noiseFuction.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.696721 musicAlgLib-1.1.1/musicAlgLib/PCC/
+-rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/PCC/Pearson_CC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/PCC/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.697217 musicAlgLib-1.1.1/musicAlgLib/PEAQ/
+-rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/PEAQ/PEAQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/PEAQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.698706 musicAlgLib-1.1.1/musicAlgLib/PESQ/
+-rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/PESQ/PESQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/PESQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.699201 musicAlgLib-1.1.1/musicAlgLib/PLAY_DELAY/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.1.1/musicAlgLib/PLAY_DELAY/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.702189 musicAlgLib-1.1.1/musicAlgLib/POLQA/
+-rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/POLQA/POLQA.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/POLQA/__init__.py
+-rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/POLQA/file_server.py
+-rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/POLQA/polqa_client.py
+-rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/POLQA/polqa_server.py
+-rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/POLQA/socketClient.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.703169 musicAlgLib-1.1.1/musicAlgLib/SNR_ESTIMATION/
+-rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.1.1/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
+-rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/SNR_ESTIMATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.704657 musicAlgLib-1.1.1/musicAlgLib/STI/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/STI/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/STI/cal_sti.py
+-rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/STI/sti.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.705153 musicAlgLib-1.1.1/musicAlgLib/VAD_NN/
+-rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.1.1/musicAlgLib/VAD_NN/__init__.py
+-rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.1.1/musicAlgLib/VAD_NN/hubconf.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.707137 musicAlgLib-1.1.1/musicAlgLib/VISQOL/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.1.1/musicAlgLib/VISQOL/__init__.py
+-rw-rw-rw-   0        0        0     4781 2024-04-03 07:50:07.000000 musicAlgLib-1.1.1/musicAlgLib/__init__.py
+-rw-rw-rw-   0        0        0    15681 2024-04-03 08:34:31.000000 musicAlgLib-1.1.1/musicAlgLib/commFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.708129 musicAlgLib-1.1.1/musicAlgLib/computeAudioQuality/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/computeAudioQuality/__init__.py
+-rw-rw-rw-   0        0        0    11334 2024-04-03 08:07:32.000000 musicAlgLib-1.1.1/musicAlgLib/computeAudioQuality/mainProcess.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.709122 musicAlgLib-1.1.1/musicAlgLib/formatConvert/
+-rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/formatConvert/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/formatConvert/wav_pcm.py
+-rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/main.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.710113 musicAlgLib-1.1.1/musicAlgLib/resample/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/resample/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/resample/resampler.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.710609 musicAlgLib-1.1.1/musicAlgLib/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/tests/__init__.py
+-rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.1.1/musicAlgLib/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.711601 musicAlgLib-1.1.1/musicAlgLib/timeAligment/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.1/musicAlgLib/timeAligment/__init__.py
+-rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.1.1/musicAlgLib/timeAligment/time_align.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:35:19.681345 musicAlgLib-1.1.1/musicAlgLib.egg-info/
+-rw-rw-rw-   0        0        0     4676 2024-04-03 08:35:19.000000 musicAlgLib-1.1.1/musicAlgLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2227 2024-04-03 08:35:19.000000 musicAlgLib-1.1.1/musicAlgLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:35:19.000000 musicAlgLib-1.1.1/musicAlgLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-03 08:35:19.000000 musicAlgLib-1.1.1/musicAlgLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 08:35:19.000000 musicAlgLib-1.1.1/musicAlgLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:35:19.712098 musicAlgLib-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     5839 2024-04-03 08:35:13.000000 musicAlgLib-1.1.1/setup.py
```

### Comparing `musicAlgLib-1.0.9/PKG-INFO` & `musicAlgLib-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.0.9
+Version: 1.1.1
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.0.9/README.md` & `musicAlgLib-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py` & `musicAlgLib-1.1.1/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py` & `musicAlgLib-1.1.1/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/cygwin1.dll` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/matchsig.dll` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/matchsig.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/matchsig.dylib` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/matchsig.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/matchsig.so` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/matchsig.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/musicStability.dll` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/musicStability.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/musicStability.dylib` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/musicStability.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/musicStability.so` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/musicStability.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/pcc.dll` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/pcc.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/pcc.dylib` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/pcc.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/pcc.so` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/pcc.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/peaqb.exe` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/peaqb.exe`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/silero_vad.jit` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/silero_vad.jit`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/snr_music.dll` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/snr_music.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/snr_music.dylib` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/snr_music.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/DLLS/snr_music.so` & `musicAlgLib-1.1.1/musicAlgLib/DLLS/snr_music.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/FUNCTION/audioFunction.py` & `musicAlgLib-1.1.1/musicAlgLib/FUNCTION/audioFunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,29 +147,29 @@
         testdata, fs, ch = get_data_array(wavFileName)
         curdata = np.array([])
         for eachSection in speechSection:
             curdata = np.concatenate(
                 (curdata, testdata[int(fs * eachSection[0]):int(fs * eachSection[1])]))
 
     if rmsMode == 'total':
-        return get_rms(curdata)
+        return get_rms(curdata,fs)
     if rmsMode == 'average':
-        return get_ave_rms(curdata)
+        return get_ave_rms(curdata,fs)
     if rmsMode == 'peak':
-        return  get_peak_rms(curdata)
+        return  get_peak_rms(curdata,fs)
     if rmsMode == 'std':
-        return  get_std_rms(curdata)
+        return  get_std_rms(curdata,fs)
     if rmsMode == 'max':
-        return  get_max_rms(curdata)
+        return  get_max_rms(curdata,fs)
     if rmsMode == 'min':
-        return  get_min_rms(curdata)
+        return  get_min_rms(curdata,fs)
     if rmsMode == 'dynmic':
-        return  get_max_rms(curdata) - get_min_rms(curdata)
+        return  get_max_rms(curdata,fs) - get_min_rms(curdata,fs)
     if rmsMode == 'duration':
-        return  get_duration_above_specific_rms(curdata)
+        return  get_duration_above_specific_rms(curdata,fs)
     return None
 
 
 
 def calculate_band_energy(audio_signal, sample_rate, num_bands,freq_mode='upper'):
     # Perform FFT on audio signal
     fmin,fmax = 100,sample_rate/2 - 100
```

### Comparing `musicAlgLib-1.0.9/musicAlgLib/Noise_Suppression/noiseFuction.py` & `musicAlgLib-1.1.1/musicAlgLib/Noise_Suppression/noiseFuction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/PCC/Pearson_CC.py` & `musicAlgLib-1.1.1/musicAlgLib/PCC/Pearson_CC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/PESQ/PESQ.py` & `musicAlgLib-1.1.1/musicAlgLib/PESQ/PESQ.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/POLQA/POLQA.py` & `musicAlgLib-1.1.1/musicAlgLib/POLQA/POLQA.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/POLQA/file_server.py` & `musicAlgLib-1.1.1/musicAlgLib/POLQA/file_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/POLQA/polqa_client.py` & `musicAlgLib-1.1.1/musicAlgLib/POLQA/polqa_client.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/POLQA/polqa_server.py` & `musicAlgLib-1.1.1/musicAlgLib/POLQA/polqa_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/POLQA/socketClient.py` & `musicAlgLib-1.1.1/musicAlgLib/POLQA/socketClient.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py` & `musicAlgLib-1.1.1/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py` & `musicAlgLib-1.1.1/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/STI/cal_sti.py` & `musicAlgLib-1.1.1/musicAlgLib/STI/cal_sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/STI/sti.py` & `musicAlgLib-1.1.1/musicAlgLib/STI/sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/VAD_NN/hubconf.py` & `musicAlgLib-1.1.1/musicAlgLib/VAD_NN/hubconf.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/__init__.py` & `musicAlgLib-1.1.1/musicAlgLib/__init__.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/commFunction.py` & `musicAlgLib-1.1.1/musicAlgLib/commFunction.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import numpy as np
 import math
 import librosa
 
 
 import numpy as np
 
+windowLen = 0.05
 
 class emxArray_real_T(Structure):
  _fields_ = [
           ("pdata", POINTER(c_double)),  # c_byte
           ("psize", POINTER(c_int)),  # c_byte
           ("allocSize", c_int),  #  c_byte
           ("NumDimensions", c_int),  # c_byte
@@ -357,70 +358,71 @@
     wavfile = wave.open(tarFile, 'wb')
     wavfile.setnchannels(channel)
     wavfile.setsampwidth(databitnum)
     wavfile.setframerate(fs)
     wavfile.writeframes(outData.tobytes())
     wavfile.close()
 
-def get_ave_rms(data):
+def get_ave_rms(data,fs):
     '''
     Parameters
     ----------
     data
 
     Returns
     -------
     '''
-    frameLen = 480
-    nFrames = len(data)//frameLen
+    frameLen = windowLen * fs
+    frameshift = windowLen * fs / 2
+    nFrames = (len(data)-frameLen)//(frameshift)
     totalRms,cnt = 0,0
     for a in range(nFrames):
-        totalRms += get_rms(data[a*frameLen:(a+1)*frameLen])
+        totalRms += get_rms(data[int(a*frameshift):int(a*frameshift+frameLen)])
         cnt += 1
     return totalRms/cnt
 
-def get_std_rms(data):
+def get_std_rms(data,fs):
     '''
     Parameters
     ----------
     data
 
     Returns
     -------
     '''
-    frameLen = 960
+    frameLen = fs * windowLen * 2
     nFrames = len(data)//frameLen
     curRms = 0
     rms_list = []
     for a in range(nFrames):
         curRms = get_rms(data[a*frameLen:(a+1)*frameLen])
         rms_list.append(curRms)
     return np.std(rms_list, ddof=1)
-def get_duration_above_specific_rms(data):
+def get_duration_above_specific_rms(data,fs):
     '''
     Parameters
     ----------
     data
 
     Returns
     -------
     '''
-    frameLen = 960
+    frameLen = fs * windowLen * 2
     nFrames = len(data)//frameLen
     threshold = -45
     maxcnt,validcnt = 0,0
     for a in range(nFrames):
         maxcnt += 1
         curRms = get_rms(data[a*frameLen:(a+1)*frameLen])
         if curRms > threshold:
             validcnt += 1
 
     return validcnt/maxcnt
 
-def get_rms(records):
+def get_rms(records,fs):
     '''
     Parameters
     ----------
     records
 
     Returns
     -------
@@ -430,63 +432,66 @@
     if len(data) == 0:
         return -99.9
     rms = math.sqrt(sum([(x/32767) * (x/32767) for x in data])/len(data))
     dBrmsValue = 20*math.log10(rms + 1.0E-6)
     return dBrmsValue
 
 
-def get_peak_rms(records):
+def get_peak_rms(records,fs):
     '''
     Parameters
     ----------
     records
 
     Returns
     -------
     '''
     #return math.sqrt(sum([x * x for x in records])/len(records))
 
     maxdata = max(records)
     maxRms = 20 * math.log10(maxdata/32767 + 1.0E-6)
     return maxRms
 
-def get_max_rms(records):
+def get_max_rms(records,fs):
     '''
     Parameters
     ----------
     records
 
     Returns
     -------
     '''
     #return math.sqrt(sum([x * x for x in records])/len(records))
-    frameLen = 480 #50ms
-    nFrames = len(records)//frameLen
+    frameLen = windowLen * fs
+    frameshift = windowLen * fs/2
+    nFrames = (len(records)-frameLen)//(frameshift)
     maxRms = -99
     for a in range(nFrames):
-        curRms = get_rms(records[a*frameLen:(a+1)*frameLen])
+        curRms = get_rms(records[int(a*frameshift):int(a*frameshift+frameLen)])
         if curRms > maxRms:
             maxRms = curRms
     return maxRms
 
-def get_min_rms(records):
+
+def get_min_rms(records,fs):
     '''
     Parameters
     ----------
     records
 
     Returns
     -------
     '''
     #return math.sqrt(sum([x * x for x in records])/len(records))
-    frameLen = 480 #50ms
-    nFrames = len(records)//frameLen
+    frameLen = windowLen * fs
+    frameshift = windowLen * fs/2
+    nFrames = (len(records)-frameLen)//(frameshift)
     minrms = 100
     for a in range(nFrames):
-        curRms = get_rms(records[a*frameLen:(a+1)*frameLen])
+        curRms = get_rms(records[int(a*frameshift):int(a*frameshift+frameLen)])
         if curRms < minrms:
             minrms = curRms
     return minrms
 
 def get_one_channel_data(infile):
     """
     :return:
```

### Comparing `musicAlgLib-1.0.9/musicAlgLib/computeAudioQuality/mainProcess.py` & `musicAlgLib-1.1.1/musicAlgLib/computeAudioQuality/mainProcess.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/formatConvert/wav_pcm.py` & `musicAlgLib-1.1.1/musicAlgLib/formatConvert/wav_pcm.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/main.py` & `musicAlgLib-1.1.1/musicAlgLib/main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/resample/resampler.py` & `musicAlgLib-1.1.1/musicAlgLib/resample/resampler.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/tests/test_main.py` & `musicAlgLib-1.1.1/musicAlgLib/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib/timeAligment/time_align.py` & `musicAlgLib-1.1.1/musicAlgLib/timeAligment/time_align.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/musicAlgLib.egg-info/PKG-INFO` & `musicAlgLib-1.1.1/musicAlgLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.0.9
+Version: 1.1.1
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.0.9/musicAlgLib.egg-info/SOURCES.txt` & `musicAlgLib-1.1.1/musicAlgLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.9/setup.py` & `musicAlgLib-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setup(
     name='musicAlgLib',
-    version='1.0.09',
+    version='1.1.1',
     packages=setuptools.find_packages(),
     url='https://github.com/pypa/sampleproject',
     license='MIT',
     author=' MA JIANLI',
     author_email='majianli@corp.netease.com',
     description='audio algorithms to compute and test music quality',
     long_description="""
```

