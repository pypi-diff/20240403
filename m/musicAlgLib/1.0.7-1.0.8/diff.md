# Comparing `tmp/musicAlgLib-1.0.7.tar.gz` & `tmp/musicAlgLib-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicAlgLib-1.0.7.tar", last modified: Wed Apr  3 07:50:47 2024, max compression
+gzip compressed data, was "musicAlgLib-1.0.8.tar", last modified: Wed Apr  3 08:07:38 2024, max compression
```

## Comparing `musicAlgLib-1.0.7.tar` & `musicAlgLib-1.0.8.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.297806 musicAlgLib-1.0.7/
--rw-rw-rw-   0        0        0     4676 2024-04-03 07:50:47.297310 musicAlgLib-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.265071 musicAlgLib-1.0.7/musicAlgLib/
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.269038 musicAlgLib-1.0.7/musicAlgLib/AGC_EVALUATION/
--rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/AGC_EVALUATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.269534 musicAlgLib-1.0.7/musicAlgLib/CLIPPING_DETECTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/CLIPPING_DETECTION/__init__.py
--rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.280446 musicAlgLib-1.0.7/musicAlgLib/DLLS/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/__init__.py
--rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/cygwin1.dll
--rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.dll
--rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.dylib
--rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.so
--rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.dll
--rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.dylib
--rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.so
--rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.dll
--rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.dylib
--rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.so
--rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/peaqb.exe
--rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/silero_vad.jit
--rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.dll
--rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.dylib
--rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.so
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.280942 musicAlgLib-1.0.7/musicAlgLib/DynmicRange/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.0.7/musicAlgLib/DynmicRange/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.281438 musicAlgLib-1.0.7/musicAlgLib/FUNCTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/FUNCTION/__init__.py
--rw-rw-rw-   0        0        0    19268 2024-04-03 07:50:07.000000 musicAlgLib-1.0.7/musicAlgLib/FUNCTION/audioFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.281934 musicAlgLib-1.0.7/musicAlgLib/FrequencyResponse/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.0.7/musicAlgLib/FrequencyResponse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.282926 musicAlgLib-1.0.7/musicAlgLib/Noise_Suppression/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/Noise_Suppression/__init__.py
--rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/Noise_Suppression/noiseFuction.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.283422 musicAlgLib-1.0.7/musicAlgLib/PCC/
--rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PCC/Pearson_CC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PCC/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.284414 musicAlgLib-1.0.7/musicAlgLib/PEAQ/
--rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PEAQ/PEAQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PEAQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.285406 musicAlgLib-1.0.7/musicAlgLib/PESQ/
--rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PESQ/PESQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/PESQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.285902 musicAlgLib-1.0.7/musicAlgLib/PLAY_DELAY/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.0.7/musicAlgLib/PLAY_DELAY/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.288382 musicAlgLib-1.0.7/musicAlgLib/POLQA/
--rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/POLQA.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/__init__.py
--rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/file_server.py
--rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/polqa_client.py
--rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/polqa_server.py
--rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/POLQA/socketClient.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.289870 musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/
--rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
--rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.290862 musicAlgLib-1.0.7/musicAlgLib/STI/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/STI/__init__.py
--rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/STI/cal_sti.py
--rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/STI/sti.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.291854 musicAlgLib-1.0.7/musicAlgLib/VAD_NN/
--rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.0.7/musicAlgLib/VAD_NN/__init__.py
--rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.0.7/musicAlgLib/VAD_NN/hubconf.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.292350 musicAlgLib-1.0.7/musicAlgLib/VISQOL/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.0.7/musicAlgLib/VISQOL/__init__.py
--rw-rw-rw-   0        0        0     4781 2024-04-03 07:50:07.000000 musicAlgLib-1.0.7/musicAlgLib/__init__.py
--rw-rw-rw-   0        0        0    15523 2024-04-03 07:50:07.000000 musicAlgLib-1.0.7/musicAlgLib/commFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.292846 musicAlgLib-1.0.7/musicAlgLib/computeAudioQuality/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/computeAudioQuality/__init__.py
--rw-rw-rw-   0        0        0    11369 2024-04-03 07:50:07.000000 musicAlgLib-1.0.7/musicAlgLib/computeAudioQuality/mainProcess.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.294334 musicAlgLib-1.0.7/musicAlgLib/formatConvert/
--rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/formatConvert/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/formatConvert/wav_pcm.py
--rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/main.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.295326 musicAlgLib-1.0.7/musicAlgLib/resample/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/resample/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/resample/resampler.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.296318 musicAlgLib-1.0.7/musicAlgLib/tests/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/tests/__init__.py
--rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.0.7/musicAlgLib/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.296814 musicAlgLib-1.0.7/musicAlgLib/timeAligment/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.7/musicAlgLib/timeAligment/__init__.py
--rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.0.7/musicAlgLib/timeAligment/time_align.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:50:47.268046 musicAlgLib-1.0.7/musicAlgLib.egg-info/
--rw-rw-rw-   0        0        0     4676 2024-04-03 07:50:47.000000 musicAlgLib-1.0.7/musicAlgLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2227 2024-04-03 07:50:47.000000 musicAlgLib-1.0.7/musicAlgLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 07:50:47.000000 musicAlgLib-1.0.7/musicAlgLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-03 07:50:47.000000 musicAlgLib-1.0.7/musicAlgLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 07:50:47.000000 musicAlgLib-1.0.7/musicAlgLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 07:50:47.297806 musicAlgLib-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     5840 2024-04-03 07:50:16.000000 musicAlgLib-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.577064 musicAlgLib-1.0.8/
+-rw-rw-rw-   0        0        0     4676 2024-04-03 08:07:38.576568 musicAlgLib-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.543832 musicAlgLib-1.0.8/musicAlgLib/
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.548296 musicAlgLib-1.0.8/musicAlgLib/AGC_EVALUATION/
+-rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/AGC_EVALUATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.549288 musicAlgLib-1.0.8/musicAlgLib/CLIPPING_DETECTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/CLIPPING_DETECTION/__init__.py
+-rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.559704 musicAlgLib-1.0.8/musicAlgLib/DLLS/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/__init__.py
+-rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/cygwin1.dll
+-rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/matchsig.dll
+-rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/matchsig.dylib
+-rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/matchsig.so
+-rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/musicStability.dll
+-rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/musicStability.dylib
+-rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/musicStability.so
+-rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/pcc.dll
+-rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/pcc.dylib
+-rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/pcc.so
+-rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/peaqb.exe
+-rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/silero_vad.jit
+-rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/snr_music.dll
+-rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/snr_music.dylib
+-rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/DLLS/snr_music.so
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.560200 musicAlgLib-1.0.8/musicAlgLib/DynmicRange/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.0.8/musicAlgLib/DynmicRange/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.560696 musicAlgLib-1.0.8/musicAlgLib/FUNCTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/FUNCTION/__init__.py
+-rw-rw-rw-   0        0        0    19268 2024-04-03 07:50:07.000000 musicAlgLib-1.0.8/musicAlgLib/FUNCTION/audioFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.561192 musicAlgLib-1.0.8/musicAlgLib/FrequencyResponse/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.0.8/musicAlgLib/FrequencyResponse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.562185 musicAlgLib-1.0.8/musicAlgLib/Noise_Suppression/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/Noise_Suppression/__init__.py
+-rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/Noise_Suppression/noiseFuction.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.563176 musicAlgLib-1.0.8/musicAlgLib/PCC/
+-rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/PCC/Pearson_CC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/PCC/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.564168 musicAlgLib-1.0.8/musicAlgLib/PEAQ/
+-rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/PEAQ/PEAQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/PEAQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.565160 musicAlgLib-1.0.8/musicAlgLib/PESQ/
+-rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/PESQ/PESQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/PESQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.565656 musicAlgLib-1.0.8/musicAlgLib/PLAY_DELAY/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.0.8/musicAlgLib/PLAY_DELAY/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.567640 musicAlgLib-1.0.8/musicAlgLib/POLQA/
+-rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/POLQA/POLQA.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/POLQA/__init__.py
+-rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/POLQA/file_server.py
+-rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/POLQA/polqa_client.py
+-rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/POLQA/polqa_server.py
+-rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/POLQA/socketClient.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.569128 musicAlgLib-1.0.8/musicAlgLib/SNR_ESTIMATION/
+-rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.0.8/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
+-rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/SNR_ESTIMATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.570120 musicAlgLib-1.0.8/musicAlgLib/STI/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/STI/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/STI/cal_sti.py
+-rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/STI/sti.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.571112 musicAlgLib-1.0.8/musicAlgLib/VAD_NN/
+-rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.0.8/musicAlgLib/VAD_NN/__init__.py
+-rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.0.8/musicAlgLib/VAD_NN/hubconf.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.571608 musicAlgLib-1.0.8/musicAlgLib/VISQOL/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.0.8/musicAlgLib/VISQOL/__init__.py
+-rw-rw-rw-   0        0        0     4781 2024-04-03 07:50:07.000000 musicAlgLib-1.0.8/musicAlgLib/__init__.py
+-rw-rw-rw-   0        0        0    15381 2024-04-03 08:07:32.000000 musicAlgLib-1.0.8/musicAlgLib/commFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.573096 musicAlgLib-1.0.8/musicAlgLib/computeAudioQuality/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/computeAudioQuality/__init__.py
+-rw-rw-rw-   0        0        0    11334 2024-04-03 08:07:32.000000 musicAlgLib-1.0.8/musicAlgLib/computeAudioQuality/mainProcess.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.574088 musicAlgLib-1.0.8/musicAlgLib/formatConvert/
+-rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/formatConvert/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/formatConvert/wav_pcm.py
+-rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/main.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.575080 musicAlgLib-1.0.8/musicAlgLib/resample/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/resample/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/resample/resampler.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.575576 musicAlgLib-1.0.8/musicAlgLib/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/tests/__init__.py
+-rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.0.8/musicAlgLib/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.576568 musicAlgLib-1.0.8/musicAlgLib/timeAligment/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.0.8/musicAlgLib/timeAligment/__init__.py
+-rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.0.8/musicAlgLib/timeAligment/time_align.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:07:38.547800 musicAlgLib-1.0.8/musicAlgLib.egg-info/
+-rw-rw-rw-   0        0        0     4676 2024-04-03 08:07:38.000000 musicAlgLib-1.0.8/musicAlgLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2227 2024-04-03 08:07:38.000000 musicAlgLib-1.0.8/musicAlgLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:07:38.000000 musicAlgLib-1.0.8/musicAlgLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-03 08:07:38.000000 musicAlgLib-1.0.8/musicAlgLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 08:07:38.000000 musicAlgLib-1.0.8/musicAlgLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:07:38.577064 musicAlgLib-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     5840 2024-04-03 08:07:32.000000 musicAlgLib-1.0.8/setup.py
```

### Comparing `musicAlgLib-1.0.7/PKG-INFO` & `musicAlgLib-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.0.7
+Version: 1.0.8
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.0.7/README.md` & `musicAlgLib-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py` & `musicAlgLib-1.0.8/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py` & `musicAlgLib-1.0.8/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/cygwin1.dll` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.dll` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/matchsig.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.dylib` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/matchsig.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/matchsig.so` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/matchsig.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.dll` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/musicStability.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.dylib` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/musicStability.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/musicStability.so` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/musicStability.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.dll` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/pcc.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.dylib` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/pcc.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/pcc.so` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/pcc.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/peaqb.exe` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/peaqb.exe`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/silero_vad.jit` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/silero_vad.jit`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.dll` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/snr_music.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.dylib` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/snr_music.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/DLLS/snr_music.so` & `musicAlgLib-1.0.8/musicAlgLib/DLLS/snr_music.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/FUNCTION/audioFunction.py` & `musicAlgLib-1.0.8/musicAlgLib/FUNCTION/audioFunction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/Noise_Suppression/noiseFuction.py` & `musicAlgLib-1.0.8/musicAlgLib/Noise_Suppression/noiseFuction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/PCC/Pearson_CC.py` & `musicAlgLib-1.0.8/musicAlgLib/PCC/Pearson_CC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/PESQ/PESQ.py` & `musicAlgLib-1.0.8/musicAlgLib/PESQ/PESQ.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/POLQA/POLQA.py` & `musicAlgLib-1.0.8/musicAlgLib/POLQA/POLQA.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/POLQA/file_server.py` & `musicAlgLib-1.0.8/musicAlgLib/POLQA/file_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/POLQA/polqa_client.py` & `musicAlgLib-1.0.8/musicAlgLib/POLQA/polqa_client.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/POLQA/polqa_server.py` & `musicAlgLib-1.0.8/musicAlgLib/POLQA/polqa_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/POLQA/socketClient.py` & `musicAlgLib-1.0.8/musicAlgLib/POLQA/socketClient.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py` & `musicAlgLib-1.0.8/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py` & `musicAlgLib-1.0.8/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/STI/cal_sti.py` & `musicAlgLib-1.0.8/musicAlgLib/STI/cal_sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/STI/sti.py` & `musicAlgLib-1.0.8/musicAlgLib/STI/sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/VAD_NN/hubconf.py` & `musicAlgLib-1.0.8/musicAlgLib/VAD_NN/hubconf.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/__init__.py` & `musicAlgLib-1.0.8/musicAlgLib/__init__.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/commFunction.py` & `musicAlgLib-1.0.8/musicAlgLib/commFunction.py`

 * *Files 2% similar despite different names*

```diff
@@ -440,21 +440,17 @@
     ----------
     records
 
     Returns
     -------
     '''
     #return math.sqrt(sum([x * x for x in records])/len(records))
-    frameLen = 1
-    nFrames = len(records)//frameLen
-    maxRms = -99
-    for a in range(nFrames):
-        curRms = get_rms(records[a*frameLen:(a+1)*frameLen])
-        if curRms > maxRms:
-            maxRms = curRms
+
+    maxdata = max(records)
+    maxRms = 20 * math.log10(maxdata + 1.0E-6)
     return maxRms
 
 def get_max_rms(records):
     '''
     Parameters
     ----------
     records
```

### Comparing `musicAlgLib-1.0.7/musicAlgLib/computeAudioQuality/mainProcess.py` & `musicAlgLib-1.0.8/musicAlgLib/computeAudioQuality/mainProcess.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,16 @@
             self.__double_end_check()
     def Extract_Mono(self,audioFile):
         """
         :return:
         """
         try:
             stereo_data,frame,nchanel = get_data_array(audioFile)
-            left_data = stereo_data[1::2]
-            right_data = stereo_data[::2]
+            left_data = stereo_data[::2]
+            right_data = stereo_data[1::2]
             l_name,r_name = audioFile[:-4] + '_L.wav',audioFile[:-4] + '_R.wav'
             make_out_file(l_name, left_data, frame, 1)
             make_out_file(r_name, right_data, frame, 1)
             return  l_name,r_name
         except:
             return None,None
 
@@ -326,16 +326,14 @@
         Returns
         -------
 
         """
         self.__double_end_check()
         return cal_EQ(self.refFile_L,self.testFile_L),cal_EQ(self.refFile_R,self.testFile_R)
 
-    def DYNMIC(self):
-        pass
 
     def FR(self):
         pass
 
     def PLAY_DELAY(self):
         pass
```

### Comparing `musicAlgLib-1.0.7/musicAlgLib/formatConvert/wav_pcm.py` & `musicAlgLib-1.0.8/musicAlgLib/formatConvert/wav_pcm.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/main.py` & `musicAlgLib-1.0.8/musicAlgLib/main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/resample/resampler.py` & `musicAlgLib-1.0.8/musicAlgLib/resample/resampler.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/tests/test_main.py` & `musicAlgLib-1.0.8/musicAlgLib/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib/timeAligment/time_align.py` & `musicAlgLib-1.0.8/musicAlgLib/timeAligment/time_align.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/musicAlgLib.egg-info/PKG-INFO` & `musicAlgLib-1.0.8/musicAlgLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.0.7
+Version: 1.0.8
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.0.7/musicAlgLib.egg-info/SOURCES.txt` & `musicAlgLib-1.0.8/musicAlgLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.0.7/setup.py` & `musicAlgLib-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setup(
     name='musicAlgLib',
-    version='1.0.07',
+    version='1.0.08',
     packages=setuptools.find_packages(),
     url='https://github.com/pypa/sampleproject',
     license='MIT',
     author=' MA JIANLI',
     author_email='majianli@corp.netease.com',
     description='audio algorithms to compute and test music quality',
     long_description="""
```
