# Comparing `tmp/syncstart-1.0.1-py3-none-any.whl.zip` & `tmp/syncstart-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7434 bytes, number of entries: 8
--rw-r--r--  2.0 unx     6573 b- defN 22-Sep-18 17:30 syncstart.py
--rw-r--r--  2.0 unx     2542 b- defN 22-Sep-18 17:33 syncstart-1.0.1.data/data/man/man1/syncstart.1
--rw-r--r--  2.0 unx     1059 b- defN 22-Sep-18 17:33 syncstart-1.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3196 b- defN 22-Sep-18 17:33 syncstart-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-18 17:33 syncstart-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 22-Sep-18 17:33 syncstart-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 22-Sep-18 17:33 syncstart-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      669 b- defN 22-Sep-18 17:33 syncstart-1.0.1.dist-info/RECORD
-8 files, 14186 bytes uncompressed, 6258 bytes compressed:  55.9%
+Zip file size: 9851 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    11870 b- defN 24-Apr-02 17:04 syncstart.py
+-rw-r--r--  2.0 unx     3225 b- defN 24-Apr-03 06:29 syncstart-1.1.0.data/data/man/man1/syncstart.1
+-rw-r--r--  2.0 unx     1059 b- defN 24-Apr-03 06:29 syncstart-1.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4209 b- defN 24-Apr-03 06:29 syncstart-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 06:29 syncstart-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 24-Apr-03 06:29 syncstart-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-03 06:29 syncstart-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      670 b- defN 24-Apr-03 06:29 syncstart-1.1.0.dist-info/RECORD
+8 files, 21180 bytes uncompressed, 8675 bytes compressed:  59.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: syncstart.py
 Comment: 
 
-Filename: syncstart-1.0.1.data/data/man/man1/syncstart.1
+Filename: syncstart-1.1.0.data/data/man/man1/syncstart.1
 Comment: 
 
-Filename: syncstart-1.0.1.dist-info/LICENSE.txt
+Filename: syncstart-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: syncstart-1.0.1.dist-info/METADATA
+Filename: syncstart-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: syncstart-1.0.1.dist-info/WHEEL
+Filename: syncstart-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: syncstart-1.0.1.dist-info/entry_points.txt
+Filename: syncstart-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: syncstart-1.0.1.dist-info/top_level.txt
+Filename: syncstart-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: syncstart-1.0.1.dist-info/RECORD
+Filename: syncstart-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## syncstart.py

```diff
@@ -1,222 +1,392 @@
 #!/usr/bin/env python3
 
 """
 The steps taken by ``syncstart``:
 
-- extract start audio as ``.wav`` using ffmpeg
-- optionally normalize, denoise, lowpass the two ``.wav``
+- get the maximum audio sample frequency or video frame rate among the inputs using ffprobe
+- process and extract sample audio/video clips using ffmpeg with some default and optional filters
+- read the two clips into a 1D array and apply optional z-score normalization
 - compute offset via correlation using scipy ifft/fft
-- print result and optionally show in diagrams
+- print ffmpeg/ffprobe output or optionally quiet that
+- show diagrams to allow MANUAL correction using ZOOM or optionally suppress that
+- print result
 
 Requirements:
 
-- ffmpeg installed
+- ffmpeg and ffprobe installed
 - Python3 with tk (tk is separate on Ubuntu: python3-tk)
 
 References:
 
 - https://ffmpeg.org/ffmpeg-all.html
-- https://github.com/slhck/ffmpeg-normalize
 - https://dsp.stackexchange.com/questions/736/how-do-i-implement-cross-correlation-to-prove-two-audio-files-are-similar
+- https://dsp.stackexchange.com/questions/18846/map-time-difference-between-two-similar-videos
 
 Within Python:
 
 from syncstart import file_offset
-file_offset
 
 """
 
 import matplotlib
 matplotlib.use('TkAgg')
+import cv2
 from matplotlib import pyplot as plt
+import pylab
 import numpy as np
-from scipy import fft
-from scipy.io import wavfile
+import scipy
 import tempfile
 import os
 import pathlib
 import sys
+import subprocess
 
-__version__ = "1.0.1"
-__author__ = """Roland Puntaier"""
+__version__ = '1.1.0'
+__author__ = """Roland Puntaier, drolex2"""
 __email__ = 'roland.puntaier@gmail.com'
 
 #global
 ax = None
+video = False
+begin = 0
 take = 20
 normalize = False
 denoise = False
 lowpass = 0
-
-ffmpegwav = 'ffmpeg -i "{}" -t %s -c:a pcm_s16le -map 0:a "{}"'
-ffmpegnormalize = ('ffmpeg -y -nostdin -i "{}" -filter_complex ' +
-"'[0:0]loudnorm=i=-23.0:lra=7.0:tp=-2.0:offset=4.45:linear=true:print_format=json[norm0]' " +
-"-map_metadata 0 -map_metadata:s:a:0 0:s:a:0 -map_chapters 0 -c:v copy -map '[norm0]' " +
-'-c:a:0 pcm_s16le -c:s copy "{}"')
-ffmpegdenoise = 'ffmpeg -i "{}" -af'+" 'afftdn=nf=-25' "+'"{}"'
-ffmpeglow = 'ffmpeg -i "{}" -af'+" 'lowpass=f=%s' "+'"{}"'
-o = lambda x: '%s%s'%(x,'.wav')
+crop = False
+quiet = False
+loglevel = 32
+
+ffmpegvideo = 'ffmpeg -loglevel %s -hwaccel auto -ss %s -i "{}" %s -map 0:v -c:v mjpeg -q 1 -f mjpeg "{}"'
+ffmpegwav = 'ffmpeg -loglevel %s -ss %s -i "{}" %s -map 0:a -c:a pcm_s16le -ac 1 -f wav "{}"'
+
+audio_filters = {
+  'default': 'atrim=0:%s,aresample=%s',
+  'lowpass': 'lowpass=f=%s',
+  'denoise': 'afftdn=nr=24:nf=-25'
+}
+
+video_filters = {
+  'default': 'trim=0:%s,fps=%s,format=gray,scale=-1:300',
+  'crop': 'crop=400:300',
+  'denoise': 'hqdn3d=3:3:2:2'
+}
+
+def z_score_normalization(array):
+  mean = np.mean(array)
+  std_dev = np.std(array)
+  normalized_array = (array - mean) / std_dev
+  return normalized_array
+
+def header(cmdstr):
+  hdr = '-'*len(cmdstr)
+  print('%s\n%s\n%s'%(hdr,cmdstr,hdr))
+
+def get_max_rate(in1,in2):
+  probe_audio = 'ffprobe -v error -select_streams a:0 -show_entries stream=sample_rate -of default=noprint_wrappers=1'.split()
+  probe_video = 'ffprobe -v error -select_streams v:0 -show_entries stream=avg_frame_rate -of default=noprint_wrappers=1'.split()
+  command = probe_video if video else probe_audio
+  rates = []
+  for file in [in1,in2]:
+    cmdlist = command+[file]
+    cmdstr = ' '.join(cmdlist)
+    if not quiet: header(cmdstr)
+    result = subprocess.run(cmdlist,
+                            stdout=subprocess.PIPE,
+                            stderr=subprocess.PIPE,
+                            text=True)
+    if result.returncode == 0:
+        if not quiet:
+            print(result.stdout)
+        rates.append( eval(result.stdout.split('=')[1]) )
+    else:
+        print('FAIL in:\n',cmdstr)
+        print(result.stderr)
+        exit(1)
+  return max(rates)
+
+def read_video(input_video):
+  # Open input video
+  cap = cv2.VideoCapture(str(input_video))
+  # Check if the video file was opened successfully
+  if not cap.isOpened():
+    print('Error: Could not open the video file.')
+    return None
+  # Get video properties
+  width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+  height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+  # Initialize list to store difference in average brightness between the left and right halves of each video frame
+  brightdiff = []
+  while cap.isOpened():
+    ret, frame = cap.read()
+    if not ret:
+      break
+    # Split the frame into left and right halves
+    left_half = frame[:, :width // 2]
+    right_half = frame[:, width // 2:]
+    # Calculate the difference in average brightness between the left and right halves
+    brightdiff.append( np.mean(right_half) - np.mean(left_half) )
+  # Release the video capture object
+  cap.release()
+  return brightdiff
 
 def in_out(command,infile,outfile):
-    hdr = '-'*len(command)
-    print("%s\n%s\n%s"%(hdr,command,hdr))
-    ret = os.system(command.format(infile,outfile))
-    if 0 != ret:
-      sys.exit(ret)
+  cmdstr = command.format(infile,outfile)
+  if not quiet: header(cmdstr)
+  ret = os.system(cmdstr)
+  if 0 != ret:
+    sys.exit(ret)
 
-def normalize_denoise(infile,outname):
+def get_sample(infile,rate):
+  outname = pathlib.Path(infile).stem + '_sample'
   with tempfile.TemporaryDirectory() as tempdir:
-    outfile = o(pathlib.Path(tempdir)/outname)
-    in_out(ffmpegwav%take,infile,outfile)
-    if normalize:
-      infile, outfile = outfile,o(outfile)
-      in_out(ffmpegnormalize,infile,outfile)
-    if denoise:
-      infile, outfile = outfile,o(outfile)
-      in_out(ffmpegdenoise,infile,outfile)
-      infile, outfile = outfile,o(outfile)
-      in_out(ffmpegdenoise,infile,outfile)
-    if int(lowpass):
-      infile, outfile = outfile,o(outfile)
-      in_out(ffmpeglow%lowpass,infile,outfile)
-    r,s = wavfile.read(outfile)
-    if len(s.shape)>1: #stereo
-      s = s[:,0]
-    return r,s
+    outfile = pathlib.Path(tempdir)/(outname)
+    if video: #compare video
+      filters = [video_filters['default']%(take,rate)]
+      if crop:
+        filters.append(video_filters['crop'])
+      if denoise:
+        filters.append(video_filters['denoise'])
+      filter_string = '-vf "' + ','.join(filters) + '"'
+      in_out(ffmpegvideo%(loglevel,begin,filter_string),infile,outfile)
+      s = read_video(outfile)
+    else: #compare audio
+      filters = [audio_filters['default']%(take,rate)]
+      if int(lowpass):
+        filters.append(audio_filters['lowpass']%lowpass)
+      if denoise:
+        filters.append(audio_filters['denoise'])
+      filter_string = '-af "' + ','.join(filters) + '"'
+      in_out(ffmpegwav%(loglevel,begin,filter_string),infile,outfile)
+      r,s = scipy.io.wavfile.read(outfile)
+    return s
 
 def fig1(title=None):
   fig = plt.figure(1)
   plt.margins(0, 0.1)
   plt.grid(True, color='0.7', linestyle='-', which='major', axis='both')
   plt.grid(True, color='0.9', linestyle='-', which='minor', axis='both')
   plt.title(title or 'Signal')
   plt.xlabel('Time [seconds]')
   plt.ylabel('Amplitude')
   axs = fig.get_axes()
   global ax
   ax = axs[0]
 
-def show1(fs, s, color=None, title=None, v=None):
+def show1(sr, s, color=None, title=None, v=None):
   if not color: fig1(title)
   if ax and v: ax.axvline(x=v,color='green')
-  plt.plot(np.arange(len(s))/fs, s, color or 'black')
+  plt.plot(np.arange(len(s))/sr, s, color or 'black')
   if not color: plt.show()
 
-def show2(fs,s1,s2,title=None):
-  fig1(title)
-  show1(fs,s1,'blue')
-  show1(fs,s2,'red')
+def show2(sr,s1,s2,plus1minus2,in1,in2):
+  fig1("Matchup")
+  t1,t2 = (0,-plus1minus2) if plus1minus2 < 0 else (plus1minus2,0)
+  r = lambda x: round(x,2)
+  dt = 0
+  choice = True
+  iszoom = False
+  if plus1minus2 < 0:
+    ff,ffclr,ffo,ffoclr,toff = in2,'RED',in1,'BLUE',-plus1minus2/sr
+  else:
+    ff,ffclr,ffo,ffoclr,toff = in1,'BLUE',in2,'RED',plus1minus2/sr
+  show1(sr,s1[t1:],'blue')
+  show1(sr,s2[t2:],'red')
+  plt.legend([
+      f'{ff} ({ffclr}) cut {r(toff)}',
+      f'{ffo} ({ffoclr})',
+      ])
+
+  def on_zoom(event_ax):
+    nonlocal dt, choice, iszoom
+    choice = plt.fix.get_status()[0]
+    tt = ax.get_xlim()
+    if plus1minus2 < 0:
+      ff,ffclr,ffo,ffoclr,toff = in2,'RED',in1,'BLUE',-plus1minus2/sr
+    else:
+      ff,ffclr,ffo,ffoclr,toff = in1,'BLUE',in2,'RED',plus1minus2/sr
+    dt = tt[1]-tt[0]
+    tlabel = [
+        f'Time from {r(tt[0])} to {r(tt[1])} = {r(dt)} seconds',
+        f'After above choice ZOOM to correct',
+            ]
+    iszoom = abs(tt[0]) > 0.1
+    if iszoom:
+        poff = toff+dt
+        noff = toff-dt
+        if noff < 0:
+            ff,ffo = ffo,ff
+            ffclr,ffoclr = ffoclr,ffclr
+            noff = -noff
+        choice_from = [
+          f'Cut {r(noff)} from {ff}',
+          f'Cut {r(poff)} from {ff}',
+        ]
+        plt.xlabel('\n'.join(tlabel+[choice_from[choice]]))
+    else:
+        plt.xlabel('\n'.join(tlabel))
+
+  plt.fixax = plt.axes(np.array([0.65, 0.94, 0.15, 0.02]))
+  plt.fix = matplotlib.widgets.CheckButtons(plt.fixax,
+                          [f"Fix {ffclr} to left"], [choice])
+  plt.fix.on_clicked(on_zoom)
+  ax.callbacks.connect('xlim_changed', on_zoom)
   plt.show()
+  if iszoom:
+    poff = toff+dt
+    noff = toff-dt
+    if noff < 0:
+        ff,ffo = ffo,ff
+        ffclr,ffoclr = ffoclr,ffclr
+        noff = -noff
+    if choice:
+        return ff,poff
+    else:
+        return ff,noff
+  else:
+    return ff, toff
 
-def read_normalized(in1,in2):
-  global normalize
-  r1,s1 = normalize_denoise(in1,'out1')
-  r2,s2 = normalize_denoise(in2,'out2')
-  if r1 != r2:
-    old,normalize = normalize,True
-    r1,s1 = normalize_denoise(in1,'out1')
-    r2,s2 = normalize_denoise(in2,'out2')
-    normalize = old
-  assert r1 == r2, "not same sample rate"
-  fs = r1
-  return fs,s1,s2
 
 def corrabs(s1,s2):
   ls1 = len(s1)
   ls2 = len(s2)
   padsize = ls1+ls2+1
   padsize = 2**(int(np.log(padsize)/np.log(2))+1)
   s1pad = np.zeros(padsize)
   s1pad[:ls1] = s1
   s2pad = np.zeros(padsize)
   s2pad[:ls2] = s2
-  corr = fft.ifft(fft.fft(s1pad)*np.conj(fft.fft(s2pad)))
+  corr = scipy.fft.ifft(scipy.fft.fft(s1pad)*np.conj(scipy.fft.fft(s2pad)))
   ca = np.absolute(corr)
   xmax = np.argmax(ca)
   return ls1,ls2,padsize,xmax,ca
 
 def cli_parser(**ka):
   import argparse
-  parser = argparse.ArgumentParser(description=file_offset.__doc__,
-                      formatter_class=argparse.RawDescriptionHelpFormatter)
+  parser = argparse.ArgumentParser(
+    prog='syncstart',
+    description=file_offset.__doc__,
+    formatter_class=argparse.RawDescriptionHelpFormatter)
   parser.add_argument('--version', action='version', version = __version__)
 
   if 'in1' not in ka:
     parser.add_argument(
       'in1',
-      help='First media file to sync with second, using audio.')
+      help='First media file to sync with second.')
   if 'in2' not in ka:
     parser.add_argument(
       'in2',
-      help='Second media file to sync with first, using audio.')
+      help='Second media file to sync with first.')
+  if 'video' not in ka:
+    parser.add_argument(
+      '-v','--video',
+      dest='video',
+      action='store_true',
+      default=False,
+      help='Compare video streams. (audio is default)')
+  if 'begin' not in ka:
+    parser.add_argument(
+      '-b','--begin',
+      dest='begin',
+      action='store',
+      default=0,
+      help='Begin comparison X seconds into the inputs. (default: 0)')
   if 'take' not in ka:
     parser.add_argument(
       '-t','--take',
       dest='take',
       action='store',
       default=20,
       help='Take X seconds of the inputs to look at. (default: 20)')
-  if 'show' not in ka:
-    parser.add_argument(
-      '-s','--show',
-      dest='show',
-      action='store_false',
-      default=True,
-      help='Turn off "show diagrams", in case you are confident.')
   if 'normalize' not in ka:
     parser.add_argument(
       '-n','--normalize',
       dest='normalize',
       action='store_true',
       default=False,
-      help='Turn on normalize. It turns on by itself in a second pass, if sampling rates differ.')
+      help='Normalizes audio/video values from each stream.')
   if 'denoise' not in ka:
     parser.add_argument(
       '-d','--denoise',
       dest='denoise',
       action='store_true',
       default=False,
-      help='Turns on denoise, as experiment in case of failure.')
+      help='Reduces audio/video noise in each stream.')
   if 'lowpass' not in ka:
     parser.add_argument(
       '-l','--lowpass',
       dest='lowpass',
       action='store',
       default=0,
-      help="lowpass, just in case, because like with manual sync'ing,\
-      the low frequencies matter more. 0 == off. (default: 0)")
+      help="Audio option: Discards frequencies above the specified Hz,\
+      e.g., 300. 0 == off (default)")
+  if 'crop' not in ka:
+    parser.add_argument(
+      '-c','--crop',
+      dest='crop',
+      action='store_true',
+      default=False,
+      help='Video option: Crop to 4:3. Helpful when aspect ratios differ.')
+  if 'show' not in ka:
+    parser.add_argument(
+      '-s','--show',
+      dest='show',
+      action='store_false',
+      default=True,
+      help='Suppress "show diagrams", in case you are confident.')
+  if 'quiet' not in ka:
+    parser.add_argument(
+      '-q','--quiet',
+      dest='quiet',
+      action='store_true',
+      default=False,
+      help='Suppresses standard output except for the CSV result.\
+      Output will be: file_to_advance,seconds_to_advance')
   return parser
 
 def file_offset(**ka):
-  """CLI interface to sync two media files using their audio streams.
+  """CLI interface to sync two media files using their audio or video streams.
   ffmpeg needs to be available.
   """
 
   parser = cli_parser(**ka)
   args = parser.parse_args().__dict__
   ka.update(args)
 
-  global take,normalize,denoise,lowpass
-  in1,in2,take,show = ka['in1'],ka['in2'],ka['take'],ka['show']
+  global video,begin,take,normalize,denoise,lowpass,crop,quiet,loglevel
+  in1,in2,begin,take = ka['in1'],ka['in2'],ka['begin'],ka['take']
+  video,crop,quiet,show = ka['video'],ka['crop'],ka['quiet'],ka['show']
   normalize,denoise,lowpass = ka['normalize'],ka['denoise'],ka['lowpass']
-  fs,s1,s2 = read_normalized(in1,in2)
+  loglevel = 16 if quiet else 32
+
+  sr = get_max_rate(in1,in2)
+  s1,s2 = get_sample(in1,sr),get_sample(in2,sr)
+  if normalize:
+    s1,s2 = z_score_normalization(s1),z_score_normalization(s2)
   ls1,ls2,padsize,xmax,ca = corrabs(s1,s2)
-  if show: show1(fs,ca,title='Correlation',v=xmax/fs)
+  if show: show1(sr,ca,title='Correlation',v=xmax/sr)
   sync_text = """
 ==============================================================================
 %s needs 'ffmpeg -ss %s' cut to get in sync
 ==============================================================================
 """
   if xmax > padsize // 2:
-    if show: show2(fs,s1,s2[padsize-xmax:],title='1st=blue;2nd=red=cut(%s;%s)'%(in1,in2))
-    file,offset = in2,(padsize-xmax)/fs
+    if show:
+      file,offset = show2(sr,s1,s2,-(padsize-xmax),in1,in2)
+    else:
+      file,offset = in2,(padsize-xmax)/sr
   else:
-    if show: show2(fs,s1[xmax:],s2,title='1st=blue=cut;2nd=red (%s;%s)'%(in1,in2))
-    file,offset = in1,xmax/fs
-  print(sync_text%(file,offset))
+    if show:
+      file,offset = show2(sr,s1,s2,xmax,in1,in2)
+    else:
+      file,offset = in1,xmax/sr
+  if not quiet: #default
+    print(sync_text%(file,offset))
+  else: #quiet
+    ## print csv: file_to_advance,seconds_to_advance
+    print("%s,%s"%(file,offset))
   return file,offset
 
 main = file_offset
 if __name__ == '__main__':
     main()
-
```

## Comparing `syncstart-1.0.1.data/data/man/man1/syncstart.1` & `syncstart-1.1.0.data/data/man/man1/syncstart.1`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,94 @@
-.\" Automatically generated by Pandoc 2.18
+.\" Automatically generated by Pandoc 3.1.8
 .\"
-.\" Define V font for inline verbatim, using C font in formats
-.\" that render this, and otherwise B font.
-.ie "\f[CB]x\f[]"x" \{\
-. ftr V B
-. ftr VI BI
-. ftr VB B
-. ftr VBI BI
-.\}
-.el \{\
-. ftr V CR
-. ftr VI CI
-. ftr VB CB
-. ftr VBI CBI
-.\}
-.TH "syncstart" "1" "" "Version 1.0.1" "syncstart"
-.hy
+.TH "syncstart" "1" "" "Version 1.1.0" "syncstart"
 .SH SYNOPSIS
-.PP
 Command line help:
 .IP
-.nf
-\f[C]
-usage: stpl [-h] [--version] [-t TAKE] [-s] [-n] [-d] [-l LOWPASS] in1 in2
+.EX
+usage: syncstart [-h] [--version] [-v] [-b BEGIN] [-t TAKE] [-n] [-d] [-l LOWPASS] [-c] [-s] [-q] in1 in2
 
-CLI interface to sync two media files using their audio streams.
+CLI interface to sync two media files using their audio or video streams.
   ffmpeg needs to be available.
 
 
 positional arguments:
-  in1                   First media file to sync with second, using audio.
-  in2                   Second media file to sync with first, using audio.
+  in1                   First media file to sync with second.
+  in2                   Second media file to sync with first.
 
 options:
   -h, --help            show this help message and exit
   --version             show program\[aq]s version number and exit
+  -v, --video           Compare video streams. (audio is default)
+  -b BEGIN, --begin BEGIN
+                        Begin comparison X seconds into the inputs. (default: 0)
   -t TAKE, --take TAKE  Take X seconds of the inputs to look at. (default: 20)
-  -s, --show            Turn off \[dq]show diagrams\[dq], in case you are confident.
-  -n, --normalize       Turn on normalize. It turns on by itself in a second pass, if sampling rates
-                        differ.
-  -d, --denoise         Turns on denoise, as experiment in case of failure.
+  -n, --normalize       Normalizes audio/video values from each stream.
+  -d, --denoise         Reduces audio/video noise in each stream.
   -l LOWPASS, --lowpass LOWPASS
-                        lowpass, just in case, because like with manual sync\[aq]ing, the low frequencies
-                        matter more. 0 == off. (default: 0)
-\f[R]
-.fi
+                        Audio option: Discards frequencies above the specified Hz, e.g., 300. 0 == off (default)
+  -c, --crop            Video option: Crop to 4:3. Helpful when aspect ratios differ.
+  -s, --show            Suppress \[dq]show diagrams\[dq], in case you are confident.
+  -q, --quiet           Suppresses standard output except for the CSV result. Output will be:
+                        file_to_advance,seconds_to_advance
+.EE
 .SH DESCRIPTION
-.PP
-The steps taken by \f[V]syncstart\f[R]:
+The steps taken by \f[CR]syncstart\f[R]:
+.IP \[bu] 2
+get the maximum audio sample frequency or video frame rate among the
+inputs using ffprobe
 .IP \[bu] 2
-extract start audio as \f[V].wav\f[R] using ffmpeg
+process and extract sample audio/video clips using ffmpeg with some
+default and optional filters
 .IP \[bu] 2
-optionally normalize, denoise, lowpass the two \f[V].wav\f[R]
+read the two clips into a 1D array and apply optional z-score
+normalization
 .IP \[bu] 2
 compute offset via correlation using scipy ifft/fft
 .IP \[bu] 2
-print result and optionally show in diagrams
+print ffmpeg/ffprobe output or optionally quiet that
+.IP \[bu] 2
+show diagrams to allow MANUAL correction using ZOOM or optionally
+suppress that
+.IP \[bu] 2
+print result
 .PP
 Requirements:
 .IP \[bu] 2
-ffmpeg installed
+ffmpeg and ffprobe installed
 .IP \[bu] 2
 Python3 with tk (tk is separate on Ubuntu: python3-tk)
 .PP
 References:
 .IP \[bu] 2
 <https://ffmpeg.org/ffmpeg-all.html>
 .IP \[bu] 2
-<https://github.com/slhck/ffmpeg-normalize>
-.IP \[bu] 2
 <https://dsp.stackexchange.com/questions/736/how-do-i-implement-cross-correlation-to-prove-two-audio-files-are-similar>
+.IP \[bu] 2
+<https://dsp.stackexchange.com/questions/18846/map-time-difference-between-two-similar-videos>
 .PP
 Within Python:
 .PP
-from syncstart import file_offset file_offset
+from syncstart import file_offset
 .SH INSTALLATION
-.PP
 To install for user only, do:
 .IP
-.nf
-\f[C]
+.EX
 pip install --user syncstart
-\f[R]
-.fi
+.EE
 .SS EXAMPLES
 .IP
-.nf
-\f[C]
+.EX
+# compute audio offset with default settings:
 syncstart from_s10.m4a from_gopro.m4p
-syncstart from_s10.m4a from_gopro.m4p -t 10
-syncstart from_s10.m4a from_gopro.m4p -t 30
-syncstart from_s10.m4a from_gopro.m4p -sndl 0
-\f[R]
-.fi
+
+# compute audio offset using first 10 seconds with denoising, normalization and a 300 Hz lowpass filter:
+syncstart video1.mp4 video2.mkv -t 10 -dnl 300
+
+# compute video offset using first 20 seconds, don\[aq]t show plots, only output final result:
+syncstart video1.mp4 video2.mkv -vsq
+
+# compute video offset using seconds 15 to 25 with denoising, cropping and normalization:
+syncstart video1.mp4 video2.mkv -b 15 -t 10 -vdcn
+.EE
 .SS License
-.PP
 MIT
```

## Comparing `syncstart-1.0.1.dist-info/LICENSE.txt` & `syncstart-1.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `syncstart-1.0.1.dist-info/METADATA` & `syncstart-1.1.0.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncstart
-Version: 1.0.1
+Version: 1.1.0
 Summary: Calculate the cut needed at start to sync two media files.
 Home-page: https://github.com/rpuntaie/syncstart
 Author: Roland Puntaier
 Author-email: roland.puntaier@gmail.com
 License: MIT
 Keywords: media file synchronization
 Classifier: Development Status :: 4 - Beta
@@ -21,73 +21,80 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
+Requires-Dist: python-opencv
 
 =======================================
-syncstart(1) Version 1.0.1 \| syncstart
+syncstart(1) Version 1.1.0 \| syncstart
 =======================================
 
 SYNOPSIS
 ========
 
 Command line help::
 
-    usage: stpl [-h] [--version] [-t TAKE] [-s] [-n] [-d] [-l LOWPASS] in1 in2
+    usage: syncstart [-h] [--version] [-v] [-b BEGIN] [-t TAKE] [-n] [-d] [-l LOWPASS] [-c] [-s] [-q] in1 in2
     
-    CLI interface to sync two media files using their audio streams.
+    CLI interface to sync two media files using their audio or video streams.
       ffmpeg needs to be available.
       
     
     positional arguments:
-      in1                   First media file to sync with second, using audio.
-      in2                   Second media file to sync with first, using audio.
+      in1                   First media file to sync with second.
+      in2                   Second media file to sync with first.
     
     options:
       -h, --help            show this help message and exit
       --version             show program's version number and exit
+      -v, --video           Compare video streams. (audio is default)
+      -b BEGIN, --begin BEGIN
+                            Begin comparison X seconds into the inputs. (default: 0)
       -t TAKE, --take TAKE  Take X seconds of the inputs to look at. (default: 20)
-      -s, --show            Turn off "show diagrams", in case you are confident.
-      -n, --normalize       Turn on normalize. It turns on by itself in a second pass, if sampling rates
-                            differ.
-      -d, --denoise         Turns on denoise, as experiment in case of failure.
+      -n, --normalize       Normalizes audio/video values from each stream.
+      -d, --denoise         Reduces audio/video noise in each stream.
       -l LOWPASS, --lowpass LOWPASS
-                            lowpass, just in case, because like with manual sync'ing, the low frequencies
-                            matter more. 0 == off. (default: 0)
+                            Audio option: Discards frequencies above the specified Hz, e.g., 300. 0 == off (default)
+      -c, --crop            Video option: Crop to 4:3. Helpful when aspect ratios differ.
+      -s, --show            Suppress "show diagrams", in case you are confident.
+      -q, --quiet           Suppresses standard output except for the CSV result. Output will be:
+                            file_to_advance,seconds_to_advance
 
 
 DESCRIPTION
 ===========
 
 
 The steps taken by ``syncstart``:
 
-- extract start audio as ``.wav`` using ffmpeg
-- optionally normalize, denoise, lowpass the two ``.wav``
+- get the maximum audio sample frequency or video frame rate among the inputs using ffprobe
+- process and extract sample audio/video clips using ffmpeg with some default and optional filters
+- read the two clips into a 1D array and apply optional z-score normalization
 - compute offset via correlation using scipy ifft/fft
-- print result and optionally show in diagrams
+- print ffmpeg/ffprobe output or optionally quiet that
+- show diagrams to allow MANUAL correction using ZOOM or optionally suppress that
+- print result
 
 Requirements:
 
-- ffmpeg installed
+- ffmpeg and ffprobe installed
 - Python3 with tk (tk is separate on Ubuntu: python3-tk)
 
 References:
 
 - https://ffmpeg.org/ffmpeg-all.html
-- https://github.com/slhck/ffmpeg-normalize
 - https://dsp.stackexchange.com/questions/736/how-do-i-implement-cross-correlation-to-prove-two-audio-files-are-similar
+- https://dsp.stackexchange.com/questions/18846/map-time-difference-between-two-similar-videos
 
 Within Python:
 
 from syncstart import file_offset
-file_offset
 
 
 
 
 INSTALLATION
 ============
 
@@ -96,18 +103,24 @@
    pip install --user syncstart
 
 EXAMPLES
 --------
 
 ::
 
+  # compute audio offset with default settings:
   syncstart from_s10.m4a from_gopro.m4p
-  syncstart from_s10.m4a from_gopro.m4p -t 10
-  syncstart from_s10.m4a from_gopro.m4p -t 30
-  syncstart from_s10.m4a from_gopro.m4p -sndl 0
 
+  # compute audio offset using first 10 seconds with denoising, normalization and a 300 Hz lowpass filter:
+  syncstart video1.mp4 video2.mkv -t 10 -dnl 300
+
+  # compute video offset using first 20 seconds, don't show plots, only output final result:
+  syncstart video1.mp4 video2.mkv -vsq
+
+  # compute video offset using seconds 15 to 25 with denoising, cropping and normalization:
+  syncstart video1.mp4 video2.mkv -b 15 -t 10 -vdcn
 
 License
 -------
 
 MIT
```

## Comparing `syncstart-1.0.1.dist-info/RECORD` & `syncstart-1.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-syncstart.py,sha256=FHFlLBvddWqvk6RzY_72ZBUXF3wU_5M7TyREwsUIkMI,6573
-syncstart-1.0.1.data/data/man/man1/syncstart.1,sha256=OkOk_gmnfoqqKwajUdnyphgQZNGPCp8kKkK73cXlsBo,2542
-syncstart-1.0.1.dist-info/LICENSE.txt,sha256=NBiQmZGr90B3y_pcdH-Mfe6Vju5-hqwrdi_VdZb51Sk,1059
-syncstart-1.0.1.dist-info/METADATA,sha256=LwpJp0riPIH1GLlgTl4ig9r-5dkBa3pA5yTMDHXF46A,3196
-syncstart-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-syncstart-1.0.1.dist-info/entry_points.txt,sha256=_3eBqs1fv552S6z_GPoDGXDkaJhmNTS9OlNH80B2R-M,45
-syncstart-1.0.1.dist-info/top_level.txt,sha256=1iZBdDFmY79dA9bsWlF4roJ731X80lNmBJ9fyoKeP1s,10
-syncstart-1.0.1.dist-info/RECORD,,
+syncstart.py,sha256=RPEoDUp2jc-POpB6mW7g4suBEsvie172yvwr5czChEM,11870
+syncstart-1.1.0.data/data/man/man1/syncstart.1,sha256=qwpED3j1pYFZ-71Q_h9sy3p0PDj5tMjMSvFEZ1RsuSo,3225
+syncstart-1.1.0.dist-info/LICENSE.txt,sha256=NBiQmZGr90B3y_pcdH-Mfe6Vju5-hqwrdi_VdZb51Sk,1059
+syncstart-1.1.0.dist-info/METADATA,sha256=6UF6IQRv2dZ4s9ZdKGQQw0Dg7uvHs99kbF8lRVfuPAI,4209
+syncstart-1.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+syncstart-1.1.0.dist-info/entry_points.txt,sha256=_3eBqs1fv552S6z_GPoDGXDkaJhmNTS9OlNH80B2R-M,45
+syncstart-1.1.0.dist-info/top_level.txt,sha256=1iZBdDFmY79dA9bsWlF4roJ731X80lNmBJ9fyoKeP1s,10
+syncstart-1.1.0.dist-info/RECORD,,
```

