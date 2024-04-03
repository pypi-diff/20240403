# Comparing `tmp/feffery_utils_components-0.2.0rc8.tar.gz` & `tmp/feffery_utils_components-0.2.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_utils_components-0.2.0rc8.tar", last modified: Mon Mar 11 08:42:49 2024, max compression
+gzip compressed data, was "feffery_utils_components-0.2.0rc9.tar", last modified: Thu Mar 14 07:43:15 2024, max compression
```

## Comparing `feffery_utils_components-0.2.0rc8.tar` & `feffery_utils_components-0.2.0rc9.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 08:42:49.990223 feffery_utils_components-0.2.0rc8/
--rw-rw-rw-   0        0        0     1087 2024-03-09 14:59:59.000000 feffery_utils_components-0.2.0rc8/LICENSE
--rw-rw-rw-   0        0        0      484 2024-03-09 14:59:59.000000 feffery_utils_components-0.2.0rc8/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2024-03-11 08:42:49.990223 feffery_utils_components-0.2.0rc8/PKG-INFO
--rw-rw-rw-   0        0        0     1702 2024-03-09 14:59:59.000000 feffery_utils_components-0.2.0rc8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-11 08:42:49.983158 feffery_utils_components-0.2.0rc8/feffery_utils_components/
--rw-rw-rw-   0        0        0    13621 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyAPlayer.py
--rw-rw-rw-   0        0        0     2189 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyAnimatedImage.py
--rw-rw-rw-   0        0        0     2120 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyAutoAnimate.py
--rw-rw-rw-   0        0        0     2797 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyAutoFit.py
--rw-rw-rw-   0        0        0     4920 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyBirdsBackground.py
--rw-rw-rw-   0        0        0     2426 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyBlockColorPicker.py
--rw-rw-rw-   0        0        0     2551 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCaptcha.py
--rw-rw-rw-   0        0        0     3342 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCellsBackground.py
--rw-rw-rw-   0        0        0     2794 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCircleColorPicker.py
--rw-rw-rw-   0        0        0     3947 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCloudsBackground.py
--rw-rw-rw-   0        0        0   355866 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCloudsTwoBackground.py
--rw-rw-rw-   0        0        0     2784 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCompareSlider.py
--rw-rw-rw-   0        0        0     2504 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCookie.py
--rw-rw-rw-   0        0        0     1914 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCountDown.py
--rw-rw-rw-   0        0        0     3294 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCountUp.py
--rw-rw-rw-   0        0        0     1497 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCssVar.py
--rw-rw-rw-   0        0        0    21217 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDPlayer.py
--rw-rw-rw-   0        0        0     1931 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDebounceProp.py
--rw-rw-rw-   0        0        0     2141 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDeviceDetect.py
--rw-rw-rw-   0        0        0     7218 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDiv.py
--rw-rw-rw-   0        0        0     1604 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDocumentVisibility.py
--rw-rw-rw-   0        0        0     4009 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDraggable.py
--rw-rw-rw-   0        0        0     9792 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyEmojiPicker.py
--rw-rw-rw-   0        0        0     2573 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyExcelPreview.py
--rw-rw-rw-   0        0        0     1508 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyExecuteJs.py
--rw-rw-rw-   0        0        0     1755 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyExternalCss.py
--rw-rw-rw-   0        0        0     1746 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyExternalJs.py
--rw-rw-rw-   0        0        0     2714 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyExtraSpinner.py
--rw-rw-rw-   0        0        0     1722 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyEyeDropper.py
--rw-rw-rw-   0        0        0     3393 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFancyButton.py
--rw-rw-rw-   0        0        0     3583 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFancyMessage.py
--rw-rw-rw-   0        0        0     5203 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFancyNotification.py
--rw-rw-rw-   0        0        0     3140 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFixed.py
--rw-rw-rw-   0        0        0     3737 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFogBackground.py
--rw-rw-rw-   0        0        0     1742 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFullscreen.py
--rw-rw-rw-   0        0        0     1549 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGeolocation.py
--rw-rw-rw-   0        0        0     2507 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGithubColorPicker.py
--rw-rw-rw-   0        0        0     3518 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGlobeBackground.py
--rw-rw-rw-   0        0        0     8585 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGrid.py
--rw-rw-rw-   0        0        0     1902 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGridItem.py
--rw-rw-rw-   0        0        0     5861 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGuide.py
--rw-rw-rw-   0        0        0     3601 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyHaloBackground.py
--rw-rw-rw-   0        0        0     1924 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyHexColorPicker.py
--rw-rw-rw-   0        0        0     3143 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyHighlightWords.py
--rw-rw-rw-   0        0        0     1696 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyIdle.py
--rw-rw-rw-   0        0        0     2778 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyIframeMessenger.py
--rw-rw-rw-   0        0        0    19103 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyImageCropper.py
--rw-rw-rw-   0        0        0     4331 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyImageGallery.py
--rw-rw-rw-   0        0        0     2049 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyImagePaste.py
--rw-rw-rw-   0        0        0     1903 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyInViewport.py
--rw-rw-rw-   0        0        0     5738 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyJsonViewer.py
--rw-rw-rw-   0        0        0     1856 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyKeyPress.py
--rw-rw-rw-   0        0        0     2586 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyLazyLoad.py
--rw-rw-rw-   0        0        0     2175 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyListenPaste.py
--rw-rw-rw-   0        0        0     1695 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyListenScroll.py
--rw-rw-rw-   0        0        0     1565 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyListenUnload.py
--rw-rw-rw-   0        0        0     2008 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyLocalLargeStorage.py
--rw-rw-rw-   0        0        0     1933 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyLocalStorage.py
--rw-rw-rw-   0        0        0     2569 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyLocation.py
--rw-rw-rw-   0        0        0     1842 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyLongPress.py
--rw-rw-rw-   0        0        0    24340 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyMarkdownEditor.py
--rw-rw-rw-   0        0        0     1878 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyMediaQuery.py
--rw-rw-rw-   0        0        0     5688 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyMotion.py
--rw-rw-rw-   0        0        0     1523 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyMousePosition.py
--rw-rw-rw-   0        0        0    14140 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyMusicPlayer.py
--rw-rw-rw-   0        0        0     3815 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyNetBackground.py
--rw-rw-rw-   0        0        0     1592 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyPageLeave.py
--rw-rw-rw-   0        0        0     4620 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyPhotoSphereViewer.py
--rw-rw-rw-   0        0        0     3250 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyQRCode.py
--rw-rw-rw-   0        0        0     6543 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyRND.py
--rw-rw-rw-   0        0        0     1618 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyRawHTML.py
--rw-rw-rw-   0        0        0     1667 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyReload.py
--rw-rw-rw-   0        0        0     5349 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyResizable.py
--rw-rw-rw-   0        0        0     1552 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyResponsive.py
--rw-rw-rw-   0        0        0     1933 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyRgbColorPicker.py
--rw-rw-rw-   0        0        0    19074 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyRichTextEditor.py
--rw-rw-rw-   0        0        0     3435 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyRingsBackground.py
--rw-rw-rw-   0        0        0     3647 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyScroll.py
--rw-rw-rw-   0        0        0     3225 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyScrollbars.py
--rw-rw-rw-   0        0        0     5330 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferySeamlessScroll.py
--rw-rw-rw-   0        0        0     1945 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferySessionStorage.py
--rw-rw-rw-   0        0        0     1492 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferySetTitle.py
--rw-rw-rw-   0        0        0     1876 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyShadowDom.py
--rw-rw-rw-   0        0        0     5532 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyShortcutPanel.py
--rw-rw-rw-   0        0        0     4924 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferySortable.py
--rw-rw-rw-   0        0        0     2649 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferySticky.py
--rw-rw-rw-   0        0        0     1610 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyStyle.py
--rw-rw-rw-   0        0        0     2794 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTabMessenger.py
--rw-rw-rw-   0        0        0     2079 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTextSelection.py
--rw-rw-rw-   0        0        0     1967 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyThrottleProp.py
--rw-rw-rw-   0        0        0     6873 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTiltHover.py
--rw-rw-rw-   0        0        0     1771 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTimeout.py
--rw-rw-rw-   0        0        0     3908 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTopProgress.py
--rw-rw-rw-   0        0        0     3272 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTopologyBackground.py
--rw-rw-rw-   0        0        0     3529 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTrunkBackground.py
--rw-rw-rw-   0        0        0     2506 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTwitterColorPicker.py
--rw-rw-rw-   0        0        0     2322 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyVirtualList.py
--rw-rw-rw-   0        0        0     3653 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyWavesBackground.py
--rw-rw-rw-   0        0        0     2924 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyWebSocket.py
--rw-rw-rw-   0        0        0     1743 2024-03-11 08:41:38.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyWheelColorPicker.py
--rw-rw-rw-   0        0        0     1632 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyWindowSize.py
--rw-rw-rw-   0        0        0     1869 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyWordPreview.py
--rw-rw-rw-   0        0        0     3469 2024-03-10 13:40:58.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/__init__.py
--rw-rw-rw-   0        0        0     8058 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/_imports_.py
--rw-rw-rw-   0        0        0     8871 2024-03-10 13:29:03.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/alias.py
--rw-rw-rw-   0        0        0   826468 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_animated_3d_background_p5.js
--rw-rw-rw-   0        0        0   789712 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_animated_3d_background_three.js
--rw-rw-rw-   0        0        0    80015 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_animated_image.js
--rw-rw-rw-   0        0        0    84308 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_aplayer.js
--rw-rw-rw-   0        0        0     7109 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_auto_animate.js
--rw-rw-rw-   0        0        0     3421 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_auto_fit.js
--rw-rw-rw-   0        0        0    32766 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_captcha.js
--rw-rw-rw-   0        0        0    86638 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_color_pickers.js
--rw-rw-rw-   0        0        0  1227797 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_dplayer.js
--rw-rw-rw-   0        0        0   507227 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_emoji_picker.js
--rw-rw-rw-   0        0        0  1809348 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_excel_preview.js
--rw-rw-rw-   0        0        0   158423 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_extra_spinner.js
--rw-rw-rw-   0        0        0    51671 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_fancy_button.js
--rw-rw-rw-   0        0        0    58561 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_grid.js
--rw-rw-rw-   0        0        0    49415 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_image_cropper.js
--rw-rw-rw-   0        0        0   116139 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_json_viewer.js
--rw-rw-rw-   0        0        0    36345 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_local_large_storage.js
--rw-rw-rw-   0        0        0  4813407 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_markdown_editor.js
--rw-rw-rw-   0        0        0    95908 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_motion.js
--rw-rw-rw-   0        0        0   193585 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_music_player.js
--rw-rw-rw-   0        0        0  1288373 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_photo_sphere_viewer.js
--rw-rw-rw-   0        0        0    19297 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_resizable.js
--rw-rw-rw-   0        0        0   805743 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_rich_text_editor.js
--rw-rw-rw-   0        0        0    56072 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_rnd.js
--rw-rw-rw-   0        0        0    10166 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_seamless_scroll.js
--rw-rw-rw-   0        0        0    73763 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_shortcut_panel.js
--rw-rw-rw-   0        0        0    70073 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_sortable.js
--rw-rw-rw-   0        0        0   279104 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_word_preview.js
--rw-rw-rw-   0        0        0   395057 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/async-fuc-shared.js
--rw-rw-rw-   0        0        0  1109581 2024-03-11 08:41:35.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/feffery_utils_components.min.js
--rw-rw-rw-   0        0        0  1067166 2024-03-11 08:41:39.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/metadata.json
--rw-rw-rw-   0        0        0     5243 2024-03-11 08:41:36.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components/package-info.json
-drwxrwxrwx   0        0        0        0 2024-03-11 08:42:49.989155 feffery_utils_components-0.2.0rc8/feffery_utils_components.egg-info/
--rw-rw-rw-   0        0        0      343 2024-03-11 08:42:49.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6923 2024-03-11 08:42:49.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 08:42:49.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-03-11 08:42:49.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-03-11 08:42:49.000000 feffery_utils_components-0.2.0rc8/feffery_utils_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5243 2024-03-11 08:29:49.000000 feffery_utils_components-0.2.0rc8/package.json
--rw-rw-rw-   0        0        0       42 2024-03-11 08:42:49.991519 feffery_utils_components-0.2.0rc8/setup.cfg
--rw-rw-rw-   0        0        0      809 2024-03-11 08:28:00.000000 feffery_utils_components-0.2.0rc8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-14 07:43:15.208691 feffery_utils_components-0.2.0rc9/
+-rw-rw-rw-   0        0        0     1087 2024-03-09 14:59:59.000000 feffery_utils_components-0.2.0rc9/LICENSE
+-rw-rw-rw-   0        0        0      484 2024-03-09 14:59:59.000000 feffery_utils_components-0.2.0rc9/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2024-03-14 07:43:15.208691 feffery_utils_components-0.2.0rc9/PKG-INFO
+-rw-rw-rw-   0        0        0     1702 2024-03-14 07:43:12.000000 feffery_utils_components-0.2.0rc9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-14 07:43:15.199943 feffery_utils_components-0.2.0rc9/feffery_utils_components/
+-rw-rw-rw-   0        0        0    13621 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyAPlayer.py
+-rw-rw-rw-   0        0        0     2189 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyAnimatedImage.py
+-rw-rw-rw-   0        0        0     2120 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyAutoAnimate.py
+-rw-rw-rw-   0        0        0     2797 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyAutoFit.py
+-rw-rw-rw-   0        0        0     4920 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyBirdsBackground.py
+-rw-rw-rw-   0        0        0     2426 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyBlockColorPicker.py
+-rw-rw-rw-   0        0        0     2551 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCaptcha.py
+-rw-rw-rw-   0        0        0     3342 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCellsBackground.py
+-rw-rw-rw-   0        0        0     2794 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCircleColorPicker.py
+-rw-rw-rw-   0        0        0     3947 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCloudsBackground.py
+-rw-rw-rw-   0        0        0   355866 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCloudsTwoBackground.py
+-rw-rw-rw-   0        0        0     2784 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCompareSlider.py
+-rw-rw-rw-   0        0        0     2504 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCookie.py
+-rw-rw-rw-   0        0        0     1914 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCountDown.py
+-rw-rw-rw-   0        0        0     3294 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCountUp.py
+-rw-rw-rw-   0        0        0     1497 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCssVar.py
+-rw-rw-rw-   0        0        0    21217 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDPlayer.py
+-rw-rw-rw-   0        0        0     1931 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDebounceProp.py
+-rw-rw-rw-   0        0        0     2141 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDeviceDetect.py
+-rw-rw-rw-   0        0        0     7218 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDiv.py
+-rw-rw-rw-   0        0        0     1604 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDocumentVisibility.py
+-rw-rw-rw-   0        0        0     4009 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDraggable.py
+-rw-rw-rw-   0        0        0     9792 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyEmojiPicker.py
+-rw-rw-rw-   0        0        0     2573 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyExcelPreview.py
+-rw-rw-rw-   0        0        0     2699 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyExecuteJs.py
+-rw-rw-rw-   0        0        0     1755 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyExternalCss.py
+-rw-rw-rw-   0        0        0     1746 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyExternalJs.py
+-rw-rw-rw-   0        0        0     2714 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyExtraSpinner.py
+-rw-rw-rw-   0        0        0     1722 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyEyeDropper.py
+-rw-rw-rw-   0        0        0     3393 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFancyButton.py
+-rw-rw-rw-   0        0        0     3583 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFancyMessage.py
+-rw-rw-rw-   0        0        0     5203 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFancyNotification.py
+-rw-rw-rw-   0        0        0     3140 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFixed.py
+-rw-rw-rw-   0        0        0     3737 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFogBackground.py
+-rw-rw-rw-   0        0        0     1742 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFullscreen.py
+-rw-rw-rw-   0        0        0     1549 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGeolocation.py
+-rw-rw-rw-   0        0        0     2507 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGithubColorPicker.py
+-rw-rw-rw-   0        0        0     3518 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGlobeBackground.py
+-rw-rw-rw-   0        0        0     8585 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGrid.py
+-rw-rw-rw-   0        0        0     1902 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGridItem.py
+-rw-rw-rw-   0        0        0     5861 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGuide.py
+-rw-rw-rw-   0        0        0     3601 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyHaloBackground.py
+-rw-rw-rw-   0        0        0     1924 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyHexColorPicker.py
+-rw-rw-rw-   0        0        0     3143 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyHighlightWords.py
+-rw-rw-rw-   0        0        0     1696 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyIdle.py
+-rw-rw-rw-   0        0        0     2778 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyIframeMessenger.py
+-rw-rw-rw-   0        0        0    19103 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyImageCropper.py
+-rw-rw-rw-   0        0        0     4331 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyImageGallery.py
+-rw-rw-rw-   0        0        0     2049 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyImagePaste.py
+-rw-rw-rw-   0        0        0     1903 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyInViewport.py
+-rw-rw-rw-   0        0        0     5738 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyJsonViewer.py
+-rw-rw-rw-   0        0        0     1856 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyKeyPress.py
+-rw-rw-rw-   0        0        0     2586 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyLazyLoad.py
+-rw-rw-rw-   0        0        0     2175 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyListenPaste.py
+-rw-rw-rw-   0        0        0     1695 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyListenScroll.py
+-rw-rw-rw-   0        0        0     1565 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyListenUnload.py
+-rw-rw-rw-   0        0        0     2008 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyLocalLargeStorage.py
+-rw-rw-rw-   0        0        0     1933 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyLocalStorage.py
+-rw-rw-rw-   0        0        0     2569 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyLocation.py
+-rw-rw-rw-   0        0        0     1842 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyLongPress.py
+-rw-rw-rw-   0        0        0    24340 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyMarkdownEditor.py
+-rw-rw-rw-   0        0        0     1878 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyMediaQuery.py
+-rw-rw-rw-   0        0        0     5688 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyMotion.py
+-rw-rw-rw-   0        0        0     1523 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyMousePosition.py
+-rw-rw-rw-   0        0        0    14140 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyMusicPlayer.py
+-rw-rw-rw-   0        0        0     3815 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyNetBackground.py
+-rw-rw-rw-   0        0        0     1592 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyPageLeave.py
+-rw-rw-rw-   0        0        0     4620 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyPhotoSphereViewer.py
+-rw-rw-rw-   0        0        0     3250 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyQRCode.py
+-rw-rw-rw-   0        0        0     7051 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyRND.py
+-rw-rw-rw-   0        0        0     1618 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyRawHTML.py
+-rw-rw-rw-   0        0        0     1667 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyReload.py
+-rw-rw-rw-   0        0        0     5349 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyResizable.py
+-rw-rw-rw-   0        0        0     1552 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyResponsive.py
+-rw-rw-rw-   0        0        0     1933 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyRgbColorPicker.py
+-rw-rw-rw-   0        0        0    19074 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyRichTextEditor.py
+-rw-rw-rw-   0        0        0     3435 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyRingsBackground.py
+-rw-rw-rw-   0        0        0     3647 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyScroll.py
+-rw-rw-rw-   0        0        0     3225 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyScrollbars.py
+-rw-rw-rw-   0        0        0     5330 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferySeamlessScroll.py
+-rw-rw-rw-   0        0        0     1945 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferySessionStorage.py
+-rw-rw-rw-   0        0        0     1492 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferySetTitle.py
+-rw-rw-rw-   0        0        0     1876 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyShadowDom.py
+-rw-rw-rw-   0        0        0     5532 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyShortcutPanel.py
+-rw-rw-rw-   0        0        0     4924 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferySortable.py
+-rw-rw-rw-   0        0        0     2649 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferySticky.py
+-rw-rw-rw-   0        0        0     1610 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyStyle.py
+-rw-rw-rw-   0        0        0     2794 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTabMessenger.py
+-rw-rw-rw-   0        0        0     2079 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTextSelection.py
+-rw-rw-rw-   0        0        0     1967 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyThrottleProp.py
+-rw-rw-rw-   0        0        0     6873 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTiltHover.py
+-rw-rw-rw-   0        0        0     1771 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTimeout.py
+-rw-rw-rw-   0        0        0     3908 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTopProgress.py
+-rw-rw-rw-   0        0        0     3272 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTopologyBackground.py
+-rw-rw-rw-   0        0        0     3529 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTrunkBackground.py
+-rw-rw-rw-   0        0        0     2506 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTwitterColorPicker.py
+-rw-rw-rw-   0        0        0     2322 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyVirtualList.py
+-rw-rw-rw-   0        0        0     3653 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyWavesBackground.py
+-rw-rw-rw-   0        0        0     2924 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyWebSocket.py
+-rw-rw-rw-   0        0        0     1743 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyWheelColorPicker.py
+-rw-rw-rw-   0        0        0     1632 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyWindowSize.py
+-rw-rw-rw-   0        0        0     1869 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyWordPreview.py
+-rw-rw-rw-   0        0        0     3469 2024-03-10 13:40:58.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/__init__.py
+-rw-rw-rw-   0        0        0     8058 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/_imports_.py
+-rw-rw-rw-   0        0        0     8871 2024-03-10 13:29:03.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/alias.py
+-rw-rw-rw-   0        0        0   826468 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_animated_3d_background_p5.js
+-rw-rw-rw-   0        0        0   789712 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_animated_3d_background_three.js
+-rw-rw-rw-   0        0        0    80015 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_animated_image.js
+-rw-rw-rw-   0        0        0    84308 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_aplayer.js
+-rw-rw-rw-   0        0        0     7109 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_auto_animate.js
+-rw-rw-rw-   0        0        0     3421 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_auto_fit.js
+-rw-rw-rw-   0        0        0    32766 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_captcha.js
+-rw-rw-rw-   0        0        0    86638 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_color_pickers.js
+-rw-rw-rw-   0        0        0  1227797 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_dplayer.js
+-rw-rw-rw-   0        0        0   507227 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_emoji_picker.js
+-rw-rw-rw-   0        0        0  1809348 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_excel_preview.js
+-rw-rw-rw-   0        0        0   158423 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_extra_spinner.js
+-rw-rw-rw-   0        0        0    51671 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_fancy_button.js
+-rw-rw-rw-   0        0        0    58561 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_grid.js
+-rw-rw-rw-   0        0        0    49415 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_image_cropper.js
+-rw-rw-rw-   0        0        0   116139 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_json_viewer.js
+-rw-rw-rw-   0        0        0    36345 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_local_large_storage.js
+-rw-rw-rw-   0        0        0  4813407 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_markdown_editor.js
+-rw-rw-rw-   0        0        0    95908 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_motion.js
+-rw-rw-rw-   0        0        0   193585 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_music_player.js
+-rw-rw-rw-   0        0        0  1288373 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_photo_sphere_viewer.js
+-rw-rw-rw-   0        0        0    19297 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_resizable.js
+-rw-rw-rw-   0        0        0   805743 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_rich_text_editor.js
+-rw-rw-rw-   0        0        0    58078 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_rnd.js
+-rw-rw-rw-   0        0        0    10166 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_seamless_scroll.js
+-rw-rw-rw-   0        0        0    73763 2024-03-14 07:43:10.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_shortcut_panel.js
+-rw-rw-rw-   0        0        0    70073 2024-03-14 07:43:10.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_sortable.js
+-rw-rw-rw-   0        0        0   279104 2024-03-14 07:43:10.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_word_preview.js
+-rw-rw-rw-   0        0        0   395057 2024-03-14 07:43:09.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/async-fuc-shared.js
+-rw-rw-rw-   0        0        0  1111023 2024-03-14 07:43:10.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/feffery_utils_components.min.js
+-rw-rw-rw-   0        0        0  1070359 2024-03-14 07:43:13.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/metadata.json
+-rw-rw-rw-   0        0        0     5243 2024-03-14 07:43:11.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components/package-info.json
+drwxrwxrwx   0        0        0        0 2024-03-14 07:43:15.206659 feffery_utils_components-0.2.0rc9/feffery_utils_components.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-03-14 07:43:14.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6923 2024-03-14 07:43:14.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-14 07:43:14.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-03-14 07:43:14.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-03-14 07:43:14.000000 feffery_utils_components-0.2.0rc9/feffery_utils_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5243 2024-03-14 07:43:04.000000 feffery_utils_components-0.2.0rc9/package.json
+-rw-rw-rw-   0        0        0       42 2024-03-14 07:43:15.208691 feffery_utils_components-0.2.0rc9/setup.cfg
+-rw-rw-rw-   0        0        0      809 2024-03-11 08:28:00.000000 feffery_utils_components-0.2.0rc9/setup.py
```

### Comparing `feffery_utils_components-0.2.0rc8/LICENSE` & `feffery_utils_components-0.2.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/README.md` & `feffery_utils_components-0.2.0rc9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```bash
 pip install feffery-utils-components -U
 ```
 
 ## 2 最新预发布版本安装方式
 
 > [!NOTE]  
-> 最新预发布版本（2024-03-08）：`0.2.0rc7`
+> 最新预发布版本（2024-03-11）：`0.2.0rc9`
 
 ```bash
 pip install feffery-utils-components --pre -U
 ```
 
 ## 3 静态资源 CDN 加速方法
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
    badge/feffery-utils-components)](https://pepy.tech/project/feffery-utils-
   components) [![Downloads](https://pepy.tech/badge/feffery-utils-components/
           month)](https://pepy.tech/project/feffery-utils-components)
 `feffery-components`è®¡åå­é¡¹ç®ï¼`Plotly
 Dash`ç¬¬ä¸æ¹ç»ä»¶åºï¼å°è¶å¤å®ç¨è¾å©åè½ç»ä»¶å¼å¥`Dash`çä¸ç
 ð¥³ï¼ææ°çæ¬ï¼`0.1.29` ## 1 ææ°çæ¬å®è£æ¹å¼ ```bash pip
 install feffery-utils-components -U ``` ## 2 ææ°é¢åå¸çæ¬å®è£æ¹å¼
-> [!NOTE] > ææ°é¢åå¸çæ¬ï¼2024-03-08ï¼ï¼`0.2.0rc7` ```bash pip
+> [!NOTE] > ææ°é¢åå¸çæ¬ï¼2024-03-11ï¼ï¼`0.2.0rc9` ```bash pip
 install feffery-utils-components --pre -U ``` ## 3 éæèµæº CDN
 å éæ¹æ³ ```Python # édebugæ¨¡å¼ä¸å¯¹Dash
 ()ä¼ å¥åæ°serve_locally=Falseä¼å¼ºå¶æµè§å¨ç«¯ä»unpkg
 cdnå è½½åä¸ªä¾èµç #
 xxx.min.jsç­éæèµæºï¼ä»èé¿åå ç¨æå¡å¨å¸¦å®½ï¼éåä¸­å°åç«ç¹å éè®¿é®
 app = dash.Dash(serve_locally=False) ``` ## 4 å¨çº¿ææ¡£ _æ___æ_¡_£_å__°_å__ ## 5
 è´¡ç®è_[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_C_N_F_e_f_f_e_r_y_/_f_e_f_f_e_r_y_-_u_t_i_l_s_-_c_o_m_p_o_n_e_n_t_s_]
```

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyAPlayer.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyAPlayer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyAnimatedImage.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyAnimatedImage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyAutoAnimate.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyAutoAnimate.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyAutoFit.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyAutoFit.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyBirdsBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyBirdsBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyBlockColorPicker.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyBlockColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCaptcha.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCaptcha.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCellsBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCellsBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCircleColorPicker.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCircleColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCloudsBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCloudsBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCloudsTwoBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCloudsTwoBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCompareSlider.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCompareSlider.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCookie.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCookie.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCountDown.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCountDown.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCountUp.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCountUp.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyCssVar.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyCssVar.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDPlayer.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDPlayer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDebounceProp.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDebounceProp.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDeviceDetect.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDeviceDetect.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDiv.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDiv.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDocumentVisibility.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDocumentVisibility.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyDraggable.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyDraggable.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyEmojiPicker.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyEmojiPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyExcelPreview.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyExcelPreview.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyExecuteJs.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyStyle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
-class FefferyExecuteJs(Component):
-    """A FefferyExecuteJs component.
+class FefferyStyle(Component):
+    """A FefferyStyle component.
 
 
 Keyword arguments:
 
 - id (string; optional):
     组件id.
 
-- jsString (string; optional):
-    设置要执行的js代码字符串.
+- key (string; optional):
+    辅助刷新用唯一标识key值.
 
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
         Holds the name of the component that is loading.
 
     - is_loading (boolean; optional):
         Determines if the component is loading or not.
 
     - prop_name (string; optional):
-        Holds which property is loading."""
+        Holds which property is loading.
+
+- rawStyle (string; optional):
+    设置要添加到文档中的原生css字符."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_utils_components'
-    _type = 'FefferyExecuteJs'
+    _type = 'FefferyStyle'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, jsString=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'jsString', 'loading_state']
+    def __init__(self, id=Component.UNDEFINED, key=Component.UNDEFINED, rawStyle=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'key', 'loading_state', 'rawStyle']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'jsString', 'loading_state']
+        self.available_properties = ['id', 'key', 'loading_state', 'rawStyle']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
-        super(FefferyExecuteJs, self).__init__(**args)
+        super(FefferyStyle, self).__init__(**args)
```

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyExternalCss.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyExternalCss.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyExternalJs.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyExternalJs.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyExtraSpinner.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyExtraSpinner.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyEyeDropper.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyEyeDropper.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFancyButton.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFancyButton.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFancyMessage.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFancyMessage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFancyNotification.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFancyNotification.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFixed.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFixed.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFogBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFogBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyFullscreen.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyFullscreen.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGeolocation.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGeolocation.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGithubColorPicker.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGithubColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGlobeBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGlobeBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGrid.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGrid.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGridItem.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGridItem.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyGuide.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyGuide.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyHaloBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyHaloBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyHexColorPicker.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyHexColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyHighlightWords.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyHighlightWords.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyIdle.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyIdle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyIframeMessenger.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyIframeMessenger.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyImageCropper.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyImageCropper.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyImageGallery.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyImageGallery.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyImagePaste.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyImagePaste.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyInViewport.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyInViewport.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyJsonViewer.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyJsonViewer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyKeyPress.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyKeyPress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyLazyLoad.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyLazyLoad.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyListenPaste.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyListenPaste.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyListenScroll.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyListenScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyListenUnload.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyListenUnload.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyLocalLargeStorage.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyLocalLargeStorage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyLocalStorage.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyLocalStorage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyLocation.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyLocation.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyLongPress.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyLongPress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyMarkdownEditor.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyMarkdownEditor.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyMediaQuery.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyMediaQuery.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyMotion.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyMotion.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyMousePosition.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyMousePosition.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyMusicPlayer.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyMusicPlayer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyNetBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyNetBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyPageLeave.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyPageLeave.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyPhotoSphereViewer.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyPhotoSphereViewer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyQRCode.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyQRCode.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyRND.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyRND.py`

 * *Files 13% similar despite different names*

```diff
@@ -99,14 +99,23 @@
 
     - y (number; optional):
         竖直方向像素位置.
 
 - resizeGrid (list of numbers; optional):
     针对尺寸调整行为，设置水平和竖直方向上调整的像素步长，格式为：[水平像素步长, 竖直像素步长]  默认：[1, 1].
 
+- selected (boolean; default False):
+    设置或监听当前组件是否处于选择状态  默认：False.
+
+- selectedClassName (string; optional):
+    配置当前组件在选中状态下的css类名.
+
+- selectedStyle (dict; optional):
+    设置当前组件在选中状态下的css样式.
+
 - size (dict; optional):
     设置或监听当前组件尺寸信息.
 
     `size` is a dict with keys:
 
     - height (number | string; optional):
         高度值，数值型表示像素高度，字符型与css相关属性值格式兼容，如'300px'、'50%'等.
@@ -117,18 +126,18 @@
 - style (dict; optional):
     css样式."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_utils_components'
     _type = 'FefferyRND'
     @_explicitize_args
-    def __init__(self, children=None, id=Component.UNDEFINED, key=Component.UNDEFINED, style=Component.UNDEFINED, className=Component.UNDEFINED, defaultState=Component.UNDEFINED, size=Component.UNDEFINED, position=Component.UNDEFINED, minWidth=Component.UNDEFINED, minHeight=Component.UNDEFINED, maxWidth=Component.UNDEFINED, maxHeight=Component.UNDEFINED, resizeGrid=Component.UNDEFINED, dragGrid=Component.UNDEFINED, lockAspectRatio=Component.UNDEFINED, lockAspectRatioExtraWidth=Component.UNDEFINED, lockAspectRatioExtraHeight=Component.UNDEFINED, direction=Component.UNDEFINED, disableDragging=Component.UNDEFINED, dragAxis=Component.UNDEFINED, bounds=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['children', 'id', 'bounds', 'className', 'defaultState', 'direction', 'disableDragging', 'dragAxis', 'dragGrid', 'key', 'loading_state', 'lockAspectRatio', 'lockAspectRatioExtraHeight', 'lockAspectRatioExtraWidth', 'maxHeight', 'maxWidth', 'minHeight', 'minWidth', 'position', 'resizeGrid', 'size', 'style']
+    def __init__(self, children=None, id=Component.UNDEFINED, key=Component.UNDEFINED, style=Component.UNDEFINED, className=Component.UNDEFINED, defaultState=Component.UNDEFINED, size=Component.UNDEFINED, position=Component.UNDEFINED, minWidth=Component.UNDEFINED, minHeight=Component.UNDEFINED, maxWidth=Component.UNDEFINED, maxHeight=Component.UNDEFINED, resizeGrid=Component.UNDEFINED, dragGrid=Component.UNDEFINED, lockAspectRatio=Component.UNDEFINED, lockAspectRatioExtraWidth=Component.UNDEFINED, lockAspectRatioExtraHeight=Component.UNDEFINED, direction=Component.UNDEFINED, disableDragging=Component.UNDEFINED, dragAxis=Component.UNDEFINED, bounds=Component.UNDEFINED, selected=Component.UNDEFINED, selectedStyle=Component.UNDEFINED, selectedClassName=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['children', 'id', 'bounds', 'className', 'defaultState', 'direction', 'disableDragging', 'dragAxis', 'dragGrid', 'key', 'loading_state', 'lockAspectRatio', 'lockAspectRatioExtraHeight', 'lockAspectRatioExtraWidth', 'maxHeight', 'maxWidth', 'minHeight', 'minWidth', 'position', 'resizeGrid', 'selected', 'selectedClassName', 'selectedStyle', 'size', 'style']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['children', 'id', 'bounds', 'className', 'defaultState', 'direction', 'disableDragging', 'dragAxis', 'dragGrid', 'key', 'loading_state', 'lockAspectRatio', 'lockAspectRatioExtraHeight', 'lockAspectRatioExtraWidth', 'maxHeight', 'maxWidth', 'minHeight', 'minWidth', 'position', 'resizeGrid', 'size', 'style']
+        self.available_properties = ['children', 'id', 'bounds', 'className', 'defaultState', 'direction', 'disableDragging', 'dragAxis', 'dragGrid', 'key', 'loading_state', 'lockAspectRatio', 'lockAspectRatioExtraHeight', 'lockAspectRatioExtraWidth', 'maxHeight', 'maxWidth', 'minHeight', 'minWidth', 'position', 'resizeGrid', 'selected', 'selectedClassName', 'selectedStyle', 'size', 'style']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args if k != 'children'}
 
         super(FefferyRND, self).__init__(children=children, **args)
```

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyRawHTML.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyRawHTML.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyReload.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyReload.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyResizable.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyResizable.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyResponsive.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyResponsive.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyRgbColorPicker.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyRgbColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyRichTextEditor.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyRichTextEditor.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyRingsBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyRingsBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyScroll.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyScrollbars.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyScrollbars.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferySeamlessScroll.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferySeamlessScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferySessionStorage.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferySessionStorage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferySetTitle.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferySetTitle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyShadowDom.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyShadowDom.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyShortcutPanel.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyShortcutPanel.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferySortable.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferySortable.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferySticky.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferySticky.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyStyle.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyWheelColorPicker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
-class FefferyStyle(Component):
-    """A FefferyStyle component.
+class FefferyWheelColorPicker(Component):
+    """A FefferyWheelColorPicker component.
 
 
 Keyword arguments:
 
 - id (string; optional):
     组件id.
 
-- key (string; optional):
-    辅助刷新用唯一标识key值.
+- className (string; optional):
+    css类名.
+
+- color (string; optional):
+    设置或监听当前选中色彩对应16进制颜色值.
 
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
         Holds the name of the component that is loading.
 
     - is_loading (boolean; optional):
         Determines if the component is loading or not.
 
     - prop_name (string; optional):
         Holds which property is loading.
 
-- rawStyle (string; optional):
-    设置要添加到文档中的原生css字符."""
+- style (dict; optional):
+    css样式."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_utils_components'
-    _type = 'FefferyStyle'
+    _type = 'FefferyWheelColorPicker'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, key=Component.UNDEFINED, rawStyle=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'key', 'loading_state', 'rawStyle']
+    def __init__(self, id=Component.UNDEFINED, style=Component.UNDEFINED, className=Component.UNDEFINED, color=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'className', 'color', 'loading_state', 'style']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'key', 'loading_state', 'rawStyle']
+        self.available_properties = ['id', 'className', 'color', 'loading_state', 'style']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
-        super(FefferyStyle, self).__init__(**args)
+        super(FefferyWheelColorPicker, self).__init__(**args)
```

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTabMessenger.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTabMessenger.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTextSelection.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTextSelection.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyThrottleProp.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyThrottleProp.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTiltHover.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTiltHover.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTimeout.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTimeout.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTopProgress.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTopProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTopologyBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTopologyBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTrunkBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTrunkBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyTwitterColorPicker.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyTwitterColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyVirtualList.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyVirtualList.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyWavesBackground.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyWavesBackground.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyWebSocket.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyWebSocket.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyWheelColorPicker.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyWindowSize.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
-class FefferyWheelColorPicker(Component):
-    """A FefferyWheelColorPicker component.
+class FefferyWindowSize(Component):
+    """A FefferyWindowSize component.
 
 
 Keyword arguments:
 
 - id (string; optional):
     组件id.
 
-- className (string; optional):
-    css类名.
+- _height (number; optional):
+    监听当前浏览器窗口高度.
 
-- color (string; optional):
-    设置或监听当前选中色彩对应16进制颜色值.
+- _width (number; optional):
+    监听当前浏览器窗口像素宽度.
 
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
         Holds the name of the component that is loading.
 
     - is_loading (boolean; optional):
         Determines if the component is loading or not.
 
     - prop_name (string; optional):
-        Holds which property is loading.
-
-- style (dict; optional):
-    css样式."""
+        Holds which property is loading."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_utils_components'
-    _type = 'FefferyWheelColorPicker'
+    _type = 'FefferyWindowSize'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, style=Component.UNDEFINED, className=Component.UNDEFINED, color=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'className', 'color', 'loading_state', 'style']
+    def __init__(self, id=Component.UNDEFINED, _width=Component.UNDEFINED, _height=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', '_height', '_width', 'loading_state']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'className', 'color', 'loading_state', 'style']
+        self.available_properties = ['id', '_height', '_width', 'loading_state']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
-        super(FefferyWheelColorPicker, self).__init__(**args)
+        super(FefferyWindowSize, self).__init__(**args)
```

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/FefferyWindowSize.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/FefferyWordPreview.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
-class FefferyWindowSize(Component):
-    """A FefferyWindowSize component.
+class FefferyWordPreview(Component):
+    """A FefferyWordPreview component.
 
 
 Keyword arguments:
 
 - id (string; optional):
     组件id.
 
-- _height (number; optional):
-    监听当前浏览器窗口高度.
-
-- _width (number; optional):
-    监听当前浏览器窗口像素宽度.
+- className (string; optional):
+    css类名.
 
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
         Holds the name of the component that is loading.
 
     - is_loading (boolean; optional):
         Determines if the component is loading or not.
 
     - prop_name (string; optional):
-        Holds which property is loading."""
+        Holds which property is loading.
+
+- src (string; required):
+    必填，设置目标excel文件资源地址.
+
+- style (dict; optional):
+    css样式."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_utils_components'
-    _type = 'FefferyWindowSize'
+    _type = 'FefferyWordPreview'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, _width=Component.UNDEFINED, _height=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', '_height', '_width', 'loading_state']
+    def __init__(self, id=Component.UNDEFINED, style=Component.UNDEFINED, className=Component.UNDEFINED, src=Component.REQUIRED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'className', 'loading_state', 'src', 'style']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', '_height', '_width', 'loading_state']
+        self.available_properties = ['id', 'className', 'loading_state', 'src', 'style']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
-        super(FefferyWindowSize, self).__init__(**args)
+        for k in ['src']:
+            if k not in args:
+                raise TypeError(
+                    'Required argument `' + k + '` was not specified.')
+
+        super(FefferyWordPreview, self).__init__(**args)
```

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/__init__.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/_imports_.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/alias.py` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/alias.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_animated_3d_background_p5.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_animated_3d_background_p5.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_animated_3d_background_three.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_animated_3d_background_three.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_animated_image.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_animated_image.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_aplayer.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_aplayer.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_auto_animate.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_auto_animate.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_auto_fit.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_auto_fit.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_captcha.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_captcha.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_color_pickers.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_color_pickers.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_dplayer.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_dplayer.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_emoji_picker.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_emoji_picker.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_excel_preview.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_excel_preview.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_extra_spinner.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_extra_spinner.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_fancy_button.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_fancy_button.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_grid.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_grid.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_image_cropper.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_image_cropper.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_json_viewer.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_json_viewer.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_local_large_storage.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_local_large_storage.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_markdown_editor.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_markdown_editor.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_motion.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_motion.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_music_player.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_music_player.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_photo_sphere_viewer.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_photo_sphere_viewer.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_resizable.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_resizable.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_rich_text_editor.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_rich_text_editor.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_rnd.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_rnd.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,48 @@
 (window.webpackJsonpfeffery_utils_components = window.webpackJsonpfeffery_utils_components || []).push([
     [24], {
         533: function(k, t, e) {
             "use strict";
             e.r(t);
 
-            function d(t) {
+            function f(t) {
                 return Boolean(t.touches && t.touches.length)
             }
 
-            function a(t, e, o, i) {
+            function a(t, e, o, r) {
                 if (t && "string" == typeof t) {
-                    if (w(t, "px")) return Number(t.replace("px", ""));
-                    if (w(t, "%")) return e * (Number(t.replace("%", "")) / 100);
-                    if (w(t, "vw")) return o * (Number(t.replace("vw", "")) / 100);
-                    if (w(t, "vh")) return i * (Number(t.replace("vh", "")) / 100)
+                    if (v(t, "px")) return Number(t.replace("px", ""));
+                    if (v(t, "%")) return e * (Number(t.replace("%", "")) / 100);
+                    if (v(t, "vw")) return o * (Number(t.replace("vw", "")) / 100);
+                    if (v(t, "vh")) return r * (Number(t.replace("vh", "")) / 100)
                 }
                 return t
             }
-            var i, n, o, r, P = e(1),
+            var r, i, o, n, C = e(1),
                 s = e(865),
                 s = e.n(s),
-                l = (r = function(t, e) {
-                    return (r = Object.setPrototypeOf || ({
+                l = (n = function(t, e) {
+                    return (n = Object.setPrototypeOf || ({
                             __proto__: []
                         }
                         instanceof Array ? function(t, e) {
                             t.__proto__ = e
                         } : function(t, e) {
                             for (var o in e) Object.prototype.hasOwnProperty.call(e, o) && (t[o] = e[o])
                         }))(t, e)
                 }, function(t, e) {
                     function o() {
                         this.constructor = t
                     }
-                    r(t, e), t.prototype = null === e ? Object.create(e) : (o.prototype = e.prototype, new o)
+                    n(t, e), t.prototype = null === e ? Object.create(e) : (o.prototype = e.prototype, new o)
                 }),
                 p = function() {
                     return (p = Object.assign || function(t) {
-                        for (var e, o = 1, i = arguments.length; o < i; o++)
-                            for (var n in e = arguments[o]) Object.prototype.hasOwnProperty.call(e, n) && (t[n] = e[n]);
+                        for (var e, o = 1, r = arguments.length; o < r; o++)
+                            for (var i in e = arguments[o]) Object.prototype.hasOwnProperty.call(e, i) && (t[i] = e[i]);
                         return t
                     }).apply(this, arguments)
                 },
                 u = {
                     top: {
                         width: "100%",
                         height: "10px",
@@ -100,337 +100,337 @@
                         height: "20px",
                         position: "absolute",
                         left: "-10px",
                         top: "-10px",
                         cursor: "nw-resize"
                     }
                 },
-                h = (o = P.PureComponent, l(E, o), E.prototype.render = function() {
-                    return P.createElement("div", {
+                c = (o = C.PureComponent, l(z, o), z.prototype.render = function() {
+                    return C.createElement("div", {
                         className: this.props.className || "",
                         style: p(p({
                             position: "absolute",
                             userSelect: "none"
                         }, u[this.props.direction]), this.props.replaceStyles || {}),
                         onMouseDown: this.onMouseDown,
                         onTouchStart: this.onTouchStart
                     }, this.props.children)
-                }, E),
+                }, z),
                 l = e(869),
                 l = e.n(l),
-                c = (n = function(t, e) {
-                    return (n = Object.setPrototypeOf || ({
+                h = (i = function(t, e) {
+                    return (i = Object.setPrototypeOf || ({
                             __proto__: []
                         }
                         instanceof Array ? function(t, e) {
                             t.__proto__ = e
                         } : function(t, e) {
                             for (var o in e) Object.prototype.hasOwnProperty.call(e, o) && (t[o] = e[o])
                         }))(t, e)
                 }, function(t, e) {
                     function o() {
                         this.constructor = t
                     }
-                    n(t, e), t.prototype = null === e ? Object.create(e) : (o.prototype = e.prototype, new o)
+                    i(t, e), t.prototype = null === e ? Object.create(e) : (o.prototype = e.prototype, new o)
                 }),
-                f = function() {
-                    return (f = Object.assign || function(t) {
-                        for (var e, o = 1, i = arguments.length; o < i; o++)
-                            for (var n in e = arguments[o]) Object.prototype.hasOwnProperty.call(e, n) && (t[n] = e[n]);
+                d = function() {
+                    return (d = Object.assign || function(t) {
+                        for (var e, o = 1, r = arguments.length; o < r; o++)
+                            for (var i in e = arguments[o]) Object.prototype.hasOwnProperty.call(e, i) && (t[i] = e[i]);
                         return t
                     }).apply(this, arguments)
                 },
-                g = {
+                A = {
                     width: "auto",
                     height: "auto"
                 },
-                y = l()(function(t, e, o) {
+                g = l()(function(t, e, o) {
                     return Math.max(Math.min(t, o), e)
                 }),
-                b = l()(function(t, e) {
+                y = l()(function(t, e) {
                     return Math.round(t / e) * e
                 }),
-                m = l()(function(t, e) {
+                b = l()(function(t, e) {
                     return new RegExp(t, "i").test(e)
                 }),
-                v = l()(function(i, n, t) {
+                m = l()(function(r, i, t) {
                     void 0 === t && (t = 0);
-                    var e = n.reduce(function(t, e, o) {
-                            return Math.abs(e - i) < Math.abs(n[t] - i) ? o : t
+                    var e = i.reduce(function(t, e, o) {
+                            return Math.abs(e - r) < Math.abs(i[t] - r) ? o : t
                         }, 0),
-                        o = Math.abs(n[e] - i);
-                    return 0 === t || o < t ? n[e] : i
+                        o = Math.abs(i[e] - r);
+                    return 0 === t || o < t ? i[e] : r
                 }),
-                w = l()(function(t, e) {
+                v = l()(function(t, e) {
                     return t.substr(t.length - e.length, e.length) === e
                 }),
-                S = l()(function(t) {
-                    return "auto" === (t = t.toString()) || w(t, "px") || w(t, "%") || w(t, "vh") || w(t, "vw") || w(t, "vmax") || w(t, "vmin") ? t : t + "px"
+                w = l()(function(t) {
+                    return "auto" === (t = t.toString()) || v(t, "px") || v(t, "%") || v(t, "vh") || v(t, "vw") || v(t, "vmax") || v(t, "vmin") ? t : t + "px"
                 }),
-                x = l()(function(t, e, o, i, n, r, s) {
-                    return i = a(i, t.width, e, o), n = a(n, t.height, e, o), r = a(r, t.width, e, o), s = a(s, t.height, e, o), {
-                        maxWidth: void 0 === i ? void 0 : Number(i),
-                        maxHeight: void 0 === n ? void 0 : Number(n),
-                        minWidth: void 0 === r ? void 0 : Number(r),
+                _ = l()(function(t, e, o, r, i, n, s) {
+                    return r = a(r, t.width, e, o), i = a(i, t.height, e, o), n = a(n, t.width, e, o), s = a(s, t.height, e, o), {
+                        maxWidth: void 0 === r ? void 0 : Number(r),
+                        maxHeight: void 0 === i ? void 0 : Number(i),
+                        minWidth: void 0 === n ? void 0 : Number(n),
                         minHeight: void 0 === s ? void 0 : Number(s)
                     }
                 }),
-                z = ["as", "style", "className", "grid", "snap", "bounds", "boundsByDirection", "size", "defaultSize", "minWidth", "minHeight", "maxWidth", "maxHeight", "lockAspectRatio", "lockAspectRatioExtraWidth", "lockAspectRatioExtraHeight", "enable", "handleStyles", "handleClasses", "handleWrapperStyle", "handleWrapperClass", "children", "onResizeStart", "onResize", "onResizeStop", "handleComponent", "scale", "resizeRatio", "snapGap"],
-                R = (i = P.PureComponent, c(O, i), Object.defineProperty(O.prototype, "parentNode", {
+                L = ["as", "style", "className", "grid", "snap", "bounds", "boundsByDirection", "size", "defaultSize", "minWidth", "minHeight", "maxWidth", "maxHeight", "lockAspectRatio", "lockAspectRatioExtraWidth", "lockAspectRatioExtraHeight", "enable", "handleStyles", "handleClasses", "handleWrapperStyle", "handleWrapperClass", "children", "onResizeStart", "onResize", "onResizeStop", "handleComponent", "scale", "resizeRatio", "snapGap"],
+                B = (r = C.PureComponent, h(x, r), Object.defineProperty(x.prototype, "parentNode", {
                     get: function() {
                         return this.resizable ? this.resizable.parentNode : null
                     },
                     enumerable: !1,
                     configurable: !0
-                }), Object.defineProperty(O.prototype, "window", {
+                }), Object.defineProperty(x.prototype, "window", {
                     get: function() {
                         return this.resizable && this.resizable.ownerDocument ? this.resizable.ownerDocument.defaultView : null
                     },
                     enumerable: !1,
                     configurable: !0
-                }), Object.defineProperty(O.prototype, "propsSize", {
+                }), Object.defineProperty(x.prototype, "propsSize", {
                     get: function() {
-                        return this.props.size || this.props.defaultSize || g
+                        return this.props.size || this.props.defaultSize || A
                     },
                     enumerable: !1,
                     configurable: !0
-                }), Object.defineProperty(O.prototype, "size", {
+                }), Object.defineProperty(x.prototype, "size", {
                     get: function() {
-                        var t, e, o, i = 0,
-                            n = 0;
-                        return this.resizable && this.window && (t = this.resizable.offsetWidth, e = this.resizable.offsetHeight, "relative" !== (o = this.resizable.style.position) && (this.resizable.style.position = "relative"), i = "auto" !== this.resizable.style.width ? this.resizable.offsetWidth : t, n = "auto" !== this.resizable.style.height ? this.resizable.offsetHeight : e, this.resizable.style.position = o), {
-                            width: i,
-                            height: n
+                        var t, e, o, r = 0,
+                            i = 0;
+                        return this.resizable && this.window && (t = this.resizable.offsetWidth, e = this.resizable.offsetHeight, "relative" !== (o = this.resizable.style.position) && (this.resizable.style.position = "relative"), r = "auto" !== this.resizable.style.width ? this.resizable.offsetWidth : t, i = "auto" !== this.resizable.style.height ? this.resizable.offsetHeight : e, this.resizable.style.position = o), {
+                            width: r,
+                            height: i
                         }
                     },
                     enumerable: !1,
                     configurable: !0
-                }), Object.defineProperty(O.prototype, "sizeStyle", {
+                }), Object.defineProperty(x.prototype, "sizeStyle", {
                     get: function() {
                         function t(t) {
                             var e;
-                            return void 0 === o.state[t] || "auto" === o.state[t] ? "auto" : o.propsSize && o.propsSize[t] && w(o.propsSize[t].toString(), "%") ? w(o.state[t].toString(), "%") ? o.state[t].toString() : (e = o.getParentSize(), Number(o.state[t].toString().replace("px", "")) / e[t] * 100 + "%") : S(o.state[t])
+                            return void 0 === o.state[t] || "auto" === o.state[t] ? "auto" : o.propsSize && o.propsSize[t] && v(o.propsSize[t].toString(), "%") ? v(o.state[t].toString(), "%") ? o.state[t].toString() : (e = o.getParentSize(), Number(o.state[t].toString().replace("px", "")) / e[t] * 100 + "%") : w(o.state[t])
                         }
                         var o = this,
                             e = this.props.size;
                         return {
-                            width: e && void 0 !== e.width && !this.state.isResizing ? S(e.width) : t("width"),
-                            height: e && void 0 !== e.height && !this.state.isResizing ? S(e.height) : t("height")
+                            width: e && void 0 !== e.width && !this.state.isResizing ? w(e.width) : t("width"),
+                            height: e && void 0 !== e.height && !this.state.isResizing ? w(e.height) : t("height")
                         }
                     },
                     enumerable: !1,
                     configurable: !0
-                }), O.prototype.getParentSize = function() {
-                    var t, e, o, i;
-                    return this.parentNode ? (t = this.appendBase()) ? (e = !1, "wrap" !== (o = this.parentNode.style.flexWrap) && (e = !0, this.parentNode.style.flexWrap = "wrap"), t.style.position = "relative", t.style.minWidth = "100%", t.style.minHeight = "100%", i = {
+                }), x.prototype.getParentSize = function() {
+                    var t, e, o, r;
+                    return this.parentNode ? (t = this.appendBase()) ? (e = !1, "wrap" !== (o = this.parentNode.style.flexWrap) && (e = !0, this.parentNode.style.flexWrap = "wrap"), t.style.position = "relative", t.style.minWidth = "100%", t.style.minHeight = "100%", r = {
                         width: t.offsetWidth,
                         height: t.offsetHeight
-                    }, e && (this.parentNode.style.flexWrap = o), this.removeBase(t), i) : {
+                    }, e && (this.parentNode.style.flexWrap = o), this.removeBase(t), r) : {
                         width: 0,
                         height: 0
                     } : this.window ? {
                         width: this.window.innerWidth,
                         height: this.window.innerHeight
                     } : {
                         width: 0,
                         height: 0
                     }
-                }, O.prototype.bindEvents = function() {
+                }, x.prototype.bindEvents = function() {
                     this.window && (this.window.addEventListener("mouseup", this.onMouseUp), this.window.addEventListener("mousemove", this.onMouseMove), this.window.addEventListener("mouseleave", this.onMouseUp), this.window.addEventListener("touchmove", this.onMouseMove, {
                         capture: !0,
                         passive: !1
                     }), this.window.addEventListener("touchend", this.onMouseUp))
-                }, O.prototype.unbindEvents = function() {
+                }, x.prototype.unbindEvents = function() {
                     this.window && (this.window.removeEventListener("mouseup", this.onMouseUp), this.window.removeEventListener("mousemove", this.onMouseMove), this.window.removeEventListener("mouseleave", this.onMouseUp), this.window.removeEventListener("touchmove", this.onMouseMove, !0), this.window.removeEventListener("touchend", this.onMouseUp))
-                }, O.prototype.componentDidMount = function() {
+                }, x.prototype.componentDidMount = function() {
                     var t;
                     this.resizable && this.window && (t = this.window.getComputedStyle(this.resizable), this.setState({
                         width: this.state.width || this.size.width,
                         height: this.state.height || this.size.height,
                         flexBasis: "auto" !== t.flexBasis ? t.flexBasis : void 0
                     }))
-                }, O.prototype.componentWillUnmount = function() {
+                }, x.prototype.componentWillUnmount = function() {
                     this.window && this.unbindEvents()
-                }, O.prototype.createSizeForCssProperty = function(t, e) {
+                }, x.prototype.createSizeForCssProperty = function(t, e) {
                     var o = this.propsSize && this.propsSize[e];
                     return "auto" !== this.state[e] || this.state.original[e] !== t || void 0 !== o && "auto" !== o ? t : "auto"
-                }, O.prototype.calculateNewMaxFromBoundary = function(t, e) {
-                    var o, i, n = this.props.boundsByDirection,
-                        r = this.state.direction,
-                        s = n && m("left", r),
-                        n = n && m("top", r);
-                    return "parent" === this.props.bounds ? (r = this.parentNode) && (o = s ? this.resizableRight - this.parentLeft : r.offsetWidth + (this.parentLeft - this.resizableLeft), i = n ? this.resizableBottom - this.parentTop : r.offsetHeight + (this.parentTop - this.resizableTop)) : "window" === this.props.bounds ? this.window && (o = s ? this.resizableRight : this.window.innerWidth - this.resizableLeft, i = n ? this.resizableBottom : this.window.innerHeight - this.resizableTop) : this.props.bounds && (o = s ? this.resizableRight - this.targetLeft : this.props.bounds.offsetWidth + (this.targetLeft - this.resizableLeft), i = n ? this.resizableBottom - this.targetTop : this.props.bounds.offsetHeight + (this.targetTop - this.resizableTop)), {
+                }, x.prototype.calculateNewMaxFromBoundary = function(t, e) {
+                    var o, r, i = this.props.boundsByDirection,
+                        n = this.state.direction,
+                        s = i && b("left", n),
+                        i = i && b("top", n);
+                    return "parent" === this.props.bounds ? (n = this.parentNode) && (o = s ? this.resizableRight - this.parentLeft : n.offsetWidth + (this.parentLeft - this.resizableLeft), r = i ? this.resizableBottom - this.parentTop : n.offsetHeight + (this.parentTop - this.resizableTop)) : "window" === this.props.bounds ? this.window && (o = s ? this.resizableRight : this.window.innerWidth - this.resizableLeft, r = i ? this.resizableBottom : this.window.innerHeight - this.resizableTop) : this.props.bounds && (o = s ? this.resizableRight - this.targetLeft : this.props.bounds.offsetWidth + (this.targetLeft - this.resizableLeft), r = i ? this.resizableBottom - this.targetTop : this.props.bounds.offsetHeight + (this.targetTop - this.resizableTop)), {
                         maxWidth: t = o && Number.isFinite(o) ? t && t < o ? t : o : t,
-                        maxHeight: e = i && Number.isFinite(i) ? e && e < i ? e : i : e
+                        maxHeight: e = r && Number.isFinite(r) ? e && e < r ? e : r : e
                     }
-                }, O.prototype.calculateNewSizeFromDirection = function(t, e) {
+                }, x.prototype.calculateNewSizeFromDirection = function(t, e) {
                     var o = this.props.scale || 1,
-                        i = this.props.resizeRatio || 1,
-                        n = this.state,
-                        r = n.direction,
-                        n = n.original,
+                        r = this.props.resizeRatio || 1,
+                        i = this.state,
+                        n = i.direction,
+                        i = i.original,
                         s = this.props,
                         a = s.lockAspectRatio,
                         l = s.lockAspectRatioExtraHeight,
                         s = s.lockAspectRatioExtraWidth,
-                        p = n.width,
-                        u = n.height,
+                        p = i.width,
+                        u = i.height,
                         l = l || 0,
                         s = s || 0;
-                    return m("right", r) && (p = n.width + (t - n.x) * i / o, a) && (u = (p - s) / this.ratio + l), m("left", r) && (p = n.width - (t - n.x) * i / o, a) && (u = (p - s) / this.ratio + l), m("bottom", r) && (u = n.height + (e - n.y) * i / o, a) && (p = (u - l) * this.ratio + s), {
-                        newWidth: p = m("top", r) && (u = n.height - (e - n.y) * i / o, a) ? (u - l) * this.ratio + s : p,
+                    return b("right", n) && (p = i.width + (t - i.x) * r / o, a) && (u = (p - s) / this.ratio + l), b("left", n) && (p = i.width - (t - i.x) * r / o, a) && (u = (p - s) / this.ratio + l), b("bottom", n) && (u = i.height + (e - i.y) * r / o, a) && (p = (u - l) * this.ratio + s), {
+                        newWidth: p = b("top", n) && (u = i.height - (e - i.y) * r / o, a) ? (u - l) * this.ratio + s : p,
                         newHeight: u
                     }
-                }, O.prototype.calculateNewSizeFromAspectRatio = function(t, e, o, i) {
-                    var n, r, s = this.props,
+                }, x.prototype.calculateNewSizeFromAspectRatio = function(t, e, o, r) {
+                    var i, n, s = this.props,
                         a = s.lockAspectRatio,
                         l = s.lockAspectRatioExtraHeight,
                         s = s.lockAspectRatioExtraWidth,
-                        p = void 0 === i.width ? 10 : i.width,
+                        p = void 0 === r.width ? 10 : r.width,
                         u = void 0 === o.width || o.width < 0 ? t : o.width,
-                        i = void 0 === i.height ? 10 : i.height,
+                        r = void 0 === r.height ? 10 : r.height,
                         o = void 0 === o.height || o.height < 0 ? e : o.height,
                         l = l || 0,
                         s = s || 0;
-                    return e = a ? (a = (i - l) * this.ratio + s, n = (o - l) * this.ratio + s, r = (p - s) / this.ratio + l, s = (u - s) / this.ratio + l, l = Math.max(p, a), a = Math.min(u, n), n = Math.max(i, r), r = Math.min(o, s), t = y(t, l, a), y(e, n, r)) : (t = y(t, p, u), y(e, i, o)), {
+                    return e = a ? (a = (r - l) * this.ratio + s, i = (o - l) * this.ratio + s, n = (p - s) / this.ratio + l, s = (u - s) / this.ratio + l, l = Math.max(p, a), a = Math.min(u, i), i = Math.max(r, n), n = Math.min(o, s), t = g(t, l, a), g(e, i, n)) : (t = g(t, p, u), g(e, r, o)), {
                         newWidth: t,
                         newHeight: e
                     }
-                }, O.prototype.setBoundingClientRect = function() {
-                    var t, e, o, i;
-                    "parent" === this.props.bounds && (i = this.parentNode) && (i = i.getBoundingClientRect(), this.parentLeft = i.left, this.parentTop = i.top), this.props.bounds && "string" != typeof this.props.bounds && (i = this.props.bounds.getBoundingClientRect(), this.targetLeft = i.left, this.targetTop = i.top), this.resizable && (t = (i = this.resizable.getBoundingClientRect()).left, e = i.top, o = i.right, i = i.bottom, this.resizableLeft = t, this.resizableRight = o, this.resizableTop = e, this.resizableBottom = i)
-                }, O.prototype.onResizeStart = function(t, e) {
-                    var o, i, n, r, s;
-                    this.resizable && this.window && (n = i = 0, t.nativeEvent && (s = t.nativeEvent, Boolean((s.clientX || 0 === s.clientX) && (s.clientY || 0 === s.clientY))) ? (i = t.nativeEvent.clientX, n = t.nativeEvent.clientY) : t.nativeEvent && d(t.nativeEvent) && (i = t.nativeEvent.touches[0].clientX, n = t.nativeEvent.touches[0].clientY), this.props.onResizeStart && this.resizable && !1 === this.props.onResizeStart(t, e, this.resizable) || (this.props.size && (void 0 !== this.props.size.height && this.props.size.height !== this.state.height && this.setState({
+                }, x.prototype.setBoundingClientRect = function() {
+                    var t, e, o, r;
+                    "parent" === this.props.bounds && (r = this.parentNode) && (r = r.getBoundingClientRect(), this.parentLeft = r.left, this.parentTop = r.top), this.props.bounds && "string" != typeof this.props.bounds && (r = this.props.bounds.getBoundingClientRect(), this.targetLeft = r.left, this.targetTop = r.top), this.resizable && (t = (r = this.resizable.getBoundingClientRect()).left, e = r.top, o = r.right, r = r.bottom, this.resizableLeft = t, this.resizableRight = o, this.resizableTop = e, this.resizableBottom = r)
+                }, x.prototype.onResizeStart = function(t, e) {
+                    var o, r, i, n, s;
+                    this.resizable && this.window && (i = r = 0, t.nativeEvent && (s = t.nativeEvent, Boolean((s.clientX || 0 === s.clientX) && (s.clientY || 0 === s.clientY))) ? (r = t.nativeEvent.clientX, i = t.nativeEvent.clientY) : t.nativeEvent && f(t.nativeEvent) && (r = t.nativeEvent.touches[0].clientX, i = t.nativeEvent.touches[0].clientY), this.props.onResizeStart && this.resizable && !1 === this.props.onResizeStart(t, e, this.resizable) || (this.props.size && (void 0 !== this.props.size.height && this.props.size.height !== this.state.height && this.setState({
                         height: this.props.size.height
                     }), void 0 !== this.props.size.width) && this.props.size.width !== this.state.width && this.setState({
                         width: this.props.size.width
-                    }), this.ratio = "number" == typeof this.props.lockAspectRatio ? this.props.lockAspectRatio : this.size.width / this.size.height, "auto" !== (s = this.window.getComputedStyle(this.resizable)).flexBasis && (r = this.parentNode) && (r = this.window.getComputedStyle(r).flexDirection, this.flexDir = r.startsWith("row") ? "row" : "column", o = s.flexBasis), this.setBoundingClientRect(), this.bindEvents(), r = {
+                    }), this.ratio = "number" == typeof this.props.lockAspectRatio ? this.props.lockAspectRatio : this.size.width / this.size.height, "auto" !== (s = this.window.getComputedStyle(this.resizable)).flexBasis && (n = this.parentNode) && (n = this.window.getComputedStyle(n).flexDirection, this.flexDir = n.startsWith("row") ? "row" : "column", o = s.flexBasis), this.setBoundingClientRect(), this.bindEvents(), n = {
                         original: {
-                            x: i,
-                            y: n,
+                            x: r,
+                            y: i,
                             width: this.size.width,
                             height: this.size.height
                         },
                         isResizing: !0,
-                        backgroundStyle: f(f({}, this.state.backgroundStyle), {
+                        backgroundStyle: d(d({}, this.state.backgroundStyle), {
                             cursor: this.window.getComputedStyle(t.target).cursor || "auto"
                         }),
                         direction: e,
                         flexBasis: o
-                    }, this.setState(r)))
-                }, O.prototype.onMouseMove = function(t) {
+                    }, this.setState(n)))
+                }, x.prototype.onMouseMove = function(t) {
                     if (this.state.isResizing && this.resizable && this.window) {
-                        if (this.window.TouchEvent && d(t)) try {
+                        if (this.window.TouchEvent && f(t)) try {
                             t.preventDefault(), t.stopPropagation()
                         } catch (t) {}
                         var e = this.props,
                             o = e.maxWidth,
-                            i = e.maxHeight,
-                            n = e.minWidth,
+                            r = e.maxHeight,
+                            i = e.minWidth,
                             e = e.minHeight,
-                            r = (d(t) ? t.touches[0] : t).clientX,
-                            s = (d(t) ? t.touches[0] : t).clientY,
+                            n = (f(t) ? t.touches[0] : t).clientX,
+                            s = (f(t) ? t.touches[0] : t).clientY,
                             a = this.state,
                             l = a.direction,
                             p = a.original,
                             u = a.width,
                             a = a.height,
-                            h = this.getParentSize(),
-                            c = x(h, this.window.innerWidth, this.window.innerHeight, o, i, n, e),
-                            o = c.maxWidth,
-                            i = c.maxHeight,
-                            n = c.minWidth,
-                            e = c.minHeight,
-                            c = this.calculateNewSizeFromDirection(r, s),
-                            r = c.newHeight,
-                            s = c.newWidth,
-                            c = this.calculateNewMaxFromBoundary(o, i),
-                            o = (this.props.snap && this.props.snap.x && (s = v(s, this.props.snap.x, this.props.snapGap)), this.props.snap && this.props.snap.y && (r = v(r, this.props.snap.y, this.props.snapGap)), this.calculateNewSizeFromAspectRatio(s, r, {
-                                width: c.maxWidth,
-                                height: c.maxHeight
+                            c = this.getParentSize(),
+                            h = _(c, this.window.innerWidth, this.window.innerHeight, o, r, i, e),
+                            o = h.maxWidth,
+                            r = h.maxHeight,
+                            i = h.minWidth,
+                            e = h.minHeight,
+                            h = this.calculateNewSizeFromDirection(n, s),
+                            n = h.newHeight,
+                            s = h.newWidth,
+                            h = this.calculateNewMaxFromBoundary(o, r),
+                            o = (this.props.snap && this.props.snap.x && (s = m(s, this.props.snap.x, this.props.snapGap)), this.props.snap && this.props.snap.y && (n = m(n, this.props.snap.y, this.props.snapGap)), this.calculateNewSizeFromAspectRatio(s, n, {
+                                width: h.maxWidth,
+                                height: h.maxHeight
                             }, {
-                                width: n,
+                                width: i,
                                 height: e
                             })),
-                            e = (s = o.newWidth, r = o.newHeight, this.props.grid && (i = b(s, this.props.grid[0]), c = b(r, this.props.grid[1]), s = 0 === (n = this.props.snapGap || 0) || Math.abs(i - s) <= n ? i : s, r = 0 === n || Math.abs(c - r) <= n ? c : r), {
+                            e = (s = o.newWidth, n = o.newHeight, this.props.grid && (r = y(s, this.props.grid[0]), h = y(n, this.props.grid[1]), s = 0 === (i = this.props.snapGap || 0) || Math.abs(r - s) <= i ? r : s, n = 0 === i || Math.abs(h - n) <= i ? h : n), {
                                 width: s - p.width,
-                                height: r - p.height
+                                height: n - p.height
                             }),
-                            o = (u && "string" == typeof u && (w(u, "%") ? s = s / h.width * 100 + "%" : w(u, "vw") ? s = s / this.window.innerWidth * 100 + "vw" : w(u, "vh") && (s = s / this.window.innerHeight * 100 + "vh")), a && "string" == typeof a && (w(a, "%") ? r = r / h.height * 100 + "%" : w(a, "vw") ? r = r / this.window.innerWidth * 100 + "vw" : w(a, "vh") && (r = r / this.window.innerHeight * 100 + "vh")), {
+                            o = (u && "string" == typeof u && (v(u, "%") ? s = s / c.width * 100 + "%" : v(u, "vw") ? s = s / this.window.innerWidth * 100 + "vw" : v(u, "vh") && (s = s / this.window.innerHeight * 100 + "vh")), a && "string" == typeof a && (v(a, "%") ? n = n / c.height * 100 + "%" : v(a, "vw") ? n = n / this.window.innerWidth * 100 + "vw" : v(a, "vh") && (n = n / this.window.innerHeight * 100 + "vh")), {
                                 width: this.createSizeForCssProperty(s, "width"),
-                                height: this.createSizeForCssProperty(r, "height")
+                                height: this.createSizeForCssProperty(n, "height")
                             });
                         "row" === this.flexDir ? o.flexBasis = o.width : "column" === this.flexDir && (o.flexBasis = o.height), this.setState(o), this.props.onResize && this.props.onResize(t, l, this.resizable, e)
                     }
-                }, O.prototype.onMouseUp = function(t) {
+                }, x.prototype.onMouseUp = function(t) {
                     var e = this.state,
                         o = e.isResizing,
-                        i = e.direction,
+                        r = e.direction,
                         e = e.original;
                     o && this.resizable && (o = {
                         width: this.size.width - e.width,
                         height: this.size.height - e.height
-                    }, this.props.onResizeStop && this.props.onResizeStop(t, i, this.resizable, o), this.props.size && this.setState(this.props.size), this.unbindEvents(), this.setState({
+                    }, this.props.onResizeStop && this.props.onResizeStop(t, r, this.resizable, o), this.props.size && this.setState(this.props.size), this.unbindEvents(), this.setState({
                         isResizing: !1,
-                        backgroundStyle: f(f({}, this.state.backgroundStyle), {
+                        backgroundStyle: d(d({}, this.state.backgroundStyle), {
                             cursor: "auto"
                         })
                     }))
-                }, O.prototype.updateSize = function(t) {
+                }, x.prototype.updateSize = function(t) {
                     this.setState({
                         width: t.width,
                         height: t.height
                     })
-                }, O.prototype.renderResizer = function() {
+                }, x.prototype.renderResizer = function() {
                     var e = this,
                         t = this.props,
                         o = t.enable,
-                        i = t.handleStyles,
-                        n = t.handleClasses,
-                        r = t.handleWrapperStyle,
+                        r = t.handleStyles,
+                        i = t.handleClasses,
+                        n = t.handleWrapperStyle,
                         s = t.handleWrapperClass,
                         a = t.handleComponent;
                     return o ? (t = Object.keys(o).map(function(t) {
-                        return !1 !== o[t] ? P.createElement(h, {
+                        return !1 !== o[t] ? C.createElement(c, {
                             key: t,
                             direction: t,
                             onResizeStart: e.onResizeStart,
-                            replaceStyles: i && i[t],
-                            className: n && n[t]
+                            replaceStyles: r && r[t],
+                            className: i && i[t]
                         }, a && a[t] ? a[t] : null) : null
-                    }), P.createElement("div", {
+                    }), C.createElement("div", {
                         className: s,
-                        style: r
+                        style: n
                     }, t)) : null
-                }, O.prototype.render = function() {
+                }, x.prototype.render = function() {
                     var o = this,
                         t = Object.keys(this.props).reduce(function(t, e) {
-                            return -1 === z.indexOf(e) && (t[e] = o.props[e]), t
+                            return -1 === L.indexOf(e) && (t[e] = o.props[e]), t
                         }, {}),
-                        e = f(f(f({
+                        e = d(d(d({
                             position: "relative",
                             userSelect: this.state.isResizing ? "none" : "auto"
                         }, this.props.style), this.sizeStyle), {
                             maxWidth: this.props.maxWidth,
                             maxHeight: this.props.maxHeight,
                             minWidth: this.props.minWidth,
                             minHeight: this.props.minHeight,
                             boxSizing: "border-box",
                             flexShrink: 0
                         }),
-                        i = (this.state.flexBasis && (e.flexBasis = this.state.flexBasis), this.props.as || "div");
-                    return P.createElement(i, f({
+                        r = (this.state.flexBasis && (e.flexBasis = this.state.flexBasis), this.props.as || "div");
+                    return C.createElement(r, d({
                         ref: this.ref,
                         style: e,
                         className: this.props.className
-                    }, t), this.state.isResizing && P.createElement("div", {
+                    }, t), this.state.isResizing && C.createElement("div", {
                         style: this.state.backgroundStyle
                     }), this.props.children, this.renderResizer())
-                }, O.defaultProps = {
+                }, x.defaultProps = {
                     as: "div",
                     onResizeStart: function() {},
                     onResize: function() {},
                     onResizeStop: function() {},
                     enable: {
                         top: !0,
                         right: !0,
@@ -445,28 +445,28 @@
                     grid: [1, 1],
                     lockAspectRatio: !1,
                     lockAspectRatioExtraWidth: 0,
                     lockAspectRatioExtraHeight: 0,
                     scale: 1,
                     resizeRatio: 1,
                     snapGap: 0
-                }, O),
-                D = function(t, e) {
-                    return (D = Object.setPrototypeOf || ({
+                }, x),
+                S = function(t, e) {
+                    return (S = Object.setPrototypeOf || ({
                             __proto__: []
                         }
                         instanceof Array ? function(t, e) {
                             t.__proto__ = e
                         } : function(t, e) {
                             for (var o in e) e.hasOwnProperty(o) && (t[o] = e[o])
                         }))(t, e)
                 };
 
-            function O(t) {
-                var o = i.call(this, t) || this;
+            function x(t) {
+                var o = r.call(this, t) || this;
                 return o.ratio = 1, o.resizable = null, o.parentLeft = 0, o.parentTop = 0, o.resizableLeft = 0, o.resizableRight = 0, o.resizableTop = 0, o.resizableBottom = 0, o.targetLeft = 0, o.targetTop = 0, o.appendBase = function() {
                     var t, e;
                     return o.resizable && o.window && (t = o.parentNode) ? ((e = o.window.document.createElement("div")).style.width = "100%", e.style.height = "100%", e.style.position = "absolute", e.style.transform = "scale(0, 0)", e.style.left = "0", e.style.flex = "0 0 100%", e.classList ? e.classList.add("__resizable_base__") : e.className += "__resizable_base__", t.appendChild(e), e) : null
                 }, o.removeBase = function(t) {
                     var e = o.parentNode;
                     e && e.removeChild(t)
                 }, o.ref = function(t) {
@@ -495,295 +495,295 @@
                         bottom: "0",
                         right: "0"
                     },
                     flexBasis: void 0
                 }, o.onResizeStart = o.onResizeStart.bind(o), o.onMouseMove = o.onMouseMove.bind(o), o.onMouseUp = o.onMouseUp.bind(o), o
             }
 
-            function E() {
+            function z() {
                 var e = null !== o && o.apply(this, arguments) || this;
                 return e.onMouseDown = function(t) {
                     e.props.onResizeStart(t, e.props.direction)
                 }, e.onTouchStart = function(t) {
                     e.props.onResizeStart(t, e.props.direction)
                 }, e
             }
-            var M, j, N = function() {
-                    return (N = Object.assign || function(t) {
-                        for (var e, o = 1, i = arguments.length; o < i; o++)
-                            for (var n in e = arguments[o]) Object.prototype.hasOwnProperty.call(e, n) && (t[n] = e[n]);
+            var O, D, P = function() {
+                    return (P = Object.assign || function(t) {
+                        for (var e, o = 1, r = arguments.length; o < r; o++)
+                            for (var i in e = arguments[o]) Object.prototype.hasOwnProperty.call(e, i) && (t[i] = e[i]);
                         return t
                     }).apply(this, arguments)
                 },
-                A = s.a,
-                _ = {
+                F = s.a,
+                X = {
                     width: "auto",
                     height: "auto",
                     display: "inline-block",
                     position: "absolute",
                     top: 0,
                     left: 0
                 },
-                L = (M = P.PureComponent, D(j = W, l = M), j.prototype = null === l ? Object.create(l) : (C.prototype = l.prototype, new C), W.prototype.componentDidMount = function() {
+                U = (O = C.PureComponent, S(D = R, l = O), D.prototype = null === l ? Object.create(l) : (j.prototype = l.prototype, new j), R.prototype.componentDidMount = function() {
                     this.updateOffsetFromParent();
                     var t = this.offsetFromParent,
                         e = t.left,
                         t = t.top,
                         o = this.getDraggablePosition(),
-                        i = o.x,
+                        r = o.x,
                         o = o.y;
                     this.draggable.setState({
-                        x: i - e,
+                        x: r - e,
                         y: o - t
                     }), this.forceUpdate()
-                }, W.prototype.getDraggablePosition = function() {
+                }, R.prototype.getDraggablePosition = function() {
                     var t = this.draggable.state;
                     return {
                         x: t.x,
                         y: t.y
                     }
-                }, W.prototype.getParent = function() {
+                }, R.prototype.getParent = function() {
                     return this.resizable && this.resizable.parentNode
-                }, W.prototype.getParentSize = function() {
+                }, R.prototype.getParentSize = function() {
                     return this.resizable.getParentSize()
-                }, W.prototype.getMaxSizesFromProps = function() {
+                }, R.prototype.getMaxSizesFromProps = function() {
                     return {
                         maxWidth: void 0 === this.props.maxWidth ? Number.MAX_SAFE_INTEGER : this.props.maxWidth,
                         maxHeight: void 0 === this.props.maxHeight ? Number.MAX_SAFE_INTEGER : this.props.maxHeight
                     }
-                }, W.prototype.getSelfElement = function() {
+                }, R.prototype.getSelfElement = function() {
                     return this.resizable && this.resizable.resizable
-                }, W.prototype.getOffsetHeight = function(t) {
+                }, R.prototype.getOffsetHeight = function(t) {
                     var e = this.props.scale;
                     switch (this.props.bounds) {
                         case "window":
                             return window.innerHeight / e;
                         case "body":
                             return document.body.offsetHeight / e;
                         default:
                             return t.offsetHeight
                     }
-                }, W.prototype.getOffsetWidth = function(t) {
+                }, R.prototype.getOffsetWidth = function(t) {
                     var e = this.props.scale;
                     switch (this.props.bounds) {
                         case "window":
                             return window.innerWidth / e;
                         case "body":
                             return document.body.offsetWidth / e;
                         default:
                             return t.offsetWidth
                     }
-                }, W.prototype.onDragStart = function(t, e) {
+                }, R.prototype.onDragStart = function(t, e) {
                     this.props.onDragStart && this.props.onDragStart(t, e);
                     t = this.getDraggablePosition();
                     if (this.originalPosition = t, this.props.bounds) {
-                        var o, i, n, r, s, e = this.getParent(),
+                        var o, r, i, n, s, e = this.getParent(),
                             t = this.props.scale;
                         if ("parent" === this.props.bounds) o = e;
                         else {
-                            if ("body" === this.props.bounds) return n = (r = e.getBoundingClientRect()).left, r = r.top, s = document.body.getBoundingClientRect(), n = -(n - e.offsetLeft * t - s.left) / t, r = -(r - e.offsetTop * t - s.top) / t, s = (document.body.offsetWidth - this.resizable.size.width * t) / t + n, i = (document.body.offsetHeight - this.resizable.size.height * t) / t + r, this.setState({
+                            if ("body" === this.props.bounds) return i = (n = e.getBoundingClientRect()).left, n = n.top, s = document.body.getBoundingClientRect(), i = -(i - e.offsetLeft * t - s.left) / t, n = -(n - e.offsetTop * t - s.top) / t, s = (document.body.offsetWidth - this.resizable.size.width * t) / t + i, r = (document.body.offsetHeight - this.resizable.size.height * t) / t + n, this.setState({
                                 bounds: {
-                                    top: r,
+                                    top: n,
                                     right: s,
-                                    bottom: i,
-                                    left: n
+                                    bottom: r,
+                                    left: i
                                 }
                             });
-                            if ("window" === this.props.bounds) return this.resizable ? (n = (r = e.getBoundingClientRect()).left, r = r.top, n = -(n - e.offsetLeft * t) / t, r = -(r - e.offsetTop * t) / t, s = (window.innerWidth - this.resizable.size.width * t) / t + n, i = (window.innerHeight - this.resizable.size.height * t) / t + r, this.setState({
+                            if ("window" === this.props.bounds) return this.resizable ? (i = (n = e.getBoundingClientRect()).left, n = n.top, i = -(i - e.offsetLeft * t) / t, n = -(n - e.offsetTop * t) / t, s = (window.innerWidth - this.resizable.size.width * t) / t + i, r = (window.innerHeight - this.resizable.size.height * t) / t + n, this.setState({
                                 bounds: {
-                                    top: r,
+                                    top: n,
                                     right: s,
-                                    bottom: i,
-                                    left: n
+                                    bottom: r,
+                                    left: i
                                 }
                             })) : void 0;
                             "string" == typeof this.props.bounds ? o = document.querySelector(this.props.bounds) : this.props.bounds instanceof HTMLElement && (o = this.props.bounds)
                         }
-                        o instanceof HTMLElement && e instanceof HTMLElement && (s = (r = o.getBoundingClientRect()).left, i = r.top, r = (s - (n = e.getBoundingClientRect()).left) / t, s = i - n.top, this.resizable) && (this.updateOffsetFromParent(), e = this.offsetFromParent, this.setState({
+                        o instanceof HTMLElement && e instanceof HTMLElement && (s = (n = o.getBoundingClientRect()).left, r = n.top, n = (s - (i = e.getBoundingClientRect()).left) / t, s = r - i.top, this.resizable) && (this.updateOffsetFromParent(), e = this.offsetFromParent, this.setState({
                             bounds: {
                                 top: s - e.top,
-                                right: r + (o.offsetWidth - this.resizable.size.width) - e.left / t,
+                                right: n + (o.offsetWidth - this.resizable.size.width) - e.left / t,
                                 bottom: s + (o.offsetHeight - this.resizable.size.height) - e.top,
-                                left: r - e.left / t
+                                left: n - e.left / t
                             }
                         }))
                     }
-                }, W.prototype.onDrag = function(t, e) {
-                    var o, i;
-                    if (this.props.onDrag) return o = (i = this.offsetFromParent).left, i = i.top, this.props.dragAxis && "both" !== this.props.dragAxis ? "x" === this.props.dragAxis ? this.props.onDrag(t, N(N({}, e), {
+                }, R.prototype.onDrag = function(t, e) {
+                    var o, r;
+                    if (this.props.onDrag) return o = (r = this.offsetFromParent).left, r = r.top, this.props.dragAxis && "both" !== this.props.dragAxis ? "x" === this.props.dragAxis ? this.props.onDrag(t, P(P({}, e), {
                         x: e.x + o,
-                        y: this.originalPosition.y + i,
+                        y: this.originalPosition.y + r,
                         deltaY: 0
-                    })) : "y" === this.props.dragAxis ? this.props.onDrag(t, N(N({}, e), {
+                    })) : "y" === this.props.dragAxis ? this.props.onDrag(t, P(P({}, e), {
                         x: this.originalPosition.x + o,
-                        y: e.y + i,
+                        y: e.y + r,
                         deltaX: 0
-                    })) : void 0 : this.props.onDrag(t, N(N({}, e), {
+                    })) : void 0 : this.props.onDrag(t, P(P({}, e), {
                         x: e.x - o,
-                        y: e.y - i
+                        y: e.y - r
                     }))
-                }, W.prototype.onDragStop = function(t, e) {
-                    var o, i;
-                    if (this.props.onDragStop) return o = (i = this.offsetFromParent).left, i = i.top, this.props.dragAxis && "both" !== this.props.dragAxis ? "x" === this.props.dragAxis ? this.props.onDragStop(t, N(N({}, e), {
+                }, R.prototype.onDragStop = function(t, e) {
+                    var o, r;
+                    if (this.props.onDragStop) return o = (r = this.offsetFromParent).left, r = r.top, this.props.dragAxis && "both" !== this.props.dragAxis ? "x" === this.props.dragAxis ? this.props.onDragStop(t, P(P({}, e), {
                         x: e.x + o,
-                        y: this.originalPosition.y + i,
+                        y: this.originalPosition.y + r,
                         deltaY: 0
-                    })) : "y" === this.props.dragAxis ? this.props.onDragStop(t, N(N({}, e), {
+                    })) : "y" === this.props.dragAxis ? this.props.onDragStop(t, P(P({}, e), {
                         x: this.originalPosition.x + o,
-                        y: e.y + i,
+                        y: e.y + r,
                         deltaX: 0
-                    })) : void 0 : this.props.onDragStop(t, N(N({}, e), {
+                    })) : void 0 : this.props.onDragStop(t, P(P({}, e), {
                         x: e.x + o,
-                        y: e.y + i
+                        y: e.y + r
                     }))
-                }, W.prototype.onResizeStart = function(t, e, o) {
+                }, R.prototype.onResizeStart = function(t, e, o) {
                     t.stopPropagation(), this.setState({
                         resizing: !0
                     });
-                    var i, n, r, s, a, l, p, u, h, c, d, f = this.props.scale,
+                    var r, i, n, s, a, l, p, u, c, h, f, d = this.props.scale,
                         g = this.offsetFromParent,
                         y = this.getDraggablePosition();
                     this.resizingPosition = {
                         x: y.x + g.left,
                         y: y.y + g.top
-                    }, this.originalPosition = y, this.props.bounds ? (g = this.getParent(), y = void 0, "parent" === this.props.bounds ? y = g : "body" === this.props.bounds ? y = document.body : "window" === this.props.bounds ? y = window : "string" == typeof this.props.bounds ? y = document.querySelector(this.props.bounds) : this.props.bounds instanceof HTMLElement && (y = this.props.bounds), (r = this.getSelfElement()) instanceof Element && (y instanceof HTMLElement || y === window) && g instanceof HTMLElement && (i = (g = this.getMaxSizesFromProps()).maxWidth, g = g.maxHeight, a = this.getParentSize(), i && "string" == typeof i && (i.endsWith("%") ? (n = Number(i.replace("%", "")) / 100, i = a.width * n) : i.endsWith("px") && (i = Number(i.replace("px", "")))), g && "string" == typeof g && (g.endsWith("%") ? (n = Number(g.replace("%", "")) / 100, g = a.width * n) : g.endsWith("px") && (g = Number(g.replace("px", "")))), n = (a = r.getBoundingClientRect()).left, r = a.top, s = (a = "window" === this.props.bounds ? {
+                    }, this.originalPosition = y, this.props.bounds ? (g = this.getParent(), y = void 0, "parent" === this.props.bounds ? y = g : "body" === this.props.bounds ? y = document.body : "window" === this.props.bounds ? y = window : "string" == typeof this.props.bounds ? y = document.querySelector(this.props.bounds) : this.props.bounds instanceof HTMLElement && (y = this.props.bounds), (n = this.getSelfElement()) instanceof Element && (y instanceof HTMLElement || y === window) && g instanceof HTMLElement && (r = (g = this.getMaxSizesFromProps()).maxWidth, g = g.maxHeight, a = this.getParentSize(), r && "string" == typeof r && (r.endsWith("%") ? (i = Number(r.replace("%", "")) / 100, r = a.width * i) : r.endsWith("px") && (r = Number(r.replace("px", "")))), g && "string" == typeof g && (g.endsWith("%") ? (i = Number(g.replace("%", "")) / 100, g = a.width * i) : g.endsWith("px") && (g = Number(g.replace("px", "")))), i = (a = n.getBoundingClientRect()).left, n = a.top, s = (a = "window" === this.props.bounds ? {
                         left: 0,
                         top: 0
-                    } : y.getBoundingClientRect()).left, a = a.top, l = this.getOffsetWidth(y), y = this.getOffsetHeight(y), p = e.toLowerCase().endsWith("left"), u = e.toLowerCase().endsWith("right"), h = e.startsWith("top"), c = e.startsWith("bottom"), (p || h) && this.resizable && (d = (n - s) / f + this.resizable.size.width, this.setState({
-                        maxWidth: d > Number(i) ? i : d
-                    })), (u || this.props.lockAspectRatio && !p && !h) && this.setState({
-                        maxWidth: (d = l + (s - n) / f) > Number(i) ? i : d
-                    }), (h || p) && this.resizable && (d = (r - a) / f + this.resizable.size.height, this.setState({
-                        maxHeight: d > Number(g) ? g : d
-                    })), c || this.props.lockAspectRatio && !h && !p) && this.setState({
-                        maxHeight: (d = y + (a - r) / f) > Number(g) ? g : d
+                    } : y.getBoundingClientRect()).left, a = a.top, l = this.getOffsetWidth(y), y = this.getOffsetHeight(y), p = e.toLowerCase().endsWith("left"), u = e.toLowerCase().endsWith("right"), c = e.startsWith("top"), h = e.startsWith("bottom"), (p || c) && this.resizable && (f = (i - s) / d + this.resizable.size.width, this.setState({
+                        maxWidth: f > Number(r) ? r : f
+                    })), (u || this.props.lockAspectRatio && !p && !c) && this.setState({
+                        maxWidth: (f = l + (s - i) / d) > Number(r) ? r : f
+                    }), (c || p) && this.resizable && (f = (n - a) / d + this.resizable.size.height, this.setState({
+                        maxHeight: f > Number(g) ? g : f
+                    })), h || this.props.lockAspectRatio && !c && !p) && this.setState({
+                        maxHeight: (f = y + (a - n) / d) > Number(g) ? g : f
                     })) : this.setState({
                         maxWidth: this.props.maxWidth,
                         maxHeight: this.props.maxHeight
                     }), this.props.onResizeStart && this.props.onResizeStart(t, e, o)
-                }, W.prototype.onResize = function(t, e, o, i) {
-                    var n = {
+                }, R.prototype.onResize = function(t, e, o, r) {
+                    var i = {
                             x: this.originalPosition.x,
                             y: this.originalPosition.y
                         },
-                        r = -i.width,
-                        s = -i.height,
-                        r = (-1 !== ["top", "left", "topLeft", "bottomLeft", "topRight"].indexOf(e) && ("bottomLeft" === e ? n.x += r : ("topRight" !== e && (n.x += r), n.y += s)), n.x === this.draggable.state.x && n.y === this.draggable.state.y || this.draggable.setState(n), this.updateOffsetFromParent(), this.offsetFromParent),
-                        s = this.getDraggablePosition().x + r.left,
-                        n = this.getDraggablePosition().y + r.top;
+                        n = -r.width,
+                        s = -r.height,
+                        n = (-1 !== ["top", "left", "topLeft", "bottomLeft", "topRight"].indexOf(e) && ("bottomLeft" === e ? i.x += n : ("topRight" !== e && (i.x += n), i.y += s)), i.x === this.draggable.state.x && i.y === this.draggable.state.y || this.draggable.setState(i), this.updateOffsetFromParent(), this.offsetFromParent),
+                        s = this.getDraggablePosition().x + n.left,
+                        i = this.getDraggablePosition().y + n.top;
                     this.resizingPosition = {
                         x: s,
-                        y: n
-                    }, this.props.onResize && this.props.onResize(t, e, o, i, {
+                        y: i
+                    }, this.props.onResize && this.props.onResize(t, e, o, r, {
                         x: s,
-                        y: n
+                        y: i
                     })
-                }, W.prototype.onResizeStop = function(t, e, o, i) {
+                }, R.prototype.onResizeStop = function(t, e, o, r) {
                     this.setState({
                         resizing: !1
                     });
-                    var n = this.getMaxSizesFromProps(),
-                        r = n.maxWidth,
-                        n = n.maxHeight;
+                    var i = this.getMaxSizesFromProps(),
+                        n = i.maxWidth,
+                        i = i.maxHeight;
                     this.setState({
-                        maxWidth: r,
-                        maxHeight: n
-                    }), this.props.onResizeStop && this.props.onResizeStop(t, e, o, i, this.resizingPosition)
-                }, W.prototype.updateSize = function(t) {
+                        maxWidth: n,
+                        maxHeight: i
+                    }), this.props.onResizeStop && this.props.onResizeStop(t, e, o, r, this.resizingPosition)
+                }, R.prototype.updateSize = function(t) {
                     this.resizable && this.resizable.updateSize({
                         width: t.width,
                         height: t.height
                     })
-                }, W.prototype.updatePosition = function(t) {
+                }, R.prototype.updatePosition = function(t) {
                     this.draggable.setState(t)
-                }, W.prototype.updateOffsetFromParent = function() {
+                }, R.prototype.updateOffsetFromParent = function() {
                     var t = this.props.scale,
                         e = this.getParent(),
                         o = this.getSelfElement();
                     if (!e || null === o) return {
                         top: 0,
                         left: 0
                     };
-                    var i = e.getBoundingClientRect(),
-                        n = i.left,
-                        i = i.top,
+                    var r = e.getBoundingClientRect(),
+                        i = r.left,
+                        r = r.top,
                         o = o.getBoundingClientRect(),
-                        r = this.getDraggablePosition(),
+                        n = this.getDraggablePosition(),
                         s = e.scrollLeft,
                         e = e.scrollTop;
                     this.offsetFromParent = {
-                        left: o.left - n + s - r.x * t,
-                        top: o.top - i + e - r.y * t
+                        left: o.left - i + s - n.x * t,
+                        top: o.top - r + e - n.y * t
                     }
-                }, W.prototype.render = function() {
+                }, R.prototype.render = function() {
                     var t = this.props,
                         e = t.disableDragging,
                         o = t.style,
-                        i = t.dragHandleClassName,
-                        n = t.position,
-                        r = t.onMouseDown,
+                        r = t.dragHandleClassName,
+                        i = t.position,
+                        n = t.onMouseDown,
                         s = t.onMouseUp,
                         a = t.dragAxis,
                         l = t.dragGrid,
                         p = t.bounds,
                         u = t.enableUserSelectHack,
-                        h = t.cancel,
-                        c = t.children,
-                        d = (t.onResizeStart, t.onResize, t.onResizeStop, t.onDragStart, t.onDrag, t.onDragStop, t.resizeHandleStyles),
-                        f = t.resizeHandleClasses,
+                        c = t.cancel,
+                        h = t.children,
+                        f = (t.onResizeStart, t.onResize, t.onResizeStop, t.onDragStart, t.onDrag, t.onDragStop, t.resizeHandleStyles),
+                        d = t.resizeHandleClasses,
                         g = t.resizeHandleComponent,
                         y = t.enableResizing,
                         b = t.resizeGrid,
                         m = t.resizeHandleWrapperClass,
                         v = t.resizeHandleWrapperStyle,
                         w = t.scale,
                         S = t.allowAnyClick,
                         t = function(t, e) {
                             var o = {};
-                            for (n in t) Object.prototype.hasOwnProperty.call(t, n) && e.indexOf(n) < 0 && (o[n] = t[n]);
+                            for (i in t) Object.prototype.hasOwnProperty.call(t, i) && e.indexOf(i) < 0 && (o[i] = t[i]);
                             if (null != t && "function" == typeof Object.getOwnPropertySymbols)
-                                for (var i = 0, n = Object.getOwnPropertySymbols(t); i < n.length; i++) e.indexOf(n[i]) < 0 && Object.prototype.propertyIsEnumerable.call(t, n[i]) && (o[n[i]] = t[n[i]]);
+                                for (var r = 0, i = Object.getOwnPropertySymbols(t); r < i.length; r++) e.indexOf(i[r]) < 0 && Object.prototype.propertyIsEnumerable.call(t, i[r]) && (o[i[r]] = t[i[r]]);
                             return o
                         }(t, ["disableDragging", "style", "dragHandleClassName", "position", "onMouseDown", "onMouseUp", "dragAxis", "dragGrid", "bounds", "enableUserSelectHack", "cancel", "children", "onResizeStart", "onResize", "onResizeStop", "onDragStart", "onDrag", "onDragStop", "resizeHandleStyles", "resizeHandleClasses", "resizeHandleComponent", "enableResizing", "resizeGrid", "resizeHandleWrapperClass", "resizeHandleWrapperStyle", "scale", "allowAnyClick"]),
-                        x = this.props.default ? N({}, this.props.default) : void 0;
+                        x = this.props.default ? P({}, this.props.default) : void 0;
                     delete t.default;
-                    var z, D = e || i ? {
+                    var z, O = e || r ? {
                             cursor: "auto"
                         } : {
                             cursor: "move"
                         },
-                        D = N(N(N({}, _), D), o),
+                        O = P(P(P({}, X), O), o),
                         o = this.offsetFromParent,
-                        O = o.left,
+                        D = o.left,
                         o = o.top;
-                    n && (z = {
-                        x: n.x - O,
-                        y: n.y - o
+                    i && (z = {
+                        x: i.x - D,
+                        y: i.y - o
                     });
-                    O = this.state.resizing ? void 0 : z, n = this.state.resizing ? "both" : a;
-                    return Object(P.createElement)(A, {
+                    D = this.state.resizing ? void 0 : z, i = this.state.resizing ? "both" : a;
+                    return Object(C.createElement)(F, {
                         ref: this.refDraggable,
-                        handle: i ? ".".concat(i) : void 0,
+                        handle: r ? ".".concat(r) : void 0,
                         defaultPosition: x,
-                        onMouseDown: r,
+                        onMouseDown: n,
                         onMouseUp: s,
                         onStart: this.onDragStart,
                         onDrag: this.onDrag,
                         onStop: this.onDragStop,
-                        axis: n,
+                        axis: i,
                         disabled: e,
                         grid: l,
                         bounds: p ? this.state.bounds : void 0,
-                        position: O,
+                        position: D,
                         enableUserSelectHack: u,
-                        cancel: h,
+                        cancel: c,
                         scale: w,
                         allowAnyClick: S,
                         nodeRef: this.resizableElement
-                    }, Object(P.createElement)(R, N({}, t, {
+                    }, Object(C.createElement)(B, P({}, t, {
                         ref: this.refResizable,
                         defaultSize: x,
                         size: this.props.size,
                         enable: "boolean" == typeof y ? {
                             bottom: y,
                             bottomLeft: y,
                             bottomRight: y,
@@ -792,46 +792,46 @@
                             top: y,
                             topLeft: y,
                             topRight: y
                         } : y,
                         onResizeStart: this.onResizeStart,
                         onResize: this.onResize,
                         onResizeStop: this.onResizeStop,
-                        style: D,
+                        style: O,
                         minWidth: this.props.minWidth,
                         minHeight: this.props.minHeight,
                         maxWidth: (this.state.resizing ? this.state : this.props).maxWidth,
                         maxHeight: (this.state.resizing ? this.state : this.props).maxHeight,
                         grid: b,
                         handleWrapperClass: m,
                         handleWrapperStyle: v,
                         lockAspectRatio: this.props.lockAspectRatio,
                         lockAspectRatioExtraWidth: this.props.lockAspectRatioExtraWidth,
                         lockAspectRatioExtraHeight: this.props.lockAspectRatioExtraHeight,
-                        handleStyles: d,
-                        handleClasses: f,
+                        handleStyles: f,
+                        handleClasses: d,
                         handleComponent: g,
                         scale: this.props.scale
-                    }), c))
-                }, W.defaultProps = {
+                    }), h))
+                }, R.defaultProps = {
                     maxWidth: Number.MAX_SAFE_INTEGER,
                     maxHeight: Number.MAX_SAFE_INTEGER,
                     scale: 1,
                     onResizeStart: function() {},
                     onResize: function() {},
                     onResizeStop: function() {},
                     onDragStart: function() {},
                     onDrag: function() {},
                     onDragStop: function() {}
-                }, W),
-                c = e(225),
-                B = e(22);
+                }, R),
+                h = e(225),
+                Y = e(22);
 
-            function W(t) {
-                var e = M.call(this, t) || this;
+            function R(t) {
+                var e = O.call(this, t) || this;
                 return e.resizingPosition = {
                     x: 0,
                     y: 0
                 }, e.offsetFromParent = {
                     left: 0,
                     top: 0
                 }, e.resizableElement = {
@@ -852,170 +852,250 @@
                         left: 0
                     },
                     maxWidth: t.maxWidth,
                     maxHeight: t.maxHeight
                 }, e.onResizeStart = e.onResizeStart.bind(e), e.onResize = e.onResize.bind(e), e.onResizeStop = e.onResizeStop.bind(e), e.onDragStart = e.onDragStart.bind(e), e.onDrag = e.onDrag.bind(e), e.onDragStop = e.onDragStop.bind(e), e.getMaxSizesFromProps = e.getMaxSizesFromProps.bind(e), e
             }
 
-            function C() {
-                this.constructor = j
+            function j() {
+                this.constructor = D
             }
 
-            function H(t, e) {
-                (null == e || e > t.length) && (e = t.length);
-                for (var o = 0, i = new Array(e); o < e; o++) i[o] = t[o];
+            function E(t) {
+                return (E = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+                    return typeof t
+                } : function(t) {
+                    return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
+                })(t)
+            }
+
+            function M(e, t) {
+                var o, r = Object.keys(e);
+                return Object.getOwnPropertySymbols && (o = Object.getOwnPropertySymbols(e), t && (o = o.filter(function(t) {
+                    return Object.getOwnPropertyDescriptor(e, t).enumerable
+                })), r.push.apply(r, o)), r
+            }
+
+            function H(i) {
+                for (var t = 1; t < arguments.length; t++) {
+                    var n = null != arguments[t] ? arguments[t] : {};
+                    t % 2 ? M(Object(n), !0).forEach(function(t) {
+                        var e, o, r;
+                        e = i, o = n[t = t], r = function(t) {
+                            if ("object" != E(t) || !t) return t;
+                            var e = t[Symbol.toPrimitive];
+                            if (void 0 === e) return String(t);
+                            e = e.call(t, "string");
+                            if ("object" != E(e)) return e;
+                            throw new TypeError("@@toPrimitive must return a primitive value.")
+                        }(t), (t = "symbol" == E(r) ? r : String(r)) in e ? Object.defineProperty(e, t, {
+                            value: o,
+                            enumerable: !0,
+                            configurable: !0,
+                            writable: !0
+                        }) : e[t] = o
+                    }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(i, Object.getOwnPropertyDescriptors(n)) : M(Object(n)).forEach(function(t) {
+                        Object.defineProperty(i, t, Object.getOwnPropertyDescriptor(n, t))
+                    })
+                }
                 return i
             }
 
-            function T(t) {
-                var e = t.id,
-                    o = t.style,
+            function T(t, e) {
+                var o;
+                if (t) return "string" == typeof t ? N(t, e) : "Map" === (o = "Object" === (o = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : o) || "Set" === o ? Array.from(t) : "Arguments" === o || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(o) ? N(t, e) : void 0
+            }
+
+            function N(t, e) {
+                (null == e || e > t.length) && (e = t.length);
+                for (var o = 0, r = new Array(e); o < e; o++) r[o] = t[o];
+                return r
+            }
+
+            function W(t) {
+                var e, o = t.id,
+                    r = t.style,
                     i = t.className,
                     n = t.children,
-                    r = t.defaultState,
-                    s = t.size,
-                    a = t.position,
-                    l = t.minWidth,
-                    p = t.minHeight,
-                    u = t.maxWidth,
+                    s = t.defaultState,
+                    a = t.size,
+                    l = t.position,
+                    p = t.minWidth,
+                    u = t.minHeight,
+                    c = t.maxWidth,
                     h = t.maxHeight,
-                    c = t.resizeGrid,
+                    f = t.resizeGrid,
                     d = t.dragGrid,
-                    f = t.lockAspectRatio,
-                    g = t.lockAspectRatioExtraWidth,
-                    y = t.lockAspectRatioExtraHeight,
-                    b = t.direction,
-                    m = t.disableDragging,
-                    v = t.dragAxis,
-                    w = t.bounds,
-                    S = t.setProps,
-                    x = t.loading_state;
-                Object(P.useEffect)(function() {
-                    !s && r.width && r.height && S({
+                    g = t.lockAspectRatio,
+                    y = t.lockAspectRatioExtraWidth,
+                    b = t.lockAspectRatioExtraHeight,
+                    m = t.direction,
+                    v = t.disableDragging,
+                    w = t.dragAxis,
+                    S = t.bounds,
+                    x = t.selected,
+                    z = t.selectedStyle,
+                    O = t.selectedClassName,
+                    D = t.setProps,
+                    P = t.loading_state,
+                    R = (R = Object(C.useState)(0), e = 2, function(t) {
+                        if (Array.isArray(t)) return t
+                    }(R) || function(t, e) {
+                        var o = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
+                        if (null != o) {
+                            var r, i, n, s, a = [],
+                                l = !0,
+                                p = !1;
+                            try {
+                                if (n = (o = o.call(t)).next, 0 === e) {
+                                    if (Object(o) !== o) return;
+                                    l = !1
+                                } else
+                                    for (; !(l = (r = n.call(o)).done) && (a.push(r.value), a.length !== e); l = !0);
+                            } catch (t) {
+                                p = !0, i = t
+                            } finally {
+                                try {
+                                    if (!l && null != o.return && (s = o.return(), Object(s) !== s)) return
+                                } finally {
+                                    if (p) throw i
+                                }
+                            }
+                            return a
+                        }
+                    }(R, e) || T(R, e) || function() {
+                        throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
+                    }()),
+                    j = R[0],
+                    E = R[1];
+                Object(C.useEffect)(function() {
+                    !a && s.width && s.height && D({
                         size: {
-                            width: r.width,
-                            height: r.height
+                            width: s.width,
+                            height: s.height
                         }
-                    }), a || !r.x && 0 !== r.x || !r.y && 0 !== r.y || S({
+                    }), l || !s.x && 0 !== s.x || !s.y && 0 !== s.y || D({
                         position: {
-                            x: r.x,
-                            y: r.y
+                            x: s.x,
+                            y: s.y
                         }
                     })
                 }, []);
-                var z, D = Object(B.clone)({
+                var M, N = Object(Y.clone)({
                         top: !1,
                         right: !1,
                         bottom: !1,
                         left: !1,
                         topRight: !1,
                         bottomRight: !1,
                         bottomLeft: !1,
                         topLeft: !1
                     }),
-                    O = function(t, e) {
-                        var o, i, n, r, s = "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
-                        if (s) return n = !(i = !0), {
+                    W = function(t) {
+                        var e, o, r, i, n, s = "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
+                        if (s) return r = !(o = !0), {
                             s: function() {
                                 s = s.call(t)
                             },
                             n: function() {
                                 var t = s.next();
-                                return i = t.done, t
+                                return o = t.done, t
                             },
                             e: function(t) {
-                                n = !0, o = t
+                                r = !0, e = t
                             },
                             f: function() {
                                 try {
-                                    i || null == s.return || s.return()
+                                    o || null == s.return || s.return()
                                 } finally {
-                                    if (n) throw o
+                                    if (r) throw e
                                 }
                             }
                         };
-                        if (Array.isArray(t) || (s = function(t) {
-                                var e;
-                                if (t) return "string" == typeof t ? H(t, void 0) : "Map" === (e = "Object" === (e = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : e) || "Set" === e ? Array.from(t) : "Arguments" === e || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(e) ? H(t, void 0) : void 0
-                            }(t)) || e && t && "number" == typeof t.length) return s && (t = s), r = 0, {
-                            s: e = function() {},
+                        if (Array.isArray(t) || (s = T(t))) return s && (t = s), i = 0, {
+                            s: n = function() {},
                             n: function() {
-                                return r >= t.length ? {
+                                return i >= t.length ? {
                                     done: !0
                                 } : {
                                     done: !1,
-                                    value: t[r++]
+                                    value: t[i++]
                                 }
                             },
                             e: function(t) {
                                 throw t
                             },
-                            f: e
+                            f: n
                         };
                         throw new TypeError("Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
-                    }(b);
+                    }(m);
                 try {
-                    for (O.s(); !(z = O.n()).done;) D[z.value] = !0
+                    for (W.s(); !(M = W.n()).done;) N[M.value] = !0
                 } catch (t) {
-                    O.e(t)
+                    W.e(t)
                 } finally {
-                    O.f()
+                    W.f()
                 }
-                return React.createElement(L, {
-                    id: e,
-                    style: o,
-                    className: i,
-                    default: r,
-                    size: s,
-                    position: a,
-                    minWidth: l,
-                    minHeight: p,
-                    maxWidth: u,
+                return React.createElement(U, {
+                    id: o,
+                    style: H(H({}, r), x ? z : {}),
+                    className: x && O ? i + " " + O : i,
+                    default: s,
+                    size: a,
+                    position: l,
+                    minWidth: p,
+                    minHeight: u,
+                    maxWidth: c,
                     maxHeight: h,
-                    resizeGrid: c,
+                    resizeGrid: f,
                     dragGrid: d,
-                    lockAspectRatio: f,
-                    lockAspectRatioExtraWidth: g,
-                    lockAspectRatioExtraHeight: y,
-                    enableResizing: D,
-                    disableDragging: m,
-                    dragAxis: v,
-                    bounds: w,
+                    lockAspectRatio: g,
+                    lockAspectRatioExtraWidth: y,
+                    lockAspectRatioExtraHeight: b,
+                    enableResizing: N,
+                    disableDragging: v,
+                    dragAxis: w,
+                    bounds: S,
                     onDragStop: function(t, e) {
-                        return S({
+                        !l || l.x === e.x && l.y === e.y || E((new Date).getTime()), D({
                             position: {
                                 x: e.x,
                                 y: e.y
                             }
                         })
                     },
-                    onResizeStop: function(t, e, o, i, n) {
-                        S({
+                    onResizeStop: function(t, e, o, r, i) {
+                        E((new Date).getTime()), D({
                             size: {
                                 width: o.style.width,
                                 height: o.style.height
                             },
                             position: {
-                                x: n.x,
-                                y: n.y
+                                x: i.x,
+                                y: i.y
                             }
                         })
                     },
-                    "data-dash-is-loading": x && x.is_loading || void 0
+                    onClick: function() {
+                        200 <= (new Date).getTime() - j && D({
+                            selected: !x
+                        })
+                    },
+                    "data-dash-is-loading": P && P.is_loading || void 0
                 }, n)
-            }(t.default = T).defaultProps = c.b, T.propTypes = c.c
+            }(t.default = W).defaultProps = h.b, W.propTypes = h.c
         },
         570: function(t, e, o) {
             "use strict";
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), e.dontSetMe = function(t, e, o) {
                 if (t[e]) return new Error("Invalid prop ".concat(e, " passed to ").concat(o, " - do not set this, set it on the child."))
             }, e.findInArray = function(t, e) {
-                for (var o = 0, i = t.length; o < i; o++)
+                for (var o = 0, r = t.length; o < r; o++)
                     if (e.apply(e, [t[o], o, t])) return t[o]
             }, e.int = function(t) {
                 return parseInt(t, 10)
             }, e.isFunction = function(t) {
                 return "function" == typeof t || "[object Function]" === Object.prototype.toString.call(t)
             }, e.isNum = function(t) {
                 return "number" == typeof t && !isNaN(t)
@@ -1029,110 +1109,110 @@
                     return typeof t
                 } : function(t) {
                     return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
                 })(t)
             }
             Object.defineProperty(e, "__esModule", {
                 value: !0
-            }), e.addClassName = d, e.addEvent = function(t, e, o, i) {
-                t && (i = l({
+            }), e.addClassName = f, e.addEvent = function(t, e, o, r) {
+                t && (r = l({
                     capture: !0
-                }, i), t.addEventListener ? t.addEventListener(e, o, i) : t.attachEvent ? t.attachEvent("on" + e, o) : t["on" + e] = o)
+                }, r), t.addEventListener ? t.addEventListener(e, o, r) : t.attachEvent ? t.attachEvent("on" + e, o) : t["on" + e] = o)
             }, e.addUserSelectStyles = function(t) {
                 var e;
-                t && ((e = t.getElementById("react-draggable-style-el")) || ((e = t.createElement("style")).type = "text/css", e.id = "react-draggable-style-el", e.innerHTML = ".react-draggable-transparent-selection *::-moz-selection {all: inherit;}\n", e.innerHTML += ".react-draggable-transparent-selection *::selection {all: inherit;}\n", t.getElementsByTagName("head")[0].appendChild(e)), t.body) && d(t.body, "react-draggable-transparent-selection")
+                t && ((e = t.getElementById("react-draggable-style-el")) || ((e = t.createElement("style")).type = "text/css", e.id = "react-draggable-style-el", e.innerHTML = ".react-draggable-transparent-selection *::-moz-selection {all: inherit;}\n", e.innerHTML += ".react-draggable-transparent-selection *::selection {all: inherit;}\n", t.getElementsByTagName("head")[0].appendChild(e)), t.body) && f(t.body, "react-draggable-transparent-selection")
             }, e.createCSSTransform = function(t, e) {
-                t = c(t, e, "px");
-                return p({}, (0, n.browserPrefixToKey)("transform", n.default), t)
+                t = h(t, e, "px");
+                return p({}, (0, i.browserPrefixToKey)("transform", i.default), t)
             }, e.createSVGTransform = function(t, e) {
-                return c(t, e, "")
+                return h(t, e, "")
             }, e.getTouch = function(t, e) {
-                return t.targetTouches && (0, i.findInArray)(t.targetTouches, function(t) {
+                return t.targetTouches && (0, r.findInArray)(t.targetTouches, function(t) {
                     return e === t.identifier
-                }) || t.changedTouches && (0, i.findInArray)(t.changedTouches, function(t) {
+                }) || t.changedTouches && (0, r.findInArray)(t.changedTouches, function(t) {
                     return e === t.identifier
                 })
             }, e.getTouchIdentifier = function(t) {
                 return t.targetTouches && t.targetTouches[0] ? t.targetTouches[0].identifier : t.changedTouches && t.changedTouches[0] ? t.changedTouches[0].identifier : void 0
-            }, e.getTranslation = c, e.innerHeight = function(t) {
+            }, e.getTranslation = h, e.innerHeight = function(t) {
                 var e = t.clientHeight,
                     t = t.ownerDocument.defaultView.getComputedStyle(t);
-                return (e -= (0, i.int)(t.paddingTop)) - (0, i.int)(t.paddingBottom)
+                return (e -= (0, r.int)(t.paddingTop)) - (0, r.int)(t.paddingBottom)
             }, e.innerWidth = function(t) {
                 var e = t.clientWidth,
                     t = t.ownerDocument.defaultView.getComputedStyle(t);
-                return (e -= (0, i.int)(t.paddingLeft)) - (0, i.int)(t.paddingRight)
-            }, e.matchesSelector = h, e.matchesSelectorAndParentsTo = function(t, e, o) {
-                var i = t;
+                return (e -= (0, r.int)(t.paddingLeft)) - (0, r.int)(t.paddingRight)
+            }, e.matchesSelector = c, e.matchesSelectorAndParentsTo = function(t, e, o) {
+                var r = t;
                 do {
-                    if (h(i, e)) return !0;
-                    if (i === o) return !1
-                } while (i = i.parentNode);
+                    if (c(r, e)) return !0;
+                    if (r === o) return !1
+                } while (r = r.parentNode);
                 return !1
             }, e.offsetXYFromParent = function(t, e, o) {
-                var i = e === e.ownerDocument.body ? {
+                var r = e === e.ownerDocument.body ? {
                     left: 0,
                     top: 0
                 } : e.getBoundingClientRect();
                 return {
-                    x: (t.clientX + e.scrollLeft - i.left) / o,
-                    y: (t.clientY + e.scrollTop - i.top) / o
+                    x: (t.clientX + e.scrollLeft - r.left) / o,
+                    y: (t.clientY + e.scrollTop - r.top) / o
                 }
             }, e.outerHeight = function(t) {
                 var e = t.clientHeight,
                     t = t.ownerDocument.defaultView.getComputedStyle(t);
-                return (e += (0, i.int)(t.borderTopWidth)) + (0, i.int)(t.borderBottomWidth)
+                return (e += (0, r.int)(t.borderTopWidth)) + (0, r.int)(t.borderBottomWidth)
             }, e.outerWidth = function(t) {
                 var e = t.clientWidth,
                     t = t.ownerDocument.defaultView.getComputedStyle(t);
-                return (e += (0, i.int)(t.borderLeftWidth)) + (0, i.int)(t.borderRightWidth)
-            }, e.removeClassName = f, e.removeEvent = function(t, e, o, i) {
-                t && (i = l({
+                return (e += (0, r.int)(t.borderLeftWidth)) + (0, r.int)(t.borderRightWidth)
+            }, e.removeClassName = d, e.removeEvent = function(t, e, o, r) {
+                t && (r = l({
                     capture: !0
-                }, i), t.removeEventListener ? t.removeEventListener(e, o, i) : t.detachEvent ? t.detachEvent("on" + e, o) : t["on" + e] = null)
+                }, r), t.removeEventListener ? t.removeEventListener(e, o, r) : t.detachEvent ? t.detachEvent("on" + e, o) : t["on" + e] = null)
             }, e.removeUserSelectStyles = function(t) {
                 if (t) try {
                     var e;
-                    t.body && f(t.body, "react-draggable-transparent-selection"), t.selection ? t.selection.empty() : (e = (t.defaultView || window).getSelection()) && "Caret" !== e.type && e.removeAllRanges()
+                    t.body && d(t.body, "react-draggable-transparent-selection"), t.selection ? t.selection.empty() : (e = (t.defaultView || window).getSelection()) && "Caret" !== e.type && e.removeAllRanges()
                 } catch (t) {}
             };
-            var i = o(570),
-                n = function(t) {
+            var r = o(570),
+                i = function(t) {
                     if (t && t.__esModule) return t;
                     if (null === t || "object" !== s(t) && "function" != typeof t) return {
                         default: t
                     };
                     var e = a(void 0);
                     if (e && e.has(t)) return e.get(t);
-                    var o, i, n = {},
-                        r = Object.defineProperty && Object.getOwnPropertyDescriptor;
-                    for (o in t) "default" !== o && Object.prototype.hasOwnProperty.call(t, o) && ((i = r ? Object.getOwnPropertyDescriptor(t, o) : null) && (i.get || i.set) ? Object.defineProperty(n, o, i) : n[o] = t[o]);
-                    return n.default = t, e && e.set(t, n), n
+                    var o, r, i = {},
+                        n = Object.defineProperty && Object.getOwnPropertyDescriptor;
+                    for (o in t) "default" !== o && Object.prototype.hasOwnProperty.call(t, o) && ((r = n ? Object.getOwnPropertyDescriptor(t, o) : null) && (r.get || r.set) ? Object.defineProperty(i, o, r) : i[o] = t[o]);
+                    return i.default = t, e && e.set(t, i), i
                 }(o(867));
 
             function a(t) {
                 var e, o;
                 return "function" != typeof WeakMap ? null : (e = new WeakMap, o = new WeakMap, (a = function(t) {
                     return t ? o : e
                 })(t))
             }
 
-            function r(e, t) {
-                var o, i = Object.keys(e);
+            function n(e, t) {
+                var o, r = Object.keys(e);
                 return Object.getOwnPropertySymbols && (o = Object.getOwnPropertySymbols(e), t && (o = o.filter(function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
-                })), i.push.apply(i, o)), i
+                })), r.push.apply(r, o)), r
             }
 
             function l(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var o = null != arguments[t] ? arguments[t] : {};
-                    t % 2 ? r(Object(o), !0).forEach(function(t) {
+                    t % 2 ? n(Object(o), !0).forEach(function(t) {
                         p(e, t, o[t])
-                    }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(o)) : r(Object(o)).forEach(function(t) {
+                    }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(o)) : n(Object(o)).forEach(function(t) {
                         Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(o, t))
                     })
                 }
                 return e
             }
 
             function p(t, e, o) {
@@ -1141,61 +1221,61 @@
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : t[e] = o, t
             }
             var u = "";
 
-            function h(e, t) {
-                return u = u || (0, i.findInArray)(["matches", "webkitMatchesSelector", "mozMatchesSelector", "msMatchesSelector", "oMatchesSelector"], function(t) {
-                    return (0, i.isFunction)(e[t])
-                }), !!(0, i.isFunction)(e[u]) && e[u](t)
+            function c(e, t) {
+                return u = u || (0, r.findInArray)(["matches", "webkitMatchesSelector", "mozMatchesSelector", "msMatchesSelector", "oMatchesSelector"], function(t) {
+                    return (0, r.isFunction)(e[t])
+                }), !!(0, r.isFunction)(e[u]) && e[u](t)
             }
 
-            function c(t, e, o) {
-                var i = t.x,
+            function h(t, e, o) {
+                var r = t.x,
                     t = t.y,
-                    i = "translate(".concat(i).concat(o, ",").concat(t).concat(o, ")");
-                return e && (t = "".concat("string" == typeof e.x ? e.x : e.x + o), e = "".concat("string" == typeof e.y ? e.y : e.y + o), i = "translate(".concat(t, ", ").concat(e, ")") + i), i
+                    r = "translate(".concat(r).concat(o, ",").concat(t).concat(o, ")");
+                return e && (t = "".concat("string" == typeof e.x ? e.x : e.x + o), e = "".concat("string" == typeof e.y ? e.y : e.y + o), r = "translate(".concat(t, ", ").concat(e, ")") + r), r
             }
 
-            function d(t, e) {
+            function f(t, e) {
                 t.classList ? t.classList.add(e) : t.className.match(new RegExp("(?:^|\\s)".concat(e, "(?!\\S)"))) || (t.className += " ".concat(e))
             }
 
-            function f(t, e) {
+            function d(t, e) {
                 t.classList ? t.classList.remove(e) : t.className = t.className.replace(new RegExp("(?:^|\\s)".concat(e, "(?!\\S)"), "g"), "")
             }
         },
         644: function(t, e, o) {
             "use strict";
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), e.canDragX = function(t) {
                 return "both" === t.props.axis || "x" === t.props.axis
             }, e.canDragY = function(t) {
                 return "both" === t.props.axis || "y" === t.props.axis
             }, e.createCoreData = function(t, e, o) {
-                var i = t.state,
-                    n = !(0, a.isNum)(i.lastX),
+                var r = t.state,
+                    i = !(0, a.isNum)(r.lastX),
                     t = p(t);
-                return n ? {
+                return i ? {
                     node: t,
                     deltaX: 0,
                     deltaY: 0,
                     lastX: e,
                     lastY: o,
                     x: e,
                     y: o
                 } : {
                     node: t,
-                    deltaX: e - i.lastX,
-                    deltaY: o - i.lastY,
-                    lastX: i.lastX,
-                    lastY: i.lastY,
+                    deltaX: e - r.lastX,
+                    deltaY: o - r.lastY,
+                    lastX: r.lastX,
+                    lastY: r.lastY,
                     x: e,
                     y: o
                 }
             }, e.createDraggableData = function(t, e) {
                 var o = t.props.scale;
                 return {
                     node: e.node,
@@ -1205,38 +1285,38 @@
                     deltaY: e.deltaY / o,
                     lastX: t.state.x,
                     lastY: t.state.y
                 }
             }, e.getBoundPosition = function(t, e, o) {
                 if (t.props.bounds) {
                     s = "string" == typeof(s = t.props.bounds) ? s : {
-                        left: (i = s).left,
-                        top: i.top,
-                        right: i.right,
-                        bottom: i.bottom
+                        left: (r = s).left,
+                        top: r.top,
+                        right: r.right,
+                        bottom: r.bottom
                     };
-                    var i = p(t);
+                    var r = p(t);
                     if ("string" == typeof s) {
-                        var t = i.ownerDocument,
-                            n = t.defaultView;
-                        if (!((t = "parent" === s ? i.parentNode : t.querySelector(s)) instanceof n.HTMLElement)) throw new Error('Bounds selector "' + s + '" could not find an element.');
-                        var r = n.getComputedStyle(i),
-                            n = n.getComputedStyle(t),
+                        var t = r.ownerDocument,
+                            i = t.defaultView;
+                        if (!((t = "parent" === s ? r.parentNode : t.querySelector(s)) instanceof i.HTMLElement)) throw new Error('Bounds selector "' + s + '" could not find an element.');
+                        var n = i.getComputedStyle(r),
+                            i = i.getComputedStyle(t),
                             s = {
-                                left: -i.offsetLeft + (0, a.int)(n.paddingLeft) + (0, a.int)(r.marginLeft),
-                                top: -i.offsetTop + (0, a.int)(n.paddingTop) + (0, a.int)(r.marginTop),
-                                right: (0, l.innerWidth)(t) - (0, l.outerWidth)(i) - i.offsetLeft + (0, a.int)(n.paddingRight) - (0, a.int)(r.marginRight),
-                                bottom: (0, l.innerHeight)(t) - (0, l.outerHeight)(i) - i.offsetTop + (0, a.int)(n.paddingBottom) - (0, a.int)(r.marginBottom)
+                                left: -r.offsetLeft + (0, a.int)(i.paddingLeft) + (0, a.int)(n.marginLeft),
+                                top: -r.offsetTop + (0, a.int)(i.paddingTop) + (0, a.int)(n.marginTop),
+                                right: (0, l.innerWidth)(t) - (0, l.outerWidth)(r) - r.offsetLeft + (0, a.int)(i.paddingRight) - (0, a.int)(n.marginRight),
+                                bottom: (0, l.innerHeight)(t) - (0, l.outerHeight)(r) - r.offsetTop + (0, a.int)(i.paddingBottom) - (0, a.int)(n.marginBottom)
                             }
                     }(0, a.isNum)(s.right) && (e = Math.min(e, s.right)), (0, a.isNum)(s.bottom) && (o = Math.min(o, s.bottom)), (0, a.isNum)(s.left) && (e = Math.max(e, s.left)), (0, a.isNum)(s.top) && (o = Math.max(o, s.top))
                 }
                 return [e, o]
             }, e.getControlPosition = function(t, e, o) {
-                var i = "number" == typeof e ? (0, l.getTouch)(t, e) : null;
-                return "number" != typeof e || i ? (e = p(o), e = o.props.offsetParent || e.offsetParent || e.ownerDocument.body, (0, l.offsetXYFromParent)(i || t, e, o.props.scale)) : null
+                var r = "number" == typeof e ? (0, l.getTouch)(t, e) : null;
+                return "number" != typeof e || r ? (e = p(o), e = o.props.offsetParent || e.offsetParent || e.ownerDocument.body, (0, l.offsetXYFromParent)(r || t, e, o.props.scale)) : null
             }, e.snapToGrid = function(t, e, o) {
                 return [Math.round(e / t[0]) * t[0], Math.round(o / t[1]) * t[1]]
             };
             var a = o(570),
                 l = o(590);
 
             function p(t) {
@@ -1250,17 +1330,17 @@
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), e.default = function() {}
         },
         865: function(t, e, o) {
             "use strict";
             var o = o(866),
-                i = o.default,
+                r = o.default,
                 o = o.DraggableCore;
-            t.exports = i, t.exports.default = i, t.exports.DraggableCore = o
+            t.exports = r, t.exports.default = r, t.exports.DraggableCore = o
         },
         866: function(t, e, o) {
             "use strict";
 
             function s(t) {
                 return (s = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
                     return typeof t
@@ -1272,32 +1352,32 @@
                 value: !0
             }), Object.defineProperty(e, "DraggableCore", {
                 enumerable: !0,
                 get: function() {
                     return g.default
                 }
             }), e.default = void 0;
-            var h = function(t) {
+            var c = function(t) {
                     if (t && t.__esModule) return t;
                     if (null === t || "object" !== s(t) && "function" != typeof t) return {
                         default: t
                     };
                     var e = p(void 0);
                     if (e && e.has(t)) return e.get(t);
-                    var o, i, n = {},
-                        r = Object.defineProperty && Object.getOwnPropertyDescriptor;
-                    for (o in t) "default" !== o && Object.prototype.hasOwnProperty.call(t, o) && ((i = r ? Object.getOwnPropertyDescriptor(t, o) : null) && (i.get || i.set) ? Object.defineProperty(n, o, i) : n[o] = t[o]);
-                    return n.default = t, e && e.set(t, n), n
+                    var o, r, i = {},
+                        n = Object.defineProperty && Object.getOwnPropertyDescriptor;
+                    for (o in t) "default" !== o && Object.prototype.hasOwnProperty.call(t, o) && ((r = n ? Object.getOwnPropertyDescriptor(t, o) : null) && (r.get || r.set) ? Object.defineProperty(i, o, r) : i[o] = t[o]);
+                    return i.default = t, e && e.set(t, i), i
                 }(o(1)),
-                i = a(o(0)),
-                n = a(o(29)),
-                c = a(o(43)),
-                d = o(590),
-                f = o(644),
-                r = o(570),
+                r = a(o(0)),
+                i = a(o(29)),
+                h = a(o(43)),
+                f = o(590),
+                d = o(644),
+                n = o(570),
                 g = a(o(868)),
                 l = a(o(645)),
                 y = ["axis", "bounds", "children", "defaultPosition", "defaultClassName", "defaultClassNameDragging", "defaultClassNameDragged", "position", "positionOffset", "scale"];
 
             function a(t) {
                 return t && t.__esModule ? t : {
                     default: t
@@ -1310,159 +1390,159 @@
                     return t ? o : e
                 })(t))
             }
 
             function b() {
                 return (b = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
-                        var o, i = arguments[e];
-                        for (o in i) Object.prototype.hasOwnProperty.call(i, o) && (t[o] = i[o])
+                        var o, r = arguments[e];
+                        for (o in r) Object.prototype.hasOwnProperty.call(r, o) && (t[o] = r[o])
                     }
                     return t
                 }).apply(this, arguments)
             }
 
             function u(e, t) {
-                var o, i = Object.keys(e);
+                var o, r = Object.keys(e);
                 return Object.getOwnPropertySymbols && (o = Object.getOwnPropertySymbols(e), t && (o = o.filter(function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
-                })), i.push.apply(i, o)), i
+                })), r.push.apply(r, o)), r
             }
 
             function m(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var o = null != arguments[t] ? arguments[t] : {};
                     t % 2 ? u(Object(o), !0).forEach(function(t) {
-                        O(e, t, o[t])
+                        D(e, t, o[t])
                     }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(o)) : u(Object(o)).forEach(function(t) {
                         Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(o, t))
                     })
                 }
                 return e
             }
 
             function v(t, e) {
                 (null == e || e > t.length) && (e = t.length);
-                for (var o = 0, i = new Array(e); o < e; o++) i[o] = t[o];
-                return i
+                for (var o = 0, r = new Array(e); o < e; o++) r[o] = t[o];
+                return r
             }
 
             function w(t, e) {
                 for (var o = 0; o < e.length; o++) {
-                    var i = e[o];
-                    i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
+                    var r = e[o];
+                    r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(t, r.key, r)
                 }
             }
 
             function S(t, e) {
                 return (S = Object.setPrototypeOf || function(t, e) {
                     return t.__proto__ = e, t
                 })(t, e)
             }
 
             function x(o) {
-                var i = function() {
+                var r = function() {
                     if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                     if (Reflect.construct.sham) return !1;
                     if ("function" == typeof Proxy) return !0;
                     try {
                         return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
                     } catch (t) {
                         return !1
                     }
                 }();
                 return function() {
-                    var t, e = D(o),
-                        e = (t = i ? (t = D(this).constructor, Reflect.construct(e, arguments, t)) : e.apply(this, arguments), this);
+                    var t, e = O(o),
+                        e = (t = r ? (t = O(this).constructor, Reflect.construct(e, arguments, t)) : e.apply(this, arguments), this);
                     if (t && ("object" === s(t) || "function" == typeof t)) return t;
                     if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
                     return z(e)
                 }
             }
 
             function z(t) {
                 if (void 0 === t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                 return t
             }
 
-            function D(t) {
-                return (D = Object.setPrototypeOf ? Object.getPrototypeOf : function(t) {
+            function O(t) {
+                return (O = Object.setPrototypeOf ? Object.getPrototypeOf : function(t) {
                     return t.__proto__ || Object.getPrototypeOf(t)
                 })(t)
             }
 
-            function O(t, e, o) {
+            function D(t, e, o) {
                 e in t ? Object.defineProperty(t, e, {
                     value: o,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : t[e] = o
             }
             o = function(t) {
-                var e = i;
+                var e = r;
                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                 e.prototype = Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }), Object.defineProperty(e, "prototype", {
                     writable: !1
                 }), t && S(e, t);
-                var o = x(i);
+                var o = x(r);
 
-                function i(t) {
+                function r(t) {
                     var a;
-                    if (this instanceof i) return O(z(a = o.call(this, t)), "onDragStart", function(t, e) {
-                        if ((0, l.default)("Draggable: onDragStart: %j", e), !1 === a.props.onStart(t, (0, f.createDraggableData)(z(a), e))) return !1;
+                    if (this instanceof r) return D(z(a = o.call(this, t)), "onDragStart", function(t, e) {
+                        if ((0, l.default)("Draggable: onDragStart: %j", e), !1 === a.props.onStart(t, (0, d.createDraggableData)(z(a), e))) return !1;
                         a.setState({
                             dragging: !0,
                             dragged: !0
                         })
-                    }), O(z(a), "onDrag", function(t, e) {
+                    }), D(z(a), "onDrag", function(t, e) {
                         if (!a.state.dragging) return !1;
                         (0, l.default)("Draggable: onDrag: %j", e);
-                        var o, i, n, r, e = (0, f.createDraggableData)(z(a), e),
+                        var o, r, i, n, e = (0, d.createDraggableData)(z(a), e),
                             s = {
                                 x: e.x,
                                 y: e.y
                             };
-                        if (a.props.bounds && (o = s.x, i = s.y, s.x += a.state.slackX, s.y += a.state.slackY, n = (0, f.getBoundPosition)(z(a), s.x, s.y), r = 2, r = (n = function(t) {
+                        if (a.props.bounds && (o = s.x, r = s.y, s.x += a.state.slackX, s.y += a.state.slackY, i = (0, d.getBoundPosition)(z(a), s.x, s.y), n = 2, n = (i = function(t) {
                                 if (Array.isArray(t)) return t
-                            }(n) || function(t, e) {
+                            }(i) || function(t, e) {
                                 var o = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
                                 if (null != o) {
-                                    var i, n, r = [],
+                                    var r, i, n = [],
                                         s = !0,
                                         a = !1;
                                     try {
-                                        for (o = o.call(t); !(s = (i = o.next()).done) && (r.push(i.value), !e || r.length !== e); s = !0);
+                                        for (o = o.call(t); !(s = (r = o.next()).done) && (n.push(r.value), !e || n.length !== e); s = !0);
                                     } catch (t) {
-                                        a = !0, n = t
+                                        a = !0, i = t
                                     } finally {
                                         try {
                                             s || null == o.return || o.return()
                                         } finally {
-                                            if (a) throw n
+                                            if (a) throw i
                                         }
                                     }
-                                    return r
+                                    return n
                                 }
-                            }(n, r) || function(t, e) {
+                            }(i, n) || function(t, e) {
                                 var o;
                                 if (t) return "string" == typeof t ? v(t, e) : "Map" === (o = "Object" === (o = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : o) || "Set" === o ? Array.from(t) : "Arguments" === o || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(o) ? v(t, e) : void 0
-                            }(n, r) || function() {
+                            }(i, n) || function() {
                                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
-                            }())[0], n = n[1], s.x = r, s.y = n, s.slackX = a.state.slackX + (o - s.x), s.slackY = a.state.slackY + (i - s.y), e.x = s.x, e.y = s.y, e.deltaX = s.x - a.state.x, e.deltaY = s.y - a.state.y), !1 === a.props.onDrag(t, e)) return !1;
+                            }())[0], i = i[1], s.x = n, s.y = i, s.slackX = a.state.slackX + (o - s.x), s.slackY = a.state.slackY + (r - s.y), e.x = s.x, e.y = s.y, e.deltaX = s.x - a.state.x, e.deltaY = s.y - a.state.y), !1 === a.props.onDrag(t, e)) return !1;
                         a.setState(s)
-                    }), O(z(a), "onDragStop", function(t, e) {
+                    }), D(z(a), "onDragStop", function(t, e) {
                         if (!a.state.dragging) return !1;
-                        if (!1 === a.props.onStop(t, (0, f.createDraggableData)(z(a), e))) return !1;
+                        if (!1 === a.props.onStop(t, (0, d.createDraggableData)(z(a), e))) return !1;
                         (0, l.default)("Draggable: onDragStop: %j", e);
                         var o, t = {
                             dragging: !1,
                             slackX: 0,
                             slackY: 0
                         };
                         Boolean(a.props.position) && (o = (e = a.props.position).x, e = e.y, t.x = o, t.y = e), a.setState(t)
@@ -1487,15 +1567,15 @@
                             prevPropsPosition: e
                         }), {
                             x: t.x,
                             y: t.y,
                             prevPropsPosition: m({}, t)
                         })
                     }
-                }], w((t = i).prototype, [{
+                }], w((t = r).prototype, [{
                     key: "componentDidMount",
                     value: function() {
                         void 0 !== window.SVGElement && this.findDOMNode() instanceof window.SVGElement && this.setState({
                             isElementSVG: !0
                         })
                     }
                 }, {
@@ -1505,88 +1585,88 @@
                             dragging: !1
                         })
                     }
                 }, {
                     key: "findDOMNode",
                     value: function() {
                         var t;
-                        return null != (t = null == (t = this.props) || null == (t = t.nodeRef) ? void 0 : t.current) ? t : n.default.findDOMNode(this)
+                        return null != (t = null == (t = this.props) || null == (t = t.nodeRef) ? void 0 : t.current) ? t : i.default.findDOMNode(this)
                     }
                 }, {
                     key: "render",
                     value: function() {
                         var t = this.props,
                             e = (t.axis, t.bounds, t.children),
                             o = t.defaultPosition,
-                            i = t.defaultClassName,
-                            n = t.defaultClassNameDragging,
-                            r = t.defaultClassNameDragged,
+                            r = t.defaultClassName,
+                            i = t.defaultClassNameDragging,
+                            n = t.defaultClassNameDragged,
                             s = t.position,
                             a = t.positionOffset,
                             t = (t.scale, function(t, e) {
                                 if (null == t) return {};
-                                var o, i = function(t, e) {
+                                var o, r = function(t, e) {
                                     if (null == t) return {};
-                                    for (var o, i = {}, n = Object.keys(t), r = 0; r < n.length; r++) o = n[r], 0 <= e.indexOf(o) || (i[o] = t[o]);
-                                    return i
+                                    for (var o, r = {}, i = Object.keys(t), n = 0; n < i.length; n++) o = i[n], 0 <= e.indexOf(o) || (r[o] = t[o]);
+                                    return r
                                 }(t, e);
                                 if (Object.getOwnPropertySymbols)
-                                    for (var n = Object.getOwnPropertySymbols(t), r = 0; r < n.length; r++) o = n[r], 0 <= e.indexOf(o) || Object.prototype.propertyIsEnumerable.call(t, o) && (i[o] = t[o]);
-                                return i
+                                    for (var i = Object.getOwnPropertySymbols(t), n = 0; n < i.length; n++) o = i[n], 0 <= e.indexOf(o) || Object.prototype.propertyIsEnumerable.call(t, o) && (r[o] = t[o]);
+                                return r
                             }(t, y)),
                             l = {},
                             p = null,
                             u = !Boolean(s) || this.state.dragging,
                             s = s || o,
                             o = {
-                                x: ((0, f.canDragX)(this) && u ? this.state : s).x,
-                                y: ((0, f.canDragY)(this) && u ? this.state : s).y
+                                x: ((0, d.canDragX)(this) && u ? this.state : s).x,
+                                y: ((0, d.canDragY)(this) && u ? this.state : s).y
                             },
-                            s = (this.state.isElementSVG ? p = (0, d.createSVGTransform)(o, a) : l = (0, d.createCSSTransform)(o, a), (0, c.default)(e.props.className || "", i, (O(u = {}, n, this.state.dragging), O(u, r, this.state.dragged), u)));
-                        return h.createElement(g.default, b({}, t, {
+                            s = (this.state.isElementSVG ? p = (0, f.createSVGTransform)(o, a) : l = (0, f.createCSSTransform)(o, a), (0, h.default)(e.props.className || "", r, (D(u = {}, i, this.state.dragging), D(u, n, this.state.dragged), u)));
+                        return c.createElement(g.default, b({}, t, {
                             onStart: this.onDragStart,
                             onDrag: this.onDrag,
                             onStop: this.onDragStop
-                        }), h.cloneElement(h.Children.only(e), {
+                        }), c.cloneElement(c.Children.only(e), {
                             className: s,
                             style: m(m({}, e.props.style), l),
                             transform: p
                         }))
                     }
                 }]), w(t, e), Object.defineProperty(t, "prototype", {
                     writable: !1
-                }), i
-            }(h.Component);
-            O(e.default = o, "displayName", "Draggable"), O(o, "propTypes", m(m({}, g.default.propTypes), {}, {
-                axis: i.default.oneOf(["both", "x", "y", "none"]),
-                bounds: i.default.oneOfType([i.default.shape({
-                    left: i.default.number,
-                    right: i.default.number,
-                    top: i.default.number,
-                    bottom: i.default.number
-                }), i.default.string, i.default.oneOf([!1])]),
-                defaultClassName: i.default.string,
-                defaultClassNameDragging: i.default.string,
-                defaultClassNameDragged: i.default.string,
-                defaultPosition: i.default.shape({
-                    x: i.default.number,
-                    y: i.default.number
+                }), r
+            }(c.Component);
+            D(e.default = o, "displayName", "Draggable"), D(o, "propTypes", m(m({}, g.default.propTypes), {}, {
+                axis: r.default.oneOf(["both", "x", "y", "none"]),
+                bounds: r.default.oneOfType([r.default.shape({
+                    left: r.default.number,
+                    right: r.default.number,
+                    top: r.default.number,
+                    bottom: r.default.number
+                }), r.default.string, r.default.oneOf([!1])]),
+                defaultClassName: r.default.string,
+                defaultClassNameDragging: r.default.string,
+                defaultClassNameDragged: r.default.string,
+                defaultPosition: r.default.shape({
+                    x: r.default.number,
+                    y: r.default.number
                 }),
-                positionOffset: i.default.shape({
-                    x: i.default.oneOfType([i.default.number, i.default.string]),
-                    y: i.default.oneOfType([i.default.number, i.default.string])
+                positionOffset: r.default.shape({
+                    x: r.default.oneOfType([r.default.number, r.default.string]),
+                    y: r.default.oneOfType([r.default.number, r.default.string])
                 }),
-                position: i.default.shape({
-                    x: i.default.number,
-                    y: i.default.number
+                position: r.default.shape({
+                    x: r.default.number,
+                    y: r.default.number
                 }),
-                className: r.dontSetMe,
-                style: r.dontSetMe,
-                transform: r.dontSetMe
-            })), O(o, "defaultProps", m(m({}, g.default.defaultProps), {}, {
+                className: n.dontSetMe,
+                style: n.dontSetMe,
+                transform: n.dontSetMe
+            })), D(o, "defaultProps", m(m({}, g.default.defaultProps), {}, {
                 axis: "both",
                 bounds: !1,
                 defaultClassName: "react-draggable",
                 defaultClassNameDragging: "react-draggable-dragging",
                 defaultClassNameDragged: "react-draggable-dragged",
                 defaultPosition: {
                     x: 0,
@@ -1595,37 +1675,37 @@
                 scale: 1
             }))
         },
         867: function(t, e, o) {
             "use strict";
             Object.defineProperty(e, "__esModule", {
                 value: !0
-            }), e.browserPrefixToKey = r, e.browserPrefixToStyle = function(t, e) {
+            }), e.browserPrefixToKey = n, e.browserPrefixToStyle = function(t, e) {
                 return e ? "-".concat(e.toLowerCase(), "-").concat(t) : t
-            }, e.default = void 0, e.getPrefix = i;
-            var n = ["Moz", "Webkit", "O", "ms"];
+            }, e.default = void 0, e.getPrefix = r;
+            var i = ["Moz", "Webkit", "O", "ms"];
 
-            function i() {
+            function r() {
                 var t, e = 0 < arguments.length && void 0 !== arguments[0] ? arguments[0] : "transform";
                 if ("undefined" != typeof window) {
                     var o = null == (t = window.document) || null == (t = t.documentElement) ? void 0 : t.style;
                     if (o && !(e in o))
-                        for (var i = 0; i < n.length; i++)
-                            if (r(e, n[i]) in o) return n[i]
+                        for (var r = 0; r < i.length; r++)
+                            if (n(e, i[r]) in o) return i[r]
                 }
                 return ""
             }
 
-            function r(t, e) {
+            function n(t, e) {
                 return e ? "".concat(e).concat(function(t) {
-                    for (var e = "", o = !0, i = 0; i < t.length; i++) o ? (e += t[i].toUpperCase(), o = !1) : "-" === t[i] ? o = !0 : e += t[i];
+                    for (var e = "", o = !0, r = 0; r < t.length; r++) o ? (e += t[r].toUpperCase(), o = !1) : "-" === t[r] ? o = !0 : e += t[r];
                     return e
                 }(t)) : t
             }
-            var s = i();
+            var s = r();
             e.default = s
         },
         868: function(t, e, o) {
             "use strict";
 
             function s(t) {
                 return (s = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
@@ -1633,109 +1713,109 @@
                 } : function(t) {
                     return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
                 })(t)
             }
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), e.default = void 0;
-            var i = function(t) {
+            var r = function(t) {
                     if (t && t.__esModule) return t;
                     if (null === t || "object" !== s(t) && "function" != typeof t) return {
                         default: t
                     };
-                    var e = c(void 0);
+                    var e = h(void 0);
                     if (e && e.has(t)) return e.get(t);
-                    var o, i, n = {},
-                        r = Object.defineProperty && Object.getOwnPropertyDescriptor;
-                    for (o in t) "default" !== o && Object.prototype.hasOwnProperty.call(t, o) && ((i = r ? Object.getOwnPropertyDescriptor(t, o) : null) && (i.get || i.set) ? Object.defineProperty(n, o, i) : n[o] = t[o]);
-                    return n.default = t, e && e.set(t, n), n
+                    var o, r, i = {},
+                        n = Object.defineProperty && Object.getOwnPropertyDescriptor;
+                    for (o in t) "default" !== o && Object.prototype.hasOwnProperty.call(t, o) && ((r = n ? Object.getOwnPropertyDescriptor(t, o) : null) && (r.get || r.set) ? Object.defineProperty(i, o, r) : i[o] = t[o]);
+                    return i.default = t, e && e.set(t, i), i
                 }(o(1)),
-                n = a(o(0)),
+                i = a(o(0)),
                 l = a(o(29)),
                 p = o(590),
                 u = o(644),
-                r = o(570),
-                h = a(o(645));
+                n = o(570),
+                c = a(o(645));
 
             function a(t) {
                 return t && t.__esModule ? t : {
                     default: t
                 }
             }
 
-            function c(t) {
+            function h(t) {
                 var e, o;
-                return "function" != typeof WeakMap ? null : (e = new WeakMap, o = new WeakMap, (c = function(t) {
+                return "function" != typeof WeakMap ? null : (e = new WeakMap, o = new WeakMap, (h = function(t) {
                     return t ? o : e
                 })(t))
             }
 
-            function d(t, e) {
+            function f(t, e) {
                 return function(t) {
                     if (Array.isArray(t)) return t
                 }(t) || function(t, e) {
                     var o = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
                     if (null != o) {
-                        var i, n, r = [],
+                        var r, i, n = [],
                             s = !0,
                             a = !1;
                         try {
-                            for (o = o.call(t); !(s = (i = o.next()).done) && (r.push(i.value), !e || r.length !== e); s = !0);
+                            for (o = o.call(t); !(s = (r = o.next()).done) && (n.push(r.value), !e || n.length !== e); s = !0);
                         } catch (t) {
-                            a = !0, n = t
+                            a = !0, i = t
                         } finally {
                             try {
                                 s || null == o.return || o.return()
                             } finally {
-                                if (a) throw n
+                                if (a) throw i
                             }
                         }
-                        return r
+                        return n
                     }
                 }(t, e) || function(t, e) {
                     var o;
-                    if (t) return "string" == typeof t ? f(t, e) : "Map" === (o = "Object" === (o = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : o) || "Set" === o ? Array.from(t) : "Arguments" === o || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(o) ? f(t, e) : void 0
+                    if (t) return "string" == typeof t ? d(t, e) : "Map" === (o = "Object" === (o = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : o) || "Set" === o ? Array.from(t) : "Arguments" === o || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(o) ? d(t, e) : void 0
                 }(t, e) || function() {
                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                 }()
             }
 
-            function f(t, e) {
+            function d(t, e) {
                 (null == e || e > t.length) && (e = t.length);
-                for (var o = 0, i = new Array(e); o < e; o++) i[o] = t[o];
-                return i
+                for (var o = 0, r = new Array(e); o < e; o++) r[o] = t[o];
+                return r
             }
 
             function g(t, e) {
                 for (var o = 0; o < e.length; o++) {
-                    var i = e[o];
-                    i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
+                    var r = e[o];
+                    r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(t, r.key, r)
                 }
             }
 
             function y(t, e) {
                 return (y = Object.setPrototypeOf || function(t, e) {
                     return t.__proto__ = e, t
                 })(t, e)
             }
 
             function b(o) {
-                var i = function() {
+                var r = function() {
                     if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                     if (Reflect.construct.sham) return !1;
                     if ("function" == typeof Proxy) return !0;
                     try {
                         return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
                     } catch (t) {
                         return !1
                     }
                 }();
                 return function() {
                     var t, e = v(o),
-                        e = (t = i ? (t = v(this).constructor, Reflect.construct(e, arguments, t)) : e.apply(this, arguments), this);
+                        e = (t = r ? (t = v(this).constructor, Reflect.construct(e, arguments, t)) : e.apply(this, arguments), this);
                     if (t && ("object" === s(t) || "function" == typeof t)) return t;
                     if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
                     return m(e)
                 }
             }
 
             function m(t) {
@@ -1776,78 +1856,78 @@
                             value: e,
                             writable: !0,
                             configurable: !0
                         }
                     }), Object.defineProperty(e, "prototype", {
                         writable: !1
                     }), t && y(e, t);
-                    var r = b(a);
+                    var n = b(a);
 
                     function a() {
                         var s, t = this,
                             e = a;
                         if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function");
-                        for (var o = arguments.length, i = new Array(o), n = 0; n < o; n++) i[n] = arguments[n];
-                        return w(m(s = r.call.apply(r, [this].concat(i))), "state", {
+                        for (var o = arguments.length, r = new Array(o), i = 0; i < o; i++) r[i] = arguments[i];
+                        return w(m(s = n.call.apply(n, [this].concat(r))), "state", {
                             dragging: !1,
                             lastX: NaN,
                             lastY: NaN,
                             touchIdentifier: null
                         }), w(m(s), "mounted", !1), w(m(s), "handleDragStart", function(t) {
                             if (s.props.onMouseDown(t), !s.props.allowAnyClick && "number" == typeof t.button && 0 !== t.button) return !1;
                             var e = s.findDOMNode();
                             if (!e || !e.ownerDocument || !e.ownerDocument.body) throw new Error("<DraggableCore> not mounted on DragStart!");
-                            var o, i, n = e.ownerDocument;
-                            s.props.disabled || !(t.target instanceof n.defaultView.Node) || s.props.handle && !(0, p.matchesSelectorAndParentsTo)(t.target, s.props.handle, e) || s.props.cancel && (0, p.matchesSelectorAndParentsTo)(t.target, s.props.cancel, e) || ("touchstart" === t.type && t.preventDefault(), e = (0, p.getTouchIdentifier)(t), s.setState({
+                            var o, r, i = e.ownerDocument;
+                            s.props.disabled || !(t.target instanceof i.defaultView.Node) || s.props.handle && !(0, p.matchesSelectorAndParentsTo)(t.target, s.props.handle, e) || s.props.cancel && (0, p.matchesSelectorAndParentsTo)(t.target, s.props.cancel, e) || ("touchstart" === t.type && t.preventDefault(), e = (0, p.getTouchIdentifier)(t), s.setState({
                                 touchIdentifier: e
-                            }), null != (e = (0, u.getControlPosition)(t, e, m(s))) && (o = e.x, e = e.y, i = (0, u.createCoreData)(m(s), o, e), (0, h.default)("DraggableCore: handleDragStart: %j", i), (0, h.default)("calling", s.props.onStart), !1 !== s.props.onStart(t, i)) && !1 !== s.mounted && (s.props.enableUserSelectHack && (0, p.addUserSelectStyles)(n), s.setState({
+                            }), null != (e = (0, u.getControlPosition)(t, e, m(s))) && (o = e.x, e = e.y, r = (0, u.createCoreData)(m(s), o, e), (0, c.default)("DraggableCore: handleDragStart: %j", r), (0, c.default)("calling", s.props.onStart), !1 !== s.props.onStart(t, r)) && !1 !== s.mounted && (s.props.enableUserSelectHack && (0, p.addUserSelectStyles)(i), s.setState({
                                 dragging: !0,
                                 lastX: o,
                                 lastY: e
-                            }), (0, p.addEvent)(n, z.move, s.handleDrag), (0, p.addEvent)(n, z.stop, s.handleDragStop)))
+                            }), (0, p.addEvent)(i, z.move, s.handleDrag), (0, p.addEvent)(i, z.stop, s.handleDragStop)))
                         }), w(m(s), "handleDrag", function(t) {
                             var e = (0, u.getControlPosition)(t, s.state.touchIdentifier, m(s));
                             if (null != e) {
                                 var o = e.x,
                                     e = e.y;
                                 if (Array.isArray(s.props.grid)) {
-                                    var i = o - s.state.lastX,
-                                        n = e - s.state.lastY,
-                                        r = d((0, u.snapToGrid)(s.props.grid, i, n), 2),
-                                        i = r[0],
-                                        n = r[1];
-                                    if (!i && !n) return;
-                                    o = s.state.lastX + i, e = s.state.lastY + n
+                                    var r = o - s.state.lastX,
+                                        i = e - s.state.lastY,
+                                        n = f((0, u.snapToGrid)(s.props.grid, r, i), 2),
+                                        r = n[0],
+                                        i = n[1];
+                                    if (!r && !i) return;
+                                    o = s.state.lastX + r, e = s.state.lastY + i
                                 }
-                                r = (0, u.createCoreData)(m(s), o, e);
-                                if ((0, h.default)("DraggableCore: handleDrag: %j", r), !1 !== s.props.onDrag(t, r) && !1 !== s.mounted) s.setState({
+                                n = (0, u.createCoreData)(m(s), o, e);
+                                if ((0, c.default)("DraggableCore: handleDrag: %j", n), !1 !== s.props.onDrag(t, n) && !1 !== s.mounted) s.setState({
                                     lastX: o,
                                     lastY: e
                                 });
                                 else try {
                                     s.handleDragStop(new MouseEvent("mouseup"))
                                 } catch (t) {
-                                    i = document.createEvent("MouseEvents");
-                                    i.initMouseEvent("mouseup", !0, !0, window, 0, 0, 0, 0, 0, !1, !1, !1, !1, 0, null), s.handleDragStop(i)
+                                    r = document.createEvent("MouseEvents");
+                                    r.initMouseEvent("mouseup", !0, !0, window, 0, 0, 0, 0, 0, !1, !1, !1, !1, 0, null), s.handleDragStop(r)
                                 }
                             }
                         }), w(m(s), "handleDragStop", function(t) {
                             if (s.state.dragging) {
                                 var e = (0, u.getControlPosition)(t, s.state.touchIdentifier, m(s));
                                 if (null != e) {
-                                    var o, i = e.x,
+                                    var o, r = e.x,
                                         e = e.y,
-                                        n = (Array.isArray(s.props.grid) && (r = i - s.state.lastX || 0, o = e - s.state.lastY || 0, r = (n = d((0, u.snapToGrid)(s.props.grid, r, o), 2))[0], o = n[1], i = s.state.lastX + r, e = s.state.lastY + o), (0, u.createCoreData)(m(s), i, e));
-                                    if (!1 === s.props.onStop(t, n) || !1 === s.mounted) return !1;
-                                    var r = s.findDOMNode();
-                                    r && s.props.enableUserSelectHack && (0, p.removeUserSelectStyles)(r.ownerDocument), (0, h.default)("DraggableCore: handleDragStop: %j", n), s.setState({
+                                        i = (Array.isArray(s.props.grid) && (n = r - s.state.lastX || 0, o = e - s.state.lastY || 0, n = (i = f((0, u.snapToGrid)(s.props.grid, n, o), 2))[0], o = i[1], r = s.state.lastX + n, e = s.state.lastY + o), (0, u.createCoreData)(m(s), r, e));
+                                    if (!1 === s.props.onStop(t, i) || !1 === s.mounted) return !1;
+                                    var n = s.findDOMNode();
+                                    n && s.props.enableUserSelectHack && (0, p.removeUserSelectStyles)(n.ownerDocument), (0, c.default)("DraggableCore: handleDragStop: %j", i), s.setState({
                                         dragging: !1,
                                         lastX: NaN,
                                         lastY: NaN
-                                    }), r && ((0, h.default)("DraggableCore: Removing handlers"), (0, p.removeEvent)(r.ownerDocument, z.move, s.handleDrag), (0, p.removeEvent)(r.ownerDocument, z.stop, s.handleDragStop))
+                                    }), n && ((0, c.default)("DraggableCore: Removing handlers"), (0, p.removeEvent)(n.ownerDocument, z.move, s.handleDrag), (0, p.removeEvent)(n.ownerDocument, z.stop, s.handleDragStop))
                                 }
                             }
                         }), w(m(s), "onMouseDown", function(t) {
                             return z = x, s.handleDragStart(t)
                         }), w(m(s), "onMouseUp", function(t) {
                             return z = x, s.handleDragStop(t)
                         }), w(m(s), "onTouchStart", function(t) {
@@ -1879,70 +1959,70 @@
                         value: function() {
                             var t;
                             return null != (t = this.props) && t.nodeRef ? null == (t = this.props) || null == (t = t.nodeRef) ? void 0 : t.current : l.default.findDOMNode(this)
                         }
                     }, {
                         key: "render",
                         value: function() {
-                            return i.cloneElement(i.Children.only(this.props.children), {
+                            return r.cloneElement(r.Children.only(this.props.children), {
                                 onMouseDown: this.onMouseDown,
                                 onMouseUp: this.onMouseUp,
                                 onTouchEnd: this.onTouchEnd
                             })
                         }
                     }]), Object.defineProperty(e, "prototype", {
                         writable: !1
                     }), a
-                }(i.Component);
+                }(r.Component);
             w(e.default = o, "displayName", "DraggableCore"), w(o, "propTypes", {
-                allowAnyClick: n.default.bool,
-                disabled: n.default.bool,
-                enableUserSelectHack: n.default.bool,
+                allowAnyClick: i.default.bool,
+                disabled: i.default.bool,
+                enableUserSelectHack: i.default.bool,
                 offsetParent: function(t, e) {
                     if (t[e] && 1 !== t[e].nodeType) throw new Error("Draggable's offsetParent must be a DOM Node.")
                 },
-                grid: n.default.arrayOf(n.default.number),
-                handle: n.default.string,
-                cancel: n.default.string,
-                nodeRef: n.default.object,
-                onStart: n.default.func,
-                onDrag: n.default.func,
-                onStop: n.default.func,
-                onMouseDown: n.default.func,
-                scale: n.default.number,
-                className: r.dontSetMe,
-                style: r.dontSetMe,
-                transform: r.dontSetMe
+                grid: i.default.arrayOf(i.default.number),
+                handle: i.default.string,
+                cancel: i.default.string,
+                nodeRef: i.default.object,
+                onStart: i.default.func,
+                onDrag: i.default.func,
+                onStop: i.default.func,
+                onMouseDown: i.default.func,
+                scale: i.default.number,
+                className: n.dontSetMe,
+                style: n.dontSetMe,
+                transform: n.dontSetMe
             }), w(o, "defaultProps", {
                 allowAnyClick: !1,
                 disabled: !1,
                 enableUserSelectHack: !0,
                 onStart: function() {},
                 onDrag: function() {},
                 onStop: function() {},
                 onMouseDown: function() {},
                 scale: 1
             })
         },
         869: function(t, e) {
-            function n(t, e, o, i) {
-                var o = null == i || "number" == typeof i || "boolean" == typeof i ? i : o(i),
-                    n = e.get(o);
-                return void 0 === n && (n = t.call(this, i), e.set(o, n)), n
+            function i(t, e, o, r) {
+                var o = null == r || "number" == typeof r || "boolean" == typeof r ? r : o(r),
+                    i = e.get(o);
+                return void 0 === i && (i = t.call(this, r), e.set(o, i)), i
             }
 
-            function r(t, e, o) {
-                var i = Array.prototype.slice.call(arguments, 3),
-                    n = o(i),
-                    r = e.get(n);
-                return void 0 === r && (r = t.apply(this, i), e.set(n, r)), r
+            function n(t, e, o) {
+                var r = Array.prototype.slice.call(arguments, 3),
+                    i = o(r),
+                    n = e.get(i);
+                return void 0 === n && (n = t.apply(this, r), e.set(i, n)), n
             }
 
-            function s(t, e, o, i, n) {
-                return o.bind(e, t, i, n)
+            function s(t, e, o, r, i) {
+                return o.bind(e, t, r, i)
             }
 
             function a() {
                 return JSON.stringify(arguments)
             }
 
             function o() {
@@ -1958,25 +2038,25 @@
             var l = {
                 create: function() {
                     return new o
                 }
             };
             t.exports = function(t, e) {
                 var o = e && e.cache ? e.cache : l,
-                    i = e && e.serializer ? e.serializer : a;
+                    r = e && e.serializer ? e.serializer : a;
                 return (e && e.strategy ? e.strategy : function(t, e) {
-                    return s(t, this, 1 === t.length ? n : r, e.cache.create(), e.serializer)
+                    return s(t, this, 1 === t.length ? i : n, e.cache.create(), e.serializer)
                 })(t, {
                     cache: o,
-                    serializer: i
+                    serializer: r
                 })
             }, t.exports.strategies = {
                 variadic: function(t, e) {
-                    return s(t, this, r, e.cache.create(), e.serializer)
+                    return s(t, this, n, e.cache.create(), e.serializer)
                 },
                 monadic: function(t, e) {
-                    return s(t, this, n, e.cache.create(), e.serializer)
+                    return s(t, this, i, e.cache.create(), e.serializer)
                 }
             }
         }
     }
 ]);
```

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_seamless_scroll.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_seamless_scroll.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_shortcut_panel.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_shortcut_panel.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_sortable.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_sortable.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-feffery_word_preview.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-feffery_word_preview.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/async-fuc-shared.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/async-fuc-shared.js`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/feffery_utils_components.min.js` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/feffery_utils_components.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -116,15 +116,15 @@
     Object.defineProperty(c, "p", {
         get: (t = r().src.split("/").slice(0, -1).join("/") + "/", function() {
             return t
         })
     }), void 0 !== u && (o = u, u = function(e) {
         var t, n = /\/_dash-component-suites\//.test(r().src),
             e = o(e);
-        return n ? ((t = (n = e.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-rc8m1710146411"), n.splice(-1, 1, t.join(".")), n.join("/")) : e
+        return n ? ((t = (n = e.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-rc9m1710402078"), n.splice(-1, 1, t.join(".")), n.join("/")) : e
     });
     var i = (a = window.webpackJsonpfeffery_utils_components = window.webpackJsonpfeffery_utils_components || []).push.bind(a);
     a.push = e;
     for (var a = a.slice(), f = 0; f < a.length; f++) e(a[f]);
     var d = i;
     return c(c.s = 493)
 }([function(e, t) {
@@ -12194,22 +12194,26 @@
             lockAspectRatio: a.a.oneOfType([a.a.bool, a.a.number]),
             lockAspectRatioExtraWidth: a.a.number,
             lockAspectRatioExtraHeight: a.a.number,
             direction: a.a.arrayOf(a.a.oneOf(["top", "right", "bottom", "left", "topRight", "bottomRight", "bottomLeft", "topLeft"])),
             disableDragging: a.a.bool,
             dragAxis: a.a.oneOf(["x", "y", "both", "none"]),
             bounds: a.a.oneOf(["window", "parent"]),
+            selected: a.a.bool,
+            selectedStyle: a.a.object,
+            selectedClassName: a.a.string,
             setProps: a.a.func,
             loading_state: a.a.shape({
                 is_loading: a.a.bool,
                 prop_name: a.a.string,
                 component_name: a.a.string
             })
         }, r.defaultProps = {
-            direction: ["top", "right", "bottom", "left", "topRight", "bottomRight", "bottomLeft", "topLeft"]
+            direction: ["top", "right", "bottom", "left", "topRight", "bottomRight", "bottomLeft", "topLeft"],
+            selected: !1
         }, (t.a = r).propTypes),
         u = r.defaultProps
 }, function(e, t, n) {
     "use strict";
     n.d(t, "c", function() {
         return l
     }), n.d(t, "b", function() {
@@ -12732,41 +12736,95 @@
 }, function(module, __webpack_exports__, __webpack_require__) {
     "use strict";
     var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(1),
         react__WEBPACK_IMPORTED_MODULE_0___default = __webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__),
         prop_types__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(0),
         prop_types__WEBPACK_IMPORTED_MODULE_1___default = __webpack_require__.n(prop_types__WEBPACK_IMPORTED_MODULE_1__),
         FefferyExecuteJs = function FefferyExecuteJs(props) {
-            var id = props.id,
-                jsString = props.jsString,
+            var jsString = props.jsString,
+                mode = props.mode,
+                delay = props.delay,
+                interval = props.interval,
+                targetSelector = props.targetSelector,
+                targetWaitTimeout = props.targetWaitTimeout,
                 setProps = props.setProps,
                 loading_state = props.loading_state;
             return Object(react__WEBPACK_IMPORTED_MODULE_0__.useEffect)(function() {
-                if (jsString) {
+                if ("delay" === mode) jsString && setTimeout(function() {
+                    try {
+                        eval(jsString)
+                    } catch (e) {
+                        console.error(e)
+                    }
+                    setProps({
+                        jsString: null
+                    })
+                }, delay);
+                else if ("interval" === mode) {
+                    var _interval;
+                    if (jsString) return _interval = setInterval(function() {
+                            try {
+                                eval(jsString)
+                            } catch (e) {
+                                console.error(e)
+                            }
+                        }, interval),
+                        function() {
+                            return clearInterval(_interval)
+                        }
+                } else if ("wait-until-element-rendered" === mode) {
+                    var startTime, _interval2;
+                    if (jsString) return startTime = Date.now(), _interval2 = setInterval(function() {
+                            if (document.querySelector(targetSelector)) {
+                                clearInterval(_interval2), _interval2 = !1;
+                                try {
+                                    eval(jsString)
+                                } catch (e) {
+                                    console.error(e)
+                                }
+                                setProps({
+                                    jsString: null
+                                })
+                            }
+                            targetWaitTimeout && Date.now() - startTime > targetWaitTimeout && (clearInterval(_interval2), _interval2 = !1, setProps({
+                                jsString: null
+                            }))
+                        }, 200),
+                        function() {
+                            return !_interval2 && clearInterval(_interval2)
+                        }
+                } else if (jsString) {
                     try {
                         eval(jsString)
                     } catch (e) {
-                        console.log(e)
+                        console.error(e)
                     }
                     setProps({
-                        jsString: ""
+                        jsString: null
                     })
                 }
             }, [jsString]), React.createElement(React.Fragment, null)
         };
     FefferyExecuteJs.propTypes = {
         id: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
         jsString: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
+        mode: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOf(["default", "delay", "interval", "wait-until-element-rendered"]),
+        delay: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
+        interval: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
+        targetSelector: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
+        targetWaitTimeout: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
         loading_state: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.shape({
             is_loading: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             prop_name: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
             component_name: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string
         }),
         setProps: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.func
-    }, FefferyExecuteJs.defaultProps = {}, __webpack_exports__.a = FefferyExecuteJs
+    }, FefferyExecuteJs.defaultProps = {
+        mode: "default"
+    }, __webpack_exports__.a = FefferyExecuteJs
 }, function(e, t, n) {
     "use strict";
     Object.defineProperty(t, "__esModule", {
         value: !0
     });
     var r = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
```

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/metadata.json` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989761396011396%*

 * *Differences: {"'src/lib/components/FefferyExecuteJs.react.js'": "{'description': 'js直接执行组件FefferyExecuteJs', "*

 * *                                                   "'props': {'mode': OrderedDict([('type', "*

 * *                                                   "OrderedDict([('name', 'enum'), ('value', "*

 * *                                                   '[OrderedDict([(\'value\', "\'default\'"), '*

 * *                                                   "('computed', False)]), OrderedDict([('value', "*

 * *                              […]*

```diff
@@ -1823,25 +1823,39 @@
                 "type": {
                     "name": "object"
                 }
             }
         }
     },
     "src/lib/components/FefferyExecuteJs.react.js": {
-        "description": "",
+        "description": "js\u76f4\u63a5\u6267\u884c\u7ec4\u4ef6FefferyExecuteJs",
         "displayName": "FefferyExecuteJs",
         "methods": [],
         "props": {
+            "delay": {
+                "description": "delay\u6a21\u5f0f\u4e0b\uff0c\u8bbe\u7f6e\u5ef6\u65f6\u6267\u884c\u65f6\u957f\uff0c\u5355\u4f4d\uff1a\u6beb\u79d2",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
             "id": {
                 "description": "\u7ec4\u4ef6id",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
+            "interval": {
+                "description": "interval\u6a21\u5f0f\u4e0b\uff0c\u8bbe\u7f6e\u8f6e\u8be2\u6267\u884c\u95f4\u9694\u65f6\u957f\uff0c\u5355\u4f4d\uff1a\u6beb\u79d2",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
             "jsString": {
                 "description": "\u8bbe\u7f6e\u8981\u6267\u884c\u7684js\u4ee3\u7801\u5b57\u7b26\u4e32",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
@@ -1865,20 +1879,63 @@
                             "description": "Holds which property is loading",
                             "name": "string",
                             "required": false
                         }
                     }
                 }
             },
+            "mode": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "'default'"
+                },
+                "description": "\u8bbe\u7f6e\u6267\u884c\u6a21\u5f0f\uff0c\u53ef\u9009\u7684\u6709'default'\uff08\u7acb\u5373\u6267\u884c\uff09\u3001'delay'\uff08\u5ef6\u8fdf\u6267\u884c\uff09\u3001'interval'\uff08\u5b9a\u65f6\u8f6e\u8be2\u6267\u884c\uff09\u3001'wait-until-element-rendered'\uff08\u7b49\u5f85\u76ee\u6807\u5143\u7d20\u6e32\u67d3\u540e\u6267\u884c\uff09\r\n\u9ed8\u8ba4\uff1a'default'",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "'default'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'delay'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'interval'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'wait-until-element-rendered'"
+                        }
+                    ]
+                }
+            },
             "setProps": {
                 "description": "Dash-assigned callback that should be called to report property changes\r\nto Dash, to make them available for callbacks.",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
+            },
+            "targetSelector": {
+                "description": "wait-until-element-rendered\u6a21\u5f0f\u4e0b\uff0c\u8bbe\u7f6e\u9700\u8981\u7b49\u5f85\u6e32\u67d3\u5b8c\u6210\u7684\u76ee\u6807\u5143\u7d20css\u9009\u62e9\u5668",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "targetWaitTimeout": {
+                "description": "wait-until-element-rendered\u6a21\u5f0f\u4e0b\uff0c\u8bbe\u7f6e\u76ee\u6807\u5143\u7d20\u6e32\u67d3\u68c0\u6d4b\u6700\u5927\u7b49\u5f85\u65f6\u957f\uff0c\u5355\u4f4d\uff1a\u6beb\u79d2\uff0c\u9ed8\u8ba4\u65e0\u9650\u5236",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
             }
         }
     },
     "src/lib/components/FefferyExternalCss.react.js": {
         "description": "",
         "displayName": "FefferyExternalCss",
         "methods": [],
@@ -14014,14 +14071,39 @@
                 "type": {
                     "name": "arrayOf",
                     "value": {
                         "name": "number"
                     }
                 }
             },
+            "selected": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "false"
+                },
+                "description": "\u8bbe\u7f6e\u6216\u76d1\u542c\u5f53\u524d\u7ec4\u4ef6\u662f\u5426\u5904\u4e8e\u9009\u62e9\u72b6\u6001\r\n\u9ed8\u8ba4\uff1afalse",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "selectedClassName": {
+                "description": "\u914d\u7f6e\u5f53\u524d\u7ec4\u4ef6\u5728\u9009\u4e2d\u72b6\u6001\u4e0b\u7684css\u7c7b\u540d",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "selectedStyle": {
+                "description": "\u8bbe\u7f6e\u5f53\u524d\u7ec4\u4ef6\u5728\u9009\u4e2d\u72b6\u6001\u4e0b\u7684css\u6837\u5f0f",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
             "setProps": {
                 "description": "Dash-assigned callback that should be called to report property changes\r\nto Dash, to make them available for callbacks.",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
```

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components/package-info.json` & `feffery_utils_components-0.2.0rc9/feffery_utils_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.0-rc9'"}*

```diff
@@ -146,9 +146,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_utils_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-rc8"
+    "version": "0.2.0-rc9"
 }
```

### Comparing `feffery_utils_components-0.2.0rc8/feffery_utils_components.egg-info/SOURCES.txt` & `feffery_utils_components-0.2.0rc9/feffery_utils_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0rc8/package.json` & `feffery_utils_components-0.2.0rc9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.0-rc9'"}*

```diff
@@ -146,9 +146,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_utils_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-rc8"
+    "version": "0.2.0-rc9"
 }
```

### Comparing `feffery_utils_components-0.2.0rc8/setup.py` & `feffery_utils_components-0.2.0rc9/setup.py`

 * *Files identical despite different names*

